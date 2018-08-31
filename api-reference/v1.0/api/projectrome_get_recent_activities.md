# <a name="get-recent-user-activities"></a><span data-ttu-id="75bb8-101">最近のユーザーのアクティビティを取得する</span><span class="sxs-lookup"><span data-stu-id="75bb8-101">Get recent activities</span></span>

<span data-ttu-id="75bb8-102">特定のユーザーの最近のアクティビティを取得します。</span><span class="sxs-lookup"><span data-stu-id="75bb8-102">Get recent activities for a given user.</span></span> <span data-ttu-id="75bb8-103">この OData 関数には、「直近に使用された」API のように動作させるためのいくつかの既定の動作が含まれています。</span><span class="sxs-lookup"><span data-stu-id="75bb8-103">This OData function has some default behaviors included to make it operate like a "most recently used" API.</span></span> <span data-ttu-id="75bb8-104">このサービスは、直近の [historyItems](../resources/projectrome_historyitem.md) のクエリを実行し、関連するアクティビティを引き出します。</span><span class="sxs-lookup"><span data-stu-id="75bb8-104">The service will query for the most recent [historyItems](../resources/projectrome_historyitem.md), and then pull those related activities.</span></span> <span data-ttu-id="75bb8-105">アクティビティは、 **historyItem** で、直近の **lastModified** に従って並べ替えられます。</span><span class="sxs-lookup"><span data-stu-id="75bb8-105">Activities will be sorted according to the most recent **lastModified** on the **historyItem**.</span></span> <span data-ttu-id="75bb8-106">これは、**historyItems** のないアクティビティは応答に含まれないことを意味します。</span><span class="sxs-lookup"><span data-stu-id="75bb8-106">This means that activities without **historyItems** will not be included in the response.</span></span> <span data-ttu-id="75bb8-107">UserActivity.ReadWrite.CreatedByApp アクセス許可も、応答に対し追加のフィルタリングを適用するので、アプリケーションによって作成されたアクティビティのみが返されるようになります。</span><span class="sxs-lookup"><span data-stu-id="75bb8-107">The UserActivity.ReadWrite.CreatedByApp permission will also apply extra filtering to the response, so that only activities created by your application are returned.</span></span> <span data-ttu-id="75bb8-108">ユーザーが特にアクティブで、他のアプリケーションが最近より多くのアクティビティを作成した場合、このサーバー側のフィルター処理によって空のページが発生することがあります。</span><span class="sxs-lookup"><span data-stu-id="75bb8-108">This server-side filtering might result in empty pages if the user is particularly active and other applications have created more recent activities.</span></span> <span data-ttu-id="75bb8-109">アプリケーションのアクティビティを取得するには **nextLink** プロパティを使ってページ割りをします。</span><span class="sxs-lookup"><span data-stu-id="75bb8-109">To get your application's activities, use the **nextLink** property to paginate.</span></span>

## <a name="permissions"></a><span data-ttu-id="75bb8-110">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="75bb8-110">Permissions</span></span>

<span data-ttu-id="75bb8-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="75bb8-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="75bb8-113">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="75bb8-113">Permission type</span></span>      | <span data-ttu-id="75bb8-114">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="75bb8-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="75bb8-115">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="75bb8-115">Delegated (work or school account)</span></span> | <span data-ttu-id="75bb8-116">UserActivity.ReadWrite.CreatedByApp</span><span class="sxs-lookup"><span data-stu-id="75bb8-116">UserActivity.ReadWrite.CreatedByApp</span></span>    |
|<span data-ttu-id="75bb8-117">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="75bb8-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="75bb8-118">UserActivity.ReadWrite.CreatedByApp</span><span class="sxs-lookup"><span data-stu-id="75bb8-118">UserActivity.ReadWrite.CreatedByApp</span></span>    |
|<span data-ttu-id="75bb8-119">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="75bb8-119">Application</span></span> | <span data-ttu-id="75bb8-120">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="75bb8-120">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="75bb8-121">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="75bb8-121">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /me/activities/recent
```

## <a name="optional-query-parameters"></a><span data-ttu-id="75bb8-122">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="75bb8-122">Optional query parameters</span></span>

<span data-ttu-id="75bb8-123">このメソッドは、応答をカスタマイズするのに役立つ [OData クエリ パラメータ](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) をサポートします。</span><span class="sxs-lookup"><span data-stu-id="75bb8-123">This method supports the [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span> <span data-ttu-id="75bb8-124">次のクエリ パラメータがサポートされています。</span><span class="sxs-lookup"><span data-stu-id="75bb8-124">The following query parameters are supported:</span></span>

- <span data-ttu-id="75bb8-125">**historyItems** のナビゲーション プロパティの $expand。</span><span class="sxs-lookup"><span data-stu-id="75bb8-125">$expand for the **historyItems** navigation property.</span></span>
- <span data-ttu-id="75bb8-126">ページ間での最大項目数を制限する $top。</span><span class="sxs-lookup"><span data-stu-id="75bb8-126">$top to limit the maximum number of items across pages.</span></span>
- <span data-ttu-id="75bb8-127">展開されている場合の **activities** または **historyItems** のいずれかの **lastModifiedDateTime**プロパティに対する $filter。</span><span class="sxs-lookup"><span data-stu-id="75bb8-127">$filter on the **lastModifiedDateTime** property for either **activities** or **historyItems**, if expanded.</span></span>

<span data-ttu-id="75bb8-128">URL エンコーディングを使ったサポートされているクエリの例をいくつか下に示します。</span><span class="sxs-lookup"><span data-stu-id="75bb8-128">The following are some examples of supported queries with URL encoding.</span></span>

```
/me/activities/recent?$expand=historyItems($filter=lastModifiedDateTime%20gt%202018-01-22T21:45:00.347Z%20and%20lastModifiedDateTime%20lt%202018-01-22T22:00:00.347Z)

/me/activities/recent?$filter=lastModifiedDateTime%20lt%202018-01-16T01:03:21.347Z%20and%20lastModifiedDateTime%20gt%202018-01-03T01:03:21.347Z

/me/activities/recent?$top=5
```

## <a name="request-headers"></a><span data-ttu-id="75bb8-129">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="75bb8-129">Request headers</span></span>

|<span data-ttu-id="75bb8-130">名前</span><span class="sxs-lookup"><span data-stu-id="75bb8-130">Name</span></span> | <span data-ttu-id="75bb8-131">型</span><span class="sxs-lookup"><span data-stu-id="75bb8-131">Type</span></span> | <span data-ttu-id="75bb8-132">説明</span><span class="sxs-lookup"><span data-stu-id="75bb8-132">Description</span></span>|
|:----|:-----|:-----------|
|<span data-ttu-id="75bb8-133">承認</span><span class="sxs-lookup"><span data-stu-id="75bb8-133">Authorization</span></span> | <span data-ttu-id="75bb8-134">文字列</span><span class="sxs-lookup"><span data-stu-id="75bb8-134">string</span></span> | <span data-ttu-id="75bb8-p104">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="75bb8-p104">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="75bb8-137">要求本文</span><span class="sxs-lookup"><span data-stu-id="75bb8-137">Request body</span></span>

<span data-ttu-id="75bb8-138">要求本文を指定しないでください。</span><span class="sxs-lookup"><span data-stu-id="75bb8-138">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="75bb8-139">応答</span><span class="sxs-lookup"><span data-stu-id="75bb8-139">Response</span></span>

<span data-ttu-id="75bb8-140">|||UNTRANSLATED_CONTENT_START|||If successful, this method returns the `200 OK` response code with the user's recent activities for your application.|||UNTRANSLATED_CONTENT_END|||</span><span class="sxs-lookup"><span data-stu-id="75bb8-140">If successful, this method returns the `200 OK` response code with the user's recent activities for your application.</span></span>

## <a name="example"></a><span data-ttu-id="75bb8-141">例</span><span class="sxs-lookup"><span data-stu-id="75bb8-141">Example</span></span>

##### <a name="request"></a><span data-ttu-id="75bb8-142">要求</span><span class="sxs-lookup"><span data-stu-id="75bb8-142">Request</span></span>

<span data-ttu-id="75bb8-143">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="75bb8-143">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_recent_activities"
}-->

```http
GET https://graph.microsoft.com/v1.0/me/activities/recent
```

##### <a name="response"></a><span data-ttu-id="75bb8-144">応答</span><span class="sxs-lookup"><span data-stu-id="75bb8-144">Response</span></span>

<span data-ttu-id="75bb8-145">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="75bb8-145">The following is an example of the response.</span></span>

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
