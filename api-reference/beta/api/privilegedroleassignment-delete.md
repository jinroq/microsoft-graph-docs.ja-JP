---
title: privilegedRoleAssignment を削除する
description: PrivilegedRoleAssignment を削除します。
localization_priority: Normal
doc_type: apiPageType
ms.prod: ''
author: ''
ms.openlocfilehash: 38500f75e52d8ebeddd1dc5875bb6746c26d5a39
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/15/2019
ms.locfileid: "36412762"
---
# <a name="delete-privilegedroleassignment"></a><span data-ttu-id="04ef5-103">privilegedRoleAssignment を削除する</span><span class="sxs-lookup"><span data-stu-id="04ef5-103">Delete privilegedRoleAssignment</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="04ef5-104">[PrivilegedRoleAssignment](../resources/privilegedroleassignment.md)を削除します。</span><span class="sxs-lookup"><span data-stu-id="04ef5-104">Delete [privilegedRoleAssignment](../resources/privilegedroleassignment.md).</span></span>
## <a name="permissions"></a><span data-ttu-id="04ef5-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="04ef5-105">Permissions</span></span>
<span data-ttu-id="04ef5-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="04ef5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="04ef5-108">リクエスターは、特権の_役割管理者_の役割を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="04ef5-108">The requestor needs to have _Privileged Role Administrator_ role.</span></span>
 

|<span data-ttu-id="04ef5-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="04ef5-109">Permission type</span></span>      | <span data-ttu-id="04ef5-110">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="04ef5-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="04ef5-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="04ef5-111">Delegated (work or school account)</span></span> | <span data-ttu-id="04ef5-112">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="04ef5-112">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="04ef5-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="04ef5-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="04ef5-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="04ef5-114">Not supported.</span></span>    |
|<span data-ttu-id="04ef5-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="04ef5-115">Application</span></span> | <span data-ttu-id="04ef5-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="04ef5-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="04ef5-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="04ef5-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /privilegedRoleAssignments/{id}
```

<span data-ttu-id="04ef5-118">ここで``{id}`` 、は ' userId_roleId ' の形式になっています。ここで、UserId は azure AD ユーザー ID の guid 文字列で、RoleId は azure 管理者の役割 ID の guid 文字列です。</span><span class="sxs-lookup"><span data-stu-id="04ef5-118">Note that ``{id}`` is in the format of 'userId_roleId', where userId is the GUID string for Azure AD user id, and roleId is the GUID string for Azure administrator role id.</span></span>

## <a name="request-headers"></a><span data-ttu-id="04ef5-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="04ef5-119">Request headers</span></span>
| <span data-ttu-id="04ef5-120">名前</span><span class="sxs-lookup"><span data-stu-id="04ef5-120">Name</span></span>       | <span data-ttu-id="04ef5-121">説明</span><span class="sxs-lookup"><span data-stu-id="04ef5-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="04ef5-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="04ef5-122">Authorization</span></span>  | <span data-ttu-id="04ef5-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="04ef5-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="04ef5-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="04ef5-125">Request body</span></span>
<span data-ttu-id="04ef5-126">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="04ef5-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="04ef5-127">応答</span><span class="sxs-lookup"><span data-stu-id="04ef5-127">Response</span></span>

<span data-ttu-id="04ef5-p103">成功した場合、このメソッドは `204 No Content` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="04ef5-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

<span data-ttu-id="04ef5-130">テナントが PIM に登録されている必要があることに注意してください。</span><span class="sxs-lookup"><span data-stu-id="04ef5-130">Note that the tenant needs to be registered to PIM.</span></span> <span data-ttu-id="04ef5-131">それ以外の場合、HTTP 403 の禁止状態コードが返されます。</span><span class="sxs-lookup"><span data-stu-id="04ef5-131">Otherwise, the HTTP 403 Forbidden status code will be returned.</span></span>
## <a name="example"></a><span data-ttu-id="04ef5-132">例</span><span class="sxs-lookup"><span data-stu-id="04ef5-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="04ef5-133">要求</span><span class="sxs-lookup"><span data-stu-id="04ef5-133">Request</span></span>
<span data-ttu-id="04ef5-134">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="04ef5-134">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="04ef5-135">プロトコル</span><span class="sxs-lookup"><span data-stu-id="04ef5-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_privilegedroleassignment"
}-->
```http
DELETE https://graph.microsoft.com/beta/privilegedRoleAssignments/{id}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="04ef5-136">C#</span><span class="sxs-lookup"><span data-stu-id="04ef5-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-privilegedroleassignment-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="04ef5-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="04ef5-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-privilegedroleassignment-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="04ef5-138">目的-C</span><span class="sxs-lookup"><span data-stu-id="04ef5-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-privilegedroleassignment-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="04ef5-139">応答</span><span class="sxs-lookup"><span data-stu-id="04ef5-139">Response</span></span>
<span data-ttu-id="04ef5-p105">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="04ef5-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "Delete privilegedRoleAssignment",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
