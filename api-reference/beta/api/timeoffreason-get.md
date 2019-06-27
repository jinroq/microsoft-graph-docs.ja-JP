---
title: TimeOffReason を取得する
description: ID で timeOffReason を取得します。
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 20ee24e4c3fb5c859c35a4e9196c1d8c6eb0b79f
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/27/2019
ms.locfileid: "35270568"
---
# <a name="get-timeoffreason"></a><span data-ttu-id="31e5f-103">TimeOffReason を取得する</span><span class="sxs-lookup"><span data-stu-id="31e5f-103">Get timeOffReason</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="31e5f-104">[Timeoffreason](../resources/timeoffreason.md)オブジェクトのプロパティと関係を ID で取得します。</span><span class="sxs-lookup"><span data-stu-id="31e5f-104">Retrieve the properties and relationships of a [timeOffReason](../resources/timeoffreason.md) object by ID.</span></span>

## <a name="permissions"></a><span data-ttu-id="31e5f-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="31e5f-105">Permissions</span></span>

<span data-ttu-id="31e5f-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="31e5f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="31e5f-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="31e5f-108">Permission type</span></span>      | <span data-ttu-id="31e5f-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="31e5f-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="31e5f-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="31e5f-110">Delegated (work or school account)</span></span> | <span data-ttu-id="31e5f-111">Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="31e5f-111">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="31e5f-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="31e5f-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="31e5f-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="31e5f-113">Not supported.</span></span>    |
|<span data-ttu-id="31e5f-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="31e5f-114">Application</span></span> | <span data-ttu-id="31e5f-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="31e5f-115">Not supported.</span></span> |

> <span data-ttu-id="31e5f-116">**注**: この API は、管理者のアクセス許可をサポートします。</span><span class="sxs-lookup"><span data-stu-id="31e5f-116">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="31e5f-117">グローバル管理者は、所属していないグループにアクセスできます。</span><span class="sxs-lookup"><span data-stu-id="31e5f-117">Global admins can access groups that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="31e5f-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="31e5f-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /teams/{teamId}/schedule/timeOffReasons/{timeOffReasonId}
```

## <a name="request-headers"></a><span data-ttu-id="31e5f-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="31e5f-119">Request headers</span></span>

| <span data-ttu-id="31e5f-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="31e5f-120">Header</span></span>       | <span data-ttu-id="31e5f-121">値</span><span class="sxs-lookup"><span data-stu-id="31e5f-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="31e5f-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="31e5f-122">Authorization</span></span>  | <span data-ttu-id="31e5f-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="31e5f-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="31e5f-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="31e5f-125">Content-Type</span></span>  | <span data-ttu-id="31e5f-126">application/json</span><span class="sxs-lookup"><span data-stu-id="31e5f-126">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="31e5f-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="31e5f-127">Request body</span></span>
<span data-ttu-id="31e5f-128">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="31e5f-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="31e5f-129">応答</span><span class="sxs-lookup"><span data-stu-id="31e5f-129">Response</span></span>

<span data-ttu-id="31e5f-130">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で[timeoffreason](../resources/timeoffreason.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="31e5f-130">If successful, this method returns a `200 OK` response code and a [timeOffReason](../resources/timeoffreason.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="31e5f-131">例</span><span class="sxs-lookup"><span data-stu-id="31e5f-131">Example</span></span>

#### <a name="request"></a><span data-ttu-id="31e5f-132">要求</span><span class="sxs-lookup"><span data-stu-id="31e5f-132">Request</span></span>

<span data-ttu-id="31e5f-133">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="31e5f-133">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "timeoffreason-get"
}-->
```http
GET https://graph.microsoft.com/beta/teams/{teamId}/schedule/timeOffReasons/{timeOffReasonId}
```

#### <a name="response"></a><span data-ttu-id="31e5f-134">応答</span><span class="sxs-lookup"><span data-stu-id="31e5f-134">Response</span></span>

<span data-ttu-id="31e5f-135">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="31e5f-135">The following is an example of the response.</span></span> 

><span data-ttu-id="31e5f-p104">**注:** 読みやすくするために、ここに示す応答オブジェクトは短縮されている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="31e5f-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.timeOffReason"
} -->

```http
HTTP/1.1 200 OK
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="31e5f-138">SDK サンプル コード</span><span class="sxs-lookup"><span data-stu-id="31e5f-138">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="31e5f-139">C#</span><span class="sxs-lookup"><span data-stu-id="31e5f-139">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/timeoffreason-get-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="31e5f-140">Javascript</span><span class="sxs-lookup"><span data-stu-id="31e5f-140">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/timeoffreason-get-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="31e5f-141">目的-C</span><span class="sxs-lookup"><span data-stu-id="31e5f-141">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/timeoffreason-get-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get a timeOffReason by id",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/timeoffreason-get.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/timeoffreason-get.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/timeoffreason-get.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
