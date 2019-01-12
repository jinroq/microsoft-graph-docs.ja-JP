---
title: アクティビティを作成または置換する
description: 新規作成またはアプリケーションが既存のユーザー アクティビティを交換します。 1 つの要求でユーザーの利用状況とその関連する**historyItems**を作成したい場合は、深い挿入を使用できます。
localization_priority: Normal
ms.prod: project-rome
ms.openlocfilehash: 1e5a7956ab5ac151613ac3559415b16570a2b087
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27966686"
---
# <a name="create-or-replace-an-activity"></a><span data-ttu-id="1c600-104">アクティビティを作成または置換する</span><span class="sxs-lookup"><span data-stu-id="1c600-104">Create or replace an activity</span></span>

<span data-ttu-id="1c600-105">新規作成またはアプリケーションが既存のユーザー アクティビティを交換します。</span><span class="sxs-lookup"><span data-stu-id="1c600-105">Create a new or replace an existing user activity for your app.</span></span> <span data-ttu-id="1c600-106">1 つの要求でユーザーの利用状況とその関連する**historyItems**を作成したい場合は、[深い挿入](projectrome-put-activity.md#example-2---deep-insert)を使用できます。</span><span class="sxs-lookup"><span data-stu-id="1c600-106">If you'd like to create a user activity and its related **historyItems** in one request, you can use [deep insert](projectrome-put-activity.md#example-2---deep-insert).</span></span>

## <a name="permissions"></a><span data-ttu-id="1c600-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="1c600-107">Permissions</span></span>

<span data-ttu-id="1c600-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="1c600-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="1c600-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="1c600-110">Permission type</span></span>      | <span data-ttu-id="1c600-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="1c600-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1c600-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="1c600-112">Delegated (work or school account)</span></span> | <span data-ttu-id="1c600-113">UserActivity.ReadWrite.CreatedByApp</span><span class="sxs-lookup"><span data-stu-id="1c600-113">UserActivity.ReadWrite.CreatedByApp</span></span>    |
|<span data-ttu-id="1c600-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="1c600-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1c600-115">UserActivity.ReadWrite.CreatedByApp</span><span class="sxs-lookup"><span data-stu-id="1c600-115">UserActivity.ReadWrite.CreatedByApp</span></span>    |
|<span data-ttu-id="1c600-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="1c600-116">Application</span></span> | <span data-ttu-id="1c600-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="1c600-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="1c600-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="1c600-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PUT /me/activities/{appActivityId}
```

><span data-ttu-id="1c600-119">**注:** URL に appActivityId を (RFC 2396 の予約文字は、16 進表現に変換する必要がありますを除くすべての文字) を URL セーフである必要がありますが、元の appActivityId は、URL セーフである必要はありません。</span><span class="sxs-lookup"><span data-stu-id="1c600-119">**Note:** The appActivityId in the URL needs to be URL-safe (all characters except for RFC 2396 unreserved characters must be converted to their hexadecimal representation), but the original appActivityId does not have to be URL-safe.</span></span>

## <a name="request-headers"></a><span data-ttu-id="1c600-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="1c600-120">Request headers</span></span>

|<span data-ttu-id="1c600-121">名前</span><span class="sxs-lookup"><span data-stu-id="1c600-121">Name</span></span> | <span data-ttu-id="1c600-122">種類</span><span class="sxs-lookup"><span data-stu-id="1c600-122">Type</span></span> | <span data-ttu-id="1c600-123">説明</span><span class="sxs-lookup"><span data-stu-id="1c600-123">Description</span></span>|
|:----|:-----|:-----------|
|<span data-ttu-id="1c600-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="1c600-124">Authorization</span></span> | <span data-ttu-id="1c600-125">string</span><span class="sxs-lookup"><span data-stu-id="1c600-125">string</span></span> | <span data-ttu-id="1c600-p104">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="1c600-p104">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="1c600-128">要求本文</span><span class="sxs-lookup"><span data-stu-id="1c600-128">Request body</span></span>

<span data-ttu-id="1c600-129">要求の本文には、[アクティビティ](../resources/projectrome-activity.md)オブジェクトの JSON の形式を指定します。</span><span class="sxs-lookup"><span data-stu-id="1c600-129">In the request body, supply a JSON representation of an [activity](../resources/projectrome-activity.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="1c600-130">応答</span><span class="sxs-lookup"><span data-stu-id="1c600-130">Response</span></span>

<span data-ttu-id="1c600-131">かどうかは成功すると、このメソッドが返されます、 `201 Created` 、活動が作成された場合の応答コードまたは`200 OK`アクティビティが表示された場合。</span><span class="sxs-lookup"><span data-stu-id="1c600-131">If successful, this method returns the `201 Created` response code if the activity was created or `200 OK` if the activity was replaced.</span></span>

## <a name="example-1"></a><span data-ttu-id="1c600-132">例 1</span><span class="sxs-lookup"><span data-stu-id="1c600-132">Example 1</span></span>

#### <a name="request"></a><span data-ttu-id="1c600-133">要求</span><span class="sxs-lookup"><span data-stu-id="1c600-133">Request</span></span>

<span data-ttu-id="1c600-134">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="1c600-134">The following is an example of the request.</span></span>

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

#### <a name="response"></a><span data-ttu-id="1c600-135">応答</span><span class="sxs-lookup"><span data-stu-id="1c600-135">Response</span></span>

<span data-ttu-id="1c600-136">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="1c600-136">The following is an example of the response.</span></span>

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

## <a name="example-2---deep-insert"></a><span data-ttu-id="1c600-137">例 2 - ディープ挿入</span><span class="sxs-lookup"><span data-stu-id="1c600-137">Example 2 - Deep insert</span></span>

#### <a name="request"></a><span data-ttu-id="1c600-138">要求</span><span class="sxs-lookup"><span data-stu-id="1c600-138">Request</span></span>

<span data-ttu-id="1c600-139">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="1c600-139">The following is an example of the request.</span></span>

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

#### <a name="response"></a><span data-ttu-id="1c600-140">応答</span><span class="sxs-lookup"><span data-stu-id="1c600-140">Response</span></span>

<span data-ttu-id="1c600-141">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="1c600-141">The following is an example of the response.</span></span>

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
