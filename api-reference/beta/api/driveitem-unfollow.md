---
author: chackman
ms.author: chackman
title: フォロー取り消しドライブ項目
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: e3ab51d5aaa4074837a0cd7126ac6548b09d4acd
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35860904"
---
# <a name="unfollow-drive-item"></a><span data-ttu-id="64613-102">フォロー取り消しドライブ項目</span><span class="sxs-lookup"><span data-stu-id="64613-102">Unfollow drive item</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="64613-103">[ドライブ](../resources/driveitem.md)のフォローを取り消します。</span><span class="sxs-lookup"><span data-stu-id="64613-103">Unfollow a [driveItem](../resources/driveitem.md).</span></span>

><span data-ttu-id="64613-104">**注:** アイテムをフォローするには、「[アイテムをフォロー](driveitem-follow.md)する」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="64613-104">**Note:** To follow an item, see [Follow Item](driveitem-follow.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="64613-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="64613-105">Permissions</span></span>

<span data-ttu-id="64613-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="64613-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="64613-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="64613-108">Permission type</span></span>      | <span data-ttu-id="64613-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="64613-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="64613-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="64613-110">Delegated (work or school account)</span></span> | <span data-ttu-id="64613-111">Files.Read、Files.ReadWrite、Files.Read.All、Files.ReadWrite.All、Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="64613-111">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="64613-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="64613-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="64613-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="64613-113">Not supported.</span></span>    |
|<span data-ttu-id="64613-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="64613-114">Application</span></span> | <span data-ttu-id="64613-115">Files.Read.All、Files.ReadWrite.All、Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="64613-115">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="64613-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="64613-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /me/drive/following/{item-id} 
DELETE /users/{user-id}/drive/following/{item-id}
```

## <a name="request-body"></a><span data-ttu-id="64613-117">要求本文</span><span class="sxs-lookup"><span data-stu-id="64613-117">Request body</span></span>

<span data-ttu-id="64613-118">要求の本文は必要ありません。</span><span class="sxs-lookup"><span data-stu-id="64613-118">No request body is required.</span></span>

## <a name="response"></a><span data-ttu-id="64613-119">応答</span><span class="sxs-lookup"><span data-stu-id="64613-119">Response</span></span>

<span data-ttu-id="64613-120">成功すると、API 呼び出しは `204 No Content` を返します。</span><span class="sxs-lookup"><span data-stu-id="64613-120">If successful, the API call returns a `204 No Content`.</span></span> <span data-ttu-id="64613-121">応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="64613-121">It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="64613-122">例</span><span class="sxs-lookup"><span data-stu-id="64613-122">Example</span></span>
### <a name="request"></a><span data-ttu-id="64613-123">要求</span><span class="sxs-lookup"><span data-stu-id="64613-123">Request</span></span>
<span data-ttu-id="64613-124">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="64613-124">Here is an example of the request.</span></span>
<span data-ttu-id="64613-125">この例では、で識別さ`{item-id}`れるアイテムのフォローを取り消します。</span><span class="sxs-lookup"><span data-stu-id="64613-125">This example unfollows an item identified by `{item-id}`.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="64613-126">プロトコル</span><span class="sxs-lookup"><span data-stu-id="64613-126">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "unfollow-item", "scopes": "files.read" } -->

```http
DELETE /me/drive/following/{item-id}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="64613-127">C#</span><span class="sxs-lookup"><span data-stu-id="64613-127">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/unfollow-item-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="64613-128">Javascript</span><span class="sxs-lookup"><span data-stu-id="64613-128">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/unfollow-item-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="64613-129">目的-C</span><span class="sxs-lookup"><span data-stu-id="64613-129">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/unfollow-item-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="64613-130">Java</span><span class="sxs-lookup"><span data-stu-id="64613-130">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/unfollow-item-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="64613-131">応答</span><span class="sxs-lookup"><span data-stu-id="64613-131">Response</span></span>
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
