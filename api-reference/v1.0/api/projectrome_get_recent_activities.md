# <a name="get-recent-user-activities"></a>最近のユーザーのアクティビティを取得する

特定のユーザーの最近のアクティビティを取得します。 この OData 関数には、「直近に使用された」API のように動作させるためのいくつかの既定の動作が含まれています。 このサービスは、直近の [historyItems](../resources/projectrome_historyitem.md) のクエリを実行し、関連するアクティビティを引き出します。 アクティビティは、 **historyItem** で、直近の **lastModified** に従って並べ替えられます。 これは、**historyItems** のないアクティビティは応答に含まれないことを意味します。 UserActivity.ReadWrite.CreatedByApp アクセス許可も、応答に対し追加のフィルタリングを適用するので、アプリケーションによって作成されたアクティビティのみが返されるようになります。 ユーザーが特にアクティブで、他のアプリケーションが最近より多くのアクティビティを作成した場合、このサーバー側のフィルター処理によって空のページが発生することがあります。 アプリケーションのアクティビティを取得するには **nextLink** プロパティを使ってページ割りをします。

## <a name="permissions"></a>アクセス許可

この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。

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

このメソッドは、応答をカスタマイズするのに役立つ [OData クエリ パラメータ](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) をサポートします。 次のクエリ パラメータがサポートされています。

- **historyItems** のナビゲーション プロパティの $expand。
- ページ間での最大項目数を制限する $top。
- 展開されている場合の **activities** または **historyItems** のいずれかの **lastModifiedDateTime**プロパティに対する $filter。

URL エンコーディングを使ったサポートされているクエリの例をいくつか下に示します。

```
/me/activities/recent?$expand=historyItems($filter=lastModifiedDateTime%20gt%202018-01-22T21:45:00.347Z%20and%20lastModifiedDateTime%20lt%202018-01-22T22:00:00.347Z)

/me/activities/recent?$filter=lastModifiedDateTime%20lt%202018-01-16T01:03:21.347Z%20and%20lastModifiedDateTime%20gt%202018-01-03T01:03:21.347Z

/me/activities/recent?$top=5
```

## <a name="request-headers"></a>要求ヘッダー

|名前 | 型 | 説明|
|:----|:-----|:-----------|
|承認 | 文字列 | ベアラー {トークン}。必須。|

## <a name="request-body"></a>要求本文

要求本文を指定しないでください。

## <a name="response"></a>応答

|||UNTRANSLATED_CONTENT_START|||If successful, this method returns the `200 OK` response code with the user's recent activities for your application.|||UNTRANSLATED_CONTENT_END|||

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
              "iconUrl": "http://www.contoso.com/icon",
              "alternateText": "Contoso, Ltd.",
              "addImageQuery": false,
              },
            "displayText": "Contoso How-To: How to Tie a Reef Knot",
            "description": "How to Tie a Reef Knot. A step-by-step visual guide to the art of nautical knot-tying.",
            "backgroundColor": "#ff0000",
            "content": {
              "$schema": "http://adaptivecards.io/schemas/adaptive-card.json",
              "type": "AdaptiveCard",
              "body":
              [{
                  "type": "TextBlock",
                  "text": "Contoso MainPage"
              }]
            }
        },
        "activationUrl": "http://www.contoso.com/article?id=12345",
        "appDisplayName": "Contoso, Ltd.",
        "userTimezone": "Africa/Casablanca",
        "fallbackUrl": "http://www.contoso.com/article?id=12345",
        "contentUrl": "http://www.contoso.com/article?id=12345",
        "contentInfo": {
            "@context": "http://schema.org",
            "@type": "Article",
            "author": "John Doe",
            "name": "How to Tie a Reef Knot"
        },
        "expirationDateTime": "2018-03-28T18:34:29.607Z",
        "status": "updated"
    }]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2017-06-07 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get recent activities",
  "keywords": "",
  "section": "documentation",
  "suppressions": [
    "Error: get_recent_activities/container/contentInfo:
      Property 'contentInfo' is of type Custom but has no custom members."
  ],
  "tocPath": ""
}-->
