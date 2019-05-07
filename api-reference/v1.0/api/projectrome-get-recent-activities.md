---
title: 最近のユーザーアクティビティを取得する
description: " トレース. サービスは最新の履歴項目を照会してから、関連するアクティビティを抽出します。 アクティビティは、**履歴アイテム**の最新の**lastModified**に従って並べ替えられます。 これは、**履歴アイテム**のないアクティビティは応答に含まれないことを意味します。 また、アプリケーションによって作成されたアクティビティのみが返されるように、アプリのアクセス許可は、応答に特別なフィルター処理も適用します。 このサーバー側のフィルタリングは、ユーザーが特にアクティブで、その他のアプリケーションがより新しいアクティビティを作成した場合に、空のページになる可能性があります。 アプリケーションのアクティビティを取得するには、 **Nextlink**プロパティを使用して改ページにします。"
localization_priority: Normal
ms.prod: project-rome
ms.openlocfilehash: 709723dfb728c169c8b596675dc26308dd60dac5
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/06/2019
ms.locfileid: "33608393"
---
# <a name="get-recent-user-activities"></a>最近のユーザーアクティビティを取得する

特定のユーザーの最近のアクティビティを取得します。 この OData 関数には、"最近使用された" API のように動作するようにするための既定の動作がいくつか含まれています。 サービスは最新の[履歴項目](../resources/projectrome-historyitem.md)を照会してから、関連するアクティビティを抽出します。 アクティビティは、**履歴アイテム**の最新の**lastModified**に従って並べ替えられます。 これは、**履歴アイテム**のないアクティビティは応答に含まれないことを意味します。 また、アプリケーションによって作成されたアクティビティのみが返されるように、アプリのアクセス許可は、応答に特別なフィルター処理も適用します。 このサーバー側のフィルタリングは、ユーザーが特にアクティブで、その他のアプリケーションがより新しいアクティビティを作成した場合に、空のページになる可能性があります。 アプリケーションのアクティビティを取得するには、 **Nextlink**プロパティを使用して改ページにします。

## <a name="permissions"></a>アクセス許可

この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。

|アクセス許可の種類      | アクセス許可 (特権の小さいものから大きいものへ)              |
|:--------------------|:---------------------------------------------------------|
|委任 (職場または学校のアカウント) | UserActivity.ReadWrite.CreatedByApp    |
|委任 (個人用 Microsoft アカウント) | UserActivity.ReadWrite.CreatedByApp    |
|アプリケーション | サポートされていません。 |

## <a name="http-request"></a>HTTP 要求

<!-- { "blockType": "ignored" } -->

```http
GET /me/activities/recent
```

## <a name="optional-query-parameters"></a>オプションのクエリ パラメーター

このメソッドは、応答をカスタマイズするための[OData クエリパラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。 次のクエリパラメーターがサポートされています。

- **履歴項目**ナビゲーションプロパティの $expand。
- ページ間でのアイテムの最大数を制限する $top。
- **lastModifiedDateTime**プロパティを使用して、**アクティビティ**または**履歴アイテム**(展開されている場合) のどちらかを $filter します。

次に、URL エンコードでサポートされているクエリの例をいくつか示します。

```
/me/activities/recent?$expand=historyItems($filter=lastModifiedDateTime%20gt%202018-01-22T21:45:00.347Z%20and%20lastModifiedDateTime%20lt%202018-01-22T22:00:00.347Z)

/me/activities/recent?$filter=lastModifiedDateTime%20lt%202018-01-16T01:03:21.347Z%20and%20lastModifiedDateTime%20gt%202018-01-03T01:03:21.347Z

/me/activities/recent?$top=5
```

## <a name="request-headers"></a>要求ヘッダー

|名前 | 型 | 説明|
|:----|:-----|:-----------|
|Authorization | string | ベアラー {トークン}。必須。|

## <a name="request-body"></a>要求本文

要求本文を指定しません。

## <a name="response"></a>応答

成功した場合、このメソッド`200 OK`は、アプリケーションのユーザーの最近のアクティビティで応答コードを返します。

## <a name="example"></a>例

##### <a name="request"></a>要求

要求の例を次に示します。

<!-- {
  "blockType": "request",
  "name": "get_recent_activities"
}-->

```http
GET https://graph.microsoft.com/v1.0/me/activities/recent
```

##### <a name="response"></a>応答

応答の例を次に示します。

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.userActivity)"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#Collection(userActivity)",
    "@odata.nextLink": "https://graph.microsoft.com/v1.0/me/activities/recent?$skiptoken=%24filter%3dlastModifiedDateTime+lt+2018-02-26T18%3a06%3a19.365Z",
    "value": [{
        "@odata.type": "#microsoft.graph.userActivity",
        "activitySourceHost": "https://www.contoso.com",
        "createdDateTime": "2018-02-26T18:34:29.592Z",
        "lastModifiedDateTime": "2018-02-26T18:34:29.607Z",
        "id": "5347642601316252694",
        "appActivityId": "/article?12345",
        "visualElements": {
            "attribution": {
              "iconUrl": "https://www.contoso.com/icon",
              "alternateText": "Contoso, Ltd.",
              "addImageQuery": false,
              },
            "displayText": "Contoso How-To: How to Tie a Reef Knot",
            "description": "How to Tie a Reef Knot. A step-by-step visual guide to the art of nautical knot-tying.",
            "backgroundColor": "#ff0000",
            "content": {
              "$schema": "https://adaptivecards.io/schemas/adaptive-card.json",
              "type": "AdaptiveCard",
              "body":
              [{
                  "type": "TextBlock",
                  "text": "Contoso MainPage"
              }]
            }
        },
        "activationUrl": "https://www.contoso.com/article?id=12345",
        "appDisplayName": "Contoso, Ltd.",
        "userTimezone": "Africa/Casablanca",
        "fallbackUrl": "https://www.contoso.com/article?id=12345",
        "contentUrl": "https://www.contoso.com/article?id=12345",
        "contentInfo": {
            "@context": "https://schema.org",
            "@type": "Article",
            "author": "John Doe",
            "name": "How to Tie a Reef Knot"
        },
        "expirationDateTime": "2018-03-28T18:34:29.607Z",
        "status": "updated"
    }]
}
```
#### <a name="sdk-sample-code"></a>SDK サンプルコード
# <a name="ctabcs"></a>[Visual](#tab/cs)
[!INCLUDE [sample-code](../includes/get_recent_activities-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[Java](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_recent_activities-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2017-06-07 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get recent activities",
  "keywords": "",
  "section": "documentation",
  "suppressions": [
    "Error: /api-reference/v1.0/api/projectrome-get-recent-activities.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/projectrome-get-recent-activities.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)",
    "Error: get_recent_activities/container/contentInfo:
      Property 'contentInfo' is of type Custom but has no custom members.",

    "Warning: get_recent_activities/container/visualElements/content/$schema:
      Undocumented property '$schema' [String] was not expected on resource microsoft.graph.Json.",

    "Warning: get_recent_activities/container/visualElements/content/body:
      Undocumented property 'body' [Collection(Object)] was not expected on resource microsoft.graph.Json.",

    "Warning: get_recent_activities/container/visualElements/content/type:
      Undocumented property 'type' [String] was not expected on resource microsoft.graph.Json."

  ],
  "tocPath": ""
}-->
