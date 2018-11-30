---
title: AppRoleAssignment を削除します。
description: AppRoleAssignment を削除します。
ms.openlocfilehash: 1673f3f04d03154242497682da3fcbdaf4248412
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27067995"
---
# <a name="delete-approleassignment"></a><span data-ttu-id="1314a-103">AppRoleAssignment を削除します。</span><span class="sxs-lookup"><span data-stu-id="1314a-103">Delete appRoleAssignment</span></span>

> <span data-ttu-id="1314a-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="1314a-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="1314a-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="1314a-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="1314a-106">AppRoleAssignment を削除します。</span><span class="sxs-lookup"><span data-stu-id="1314a-106">Delete appRoleAssignment.</span></span>
## <a name="permissions"></a><span data-ttu-id="1314a-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="1314a-107">Permissions</span></span>
<span data-ttu-id="1314a-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="1314a-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1314a-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="1314a-110">Permission type</span></span>      | <span data-ttu-id="1314a-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="1314a-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1314a-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="1314a-112">Delegated (work or school account)</span></span> | <span data-ttu-id="1314a-113">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="1314a-113">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="1314a-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="1314a-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1314a-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="1314a-115">Not supported.</span></span>    |
|<span data-ttu-id="1314a-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="1314a-116">Application</span></span> | <span data-ttu-id="1314a-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="1314a-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="1314a-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="1314a-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /users/{id | userPrincipalName}/appRoleAssignments/{id}
DELETE /servicePrincipals/{id}/appRoleAssignedTo
DELETE /groups/{id}/appRoleAssignments/{id}

```
## <a name="request-headers"></a><span data-ttu-id="1314a-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="1314a-119">Request headers</span></span>
| <span data-ttu-id="1314a-120">名前</span><span class="sxs-lookup"><span data-stu-id="1314a-120">Name</span></span>       | <span data-ttu-id="1314a-121">型</span><span class="sxs-lookup"><span data-stu-id="1314a-121">Type</span></span> | <span data-ttu-id="1314a-122">説明</span><span class="sxs-lookup"><span data-stu-id="1314a-122">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="1314a-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="1314a-123">Authorization</span></span>  | <span data-ttu-id="1314a-124">string</span><span class="sxs-lookup"><span data-stu-id="1314a-124">string</span></span>  | <span data-ttu-id="1314a-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="1314a-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="1314a-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="1314a-127">Request body</span></span>
<span data-ttu-id="1314a-128">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="1314a-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1314a-129">応答</span><span class="sxs-lookup"><span data-stu-id="1314a-129">Response</span></span>

<span data-ttu-id="1314a-p104">成功した場合、このメソッドは `204 No Content` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="1314a-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1314a-132">例</span><span class="sxs-lookup"><span data-stu-id="1314a-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="1314a-133">要求</span><span class="sxs-lookup"><span data-stu-id="1314a-133">Request</span></span>
<span data-ttu-id="1314a-134">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="1314a-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_approleassignment"
}-->
```http
DELETE https://graph.microsoft.com/beta/appRoleAssignments/{id}
```
##### <a name="response"></a><span data-ttu-id="1314a-135">応答</span><span class="sxs-lookup"><span data-stu-id="1314a-135">Response</span></span>
<span data-ttu-id="1314a-136">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="1314a-136">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete appRoleAssignment",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->