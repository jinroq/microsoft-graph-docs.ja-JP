# <a name="create-or-replace-an-activity"></a><span data-ttu-id="52d14-101">アクティビティを作成または置換する</span><span class="sxs-lookup"><span data-stu-id="52d14-101">Create or replace an activity</span></span>

<span data-ttu-id="52d14-102">新規作成またはアプリケーションが既存のユーザー アクティビティを交換します。</span><span class="sxs-lookup"><span data-stu-id="52d14-102">Create a new or replace an existing user activity for your app.</span></span> <span data-ttu-id="52d14-103">1 つの要求でユーザーの利用状況とその関連する**historyItems**を作成したい場合は、[深い挿入](projectrome_put_activity.md#example-2---deep-insert)を使用できます。</span><span class="sxs-lookup"><span data-stu-id="52d14-103">If you'd like to create a user activity and its related **historyItems** in one request, you can use [deep insert](projectrome_put_activity.md#example-2---deep-insert).</span></span>

## <a name="permissions"></a><span data-ttu-id="52d14-104">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="52d14-104">Permissions</span></span>

<span data-ttu-id="52d14-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="52d14-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>


|<span data-ttu-id="52d14-107">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="52d14-107">Permission type</span></span>      | <span data-ttu-id="52d14-108">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="52d14-108">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="52d14-109">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="52d14-109">Delegated (work or school account)</span></span> | <span data-ttu-id="52d14-110">UserActivity.ReadWrite.CreatedByApp</span><span class="sxs-lookup"><span data-stu-id="52d14-110">UserActivity.ReadWrite.CreatedByApp</span></span>    |
|<span data-ttu-id="52d14-111">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="52d14-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="52d14-112">UserActivity.ReadWrite.CreatedByApp</span><span class="sxs-lookup"><span data-stu-id="52d14-112">UserActivity.ReadWrite.CreatedByApp</span></span>    |
|<span data-ttu-id="52d14-113">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="52d14-113">Application</span></span> | <span data-ttu-id="52d14-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="52d14-114">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="52d14-115">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="52d14-115">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PUT /me/activities/{appActivityId}
```

><span data-ttu-id="52d14-116">**注:** URL に appActivityId を (RFC 2396 の予約文字は、16 進表現に変換する必要がありますを除くすべての文字) を URL セーフである必要がありますが、元の appActivityId は、URL セーフである必要はありません。</span><span class="sxs-lookup"><span data-stu-id="52d14-116">**Note:** The appActivityId in the URL needs to be URL-safe (all characters except for RFC 2396 unreserved characters must be converted to their hexadecimal representation), but the original appActivityId does not have to be URL-safe.</span></span>

## <a name="request-headers"></a><span data-ttu-id="52d14-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="52d14-117">Request headers</span></span>

|<span data-ttu-id="52d14-118">名前</span><span class="sxs-lookup"><span data-stu-id="52d14-118">Name</span></span> | <span data-ttu-id="52d14-119">型</span><span class="sxs-lookup"><span data-stu-id="52d14-119">Type</span></span> | <span data-ttu-id="52d14-120">説明</span><span class="sxs-lookup"><span data-stu-id="52d14-120">Description</span></span>|
|:----|:-----|:-----------|
|<span data-ttu-id="52d14-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="52d14-121">Authorization</span></span> | <span data-ttu-id="52d14-122">string</span><span class="sxs-lookup"><span data-stu-id="52d14-122">string</span></span> | <span data-ttu-id="52d14-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="52d14-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="52d14-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="52d14-125">Request body</span></span>

<span data-ttu-id="52d14-126">要求の本文には、[アクティビティ](../resources/projectrome_activity.md)オブジェクトの JSON の形式を指定します。</span><span class="sxs-lookup"><span data-stu-id="52d14-126">In the request body, supply a JSON representation of an [activity](../resources/projectrome_activity.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="52d14-127">応答</span><span class="sxs-lookup"><span data-stu-id="52d14-127">Response</span></span>

<span data-ttu-id="52d14-128">かどうかは成功すると、このメソッドが返されます、 `201 Created` 、活動が作成された場合の応答コードまたは`200 OK`アクティビティが表示された場合。</span><span class="sxs-lookup"><span data-stu-id="52d14-128">If successful, this method returns the `201 Created` response code if the activity was created or `200 OK` if the activity was replaced.</span></span>

## <a name="example-1"></a><span data-ttu-id="52d14-129">例 1</span><span class="sxs-lookup"><span data-stu-id="52d14-129">Example 1</span></span>

#### <a name="request"></a><span data-ttu-id="52d14-130">要求</span><span class="sxs-lookup"><span data-stu-id="52d14-130">Request</span></span>

<span data-ttu-id="52d14-131">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="52d14-131">The following is an example of the request.</span></span>

<!-- {
    "blockType": "ignored",
    "name": "upsert_activity"
} -->

```http
PUT https://graph.microsoft.com/v1.0/me/activities/%2Farticle%3F12345
Content-type: application/json
Content-length: 364

{
    "appActivityId": "/article?12345",
    "activitySourceHost": "https://www.contoso.com",
    "userTimezone": "Africa/Casablanca",
    "appDisplayName": "Contoso, Ltd.",
    "activationUrl": "https://www.contoso.com/article?id=12345",
    "contentUrl": "https://www.contoso.com/article?id=12345",
    "fallbackUrl": "https://www.contoso.com/article?id=12345",
    "contentInfo": {
        "@context": "https://schema.org",
        "@type": "Article",
        "author": "Jennifer Booth",
        "name": "How to Tie a Reef Knot"
    },
    "visualElements": {
        "attribution": {
            "iconUrl": "https://www.contoso.com/icon",
            "alternateText": "Contoso, Ltd.",
            "addImageQuery": false,
        },
        "description": "How to Tie a Reef Knot. A step-by-step visual guide to the art of nautical knot-tying.",
        "backgroundColor": "#ff0000",
        "displayText": "Contoso How-To: How to Tie a Reef Knot",
        "content": {
            "$schema": "https://adaptivecards.io/schemas/adaptive-card.json",
            "type": "AdaptiveCard",
            "body":
            [{
                "type": "TextBlock",
                "text": "Contoso MainPage"
            }]
        }
    }
}
```

#### <a name="response"></a><span data-ttu-id="52d14-132">応答</span><span class="sxs-lookup"><span data-stu-id="52d14-132">Response</span></span>

<span data-ttu-id="52d14-133">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="52d14-133">The following is an example of the response.</span></span>

<!-- {
    "blockType": "ignored",
    "truncated": true,
    "@odata.type": "microsoft.graph.userActivity"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Location: https://graph.microsoft.com/v1.0/me/activities/14332800362997268276

{
    "activitySourceHost": "https://contoso.com",
    "createdDateTime": "2017-06-09T20:54:43.969Z",
    "lastModifiedDateTime": "2017-06-09T20:54:43.969Z",
    "id": "14332800362997268276",
    "appActivityId": "/article?12345",
    "status":"updated",
    "expirationDateTime": "2017-02-26T20:20:48.114Z",
    "id": "14332800362997268276",
    "visualElements": {
        "displayText": "Contoso How-To: How to Tie a Reef Knot",
        "description": "How to Tie a Reef Knot. A step-by-step visual guide to the art of nautical knot-tying.",
        "attribution": {
            "iconUrl": "https://www.contoso.com/icon",
            "alternateText": "Contoso, Ltd.",
            "addImageQuery": false
        },
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
        "author": "Jennifer Booth",
        "name": "How to Tie a Reef Knot"
    },
}
```

## <a name="example-2---deep-insert"></a><span data-ttu-id="52d14-134">例 2 - ディープ挿入</span><span class="sxs-lookup"><span data-stu-id="52d14-134">Example 2 - Deep insert</span></span>

#### <a name="request"></a><span data-ttu-id="52d14-135">要求</span><span class="sxs-lookup"><span data-stu-id="52d14-135">Request</span></span>

<span data-ttu-id="52d14-136">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="52d14-136">The following is an example of the request.</span></span>

<!-- {
    "blockType": "ignored",
    "name": "upsert_activity"
} -->

```http
PUT https://graph.microsoft.com/v1.0/me/activities/%2Farticle%3F12345
Content-type: application/json
Content-length: 364

{
    "appActivityId": "/article?12345",
    "activitySourceHost": "https://www.contoso.com",
    "userTimezone": "Africa/Casablanca",
    "appDisplayName": "Contoso, Ltd.",
    "activationUrl": "https://www.contoso.com/article?id=12345",
    "contentUrl": "https://www.contoso.com/article?id=12345",
    "fallbackUrl": "https://www.contoso.com/article?id=12345",
    "contentInfo": {
        "@context": "https://schema.org",
        "@type": "Article",
        "author": "Jennifer Booth",
        "name": "How to Tie a Reef Knot"
    },
    "visualElements": {
        "attribution": {
            "iconUrl": "https://www.contoso.com/icon",
            "alternateText": "Contoso, Ltd.",
            "addImageQuery": false,
        },
        "description": "How to Tie a Reef Knot. A step-by-step visual guide to the art of nautical knot-tying.",
        "backgroundColor": "#ff0000",
        "displayText": "Contoso How-To: How to Tie a Reef Knot",
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
    "historyItems":[
        {
            "userTimezone": "Africa/Casablanca",
            "startedDateTime": "2018-02-26T20:54:04.345Z",
            "lastActiveDateTime": "2018-02-26T20:54:24.345Z",
        }
    ]
}
```

#### <a name="response"></a><span data-ttu-id="52d14-137">応答</span><span class="sxs-lookup"><span data-stu-id="52d14-137">Response</span></span>

<span data-ttu-id="52d14-138">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="52d14-138">The following is an example of the response.</span></span>

<!-- {
    "blockType": "ignored",
    "truncated": true,
    "@odata.type": "microsoft.graph.userActivity"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Location: https://graph.microsoft.com/v1.0/me/activities/14332800362997268276

{
    "activitySourceHost": "https://contoso.com",
    "createdDateTime": "2017-06-09T20:54:43.969Z",
    "lastModifiedDateTime": "2017-06-09T20:54:43.969Z",
    "id": "14332800362997268276",
    "appActivityId": "/article?12345",
    "status":"updated",
    "expirationDateTime": "2017-02-26T20:20:48.114Z",
    "id": "14332800362997268276",
    "visualElements": {
        "displayText": "Contoso How-To: How to Tie a Reef Knot",
        "description": "How to Tie a Reef Knot. A step-by-step visual guide to the art of nautical knot-tying.",
        "attribution": {
            "iconUrl": "https://www.contoso.com/icon",
            "alternateText": "Contoso, Ltd.",
            "addImageQuery": false
        },
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
        "author": "Jennifer Booth",
        "name": "How to Tie a Reef Knot"
    },
    "historyItems":[
        {
            "status": "updated",
            "userTimezone": "Africa/Casablanca",
            "createdDateTime": "2018-04-12T21:42:42.495Z",
            "lastModifiedDateTime": "2018-04-12T21:42:42.495Z",
            "id": "61fc8f36-919f-4b73-89d4-1cb7b159d912",
            "startedDateTime": "2018-02-26T20:54:04.345Z",
            "lastActiveDateTime": "2018-02-26T20:54:24.345Z",
            "expirationDateTime": "2018-05-12T21:42:42.495Z",
            "activeDurationSeconds": 20
        }
    ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2017-06-07 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Upsert activity",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
