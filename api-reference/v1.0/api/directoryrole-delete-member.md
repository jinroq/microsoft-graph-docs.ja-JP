---
title: ディレクトリ ロールのメンバーを削除する
description: directoryRole からメンバーを削除します。
author: davidmu1
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: be153524d166e97a42bade6070091b27e72cec98
ms.sourcegitcommit: 27e8ddb53b699f70b676c9648db8f06bb8d831a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/27/2019
ms.locfileid: "35918035"
---
# <a name="remove-directory-role-member"></a><span data-ttu-id="97457-103">ディレクトリ ロールのメンバーを削除する</span><span class="sxs-lookup"><span data-stu-id="97457-103">Remove directory role member</span></span>

<span data-ttu-id="97457-104">directoryRole からメンバーを削除します。</span><span class="sxs-lookup"><span data-stu-id="97457-104">Remove a member from a directoryRole.</span></span>

## <a name="permissions"></a><span data-ttu-id="97457-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="97457-105">Permissions</span></span>

<span data-ttu-id="97457-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="97457-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="97457-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="97457-108">Permission type</span></span>      | <span data-ttu-id="97457-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="97457-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="97457-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="97457-110">Delegated (work or school account)</span></span> | <span data-ttu-id="97457-111">RoleManagement、Directory.accessasuser.all、およびすべてのディレクトリ</span><span class="sxs-lookup"><span data-stu-id="97457-111">RoleManagement.ReadWrite.Directory, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="97457-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="97457-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="97457-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="97457-113">Not supported.</span></span>    |
|<span data-ttu-id="97457-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="97457-114">Application</span></span> | <span data-ttu-id="97457-115">RoleManagement</span><span class="sxs-lookup"><span data-stu-id="97457-115">RoleManagement.ReadWrite.Directory</span></span> |

## <a name="http-request"></a><span data-ttu-id="97457-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="97457-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /directoryRoles/{id}/members/{id}/$ref
```

## <a name="request-headers"></a><span data-ttu-id="97457-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="97457-117">Request headers</span></span>

| <span data-ttu-id="97457-118">名前</span><span class="sxs-lookup"><span data-stu-id="97457-118">Name</span></span>       | <span data-ttu-id="97457-119">型</span><span class="sxs-lookup"><span data-stu-id="97457-119">Type</span></span> | <span data-ttu-id="97457-120">説明</span><span class="sxs-lookup"><span data-stu-id="97457-120">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="97457-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="97457-121">Authorization</span></span>  | <span data-ttu-id="97457-122">string</span><span class="sxs-lookup"><span data-stu-id="97457-122">string</span></span>  | <span data-ttu-id="97457-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="97457-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="97457-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="97457-125">Request body</span></span>

<span data-ttu-id="97457-126">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="97457-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="97457-127">応答</span><span class="sxs-lookup"><span data-stu-id="97457-127">Response</span></span>

<span data-ttu-id="97457-p103">成功した場合、このメソッドは `204 No Content` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="97457-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="97457-130">例</span><span class="sxs-lookup"><span data-stu-id="97457-130">Example</span></span>

##### <a name="request"></a><span data-ttu-id="97457-131">要求</span><span class="sxs-lookup"><span data-stu-id="97457-131">Request</span></span>

<span data-ttu-id="97457-132">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="97457-132">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="97457-133">プロトコル</span><span class="sxs-lookup"><span data-stu-id="97457-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_directoryobject_from_directoryrole"
}-->

```http
DELETE https://graph.microsoft.com/v1.0/directoryRoles/{id}/members/{id}/$ref
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="97457-134">C#</span><span class="sxs-lookup"><span data-stu-id="97457-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-directoryobject-from-directoryrole-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="97457-135">Javascript</span><span class="sxs-lookup"><span data-stu-id="97457-135">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-directoryobject-from-directoryrole-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="97457-136">目的-C</span><span class="sxs-lookup"><span data-stu-id="97457-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-directoryobject-from-directoryrole-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="97457-137">Java</span><span class="sxs-lookup"><span data-stu-id="97457-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-directoryobject-from-directoryrole-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="97457-138">応答</span><span class="sxs-lookup"><span data-stu-id="97457-138">Response</span></span>

<span data-ttu-id="97457-139">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="97457-139">Here is an example of the response.</span></span> 
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
  "description": "Delete a member",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
