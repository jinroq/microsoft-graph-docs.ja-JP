---
title: TimeOffReason の削除
description: IsActive プロパティを設定して timeOffReason を非アクティブとしてマークする
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 25e07aa77790b38da5c19922060ac93490166fd3
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/02/2019
ms.locfileid: "35457934"
---
# <a name="delete-timeoffreason"></a><span data-ttu-id="2f276-103">TimeOffReason の削除</span><span class="sxs-lookup"><span data-stu-id="2f276-103">Delete timeOffReason</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2f276-104">**IsActive**プロパティを設定して、 [timeoffreason](../resources/timeoffreason.md)を非アクティブとしてマークします。</span><span class="sxs-lookup"><span data-stu-id="2f276-104">Mark a [timeOffReason](../resources/timeoffreason.md) as inactive by setting the **isActive** property.</span></span>

<span data-ttu-id="2f276-105">このメソッドでは、指定した[Timeoffreason](../resources/timeoffreason.md)インスタンスは削除されません。</span><span class="sxs-lookup"><span data-stu-id="2f276-105">This method does not remove the specified [timeOffReason](../resources/timeoffreason.md) instance.</span></span> <span data-ttu-id="2f276-106">この理由が割り当てられた[Timeoffitem](../resources/timeoffitem.md)インスタンスは、この理由に割り当てられたままになります。</span><span class="sxs-lookup"><span data-stu-id="2f276-106">[timeOffItem](../resources/timeoffitem.md) instances that have been assigned this reason remain assigned to this reason.</span></span>

## <a name="permissions"></a><span data-ttu-id="2f276-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="2f276-107">Permissions</span></span>

<span data-ttu-id="2f276-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="2f276-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2f276-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="2f276-110">Permission type</span></span>      | <span data-ttu-id="2f276-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="2f276-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2f276-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="2f276-112">Delegated (work or school account)</span></span> | <span data-ttu-id="2f276-113">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2f276-113">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="2f276-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="2f276-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2f276-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="2f276-115">Not supported.</span></span>    |
|<span data-ttu-id="2f276-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="2f276-116">Application</span></span> | <span data-ttu-id="2f276-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="2f276-117">Not supported.</span></span> |

> <span data-ttu-id="2f276-118">**注**: この API は、管理者のアクセス許可をサポートします。</span><span class="sxs-lookup"><span data-stu-id="2f276-118">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="2f276-119">グローバル管理者は、所属していないグループにアクセスできます。</span><span class="sxs-lookup"><span data-stu-id="2f276-119">Global admins can access groups that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="2f276-120">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="2f276-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /teams/{teamId}/schedule/timeOffReasons/{timeOffReasonId}
```

## <a name="request-headers"></a><span data-ttu-id="2f276-121">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="2f276-121">Request headers</span></span>

| <span data-ttu-id="2f276-122">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="2f276-122">Header</span></span>       | <span data-ttu-id="2f276-123">値</span><span class="sxs-lookup"><span data-stu-id="2f276-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="2f276-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="2f276-124">Authorization</span></span>  | <span data-ttu-id="2f276-p104">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="2f276-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="2f276-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="2f276-127">Content-Type</span></span>  | <span data-ttu-id="2f276-128">application/json</span><span class="sxs-lookup"><span data-stu-id="2f276-128">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="2f276-129">要求本文</span><span class="sxs-lookup"><span data-stu-id="2f276-129">Request body</span></span>
<span data-ttu-id="2f276-130">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="2f276-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2f276-131">応答</span><span class="sxs-lookup"><span data-stu-id="2f276-131">Response</span></span>

<span data-ttu-id="2f276-p105">成功した場合、このメソッドは `204 No Content` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="2f276-p105">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2f276-134">例</span><span class="sxs-lookup"><span data-stu-id="2f276-134">Example</span></span>

#### <a name="request"></a><span data-ttu-id="2f276-135">要求</span><span class="sxs-lookup"><span data-stu-id="2f276-135">Request</span></span>

<span data-ttu-id="2f276-136">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="2f276-136">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="2f276-137">プロトコル</span><span class="sxs-lookup"><span data-stu-id="2f276-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "timeoffreason-delete"
}-->
```http
DELETE https://graph.microsoft.com/beta/teams/{teamId}/schedule/timeOffReasons/{timeOffReasonId}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="2f276-138">C#</span><span class="sxs-lookup"><span data-stu-id="2f276-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/timeoffreason-delete-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="2f276-139">Javascript</span><span class="sxs-lookup"><span data-stu-id="2f276-139">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/timeoffreason-delete-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="2f276-140">目的-C</span><span class="sxs-lookup"><span data-stu-id="2f276-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/timeoffreason-delete-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="2f276-141">応答</span><span class="sxs-lookup"><span data-stu-id="2f276-141">Response</span></span>

<span data-ttu-id="2f276-142">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="2f276-142">The following is an example of the response.</span></span> 

><span data-ttu-id="2f276-p106">**注:** 読みやすくするために、ここに示す応答オブジェクトは短縮されている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="2f276-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.None"
} -->

```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Marks a timeOffReason as inactive",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
