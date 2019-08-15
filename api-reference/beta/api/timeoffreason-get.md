---
title: TimeOffReason を取得する
description: ID で timeOffReason を取得します。
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 221da358dd7442e669ea7e3193b22a3cd65c1160
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/15/2019
ms.locfileid: "36421212"
---
# <a name="get-timeoffreason"></a><span data-ttu-id="d3800-103">TimeOffReason を取得する</span><span class="sxs-lookup"><span data-stu-id="d3800-103">Get timeOffReason</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d3800-104">[Timeoffreason](../resources/timeoffreason.md)オブジェクトのプロパティと関係を ID で取得します。</span><span class="sxs-lookup"><span data-stu-id="d3800-104">Retrieve the properties and relationships of a [timeOffReason](../resources/timeoffreason.md) object by ID.</span></span>

## <a name="permissions"></a><span data-ttu-id="d3800-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="d3800-105">Permissions</span></span>

<span data-ttu-id="d3800-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="d3800-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d3800-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="d3800-108">Permission type</span></span>      | <span data-ttu-id="d3800-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="d3800-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d3800-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="d3800-110">Delegated (work or school account)</span></span> | <span data-ttu-id="d3800-111">Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d3800-111">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="d3800-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="d3800-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d3800-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d3800-113">Not supported.</span></span>    |
|<span data-ttu-id="d3800-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="d3800-114">Application</span></span> | <span data-ttu-id="d3800-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d3800-115">Not supported.</span></span> |

> <span data-ttu-id="d3800-116">**注**: この API は、管理者のアクセス許可をサポートします。</span><span class="sxs-lookup"><span data-stu-id="d3800-116">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="d3800-117">グローバル管理者は、所属していないグループにアクセスできます。</span><span class="sxs-lookup"><span data-stu-id="d3800-117">Global admins can access groups that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="d3800-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="d3800-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /teams/{teamId}/schedule/timeOffReasons/{timeOffReasonId}
```

## <a name="request-headers"></a><span data-ttu-id="d3800-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="d3800-119">Request headers</span></span>

| <span data-ttu-id="d3800-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="d3800-120">Header</span></span>       | <span data-ttu-id="d3800-121">値</span><span class="sxs-lookup"><span data-stu-id="d3800-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="d3800-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="d3800-122">Authorization</span></span>  | <span data-ttu-id="d3800-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="d3800-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="d3800-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="d3800-125">Content-Type</span></span>  | <span data-ttu-id="d3800-126">application/json</span><span class="sxs-lookup"><span data-stu-id="d3800-126">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="d3800-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="d3800-127">Request body</span></span>
<span data-ttu-id="d3800-128">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="d3800-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d3800-129">応答</span><span class="sxs-lookup"><span data-stu-id="d3800-129">Response</span></span>

<span data-ttu-id="d3800-130">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で[timeoffreason](../resources/timeoffreason.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="d3800-130">If successful, this method returns a `200 OK` response code and a [timeOffReason](../resources/timeoffreason.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d3800-131">例</span><span class="sxs-lookup"><span data-stu-id="d3800-131">Example</span></span>

#### <a name="request"></a><span data-ttu-id="d3800-132">要求</span><span class="sxs-lookup"><span data-stu-id="d3800-132">Request</span></span>

<span data-ttu-id="d3800-133">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="d3800-133">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="d3800-134">プロトコル</span><span class="sxs-lookup"><span data-stu-id="d3800-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "timeoffreason-get"
}-->
```http
GET https://graph.microsoft.com/beta/teams/{teamId}/schedule/timeOffReasons/{timeOffReasonId}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="d3800-135">C#</span><span class="sxs-lookup"><span data-stu-id="d3800-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/timeoffreason-get-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="d3800-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d3800-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/timeoffreason-get-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="d3800-137">目的-C</span><span class="sxs-lookup"><span data-stu-id="d3800-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/timeoffreason-get-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="d3800-138">応答</span><span class="sxs-lookup"><span data-stu-id="d3800-138">Response</span></span>

<span data-ttu-id="d3800-139">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="d3800-139">The following is an example of the response.</span></span> 

><span data-ttu-id="d3800-p104">**注:** 読みやすくするために、ここに示す応答オブジェクトは短縮されている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="d3800-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
  ]
}
-->
