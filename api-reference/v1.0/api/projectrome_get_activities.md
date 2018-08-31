# <a name="get-user-activities"></a><span data-ttu-id="f7fed-101">ユーザー アクティビティを取得する</span><span class="sxs-lookup"><span data-stu-id="f7fed-101">Get user activities</span></span>

<span data-ttu-id="f7fed-102">特定のユーザーの最近のアクティビティを取得します。</span><span class="sxs-lookup"><span data-stu-id="f7fed-102">Get activities for a given user.</span></span> <span data-ttu-id="f7fed-103">**最新の** OData 関数とは異なり、履歴のないアクティビティが返されます。</span><span class="sxs-lookup"><span data-stu-id="f7fed-103">Unlike the **recent** OData function, activities without histories will be returned.</span></span> <span data-ttu-id="f7fed-104">UserActivity.ReadWrite.CreatedByApp アクセス許可も、応答に対し追加のフィルタリングを適用するので、アプリケーションによって作成されたアクティビティのみが返されるようになります。</span><span class="sxs-lookup"><span data-stu-id="f7fed-104">The permission UserActivity.ReadWrite.CreatedByApp will apply extra filtering to the response, so that only activities created by your application are returned.</span></span> <span data-ttu-id="f7fed-105">ユーザーが特にアクティブで、他のアプリケーションが最近より多くのアクティビティを作成した場合、このサーバー側のフィルター処理によって空のページが発生することがあります。</span><span class="sxs-lookup"><span data-stu-id="f7fed-105">This server-side filtering might result in empty pages if the user is particularly active and other applications have created more recent activities.</span></span> <span data-ttu-id="f7fed-106">アプリケーションのアクティビティを取得するには **nextLink** プロパティを使ってページ化します。</span><span class="sxs-lookup"><span data-stu-id="f7fed-106">To get your application's activities, use the **nextLink** property to paginate.</span></span>

## <a name="permissions"></a><span data-ttu-id="f7fed-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="f7fed-107">Permissions</span></span>

<span data-ttu-id="f7fed-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="f7fed-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="f7fed-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="f7fed-110">Permission type</span></span>      | <span data-ttu-id="f7fed-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="f7fed-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f7fed-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="f7fed-112">Delegated (work or school account)</span></span> | <span data-ttu-id="f7fed-113">UserActivity.ReadWrite.CreatedByApp</span><span class="sxs-lookup"><span data-stu-id="f7fed-113">UserActivity.ReadWrite.CreatedByApp</span></span>    |
|<span data-ttu-id="f7fed-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="f7fed-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f7fed-115">UserActivity.ReadWrite.CreatedByApp</span><span class="sxs-lookup"><span data-stu-id="f7fed-115">UserActivity.ReadWrite.CreatedByApp</span></span>    |
|<span data-ttu-id="f7fed-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="f7fed-116">Application</span></span> | <span data-ttu-id="f7fed-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f7fed-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="f7fed-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="f7fed-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /me/activities
```

## <a name="optional-query-parameters"></a><span data-ttu-id="f7fed-119">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="f7fed-119">Optional query parameters</span></span>

<span data-ttu-id="f7fed-120">このメソッドは、応答をカスタマイズするのに役立つ [OData クエリ パラメータ](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) をサポートします。</span><span class="sxs-lookup"><span data-stu-id="f7fed-120">This method supports the [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span> <span data-ttu-id="f7fed-121">次のクエリ パラメータがサポートされています。</span><span class="sxs-lookup"><span data-stu-id="f7fed-121">The following query parameters are supported:</span></span>

- <span data-ttu-id="f7fed-122">**historyItems** のナビゲーション プロパティの $expand。</span><span class="sxs-lookup"><span data-stu-id="f7fed-122">$expand for the **historyItems** navigation property.</span></span>
- <span data-ttu-id="f7fed-123">ページ間での最大項目数を制限する $top。</span><span class="sxs-lookup"><span data-stu-id="f7fed-123">$top to limit the maximum number of items across pages.</span></span>
- <span data-ttu-id="f7fed-124">展開されている場合の activities または historyItems のいずれかの lastModifiedDateTimeプロパティに対する $filter。** ** ** **</span><span class="sxs-lookup"><span data-stu-id="f7fed-124">$filter on the **lastModifiedDateTime** property for either activities or **historyItems**, if expanded.</span></span>

<span data-ttu-id="f7fed-125">URL エンコーディングを使ったサポートされているクエリの例をいくつか下に示します。</span><span class="sxs-lookup"><span data-stu-id="f7fed-125">The following are some examples of supported queries with URL encoding:</span></span>

```
/me/activities?$expand=historyItems($filter=lastModifiedDateTime%20gt%202018-01-22T21:45:00.347Z%20and%20lastModifiedDateTime%20lt%202018-01-22T22:00:00.347Z)

/me/activities?$filter=lastModifiedDateTime%20lt%202018-01-16T01:03:21.347Z%20and%20lastModifiedDateTime%20gt%202018-01-03T01:03:21.347Z

/me/activities?$top=5
```

## <a name="request-headers"></a><span data-ttu-id="f7fed-126">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="f7fed-126">Request headers</span></span>

|<span data-ttu-id="f7fed-127">名前</span><span class="sxs-lookup"><span data-stu-id="f7fed-127">Name</span></span> | <span data-ttu-id="f7fed-128">型</span><span class="sxs-lookup"><span data-stu-id="f7fed-128">Type</span></span> | <span data-ttu-id="f7fed-129">説明</span><span class="sxs-lookup"><span data-stu-id="f7fed-129">Description</span></span>|
|:----|:-----|:-----------|
|<span data-ttu-id="f7fed-130">承認</span><span class="sxs-lookup"><span data-stu-id="f7fed-130">Authorization</span></span> | <span data-ttu-id="f7fed-131">文字列</span><span class="sxs-lookup"><span data-stu-id="f7fed-131">string</span></span> | <span data-ttu-id="f7fed-p104">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="f7fed-p104">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="f7fed-134">要求本文</span><span class="sxs-lookup"><span data-stu-id="f7fed-134">Request body</span></span>

<span data-ttu-id="f7fed-135">要求本文がありません。</span><span class="sxs-lookup"><span data-stu-id="f7fed-135">No request body is required.</span></span>

## <a name="response"></a><span data-ttu-id="f7fed-136">応答</span><span class="sxs-lookup"><span data-stu-id="f7fed-136">Response</span></span>

<span data-ttu-id="f7fed-137">成功すると、このメソッドは、アプリケーションにおけるユーザーの最近のアクティビティを含む `200 OK`  応答コードを返します。</span><span class="sxs-lookup"><span data-stu-id="f7fed-137">If successful, this method returns the `200 OK` response code with the user's activities for your application.</span></span>

## <a name="example"></a><span data-ttu-id="f7fed-138">例</span><span class="sxs-lookup"><span data-stu-id="f7fed-138">Example</span></span>

##### <a name="request"></a><span data-ttu-id="f7fed-139">要求</span><span class="sxs-lookup"><span data-stu-id="f7fed-139">Request</span></span>

<span data-ttu-id="f7fed-140">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="f7fed-140">The following is an example of the request.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_activities"
}-->

```http
GET https://graph.microsoft.com/v1.0/me/activities
```

##### <a name="response"></a><span data-ttu-id="f7fed-141">応答</span><span class="sxs-lookup"><span data-stu-id="f7fed-141">Response</span></span>

<span data-ttu-id="f7fed-142">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="f7fed-142">The following is an example of the response.</span></span>

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
  "description": "Get activities",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
