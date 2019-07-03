---
title: ディレクトリ ロールのメンバーを削除する
description: directoryRole からメンバーを削除します。
author: davidmu1
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 2f19162726a1b99de054332313982b741546237b
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/02/2019
ms.locfileid: "35459343"
---
# <a name="remove-directory-role-member"></a><span data-ttu-id="4d49e-103">ディレクトリ ロールのメンバーを削除する</span><span class="sxs-lookup"><span data-stu-id="4d49e-103">Remove directory role member</span></span>

<span data-ttu-id="4d49e-104">directoryRole からメンバーを削除します。</span><span class="sxs-lookup"><span data-stu-id="4d49e-104">Remove a member from a directoryRole.</span></span>

## <a name="permissions"></a><span data-ttu-id="4d49e-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="4d49e-105">Permissions</span></span>

<span data-ttu-id="4d49e-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="4d49e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="4d49e-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="4d49e-108">Permission type</span></span>      | <span data-ttu-id="4d49e-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="4d49e-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4d49e-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="4d49e-110">Delegated (work or school account)</span></span> | <span data-ttu-id="4d49e-111">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="4d49e-111">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="4d49e-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="4d49e-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4d49e-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="4d49e-113">Not supported.</span></span>    |
|<span data-ttu-id="4d49e-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="4d49e-114">Application</span></span> | <span data-ttu-id="4d49e-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="4d49e-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="4d49e-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="4d49e-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /directoryRoles/{id}/members/{id}/$ref
```

## <a name="request-headers"></a><span data-ttu-id="4d49e-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="4d49e-117">Request headers</span></span>

| <span data-ttu-id="4d49e-118">名前</span><span class="sxs-lookup"><span data-stu-id="4d49e-118">Name</span></span>       | <span data-ttu-id="4d49e-119">型</span><span class="sxs-lookup"><span data-stu-id="4d49e-119">Type</span></span> | <span data-ttu-id="4d49e-120">説明</span><span class="sxs-lookup"><span data-stu-id="4d49e-120">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="4d49e-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="4d49e-121">Authorization</span></span>  | <span data-ttu-id="4d49e-122">string</span><span class="sxs-lookup"><span data-stu-id="4d49e-122">string</span></span>  | <span data-ttu-id="4d49e-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="4d49e-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="4d49e-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="4d49e-125">Request body</span></span>

<span data-ttu-id="4d49e-126">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="4d49e-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4d49e-127">応答</span><span class="sxs-lookup"><span data-stu-id="4d49e-127">Response</span></span>

<span data-ttu-id="4d49e-p103">成功した場合、このメソッドは `204 No Content` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="4d49e-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4d49e-130">例</span><span class="sxs-lookup"><span data-stu-id="4d49e-130">Example</span></span>

##### <a name="request"></a><span data-ttu-id="4d49e-131">要求</span><span class="sxs-lookup"><span data-stu-id="4d49e-131">Request</span></span>

<span data-ttu-id="4d49e-132">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="4d49e-132">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="4d49e-133">プロトコル</span><span class="sxs-lookup"><span data-stu-id="4d49e-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_directoryobject_from_directoryrole"
}-->

```http
DELETE https://graph.microsoft.com/v1.0/directoryRoles/{id}/members/{id}/$ref
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="4d49e-134">C#</span><span class="sxs-lookup"><span data-stu-id="4d49e-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-directoryobject-from-directoryrole-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="4d49e-135">Javascript</span><span class="sxs-lookup"><span data-stu-id="4d49e-135">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-directoryobject-from-directoryrole-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="4d49e-136">目的-C</span><span class="sxs-lookup"><span data-stu-id="4d49e-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-directoryobject-from-directoryrole-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="4d49e-137">応答</span><span class="sxs-lookup"><span data-stu-id="4d49e-137">Response</span></span>

<span data-ttu-id="4d49e-138">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="4d49e-138">Here is an example of the response.</span></span> 
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
