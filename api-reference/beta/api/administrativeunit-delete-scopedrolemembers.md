---
title: ScopedRoleMember を削除する
description: 管理単位からスコープ付き役割のメンバーを削除します。
author: davidmu1
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 0fc95837a1d4d0079e18f2fcddd5d60180d39b66
ms.sourcegitcommit: 27e8ddb53b699f70b676c9648db8f06bb8d831a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/27/2019
ms.locfileid: "35917981"
---
# <a name="remove-a-scopedrolemember"></a><span data-ttu-id="6ca2b-103">ScopedRoleMember を削除する</span><span class="sxs-lookup"><span data-stu-id="6ca2b-103">Remove a scopedRoleMember</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6ca2b-104">管理単位からスコープ付き役割のメンバーを削除します。</span><span class="sxs-lookup"><span data-stu-id="6ca2b-104">Remove a scoped-role member from an adminstrative unit.</span></span>

## <a name="permissions"></a><span data-ttu-id="6ca2b-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="6ca2b-105">Permissions</span></span>
<span data-ttu-id="6ca2b-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="6ca2b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="6ca2b-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="6ca2b-108">Permission type</span></span>      | <span data-ttu-id="6ca2b-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="6ca2b-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6ca2b-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="6ca2b-110">Delegated (work or school account)</span></span> | <span data-ttu-id="6ca2b-111">AdministrativeUnit。すべての Directory.accessasuser.all について</span><span class="sxs-lookup"><span data-stu-id="6ca2b-111">AdministrativeUnit.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="6ca2b-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="6ca2b-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6ca2b-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="6ca2b-113">Not supported.</span></span>    |
|<span data-ttu-id="6ca2b-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="6ca2b-114">Application</span></span> | <span data-ttu-id="6ca2b-115">AdministrativeUnit</span><span class="sxs-lookup"><span data-stu-id="6ca2b-115">AdministrativeUnit.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="6ca2b-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="6ca2b-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /administrativeUnits/{id}/scopedRoleMembers/{id}

```
## <a name="request-headers"></a><span data-ttu-id="6ca2b-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="6ca2b-117">Request headers</span></span>
| <span data-ttu-id="6ca2b-118">名前</span><span class="sxs-lookup"><span data-stu-id="6ca2b-118">Name</span></span>       | <span data-ttu-id="6ca2b-119">説明</span><span class="sxs-lookup"><span data-stu-id="6ca2b-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="6ca2b-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="6ca2b-120">Authorization</span></span>  | <span data-ttu-id="6ca2b-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="6ca2b-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="6ca2b-123">要求本文</span><span class="sxs-lookup"><span data-stu-id="6ca2b-123">Request body</span></span>
<span data-ttu-id="6ca2b-124">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="6ca2b-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6ca2b-125">応答</span><span class="sxs-lookup"><span data-stu-id="6ca2b-125">Response</span></span>

<span data-ttu-id="6ca2b-p103">成功した場合、このメソッドは `204 No Content` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="6ca2b-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6ca2b-128">例</span><span class="sxs-lookup"><span data-stu-id="6ca2b-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="6ca2b-129">要求</span><span class="sxs-lookup"><span data-stu-id="6ca2b-129">Request</span></span>
<span data-ttu-id="6ca2b-130">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="6ca2b-130">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="6ca2b-131">プロトコル</span><span class="sxs-lookup"><span data-stu-id="6ca2b-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_scopedrolemember"
}-->
```http
DELETE https://graph.microsoft.com/beta/administrativeUnits/{id}/scopedRoleMembers/{id}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="6ca2b-132">C#</span><span class="sxs-lookup"><span data-stu-id="6ca2b-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-scopedrolemember-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="6ca2b-133">Javascript</span><span class="sxs-lookup"><span data-stu-id="6ca2b-133">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-scopedrolemember-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="6ca2b-134">目的-C</span><span class="sxs-lookup"><span data-stu-id="6ca2b-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-scopedrolemember-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="6ca2b-135">Java</span><span class="sxs-lookup"><span data-stu-id="6ca2b-135">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-scopedrolemember-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="6ca2b-136">応答</span><span class="sxs-lookup"><span data-stu-id="6ca2b-136">Response</span></span>
<span data-ttu-id="6ca2b-p104">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="6ca2b-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "Delete administrativeUnit",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
