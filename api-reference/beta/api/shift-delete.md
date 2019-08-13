---
title: Shift を削除する
description: スケジュールからシフトを削除します。
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: debaeead3ba2506d9dbe62fec46d569532332a4c
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36363859"
---
# <a name="delete-shift"></a><span data-ttu-id="8fded-103">Shift を削除する</span><span class="sxs-lookup"><span data-stu-id="8fded-103">Delete shift</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8fded-104">スケジュールから[シフト](../resources/shift.md)を削除します。</span><span class="sxs-lookup"><span data-stu-id="8fded-104">Deletes a [shift](../resources/shift.md) from the schedule.</span></span>

## <a name="permissions"></a><span data-ttu-id="8fded-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="8fded-105">Permissions</span></span>

<span data-ttu-id="8fded-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="8fded-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8fded-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="8fded-108">Permission type</span></span>      | <span data-ttu-id="8fded-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="8fded-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8fded-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="8fded-110">Delegated (work or school account)</span></span> | <span data-ttu-id="8fded-111">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8fded-111">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="8fded-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="8fded-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8fded-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="8fded-113">Not supported.</span></span>    |
|<span data-ttu-id="8fded-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="8fded-114">Application</span></span> | <span data-ttu-id="8fded-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="8fded-115">Not supported.</span></span> |

> <span data-ttu-id="8fded-116">**注**: この API は、管理者のアクセス許可をサポートします。</span><span class="sxs-lookup"><span data-stu-id="8fded-116">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="8fded-117">グローバル管理者は、所属していないグループにアクセスできます。</span><span class="sxs-lookup"><span data-stu-id="8fded-117">Global admins can access groups that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="8fded-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="8fded-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /teams/{teamId}/schedule/shifts/{shiftId}
```

## <a name="request-headers"></a><span data-ttu-id="8fded-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="8fded-119">Request headers</span></span>

| <span data-ttu-id="8fded-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="8fded-120">Header</span></span>       | <span data-ttu-id="8fded-121">値</span><span class="sxs-lookup"><span data-stu-id="8fded-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="8fded-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="8fded-122">Authorization</span></span>  | <span data-ttu-id="8fded-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="8fded-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="8fded-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="8fded-125">Content-Type</span></span>  | <span data-ttu-id="8fded-126">application/json</span><span class="sxs-lookup"><span data-stu-id="8fded-126">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="8fded-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="8fded-127">Request body</span></span>
<span data-ttu-id="8fded-128">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="8fded-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8fded-129">応答</span><span class="sxs-lookup"><span data-stu-id="8fded-129">Response</span></span>

<span data-ttu-id="8fded-p104">成功した場合、このメソッドは `204 No Content` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="8fded-p104">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8fded-132">例</span><span class="sxs-lookup"><span data-stu-id="8fded-132">Example</span></span>

#### <a name="request"></a><span data-ttu-id="8fded-133">要求</span><span class="sxs-lookup"><span data-stu-id="8fded-133">Request</span></span>

<span data-ttu-id="8fded-134">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="8fded-134">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="8fded-135">プロトコル</span><span class="sxs-lookup"><span data-stu-id="8fded-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "shift-delete"
}-->
```http
DELETE https://graph.microsoft.com/beta/teams/{teamId}/schedule/shifts/{shiftId}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="8fded-136">C#</span><span class="sxs-lookup"><span data-stu-id="8fded-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/shift-delete-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="8fded-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="8fded-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/shift-delete-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="8fded-138">目的-C</span><span class="sxs-lookup"><span data-stu-id="8fded-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/shift-delete-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="8fded-139">Java</span><span class="sxs-lookup"><span data-stu-id="8fded-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/shift-delete-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="8fded-140">応答</span><span class="sxs-lookup"><span data-stu-id="8fded-140">Response</span></span>

<span data-ttu-id="8fded-141">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="8fded-141">The following is an example of the response.</span></span> 

><span data-ttu-id="8fded-p105">**注:** 読みやすくするために、ここに示す応答オブジェクトは短縮されている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="8fded-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
  "description": "Deletes a shift from the schedule",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
