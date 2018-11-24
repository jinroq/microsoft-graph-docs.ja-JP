# <a name="get-recent-user-activities"></a><span data-ttu-id="3a560-101">ユーザーの最近の活動を取得します。</span><span class="sxs-lookup"><span data-stu-id="3a560-101">Get recent user activities</span></span>

<span data-ttu-id="3a560-102">特定のユーザーの最近の活動を取得します。</span><span class="sxs-lookup"><span data-stu-id="3a560-102">Get recent activities for a given user.</span></span> <span data-ttu-id="3a560-103">この OData の関数では、「最近使用した」の API と同様に動作して含まれているいくつか既定動作があります。</span><span class="sxs-lookup"><span data-stu-id="3a560-103">This OData function has some default behaviors included to make it operate like a "most recently used" API.</span></span> <span data-ttu-id="3a560-104">サービスは、最新の[historyItems](../resources/projectrome_historyitem.md)のクエリを実行し、それらの関連の活動を引き出します。</span><span class="sxs-lookup"><span data-stu-id="3a560-104">The service will query for the most recent [historyItems](../resources/projectrome_historyitem.md), and then pull those related activities.</span></span> <span data-ttu-id="3a560-105">アクティビティは、 **historyItem**で、最新の**lastModified**に従って並べ替えられます。</span><span class="sxs-lookup"><span data-stu-id="3a560-105">Activities will be sorted according to the most recent **lastModified** on the **historyItem**.</span></span> <span data-ttu-id="3a560-106">これは、なしで**historyItems**が応答に含まれないことを意味します。</span><span class="sxs-lookup"><span data-stu-id="3a560-106">This means that activities without **historyItems** will not be included in the response.</span></span> <span data-ttu-id="3a560-107">UserActivity.ReadWrite.CreatedByApp アクセス許可も適用されます応答に追加のフィルタ リング、アプリケーションによって作成された活動のみが返されるようにします。</span><span class="sxs-lookup"><span data-stu-id="3a560-107">The UserActivity.ReadWrite.CreatedByApp permission will also apply extra filtering to the response, so that only activities created by your application are returned.</span></span> <span data-ttu-id="3a560-108">このサーバー側のフィルター処理が発生空のページでユーザーが特に作業中であり、他のアプリケーションが最新の活動を作成します。</span><span class="sxs-lookup"><span data-stu-id="3a560-108">This server-side filtering might result in empty pages if the user is particularly active and other applications have created more recent activities.</span></span> <span data-ttu-id="3a560-109">アプリケーションのアクティビティを取得するには、改ページ調整**nextLink**プロパティを使用します。</span><span class="sxs-lookup"><span data-stu-id="3a560-109">To get your application's activities, use the **nextLink** property to paginate.</span></span>

## <a name="permissions"></a><span data-ttu-id="3a560-110">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="3a560-110">Permissions</span></span>

<span data-ttu-id="3a560-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="3a560-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="3a560-113">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="3a560-113">Permission type</span></span>      | <span data-ttu-id="3a560-114">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="3a560-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3a560-115">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="3a560-115">Delegated (work or school account)</span></span> | <span data-ttu-id="3a560-116">UserActivity.ReadWrite.CreatedByApp</span><span class="sxs-lookup"><span data-stu-id="3a560-116">UserActivity.ReadWrite.CreatedByApp</span></span>    |
|<span data-ttu-id="3a560-117">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="3a560-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3a560-118">UserActivity.ReadWrite.CreatedByApp</span><span class="sxs-lookup"><span data-stu-id="3a560-118">UserActivity.ReadWrite.CreatedByApp</span></span>    |
|<span data-ttu-id="3a560-119">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="3a560-119">Application</span></span> | <span data-ttu-id="3a560-120">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="3a560-120">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="3a560-121">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="3a560-121">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /me/activities/recent
```

## <a name="optional-query-parameters"></a><span data-ttu-id="3a560-122">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="3a560-122">Optional query parameters</span></span>

<span data-ttu-id="3a560-123">このメソッドは、応答をカスタマイズするためにいくつかの[OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="3a560-123">This method supports some [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span> <span data-ttu-id="3a560-124">次のクエリ パラメーターがサポートされています。</span><span class="sxs-lookup"><span data-stu-id="3a560-124">The following query parameters are supported:</span></span>

- <span data-ttu-id="3a560-125">$ は、 **historyItems**のナビゲーション プロパティを展開します。</span><span class="sxs-lookup"><span data-stu-id="3a560-125">$expand for the **historyItems** navigation property.</span></span>
- <span data-ttu-id="3a560-126">ページ間でのアイテムの最大数を制限する $top。</span><span class="sxs-lookup"><span data-stu-id="3a560-126">$top to limit the maximum number of items across pages.</span></span>
- <span data-ttu-id="3a560-127">**アクティビティ**または**historyItems**、展開されている場合のいずれかの**lastModifiedDateTime**プロパティで $filter。</span><span class="sxs-lookup"><span data-stu-id="3a560-127">$filter on the **lastModifiedDateTime** property for either **activities** or **historyItems**, if expanded.</span></span>

<span data-ttu-id="3a560-128">URL エンコーディングを使用してクエリがサポートされているいくつかの例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="3a560-128">The following are some examples of supported queries with URL encoding.</span></span>

```
/me/activities/recent?$expand=historyItems($filter=lastModifiedDateTime%20gt%202018-01-22T21:45:00.347Z%20and%20lastModifiedDateTime%20lt%202018-01-22T22:00:00.347Z)

/me/activities/recent?$filter=lastModifiedDateTime%20lt%202018-01-16T01:03:21.347Z%20and%20lastModifiedDateTime%20gt%202018-01-03T01:03:21.347Z

/me/activities/recent?$top=5
```

## <a name="request-headers"></a><span data-ttu-id="3a560-129">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="3a560-129">Request headers</span></span>

|<span data-ttu-id="3a560-130">名前</span><span class="sxs-lookup"><span data-stu-id="3a560-130">Name</span></span> | <span data-ttu-id="3a560-131">型</span><span class="sxs-lookup"><span data-stu-id="3a560-131">Type</span></span> | <span data-ttu-id="3a560-132">説明</span><span class="sxs-lookup"><span data-stu-id="3a560-132">Description</span></span>|
|:----|:-----|:-----------|
|<span data-ttu-id="3a560-133">Authorization</span><span class="sxs-lookup"><span data-stu-id="3a560-133">Authorization</span></span> | <span data-ttu-id="3a560-134">string</span><span class="sxs-lookup"><span data-stu-id="3a560-134">string</span></span> | <span data-ttu-id="3a560-p104">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="3a560-p104">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="3a560-137">要求本文</span><span class="sxs-lookup"><span data-stu-id="3a560-137">Request body</span></span>

<span data-ttu-id="3a560-138">要求の本体を指定することはしません。</span><span class="sxs-lookup"><span data-stu-id="3a560-138">Do not specify a request body.</span></span>

## <a name="response"></a><span data-ttu-id="3a560-139">応答</span><span class="sxs-lookup"><span data-stu-id="3a560-139">Response</span></span>

<span data-ttu-id="3a560-140">かどうかは成功すると、このメソッドが返されます、 `200 OK` 、アプリケーションのユーザーの最近の活動を使用して応答コード。</span><span class="sxs-lookup"><span data-stu-id="3a560-140">If successful, this method returns the `200 OK` response code with the user's recent activities for your application.</span></span>

## <a name="example"></a><span data-ttu-id="3a560-141">例</span><span class="sxs-lookup"><span data-stu-id="3a560-141">Example</span></span>

##### <a name="request"></a><span data-ttu-id="3a560-142">要求</span><span class="sxs-lookup"><span data-stu-id="3a560-142">Request</span></span>

<span data-ttu-id="3a560-143">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="3a560-143">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_recent_activities"
}-->

```http
GET https://graph.microsoft.com/v1.0/me/activities/recent
```

##### <a name="response"></a><span data-ttu-id="3a560-144">応答</span><span class="sxs-lookup"><span data-stu-id="3a560-144">Response</span></span>

<span data-ttu-id="3a560-145">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="3a560-145">The following is an example of the response.</span></span>

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

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2017-06-07 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get recent activities",
  "keywords": "",
  "section": "documentation",
  "suppressions": [
    "Error: get_recent_activities/container/contentInfo:
      Property 'contentInfo' is of type Custom but has no custom members.",

    "Warning: get_recent_activities/container/visualElements:
      Schema validation failed on property 'visualElements' ['microsoft.graph.visualInfo']",

    "Warning: get_recent_activities/container/visualElements/content:
      Schema validation failed on property 'content' ['microsoft.graph.Json']",

    "Warning: get_recent_activities/container/visualElements/content/$schema:
      Undocumented property '$schema' [String] was not expected on resource microsoft.graph.Json.",

    "Warning: get_recent_activities/container/visualElements/content/body:
      Undocumented property 'body' [Collection(Object)] was not expected on resource microsoft.graph.Json.",

    "Warning: get_recent_activities/container/visualElements/content/type:
      Undocumented property 'type' [String] was not expected on resource microsoft.graph.Json."

  ],
  "tocPath": ""
}-->
