---
title: アクティビティを作成または置換する
description: 新規作成またはアプリケーションが既存のユーザー アクティビティを交換します。 1 つの要求でユーザーの利用状況とその関連する**historyItems**を作成したい場合は、深い挿入を使用できます。
localization_priority: Normal
ms.prod: project-rome
ms.openlocfilehash: eca8e03e45a5a2d4ae6c4c08218189edcf98a03a
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27944748"
---
# <a name="create-or-replace-an-activity"></a><span data-ttu-id="156fe-104">アクティビティを作成または置換する</span><span class="sxs-lookup"><span data-stu-id="156fe-104">Create or replace an activity</span></span>

> <span data-ttu-id="156fe-105">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="156fe-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="156fe-106">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="156fe-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="156fe-107">新規作成またはアプリケーションが既存のユーザー アクティビティを交換します。</span><span class="sxs-lookup"><span data-stu-id="156fe-107">Create a new or replace an existing user activity for your app.</span></span> <span data-ttu-id="156fe-108">1 つの要求でユーザーの利用状況とその関連する**historyItems**を作成したい場合は、[深い挿入](projectrome-put-activity.md#example-2---deep-insert)を使用できます。</span><span class="sxs-lookup"><span data-stu-id="156fe-108">If you'd like to create a user activity and its related **historyItems** in one request, you can use [deep insert](projectrome-put-activity.md#example-2---deep-insert).</span></span>

## <a name="permissions"></a><span data-ttu-id="156fe-109">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="156fe-109">Permissions</span></span>

<span data-ttu-id="156fe-p104">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="156fe-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="156fe-112">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="156fe-112">Permission type</span></span>      | <span data-ttu-id="156fe-113">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="156fe-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="156fe-114">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="156fe-114">Delegated (work or school account)</span></span> | <span data-ttu-id="156fe-115">UserActivity.ReadWrite.CreatedByApp</span><span class="sxs-lookup"><span data-stu-id="156fe-115">UserActivity.ReadWrite.CreatedByApp</span></span>    |
|<span data-ttu-id="156fe-116">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="156fe-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="156fe-117">UserActivity.ReadWrite.CreatedByApp</span><span class="sxs-lookup"><span data-stu-id="156fe-117">UserActivity.ReadWrite.CreatedByApp</span></span>    |
|<span data-ttu-id="156fe-118">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="156fe-118">Application</span></span> | <span data-ttu-id="156fe-119">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="156fe-119">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="156fe-120">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="156fe-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PUT /me/activities/{appActivityId}
```

><span data-ttu-id="156fe-121">**注:** URL に appActivityId を (RFC 2396 の予約文字は、16 進表現に変換する必要がありますを除くすべての文字) を URL セーフである必要がありますが、元の appActivityId は、URL セーフである必要はありません。</span><span class="sxs-lookup"><span data-stu-id="156fe-121">**Note:** The appActivityId in the URL needs to be URL-safe (all characters except for RFC 2396 unreserved characters must be converted to their hexadecimal representation), but the original appActivityId does not have to be URL-safe.</span></span>

## <a name="request-headers"></a><span data-ttu-id="156fe-122">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="156fe-122">Request headers</span></span>

|<span data-ttu-id="156fe-123">名前</span><span class="sxs-lookup"><span data-stu-id="156fe-123">Name</span></span> | <span data-ttu-id="156fe-124">型</span><span class="sxs-lookup"><span data-stu-id="156fe-124">Type</span></span> | <span data-ttu-id="156fe-125">説明</span><span class="sxs-lookup"><span data-stu-id="156fe-125">Description</span></span>|
|:----|:-----|:-----------|
|<span data-ttu-id="156fe-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="156fe-126">Authorization</span></span> | <span data-ttu-id="156fe-127">string</span><span class="sxs-lookup"><span data-stu-id="156fe-127">string</span></span> | <span data-ttu-id="156fe-p105">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="156fe-p105">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="156fe-130">要求本文</span><span class="sxs-lookup"><span data-stu-id="156fe-130">Request body</span></span>

<span data-ttu-id="156fe-131">要求の本文には、[アクティビティ](../resources/projectrome-activity.md)オブジェクトの JSON の形式を指定します。</span><span class="sxs-lookup"><span data-stu-id="156fe-131">In the request body, supply a JSON representation of an [activity](../resources/projectrome-activity.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="156fe-132">応答</span><span class="sxs-lookup"><span data-stu-id="156fe-132">Response</span></span>

<span data-ttu-id="156fe-133">かどうかは成功すると、このメソッドが返されます、 `201 Created` 、活動が作成された場合の応答コードまたは`200 OK`アクティビティが表示された場合。</span><span class="sxs-lookup"><span data-stu-id="156fe-133">If successful, this method returns the `201 Created` response code if the activity was created or `200 OK` if the activity was replaced.</span></span>

## <a name="example-1"></a><span data-ttu-id="156fe-134">例 1</span><span class="sxs-lookup"><span data-stu-id="156fe-134">Example 1</span></span>

#### <a name="request"></a><span data-ttu-id="156fe-135">要求</span><span class="sxs-lookup"><span data-stu-id="156fe-135">Request</span></span>

<span data-ttu-id="156fe-136">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="156fe-136">The following is an example of the request.</span></span>

<!-- {
    "blockType": "ignored",
    "name": "upsert_activity"
} -->

```http
PUT https://graph.microsoft.com/beta/me/activities/%2Farticle%3F12345
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
            "addImageQuery": "false"
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

#### <a name="response"></a><span data-ttu-id="156fe-137">応答</span><span class="sxs-lookup"><span data-stu-id="156fe-137">Response</span></span>

<span data-ttu-id="156fe-138">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="156fe-138">The following is an example of the response.</span></span>

<!-- {
    "blockType": "ignored",
    "truncated": true,
    "@odata.type": "microsoft.graph.activity"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Location: https://graph.microsoft.com/beta/me/activities/14332800362997268276

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

## <a name="example-2---deep-insert"></a><span data-ttu-id="156fe-139">例 2 - ディープ挿入</span><span class="sxs-lookup"><span data-stu-id="156fe-139">Example 2 - Deep insert</span></span>

#### <a name="request"></a><span data-ttu-id="156fe-140">要求</span><span class="sxs-lookup"><span data-stu-id="156fe-140">Request</span></span>

<span data-ttu-id="156fe-141">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="156fe-141">The following is an example of the request.</span></span>

<!-- {
    "blockType": "ignored",
    "name": "upsert_activity"
} -->

```http
PUT https://graph.microsoft.com/beta/me/activities/%2Farticle%3F12345
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
            "addImageQuery": "false",
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

#### <a name="response"></a><span data-ttu-id="156fe-142">応答</span><span class="sxs-lookup"><span data-stu-id="156fe-142">Response</span></span>

<span data-ttu-id="156fe-143">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="156fe-143">The following is an example of the response.</span></span>

<!-- {
    "blockType": "ignored",
    "truncated": true,
    "@odata.type": "microsoft.graph.activity"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Location: https://graph.microsoft.com/beta/me/activities/14332800362997268276

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
