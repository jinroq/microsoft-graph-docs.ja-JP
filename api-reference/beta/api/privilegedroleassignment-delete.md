---
title: privilegedRoleAssignment を削除する
description: PrivilegedRoleAssignment を削除します。
localization_priority: Normal
ms.openlocfilehash: d6779a2cfa23cb9f947045b8c7370094790c8a10
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/27/2019
ms.locfileid: "35268160"
---
# <a name="delete-privilegedroleassignment"></a><span data-ttu-id="862ee-103">privilegedRoleAssignment を削除する</span><span class="sxs-lookup"><span data-stu-id="862ee-103">Delete privilegedRoleAssignment</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="862ee-104">[PrivilegedRoleAssignment](../resources/privilegedroleassignment.md)を削除します。</span><span class="sxs-lookup"><span data-stu-id="862ee-104">Delete [privilegedRoleAssignment](../resources/privilegedroleassignment.md).</span></span>
## <a name="permissions"></a><span data-ttu-id="862ee-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="862ee-105">Permissions</span></span>
<span data-ttu-id="862ee-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="862ee-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="862ee-108">リクエスターは、特権の_役割管理者_の役割を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="862ee-108">The requestor needs to have _Privileged Role Administrator_ role.</span></span>
 

|<span data-ttu-id="862ee-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="862ee-109">Permission type</span></span>      | <span data-ttu-id="862ee-110">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="862ee-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="862ee-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="862ee-111">Delegated (work or school account)</span></span> | <span data-ttu-id="862ee-112">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="862ee-112">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="862ee-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="862ee-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="862ee-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="862ee-114">Not supported.</span></span>    |
|<span data-ttu-id="862ee-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="862ee-115">Application</span></span> | <span data-ttu-id="862ee-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="862ee-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="862ee-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="862ee-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /privilegedRoleAssignments/{id}
```

<span data-ttu-id="862ee-118">ここで``<id>`` 、は ' userId_roleId ' の形式になっています。ここで、UserId は azure AD ユーザー ID の guid 文字列で、RoleId は azure 管理者の役割 ID の guid 文字列です。</span><span class="sxs-lookup"><span data-stu-id="862ee-118">Note that ``<id>`` is in the format of 'userId_roleId', where userId is the GUID string for Azure AD user id, and roleId is the GUID string for Azure administrator role id.</span></span>

## <a name="request-headers"></a><span data-ttu-id="862ee-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="862ee-119">Request headers</span></span>
| <span data-ttu-id="862ee-120">名前</span><span class="sxs-lookup"><span data-stu-id="862ee-120">Name</span></span>       | <span data-ttu-id="862ee-121">説明</span><span class="sxs-lookup"><span data-stu-id="862ee-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="862ee-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="862ee-122">Authorization</span></span>  | <span data-ttu-id="862ee-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="862ee-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="862ee-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="862ee-125">Request body</span></span>
<span data-ttu-id="862ee-126">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="862ee-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="862ee-127">応答</span><span class="sxs-lookup"><span data-stu-id="862ee-127">Response</span></span>

<span data-ttu-id="862ee-p103">成功した場合、このメソッドは `204 No Content` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="862ee-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

<span data-ttu-id="862ee-130">テナントが PIM に登録されている必要があることに注意してください。</span><span class="sxs-lookup"><span data-stu-id="862ee-130">Note that the tenant needs to be registered to PIM.</span></span> <span data-ttu-id="862ee-131">それ以外の場合、HTTP 403 の禁止状態コードが返されます。</span><span class="sxs-lookup"><span data-stu-id="862ee-131">Otherwise, the HTTP 403 Forbidden status code will be returned.</span></span>
## <a name="example"></a><span data-ttu-id="862ee-132">例</span><span class="sxs-lookup"><span data-stu-id="862ee-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="862ee-133">要求</span><span class="sxs-lookup"><span data-stu-id="862ee-133">Request</span></span>
<span data-ttu-id="862ee-134">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="862ee-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_privilegedroleassignment"
}-->
```http
DELETE https://graph.microsoft.com/beta/privilegedRoleAssignments/{id}
```
##### <a name="response"></a><span data-ttu-id="862ee-135">応答</span><span class="sxs-lookup"><span data-stu-id="862ee-135">Response</span></span>
<span data-ttu-id="862ee-p105">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="862ee-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="862ee-139">SDK サンプル コード</span><span class="sxs-lookup"><span data-stu-id="862ee-139">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="862ee-140">C#</span><span class="sxs-lookup"><span data-stu-id="862ee-140">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/delete_privilegedroleassignment-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="862ee-141">Javascript</span><span class="sxs-lookup"><span data-stu-id="862ee-141">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/delete_privilegedroleassignment-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="862ee-142">目的-C</span><span class="sxs-lookup"><span data-stu-id="862ee-142">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/delete_privilegedroleassignment-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

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
    "Error: /api-reference/beta/api/privilegedroleassignment-delete.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/privilegedroleassignment-delete.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/privilegedroleassignment-delete.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
