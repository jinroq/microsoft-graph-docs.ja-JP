---
title: OutlookTaskGroup の削除
description: 指定した outlookTaskGroup を削除します。
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: de9c096735e357e911ead5e788c6a67b99feecd7
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/02/2019
ms.locfileid: "35447195"
---
# <a name="delete-outlooktaskgroup"></a><span data-ttu-id="d3f89-103">OutlookTaskGroup の削除</span><span class="sxs-lookup"><span data-stu-id="d3f89-103">Delete outlookTaskGroup</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d3f89-104">指定した[Outlooktaskgroup](../resources/outlooktaskgroup.md)を削除します。</span><span class="sxs-lookup"><span data-stu-id="d3f89-104">Delete the specified [outlookTaskGroup](../resources/outlooktaskgroup.md).</span></span>
## <a name="permissions"></a><span data-ttu-id="d3f89-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="d3f89-105">Permissions</span></span>
<span data-ttu-id="d3f89-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="d3f89-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d3f89-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="d3f89-108">Permission type</span></span>      | <span data-ttu-id="d3f89-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="d3f89-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d3f89-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="d3f89-110">Delegated (work or school account)</span></span> | <span data-ttu-id="d3f89-111">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d3f89-111">Tasks.ReadWrite</span></span>    |
|<span data-ttu-id="d3f89-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="d3f89-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d3f89-113">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d3f89-113">Tasks.ReadWrite</span></span>    |
|<span data-ttu-id="d3f89-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="d3f89-114">Application</span></span> | <span data-ttu-id="d3f89-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d3f89-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="d3f89-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="d3f89-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /me/outlook/taskGroups/{id}
DELETE /users/{id|userPrincipalName}/outlook/taskGroups/{id}
```
## <a name="request-headers"></a><span data-ttu-id="d3f89-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="d3f89-117">Request headers</span></span>
| <span data-ttu-id="d3f89-118">名前</span><span class="sxs-lookup"><span data-stu-id="d3f89-118">Name</span></span>       | <span data-ttu-id="d3f89-119">説明</span><span class="sxs-lookup"><span data-stu-id="d3f89-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="d3f89-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="d3f89-120">Authorization</span></span>  | <span data-ttu-id="d3f89-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="d3f89-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="d3f89-123">要求本文</span><span class="sxs-lookup"><span data-stu-id="d3f89-123">Request body</span></span>
<span data-ttu-id="d3f89-124">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="d3f89-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d3f89-125">応答</span><span class="sxs-lookup"><span data-stu-id="d3f89-125">Response</span></span>

<span data-ttu-id="d3f89-p103">成功した場合、このメソッドは `204 No Content` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="d3f89-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d3f89-128">例</span><span class="sxs-lookup"><span data-stu-id="d3f89-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="d3f89-129">要求</span><span class="sxs-lookup"><span data-stu-id="d3f89-129">Request</span></span>
<span data-ttu-id="d3f89-130">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="d3f89-130">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="d3f89-131">プロトコル</span><span class="sxs-lookup"><span data-stu-id="d3f89-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_outlooktaskgroup"
}-->
```http
DELETE https://graph.microsoft.com/beta/me/outlook/taskgroups/AAMkADIyAAAhrbe-AAA=
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="d3f89-132">C#</span><span class="sxs-lookup"><span data-stu-id="d3f89-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-outlooktaskgroup-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="d3f89-133">Javascript</span><span class="sxs-lookup"><span data-stu-id="d3f89-133">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-outlooktaskgroup-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="d3f89-134">目的-C</span><span class="sxs-lookup"><span data-stu-id="d3f89-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-outlooktaskgroup-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="d3f89-135">応答</span><span class="sxs-lookup"><span data-stu-id="d3f89-135">Response</span></span>
<span data-ttu-id="d3f89-136">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="d3f89-136">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Delete outlookTaskGroup",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
