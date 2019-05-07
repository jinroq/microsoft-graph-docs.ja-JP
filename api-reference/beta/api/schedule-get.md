---
title: スケジュールを取得する
description: '**Schedule**オブジェクトのプロパティとリレーションシップを取得します。'
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 40e796700df1013825ed5267712619ab59803b4d
ms.sourcegitcommit: 3e5f4f515f050e16680ec44f68af40583147af9e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/06/2019
ms.locfileid: "33638999"
---
# <a name="get-schedule"></a>スケジュールを取得する

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[Schedule](../resources/schedule.md)オブジェクトのプロパティとリレーションシップを取得します。

スケジュール作成プロセスは、[リソースベースの長時間実行操作 (RELO) に関する1つの API ガイドライン](https://github.com/Microsoft/api-guidelines/blob/master/Guidelines.md#131-resource-based-long-running-operations-relo)に準拠しています。
クライアントが[PUT メソッド](team-put-schedule.md)を使用すると、スケジュールが準備されている場合、操作によってスケジュールが更新されます。それ以外の場合、操作はバックグラウンドでスケジュールプロビジョニングプロセスを開始します。

スケジュールの準備中に、クライアントは GET メソッドを使用してスケジュールを取得し`provisionStatus` 、プロパティでプロビジョニングの現在の状態を確認できます。 プロビジョニングが失敗した場合、クライアントは`provisionStatusCode`プロパティから追加情報を取得できます。

クライアントは、スケジュールの構成を検査することもできます。

## <a name="permissions"></a>アクセス許可

この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。

|アクセス許可の種類      | アクセス許可 (特権の小さいものから大きいものへ)              |
|:--------------------|:---------------------------------------------------------|
|委任 (職場または学校のアカウント) | Group.Read.All、Group.ReadWrite.All    |
|委任 (個人用 Microsoft アカウント) | サポートされていません。    |
|アプリケーション | サポートされていません。 |

> **注**: この API は、管理者のアクセス許可をサポートします。 グローバル管理者は、所属していないグループにアクセスできます。

## <a name="http-request"></a>HTTP 要求

<!-- { "blockType": "ignored" } -->

```http
GET /teams/{teamId}/schedule
```

## <a name="request-headers"></a>要求ヘッダー

| ヘッダー       | 値 |
|:---------------|:--------|
| Authorization  | ベアラー {トークン}。必須。  |
| Content-Type  | application/json  |

## <a name="request-body"></a>要求本文
このメソッドには、要求本文を指定しません。

## <a name="response"></a>応答

成功した場合、このメソッド`200 OK`は応答コードと、応答本文で[schedule](../resources/schedule.md)オブジェクトを返します。

## <a name="example"></a>例

#### <a name="request"></a>要求

要求の例を次に示します。
<!-- {
  "blockType": "request",
  "name": "schedule-get"
}-->
```http
GET https://graph.microsoft.com/beta/teams/{teamId}/schedule
```

#### <a name="response"></a>応答

応答の例を次に示します。 

>**注:** 読みやすくするために、ここに示す応答オブジェクトは短くされている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.schedule"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 401

{
  "id": "833fc4df-c88b-4398-992f-d8afcfe41df2",
  "enabled": true,
  "timeZone": "America/Chicago",
  "provisionStatus": "Completed",
  "provisionStatusCode": null
}
```
#### <a name="sdk-sample-code"></a>SDK サンプルコード
# <a name="ctabcs"></a>[Visual](#tab/cs)
[!INCLUDE [sample-code](../includes/schedule-get-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[Java](#tab/javascript)
[!INCLUDE [sample-code](../includes/schedule-get-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get the schedule",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/schedule-get.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/schedule-get.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
