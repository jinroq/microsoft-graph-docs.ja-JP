---
title: アクティビティを作成または置換する
description: アプリの既存のユーザーアクティビティを新規作成するか、置き換えます。 ユーザーアクティビティとそれに関連する**履歴項目**を1つの要求で作成する場合は、deep insert を使用できます。
localization_priority: Normal
ms.prod: project-rome
ms.openlocfilehash: 497b0e0bf4e236065dc6b44c44e80d99b22a5dc4
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33337284"
---
# <a name="create-or-replace-an-activity"></a><span data-ttu-id="a429a-104">アクティビティを作成または置換する</span><span class="sxs-lookup"><span data-stu-id="a429a-104">Create or replace an activity</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a429a-105">アプリの既存のユーザーアクティビティを新規作成するか、置き換えます。</span><span class="sxs-lookup"><span data-stu-id="a429a-105">Create a new or replace an existing user activity for your app.</span></span> <span data-ttu-id="a429a-106">ユーザーアクティビティとそれに関連する**履歴項目**を1つの要求で作成する場合は、 [deep insert](#example-2-deep-insert)を使用できます。</span><span class="sxs-lookup"><span data-stu-id="a429a-106">If you'd like to create a user activity and its related **historyItems** in one request, you can use [deep insert](#example-2-deep-insert).</span></span>

## <a name="permissions"></a><span data-ttu-id="a429a-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="a429a-107">Permissions</span></span>

<span data-ttu-id="a429a-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="a429a-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="a429a-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="a429a-110">Permission type</span></span>                        | <span data-ttu-id="a429a-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="a429a-111">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:------------------------------------|
| <span data-ttu-id="a429a-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="a429a-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="a429a-113">UserActivity.ReadWrite.CreatedByApp</span><span class="sxs-lookup"><span data-stu-id="a429a-113">UserActivity.ReadWrite.CreatedByApp</span></span> |
| <span data-ttu-id="a429a-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="a429a-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a429a-115">UserActivity.ReadWrite.CreatedByApp</span><span class="sxs-lookup"><span data-stu-id="a429a-115">UserActivity.ReadWrite.CreatedByApp</span></span> |
| <span data-ttu-id="a429a-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="a429a-116">Application</span></span>                            | <span data-ttu-id="a429a-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a429a-117">Not supported.</span></span>                      |

## <a name="http-request"></a><span data-ttu-id="a429a-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="a429a-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PUT /me/activities/{appActivityId}
```

> <span data-ttu-id="a429a-119">**注:** url の appactivityid は、url セーフである必要があります (RFC 2396 の予約されていない文字を除くすべての文字を16進表記に変換する必要があります) が、元の appactivityid を url セーフにする必要はありません。</span><span class="sxs-lookup"><span data-stu-id="a429a-119">**Note:** The appActivityId in the URL needs to be URL-safe (all characters except for RFC 2396 unreserved characters must be converted to their hexadecimal representation), but the original appActivityId does not have to be URL-safe.</span></span>

## <a name="request-headers"></a><span data-ttu-id="a429a-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="a429a-120">Request headers</span></span>

| <span data-ttu-id="a429a-121">名前</span><span class="sxs-lookup"><span data-stu-id="a429a-121">Name</span></span>          | <span data-ttu-id="a429a-122">型</span><span class="sxs-lookup"><span data-stu-id="a429a-122">Type</span></span>   | <span data-ttu-id="a429a-123">説明</span><span class="sxs-lookup"><span data-stu-id="a429a-123">Description</span></span>               |
|:--------------|:-------|:--------------------------|
| <span data-ttu-id="a429a-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="a429a-124">Authorization</span></span> | <span data-ttu-id="a429a-125">string</span><span class="sxs-lookup"><span data-stu-id="a429a-125">string</span></span> | <span data-ttu-id="a429a-p104">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="a429a-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="a429a-128">要求本文</span><span class="sxs-lookup"><span data-stu-id="a429a-128">Request body</span></span>

<span data-ttu-id="a429a-129">要求本文で、 [activity](../resources/projectrome-activity.md)オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="a429a-129">In the request body, supply a JSON representation of an [activity](../resources/projectrome-activity.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="a429a-130">応答</span><span class="sxs-lookup"><span data-stu-id="a429a-130">Response</span></span>

<span data-ttu-id="a429a-131">成功した場合、このメソッド`201 Created`は、アクティビティが作成された`200 OK`場合、またはアクティビティが置き換えられた場合に、応答コードを返します。</span><span class="sxs-lookup"><span data-stu-id="a429a-131">If successful, this method returns the `201 Created` response code if the activity was created or `200 OK` if the activity was replaced.</span></span>

## <a name="examples"></a><span data-ttu-id="a429a-132">例</span><span class="sxs-lookup"><span data-stu-id="a429a-132">Examples</span></span>

### <a name="example-1-create-an-activity"></a><span data-ttu-id="a429a-133">例 1: アクティビティを作成する</span><span class="sxs-lookup"><span data-stu-id="a429a-133">Example 1: Create an activity</span></span>

#### <a name="request"></a><span data-ttu-id="a429a-134">要求</span><span class="sxs-lookup"><span data-stu-id="a429a-134">Request</span></span>

<span data-ttu-id="a429a-135">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="a429a-135">The following is an example of the request.</span></span>

<!-- {
    "blockType": "ignored",
    "name": "upsert_activity"
} -->

```http
PUT https://graph.microsoft.com/beta/me/activities/%2Farticle%3F12345
Content-type: application/json

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
      "body": [
        {
          "type": "TextBlock",
          "text": "Contoso MainPage"
        }
      ]
    }
  }
}
```

<!-- markdownlint-disable MD024 -->

#### <a name="response"></a><span data-ttu-id="a429a-136">応答</span><span class="sxs-lookup"><span data-stu-id="a429a-136">Response</span></span>

<span data-ttu-id="a429a-137">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="a429a-137">The following is an example of the response.</span></span>

<!-- {
    "blockType": "ignored",
    "truncated": true,
    "@odata.type": "microsoft.graph.activity"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "activitySourceHost": "https://contoso.com",
  "createdDateTime": "2017-06-09T20:54:43.969Z",
  "lastModifiedDateTime": "2017-06-09T20:54:43.969Z",
  "id": "14332800362997268276",
  "appActivityId": "/article?12345",
  "status": "updated",
  "expirationDateTime": "2017-02-26T20:20:48.114Z",
  "visualElements": {
    "displayText": "Contoso How-To: How to Tie a Reef Knot",
    "description": "How to Tie a Reef Knot. A step-by-step visual guide to the art of nautical knot-tying.",
    "attribution": {
      "iconUrl": "https://www.contoso.com/icon",
      "alternateText": "Contoso, Ltd.",
      "addImageQuery": "false"
    },
    "backgroundColor": "#ff0000",
    "content": {
      "$schema": "https://adaptivecards.io/schemas/adaptive-card.json",
      "type": "AdaptiveCard",
      "body": [
        {
          "type": "TextBlock",
          "text": "Contoso MainPage"
        }
      ]
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
  }
}
```

### <a name="example-2-deep-insert"></a><span data-ttu-id="a429a-138">例 2: Deep insert</span><span class="sxs-lookup"><span data-stu-id="a429a-138">Example 2: Deep insert</span></span>

<span data-ttu-id="a429a-139">この例では、1つの要求で、そのアクティビティの新しいアクティビティと履歴アイテムを作成します。</span><span class="sxs-lookup"><span data-stu-id="a429a-139">This example creates a new activity and a history item for that activity in one request.</span></span>

#### <a name="request"></a><span data-ttu-id="a429a-140">要求</span><span class="sxs-lookup"><span data-stu-id="a429a-140">Request</span></span>

<span data-ttu-id="a429a-141">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="a429a-141">The following is an example of the request.</span></span>

<!-- {
    "blockType": "ignored",
    "name": "upsert_activity"
} -->

```http
PUT https://graph.microsoft.com/beta/me/activities/%2Farticle%3F12345
Content-type: application/json

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
      "body": [
        {
          "type": "TextBlock",
          "text": "Contoso MainPage"
        }
      ]
    }
  },
  "historyItems": [
    {
      "userTimezone": "Africa/Casablanca",
      "startedDateTime": "2018-02-26T20:54:04.345Z",
      "lastActiveDateTime": "2018-02-26T20:54:24.345Z"
    }
  ]
}
```

#### <a name="response"></a><span data-ttu-id="a429a-142">応答</span><span class="sxs-lookup"><span data-stu-id="a429a-142">Response</span></span>

<span data-ttu-id="a429a-143">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="a429a-143">The following is an example of the response.</span></span>

<!-- {
    "blockType": "ignored",
    "truncated": true,
    "@odata.type": "microsoft.graph.activity"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "activitySourceHost": "https://contoso.com",
  "createdDateTime": "2017-06-09T20:54:43.969Z",
  "lastModifiedDateTime": "2017-06-09T20:54:43.969Z",
  "id": "14332800362997268276",
  "appActivityId": "/article?12345",
  "status": "updated",
  "expirationDateTime": "2017-02-26T20:20:48.114Z",
  "visualElements": {
    "displayText": "Contoso How-To: How to Tie a Reef Knot",
    "description": "How to Tie a Reef Knot. A step-by-step visual guide to the art of nautical knot-tying.",
    "attribution": {
      "iconUrl": "https://www.contoso.com/icon",
      "alternateText": "Contoso, Ltd.",
      "addImageQuery": "false"
    },
    "backgroundColor": "#ff0000",
    "content": {
      "$schema": "https://adaptivecards.io/schemas/adaptive-card.json",
      "type": "AdaptiveCard",
      "body": [
        {
          "type": "TextBlock",
          "text": "Contoso MainPage"
        }
      ]
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
  "historyItems": [
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
<!--
{
  "type": "#page.annotation",
  "description": "Upsert activity",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
