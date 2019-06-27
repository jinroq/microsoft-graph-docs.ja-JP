---
title: TimeOffReason の作成
description: 新しい timeOffReason を作成します。
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 93d05e3b402fc9e6e67d2c5d4e77b2ab707767b0
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/27/2019
ms.locfileid: "35264926"
---
# <a name="create-timeoffreason"></a><span data-ttu-id="df68d-103">TimeOffReason の作成</span><span class="sxs-lookup"><span data-stu-id="df68d-103">Create timeOffReason</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="df68d-104">新しい[Timeoffreason](../resources/timeoffreason.md)を作成します。</span><span class="sxs-lookup"><span data-stu-id="df68d-104">Create a new [timeOffReason](../resources/timeoffreason.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="df68d-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="df68d-105">Permissions</span></span>

<span data-ttu-id="df68d-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="df68d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="df68d-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="df68d-108">Permission type</span></span>      | <span data-ttu-id="df68d-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="df68d-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="df68d-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="df68d-110">Delegated (work or school account)</span></span> | <span data-ttu-id="df68d-111">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="df68d-111">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="df68d-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="df68d-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="df68d-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="df68d-113">Not supported.</span></span>    |
|<span data-ttu-id="df68d-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="df68d-114">Application</span></span> | <span data-ttu-id="df68d-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="df68d-115">Not supported.</span></span> |

> <span data-ttu-id="df68d-116">**注**: この API は、管理者のアクセス許可をサポートします。</span><span class="sxs-lookup"><span data-stu-id="df68d-116">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="df68d-117">グローバル管理者は、所属していないグループにアクセスできます。</span><span class="sxs-lookup"><span data-stu-id="df68d-117">Global admins can access groups that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="df68d-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="df68d-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /teams/{teamId}/schedule/timeOffReasons
```

## <a name="request-headers"></a><span data-ttu-id="df68d-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="df68d-119">Request headers</span></span>

| <span data-ttu-id="df68d-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="df68d-120">Header</span></span>       | <span data-ttu-id="df68d-121">値</span><span class="sxs-lookup"><span data-stu-id="df68d-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="df68d-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="df68d-122">Authorization</span></span>  | <span data-ttu-id="df68d-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="df68d-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="df68d-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="df68d-125">Content-Type</span></span>  | <span data-ttu-id="df68d-126">application/json</span><span class="sxs-lookup"><span data-stu-id="df68d-126">application/json</span></span>  |

## <a name="response"></a><span data-ttu-id="df68d-127">応答</span><span class="sxs-lookup"><span data-stu-id="df68d-127">Response</span></span>

<span data-ttu-id="df68d-128">成功した場合、このメソッド`201 Created`は応答コードと、応答本文で[timeoffreason](../resources/timeoffreason.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="df68d-128">If successful, this method returns a `201 Created` response code and a [timeOffReason](../resources/timeoffreason.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="df68d-129">例</span><span class="sxs-lookup"><span data-stu-id="df68d-129">Example</span></span>

#### <a name="request"></a><span data-ttu-id="df68d-130">要求</span><span class="sxs-lookup"><span data-stu-id="df68d-130">Request</span></span>

<span data-ttu-id="df68d-131">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="df68d-131">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "schedule-post-timeoffreasons"
}-->
```http
POST https://graph.microsoft.com/beta/teams/{teamId}/schedule/timeOffReasons
Content-type: application/json

{
  "displayName": "Vacation",
  "iconType": "plane",
  "isActive": true
}
```

#### <a name="response"></a><span data-ttu-id="df68d-132">応答</span><span class="sxs-lookup"><span data-stu-id="df68d-132">Response</span></span>

<span data-ttu-id="df68d-133">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="df68d-133">The following is an example of the response.</span></span> 

><span data-ttu-id="df68d-p104">**注:** 読みやすくするために、ここに示す応答オブジェクトは短縮されている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="df68d-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.timeOffReason"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 401

{
  "id": "TOR_891045ca-b5d2-406b-aa06-a3c8921245d7",
  "createdDateTime": "2019-03-12T22:10:38.242Z",
  "lastModifiedDateTime": "2019-03-12T22:10:38.242Z",
  "displayName": "Vacation",
  "iconType": "plane",
  "isActive": true,
  "lastModifiedBy": {
    "application": null,
    "device": null,
    "conversation": null,
    "user": {
      "id": "366c0b19-49b1-41b5-a03f-9f3887bd0ed8",
      "displayName": "John Doe"
    }
  }
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="df68d-136">SDK サンプル コード</span><span class="sxs-lookup"><span data-stu-id="df68d-136">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="df68d-137">C#</span><span class="sxs-lookup"><span data-stu-id="df68d-137">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/schedule-post-timeoffreasons-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="df68d-138">Javascript</span><span class="sxs-lookup"><span data-stu-id="df68d-138">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/schedule-post-timeoffreasons-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="df68d-139">目的-C</span><span class="sxs-lookup"><span data-stu-id="df68d-139">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/schedule-post-timeoffreasons-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Creates a new timeOffReason",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/schedule-post-timeoffreasons.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/schedule-post-timeoffreasons.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/schedule-post-timeoffreasons.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
