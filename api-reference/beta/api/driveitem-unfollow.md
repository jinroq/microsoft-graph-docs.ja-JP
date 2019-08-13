---
author: chackman
ms.author: chackman
description: ユーザーがフォローしているアイテムのフォローを取り消します。
title: フォロー取り消しドライブ項目
localization_priority: Normal
ms.prod: sharepoint
doc_type: apiPageType
ms.openlocfilehash: 3ac8e3af809a9e324f69e66d1ef3c6f8f83aa840
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36320939"
---
# <a name="unfollow-drive-item"></a><span data-ttu-id="6b7ac-103">フォロー取り消しドライブ項目</span><span class="sxs-lookup"><span data-stu-id="6b7ac-103">Unfollow drive item</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6b7ac-104">[ドライブ](../resources/driveitem.md)のフォローを取り消します。</span><span class="sxs-lookup"><span data-stu-id="6b7ac-104">Unfollow a [driveItem](../resources/driveitem.md).</span></span>

><span data-ttu-id="6b7ac-105">**注:** アイテムをフォローするには、「[アイテムをフォロー](driveitem-follow.md)する」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="6b7ac-105">**Note:** To follow an item, see [Follow Item](driveitem-follow.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="6b7ac-106">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="6b7ac-106">Permissions</span></span>

<span data-ttu-id="6b7ac-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="6b7ac-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6b7ac-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="6b7ac-109">Permission type</span></span>      | <span data-ttu-id="6b7ac-110">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="6b7ac-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6b7ac-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="6b7ac-111">Delegated (work or school account)</span></span> | <span data-ttu-id="6b7ac-112">Files.Read、Files.ReadWrite、Files.Read.All、Files.ReadWrite.All、Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6b7ac-112">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="6b7ac-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="6b7ac-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6b7ac-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="6b7ac-114">Not supported.</span></span>    |
|<span data-ttu-id="6b7ac-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="6b7ac-115">Application</span></span> | <span data-ttu-id="6b7ac-116">Files.Read.All、Files.ReadWrite.All、Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6b7ac-116">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="6b7ac-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="6b7ac-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /me/drive/following/{item-id}
DELETE /users/{user-id}/drive/following/{item-id}
POST /me/drive/items/{item-id}/unfollow
POST /users/{user-id}/drive/items/{item-id}/unfollow
```

## <a name="request-body"></a><span data-ttu-id="6b7ac-118">要求本文</span><span class="sxs-lookup"><span data-stu-id="6b7ac-118">Request body</span></span>

<span data-ttu-id="6b7ac-119">要求の本文は必要ありません。</span><span class="sxs-lookup"><span data-stu-id="6b7ac-119">No request body is required.</span></span>

## <a name="response"></a><span data-ttu-id="6b7ac-120">応答</span><span class="sxs-lookup"><span data-stu-id="6b7ac-120">Response</span></span>

<span data-ttu-id="6b7ac-121">成功すると、API 呼び出しは `204 No Content` を返します。</span><span class="sxs-lookup"><span data-stu-id="6b7ac-121">If successful, the API call returns a `204 No Content`.</span></span> <span data-ttu-id="6b7ac-122">応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="6b7ac-122">It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6b7ac-123">例</span><span class="sxs-lookup"><span data-stu-id="6b7ac-123">Example</span></span>
### <a name="request"></a><span data-ttu-id="6b7ac-124">要求</span><span class="sxs-lookup"><span data-stu-id="6b7ac-124">Request</span></span>
<span data-ttu-id="6b7ac-125">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="6b7ac-125">Here is an example of the request.</span></span>
<span data-ttu-id="6b7ac-126">この例では、で識別さ`{item-id}`れるアイテムのフォローを取り消します。</span><span class="sxs-lookup"><span data-stu-id="6b7ac-126">This example unfollows an item identified by `{item-id}`.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="6b7ac-127">プロトコル</span><span class="sxs-lookup"><span data-stu-id="6b7ac-127">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "unfollow-item", "scopes": "files.read" } -->

```http
DELETE /me/drive/items/{item-id}/unfollow
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="6b7ac-128">C#</span><span class="sxs-lookup"><span data-stu-id="6b7ac-128">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/unfollow-item-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="6b7ac-129">JavaScript</span><span class="sxs-lookup"><span data-stu-id="6b7ac-129">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/unfollow-item-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="6b7ac-130">目的-C</span><span class="sxs-lookup"><span data-stu-id="6b7ac-130">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/unfollow-item-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="6b7ac-131">Java</span><span class="sxs-lookup"><span data-stu-id="6b7ac-131">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/unfollow-item-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="6b7ac-132">応答</span><span class="sxs-lookup"><span data-stu-id="6b7ac-132">Response</span></span>
<!-- { 
    "blockType": "response", 
    "truncated": true 
} -->
```http
HTTP/1.1 204 No Content
```
<!--
{
  "type": "#page.annotation",
  "description": "Unfollow an item that the user is following.",
  "keywords": "unfollow item",
  "section": "documentation",
  "tocPath": "Items/Unfollow",
  "suppressions": [
  ]
}
-->
