---
title: appRoleAssignment を削除する
description: AppRoleAssignment を削除します。
localization_priority: Normal
ms.openlocfilehash: f8c282a3d33560e95dcb43384227a34e6bd8ccf4
ms.sourcegitcommit: 3e5f4f515f050e16680ec44f68af40583147af9e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/06/2019
ms.locfileid: "33636514"
---
# <a name="delete-approleassignment"></a><span data-ttu-id="7af02-103">appRoleAssignment を削除する</span><span class="sxs-lookup"><span data-stu-id="7af02-103">Delete appRoleAssignment</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7af02-104">AppRoleAssignment を削除します。</span><span class="sxs-lookup"><span data-stu-id="7af02-104">Delete appRoleAssignment.</span></span>
## <a name="permissions"></a><span data-ttu-id="7af02-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="7af02-105">Permissions</span></span>
<span data-ttu-id="7af02-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="7af02-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7af02-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="7af02-108">Permission type</span></span>      | <span data-ttu-id="7af02-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="7af02-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7af02-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="7af02-110">Delegated (work or school account)</span></span> | <span data-ttu-id="7af02-111">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="7af02-111">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="7af02-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="7af02-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7af02-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="7af02-113">Not supported.</span></span>    |
|<span data-ttu-id="7af02-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="7af02-114">Application</span></span> | <span data-ttu-id="7af02-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="7af02-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="7af02-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="7af02-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /users/{id | userPrincipalName}/appRoleAssignments/{id}
DELETE /servicePrincipals/{id}/appRoleAssignedTo
DELETE /groups/{id}/appRoleAssignments/{id}

```
## <a name="request-headers"></a><span data-ttu-id="7af02-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="7af02-117">Request headers</span></span>
| <span data-ttu-id="7af02-118">名前</span><span class="sxs-lookup"><span data-stu-id="7af02-118">Name</span></span>       | <span data-ttu-id="7af02-119">型</span><span class="sxs-lookup"><span data-stu-id="7af02-119">Type</span></span> | <span data-ttu-id="7af02-120">説明</span><span class="sxs-lookup"><span data-stu-id="7af02-120">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="7af02-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="7af02-121">Authorization</span></span>  | <span data-ttu-id="7af02-122">string</span><span class="sxs-lookup"><span data-stu-id="7af02-122">string</span></span>  | <span data-ttu-id="7af02-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="7af02-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="7af02-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="7af02-125">Request body</span></span>
<span data-ttu-id="7af02-126">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="7af02-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7af02-127">応答</span><span class="sxs-lookup"><span data-stu-id="7af02-127">Response</span></span>

<span data-ttu-id="7af02-p103">成功した場合、このメソッドは `204 No Content` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="7af02-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7af02-130">例</span><span class="sxs-lookup"><span data-stu-id="7af02-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="7af02-131">要求</span><span class="sxs-lookup"><span data-stu-id="7af02-131">Request</span></span>
<span data-ttu-id="7af02-132">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="7af02-132">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_approleassignment"
}-->
```http
DELETE https://graph.microsoft.com/beta/appRoleAssignments/{id}
```
##### <a name="response"></a><span data-ttu-id="7af02-133">応答</span><span class="sxs-lookup"><span data-stu-id="7af02-133">Response</span></span>
<span data-ttu-id="7af02-134">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="7af02-134">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="7af02-135">SDK サンプルコード</span><span class="sxs-lookup"><span data-stu-id="7af02-135">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="7af02-136">Visual</span><span class="sxs-lookup"><span data-stu-id="7af02-136">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/delete_approleassignment-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="7af02-137">Java</span><span class="sxs-lookup"><span data-stu-id="7af02-137">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/delete_approleassignment-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Delete appRoleAssignment",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/approleassignment-delete.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/approleassignment-delete.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
