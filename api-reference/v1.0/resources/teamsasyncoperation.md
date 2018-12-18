---
title: teamsAsyncOperation リソースの種類
description: 'マイクロソフト チームの非同期操作は、操作を 1 つの API 要求の有効期間を超えてしまうことです。 '
author: nkramer
ms.openlocfilehash: fd64f99c20505a8e670c865faa039e9db3174ed6
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27320609"
---
# <a name="teamsasyncoperation-resource-type"></a>teamsAsyncOperation リソースの種類



マイクロソフト チームの非同期操作は、操作を 1 つの API 要求の有効期間を超えてしまうことです。 これらの操作は、実行時間の長い、または、最初の要求の時間枠で完了するのにはコストが高すぎます。

非同期操作が開始されると、メソッドは、202 の承諾済みの応答コードを返します。 応答は、teamsAsyncOperation の場所を含む場所のヘッダーも格納されます。 この場所に GET 要求を行うことによって、オペレーションのステータスを定期的にチェックします。待機 > 30 秒間隔でチェックします。
要求が正常に完了したら、状態は、"成功し、targetResourceLocation が作成/変更したリソースを指します。

## <a name="properties"></a>Properties

| プロパティ | 種類   | 説明 |
|:---------------|:--------|:----------|
|ID|string |操作の一意の id です。|
|入力|[teamsAsyncOperationType](teamsasyncoperationtype.md) |説明している操作の種類を表します。|
|createdDateTime|DateTimeOffset |操作が作成された時刻。|
|status|[teamsAsyncOperationStatus](teamsasyncoperationstatus.md)| 操作の状態です。|
|lastActionDateTime|DateTimeOffset |非同期操作が最後に更新された時間です。|
|attemptsCount|Int32|成功または失敗にマークされる前に操作が試行された回数です。|
|targetResourceId|guid |作成または[チーム](../resources/team.md)では通常、この非同期操作を受けて変更されたオブジェクトの ID です。|
|targetResourceLocation|string|作成または、この非同期操作を受けて変更されたオブジェクトの位置。 この URL は非透過値として扱われます、そのコンポーネントのパスには解析されませんする必要があります。|
|エラー|[operationError](operationerror.md)|非同期操作が失敗の原因となるすべてのエラーです。|

## <a name="json-representation"></a>JSON 表記

リソースの JSON 表記を次に示します。

<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.teamsasyncoperation"
}-->

```json
{
    "id": "string",
    "operationType": "archiveTeam",
    "createdDateTime": "2018-01-01T00:00:00.0000000Z",
    "status": "succeeded",
    "lastActionDateTime": "2018-01-01T00:00:00.0000000Z",
    "attemptsCount": 1,
    "targetResourceId": "fa4aa5a2-a75b-4769-86f4-9e2742a18fda",
    "targetResourceLocation": "/groups('fa4aa5a2-a75b-4769-86f4-9e2742a18fda')/team",
    "error": null
}
```

<!-- uuid: 20fd7863-9545-40d4-ae8f-fee2d115a690
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "teams async operation resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
