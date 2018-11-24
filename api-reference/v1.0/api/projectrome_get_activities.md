# <a name="get-user-activities"></a><span data-ttu-id="72727-101">ユーザー ・ アクティビティを取得します。</span><span class="sxs-lookup"><span data-stu-id="72727-101">Get user activities</span></span>

<span data-ttu-id="72727-102">特定のユーザーのアクティビティを取得します。</span><span class="sxs-lookup"><span data-stu-id="72727-102">Get activities for a given user.</span></span> <span data-ttu-id="72727-103">異なり、**最近使用した**OData 機能、履歴のない活動が返されます。</span><span class="sxs-lookup"><span data-stu-id="72727-103">Unlike the **recent** OData function, activities without histories will be returned.</span></span> <span data-ttu-id="72727-104">アクセス許可 UserActivity.ReadWrite.CreatedByApp はフィルターを適用余分な応答に、アプリケーションによって作成された活動のみが返されるようにします。</span><span class="sxs-lookup"><span data-stu-id="72727-104">The permission UserActivity.ReadWrite.CreatedByApp will apply extra filtering to the response, so that only activities created by your application are returned.</span></span> <span data-ttu-id="72727-105">このサーバー側のフィルター処理が発生空のページでユーザーが特に作業中であり、他のアプリケーションが最新の活動を作成します。</span><span class="sxs-lookup"><span data-stu-id="72727-105">This server-side filtering might result in empty pages if the user is particularly active and other applications have created more recent activities.</span></span> <span data-ttu-id="72727-106">アプリケーションのアクティビティを取得するには、改ページ調整**nextLink**プロパティを使用します。</span><span class="sxs-lookup"><span data-stu-id="72727-106">To get your application's activities, use the **nextLink** property to paginate.</span></span>

## <a name="permissions"></a><span data-ttu-id="72727-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="72727-107">Permissions</span></span>

<span data-ttu-id="72727-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="72727-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="72727-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="72727-110">Permission type</span></span>      | <span data-ttu-id="72727-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="72727-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="72727-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="72727-112">Delegated (work or school account)</span></span> | <span data-ttu-id="72727-113">UserActivity.ReadWrite.CreatedByApp</span><span class="sxs-lookup"><span data-stu-id="72727-113">UserActivity.ReadWrite.CreatedByApp</span></span>    |
|<span data-ttu-id="72727-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="72727-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="72727-115">UserActivity.ReadWrite.CreatedByApp</span><span class="sxs-lookup"><span data-stu-id="72727-115">UserActivity.ReadWrite.CreatedByApp</span></span>    |
|<span data-ttu-id="72727-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="72727-116">Application</span></span> | <span data-ttu-id="72727-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="72727-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="72727-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="72727-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /me/activities
```

## <a name="optional-query-parameters"></a><span data-ttu-id="72727-119">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="72727-119">Optional query parameters</span></span>

<span data-ttu-id="72727-120">このメソッドは、応答をカスタマイズするためにいくつかの[OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="72727-120">This method supports some [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span> <span data-ttu-id="72727-121">次のクエリ パラメーターがサポートされています。</span><span class="sxs-lookup"><span data-stu-id="72727-121">The following query parameters are supported:</span></span>

- <span data-ttu-id="72727-122">$ は、 **historyItems**のナビゲーション プロパティを展開します。</span><span class="sxs-lookup"><span data-stu-id="72727-122">$expand for the **historyItems** navigation property.</span></span>
- <span data-ttu-id="72727-123">ページ間でのアイテムの最大数を制限する $top。</span><span class="sxs-lookup"><span data-stu-id="72727-123">$top to limit the maximum number of items across pages.</span></span>
- <span data-ttu-id="72727-124">アクティビティまたは**historyItems**、展開されている場合のいずれかの**lastModifiedDateTime**プロパティで $filter。</span><span class="sxs-lookup"><span data-stu-id="72727-124">$filter on the **lastModifiedDateTime** property for either activities or **historyItems**, if expanded.</span></span>

<span data-ttu-id="72727-125">次に、URL エンコードがサポートされているクエリの例を示します。</span><span class="sxs-lookup"><span data-stu-id="72727-125">The following are some examples of supported queries with URL encoding:</span></span>

```
/me/activities?$expand=historyItems($filter=lastModifiedDateTime%20gt%202018-01-22T21:45:00.347Z%20and%20lastModifiedDateTime%20lt%202018-01-22T22:00:00.347Z)

/me/activities?$filter=lastModifiedDateTime%20lt%202018-01-16T01:03:21.347Z%20and%20lastModifiedDateTime%20gt%202018-01-03T01:03:21.347Z

/me/activities?$top=5
```

## <a name="request-headers"></a><span data-ttu-id="72727-126">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="72727-126">Request headers</span></span>

|<span data-ttu-id="72727-127">名前</span><span class="sxs-lookup"><span data-stu-id="72727-127">Name</span></span> | <span data-ttu-id="72727-128">型</span><span class="sxs-lookup"><span data-stu-id="72727-128">Type</span></span> | <span data-ttu-id="72727-129">説明</span><span class="sxs-lookup"><span data-stu-id="72727-129">Description</span></span>|
|:----|:-----|:-----------|
|<span data-ttu-id="72727-130">Authorization</span><span class="sxs-lookup"><span data-stu-id="72727-130">Authorization</span></span> | <span data-ttu-id="72727-131">string</span><span class="sxs-lookup"><span data-stu-id="72727-131">string</span></span> | <span data-ttu-id="72727-p104">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="72727-p104">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="72727-134">要求本文</span><span class="sxs-lookup"><span data-stu-id="72727-134">Request body</span></span>

<span data-ttu-id="72727-135">要求の本体がありません。</span><span class="sxs-lookup"><span data-stu-id="72727-135">No request body.</span></span>

## <a name="response"></a><span data-ttu-id="72727-136">応答</span><span class="sxs-lookup"><span data-stu-id="72727-136">Response</span></span>

<span data-ttu-id="72727-137">かどうかは成功すると、このメソッドが返されます、 `200 OK` 、アプリケーションのユーザーのアクティビティに応答コード。</span><span class="sxs-lookup"><span data-stu-id="72727-137">If successful, this method returns the `200 OK` response code with the user's activities for your application.</span></span>

## <a name="example"></a><span data-ttu-id="72727-138">例</span><span class="sxs-lookup"><span data-stu-id="72727-138">Example</span></span>

##### <a name="request"></a><span data-ttu-id="72727-139">要求</span><span class="sxs-lookup"><span data-stu-id="72727-139">Request</span></span>

<span data-ttu-id="72727-140">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="72727-140">The following is an example of the request.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_activities"
}-->

```http
GET https://graph.microsoft.com/v1.0/me/activities
```

##### <a name="response"></a><span data-ttu-id="72727-141">応答</span><span class="sxs-lookup"><span data-stu-id="72727-141">Response</span></span>

<span data-ttu-id="72727-142">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="72727-142">The following is an example of the response.</span></span>

<!-- {
  "blockType": "ignored",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.activity)"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#Collection(userActivity)",
    "@odata.nextLink": "https://graph.microsoft.com/v1.0/me/activities?$skiptoken=%24filter%3dlastModifiedDateTime+lt+2018-02-26T18%3a06%3a19.365Z",
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

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2017-06-07 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get activities",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
