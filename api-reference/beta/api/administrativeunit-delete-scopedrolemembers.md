---
title: ScopedRoleMember を削除する
description: 管理単位からスコープ付き役割のメンバーを削除します。
author: davidmu1
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 8e9d256323fcac125849c06331cc29e993d1b858
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36319056"
---
# <a name="remove-a-scopedrolemember"></a><span data-ttu-id="f54af-103">ScopedRoleMember を削除する</span><span class="sxs-lookup"><span data-stu-id="f54af-103">Remove a scopedRoleMember</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f54af-104">管理単位からスコープ付き役割のメンバーを削除します。</span><span class="sxs-lookup"><span data-stu-id="f54af-104">Remove a scoped-role member from an adminstrative unit.</span></span>

## <a name="permissions"></a><span data-ttu-id="f54af-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="f54af-105">Permissions</span></span>
<span data-ttu-id="f54af-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="f54af-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="f54af-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="f54af-108">Permission type</span></span>      | <span data-ttu-id="f54af-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="f54af-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f54af-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="f54af-110">Delegated (work or school account)</span></span> | <span data-ttu-id="f54af-111">RoleManagement、Directory.accessasuser.all、およびすべてのディレクトリ</span><span class="sxs-lookup"><span data-stu-id="f54af-111">RoleManagement.ReadWrite.Directory, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="f54af-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="f54af-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f54af-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f54af-113">Not supported.</span></span>    |
|<span data-ttu-id="f54af-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="f54af-114">Application</span></span> | <span data-ttu-id="f54af-115">RoleManagement</span><span class="sxs-lookup"><span data-stu-id="f54af-115">RoleManagement.ReadWrite.Directory</span></span> |

## <a name="http-request"></a><span data-ttu-id="f54af-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="f54af-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /administrativeUnits/{id}/scopedRoleMembers/{id}

```
## <a name="request-headers"></a><span data-ttu-id="f54af-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="f54af-117">Request headers</span></span>
| <span data-ttu-id="f54af-118">名前</span><span class="sxs-lookup"><span data-stu-id="f54af-118">Name</span></span>       | <span data-ttu-id="f54af-119">説明</span><span class="sxs-lookup"><span data-stu-id="f54af-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="f54af-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="f54af-120">Authorization</span></span>  | <span data-ttu-id="f54af-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="f54af-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="f54af-123">要求本文</span><span class="sxs-lookup"><span data-stu-id="f54af-123">Request body</span></span>
<span data-ttu-id="f54af-124">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="f54af-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f54af-125">応答</span><span class="sxs-lookup"><span data-stu-id="f54af-125">Response</span></span>

<span data-ttu-id="f54af-p103">成功した場合、このメソッドは `204 No Content` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="f54af-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f54af-128">例</span><span class="sxs-lookup"><span data-stu-id="f54af-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="f54af-129">要求</span><span class="sxs-lookup"><span data-stu-id="f54af-129">Request</span></span>
<span data-ttu-id="f54af-130">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="f54af-130">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="f54af-131">プロトコル</span><span class="sxs-lookup"><span data-stu-id="f54af-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_scopedrolemember"
}-->
```http
DELETE https://graph.microsoft.com/beta/administrativeUnits/{id}/scopedRoleMembers/{id}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="f54af-132">C#</span><span class="sxs-lookup"><span data-stu-id="f54af-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-scopedrolemember-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="f54af-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f54af-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-scopedrolemember-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="f54af-134">目的-C</span><span class="sxs-lookup"><span data-stu-id="f54af-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-scopedrolemember-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="f54af-135">Java</span><span class="sxs-lookup"><span data-stu-id="f54af-135">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-scopedrolemember-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="f54af-136">応答</span><span class="sxs-lookup"><span data-stu-id="f54af-136">Response</span></span>
<span data-ttu-id="f54af-p104">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="f54af-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
