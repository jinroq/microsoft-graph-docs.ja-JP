---
title: 長時間実行アクションの処理 (ベータ版)
description: この記事では、長時間実行アクションの処理について説明します。
localization_priority: Normal
author: daspek
ms.openlocfilehash: 3d1dae399147cb1aed40a045e4365faf15d753f5
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/15/2019
ms.locfileid: "36422311"
---
# <a name="working-with-long-running-actions-beta"></a>長時間実行アクションの処理 (ベータ版)


一部の API 応答では、完了までに要する時間が不明です。
アクションが完了するまで待機してから応答を返す代わりに、Microsoft Graph では長時間実行アクションのパターンを使用できます。
このパターンでは、要求がアクションの完了を待機せずに、長時間実行アクションに関する状態の最新情報のポーリングに対しての待機をアプリに提供します。

一般的なパターンでは、以下の手順を実行します。

1. アプリが API 経由で長時間実行アクションを要求します。 API はアクションを承諾し、API URL の Location ヘッダーと共に `202 Accepted` 応答を返して、アクションの状態レポートを取得します。
2. アプリは、アクションの状態レポート URL を要求して、長時間実行アクションの進行状況を含む [AsyncJobStatus](/graph/api/resources/asyncjobstatus?view=graph-rest-beta) 応答を受け取ります。
3. 長時間実行アクションが完了します。 
4. アプリはアクションの状態レポート URL を再度要求して、アクションの完了を示す [AsyncJobStatus](/graph/api/resources/asyncjobstatus?view=graph-rest-beta) 応答を受け取ります。

## <a name="initial-action-request"></a>最初のアクション要求

[DriveItem コピー](/graph/api/driveitem-copy?view=graph-rest-beta) シナリオの例を順を追って説明します。
このシナリオでは、アプリは大量のデータが格納されているフォルダーのコピーを要求します。
この要求は、データが大量であるため完了までに数秒間かかる可能性があります。


# <a name="httptabhttp"></a>[プロトコル](#tab/http)
<!-- { "blockType": "request", "name": "lro-copy-item-example", "scopes": "files.readwrite" } -->

```http
POST https://graph.microsoft.com/beta/me/drive/items/{folder-item-id}/copy
Content-Type: application/json

{
  "parentReference": {
    "path": "/drive/root:/Documents"
  },
  "name": "Copy of LargeFolder1"
}
```
# <a name="ctabcsharp"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/lro-copy-item-example-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/lro-copy-item-example-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[目的-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/lro-copy-item-example-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


API は、アクションが承諾されたことと、長時間実行アクションの状態を取得するための URL を応答で返します。

<!-- { "blockType": "response" } -->

```http
HTTP/1.1 202 Accepted
Location: https://api.onedrive.com/monitor/4A3407B5-88FC-4504-8B21-0AABD3412717
```

**注:** 場所の URL が返されても、Microsoft Graph API エンドポイントにあるとは限りません。

多くの場合、コピー アクションはアプリが追加の作業をすることなく完了するため、これが要求の最後になります。
ただし、アプリでコピー アクションの状態を表示することが必要な場合や、そのアクションがエラーなしで完了したことを確認する場合は、モニター URL を使用できます。

## <a name="retrieve-a-status-report-from-the-monitor-url"></a>モニター URL から状態レポートを取得する

コピー アクションのステータスを確認するために、アプリは前の応答で提供された URL に要求を送信します。 *注:* この要求には、認証は必要ありません。この URL の有効期間は短く、最初の呼び出し元に一意であるためです。 

<!-- { "blockType": "request", "opaqueUrl": true, "name": "lro-check-status", "scopes": "files.readwrite" } -->

```http
GET https://api.onedrive.com/monitor/4A3407B5-88FC-4504-8B21-0AABD3412717
```

サービスは、長時間実行のアクションがまだ進行中であるという情報を含む応答を返します。

<!-- { "blockType": "response", "@odata.type": "microsoft.graph.asyncJobStatus" } -->

```http
HTTP/1.1 202 Accepted
Content-type: application/json

{
  "operation": "ItemCopy",
  "percentageComplete": 27.8,
  "status": "inProgress"
}
```

この情報は、コピー アクションの進行状況に関する最新情報をユーザーに提供するために使用できます。 アプリは、ステータスの最新情報を要求してアクションの進行状況を追跡するために、モニター URL へのポーリングを継続できます。

## <a name="retrieve-a-completed-status-report-from-the-monitor-url"></a>モニター URL から完了状態レポートを取得する

コピー操作が完了してから数秒経過しています。 このときにアプリがモニター URL に要求を送信すると、完了したアクションの結果にリダイレクトする応答が返されます。

<!-- { "blockType": "request", "opaqueUrl": true, "name": "lro-check-status-complete", "scopes": "files.readwrite" } -->

```http
GET https://api.onedrive.com/monitor/4A3407B5-88FC-4504-8B21-0AABD3412717
```

アクションが完了すると、モニター サービスからの応答で、結果の resourceId が返されます。

<!-- { "blockType": "response", "@odata.type": "microsoft.graph.asyncJobStatus" } -->

```http
HTTP/1.1 202 Accepted
Content-type: application/json

{
    "percentageComplete": 100.0,
    "resourceId": "01MOWKYVJML57KN2ANMBA3JZJS2MBGC7KM",
    "status": "completed"
}
```

## <a name="retrieve-the-results-of-the-completed-operation"></a>完了した操作の結果を取得する

ジョブが完了すると、モニター URL が結果の resourceId を返します。ここでは、元のアイテムの新しいコピーを返します。
resourceId を使用してこの新しいアイテムに対処することができます。次に例を示します。


# <a name="httptabhttp"></a>[プロトコル](#tab/http)
<!-- {
  "blockType": "request",
  "name": "lro-copy-item-example-complete",
  "scopes": "files.readwrite"
} -->

```http
GET https://graph.microsoft.com/beta/me/drive/items/{item-id}
```
# <a name="ctabcsharp"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/lro-copy-item-example-complete-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/lro-copy-item-example-complete-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[目的-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/lro-copy-item-example-complete-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<!-- { "blockType": "response", "@odata.type": "microsoft.graph.driveItem", "truncated": true } -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "id": "",
    "name": "Copy of LargeFolder1",
    "folder": { },
    "size": 12019
}
```

## <a name="supported-resources"></a>サポートされているリソース

長時間実行アクションは、次の API メソッドでサポートされています。

| **リソース** | **API** |
|:------ | :------ |
| DriveItem | [コピー](/graph/api/driveitem-copy?view=graph-rest-beta) |

## <a name="prerequisites"></a>前提条件

長時間実行アクションの実行に必要な[アクセス許可](./permissions-reference.md)と同じアクセス許可は、長時間実行アクションの状態をクエリするときにも必要です。




<!-- {
  "type": "#page.annotation",
  "description": "Monitor the progress of long-running actions in the API.",
  "keywords": "monitor,long,running,operation,action",
  "section": "documentation",
  "suppressions": [
    "Error: lro-check-status:
      Unable to locate a definition for resource type: microsoft.graph.asyncJobStatus",
    "Error: lro-check-status-complete:
      Unable to locate a definition for resource type: microsoft.graph.asyncJobStatus"
  ],
  "tocPath": "Concepts/Long running actions"
} -->
