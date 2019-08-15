---
author: JeremyKelley
description: DriveItem を、ID またはパスを使用して削除します。
ms.date: 09/10/2017
title: ファイルまたはフォルダーを削除する
localization_priority: Normal
ms.prod: sharepoint
doc_type: apiPageType
ms.openlocfilehash: 5ff1e8ed83026d5b91738cff8204271bc8739068
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/15/2019
ms.locfileid: "36416848"
---
# <a name="delete-a-driveitem"></a><span data-ttu-id="6d73f-103">DriveItem を削除する</span><span class="sxs-lookup"><span data-stu-id="6d73f-103">Delete a DriveItem</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6d73f-p101">[DriveItem](../resources/driveitem.md) を、ID またはパスを使用して削除します。このメソッドを使用して項目を削除すると、アイテムは完全に削除されず、ごみ箱に移動するだけであることに注意してください。</span><span class="sxs-lookup"><span data-stu-id="6d73f-p101">Delete a [DriveItem](../resources/driveitem.md) by using its ID or path. Note that deleting items using this method will move the items to the recycle bin instead of permanently deleting the item.</span></span>

## <a name="permissions"></a><span data-ttu-id="6d73f-106">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="6d73f-106">Permissions</span></span>

<span data-ttu-id="6d73f-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="6d73f-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6d73f-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="6d73f-109">Permission type</span></span>      | <span data-ttu-id="6d73f-110">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="6d73f-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6d73f-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="6d73f-111">Delegated (work or school account)</span></span> | <span data-ttu-id="6d73f-112">Files.ReadWrite、Files.ReadWrite.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6d73f-112">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="6d73f-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="6d73f-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6d73f-114">Files.ReadWrite、Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6d73f-114">Files.ReadWrite, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="6d73f-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="6d73f-115">Application</span></span> | <span data-ttu-id="6d73f-116">Files.ReadWrite.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6d73f-116">Files.ReadWrite.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="6d73f-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="6d73f-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /drives/{drive-id}/items/{item-id}
DELETE /groups/{group-id}/drive/items/{item-id}
DELETE /me/drive/items/{item-id}
DELETE /sites/{siteId}/drive/items/{itemId}
DELETE /users/{userId}/drive/items/{itemId}
```

## <a name="optional-request-headers"></a><span data-ttu-id="6d73f-118">オプションの要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="6d73f-118">Optional request headers</span></span>

| <span data-ttu-id="6d73f-119">名前</span><span class="sxs-lookup"><span data-stu-id="6d73f-119">Name</span></span>          | <span data-ttu-id="6d73f-120">型</span><span class="sxs-lookup"><span data-stu-id="6d73f-120">Type</span></span>   | <span data-ttu-id="6d73f-121">説明</span><span class="sxs-lookup"><span data-stu-id="6d73f-121">Description</span></span>                                                                                                                                                                                       |
|:--------------|:-------|:--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="6d73f-122">if-match</span><span class="sxs-lookup"><span data-stu-id="6d73f-122">if-match</span></span>      | <span data-ttu-id="6d73f-123">String</span><span class="sxs-lookup"><span data-stu-id="6d73f-123">String</span></span> | <span data-ttu-id="6d73f-124">この要求ヘッダーが含まれていて、指定された eTag (または cTag) が項目の現在のタグに一致しない場合には、`412 Precondition Failed` 応答が返され、項目は削除されません。</span><span class="sxs-lookup"><span data-stu-id="6d73f-124">If this request header is included and the eTag (or cTag) provided does not match the current tag on the item, a `412 Precondition Failed` response is returned and the item will not be deleted.</span></span> |

## <a name="example"></a><span data-ttu-id="6d73f-125">例</span><span class="sxs-lookup"><span data-stu-id="6d73f-125">Example</span></span>

<span data-ttu-id="6d73f-126">以下は、この API を呼び出す方法の例です。</span><span class="sxs-lookup"><span data-stu-id="6d73f-126">Here is an example of how to call this API.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="6d73f-127">プロトコル</span><span class="sxs-lookup"><span data-stu-id="6d73f-127">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "delete-drive-item", "scopes": "files.readwrite" } -->

```http
DELETE /me/drive/items/{item-id}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="6d73f-128">C#</span><span class="sxs-lookup"><span data-stu-id="6d73f-128">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-drive-item-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="6d73f-129">JavaScript</span><span class="sxs-lookup"><span data-stu-id="6d73f-129">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-drive-item-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="6d73f-130">目的-C</span><span class="sxs-lookup"><span data-stu-id="6d73f-130">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-drive-item-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


## <a name="response"></a><span data-ttu-id="6d73f-131">応答</span><span class="sxs-lookup"><span data-stu-id="6d73f-131">Response</span></span>

<span data-ttu-id="6d73f-132">成功した場合、この呼び出しはリソースが削除され返すものがなかったことを示す `204 No Content` 応答を返します。</span><span class="sxs-lookup"><span data-stu-id="6d73f-132">If successful, this call returns a `204 No Content` response to indicate that resource was deleted and there was nothing to return.</span></span>

<!-- { "blockType": "response" } -->

```http
HTTP/1.1 204 No Content
```

### <a name="error-responses"></a><span data-ttu-id="6d73f-133">エラー応答</span><span class="sxs-lookup"><span data-stu-id="6d73f-133">Error responses</span></span>

<span data-ttu-id="6d73f-134">エラーがどのように返されるかについては、「[エラー応答][error-response]」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="6d73f-134">See [Error Responses][error-response] for more info about how errors are returned.</span></span>

[error-response]: /graph/errors

<!--
{
  "type": "#page.annotation",
  "description": "Delete a DriveItem from a drive",
  "keywords": "delete,existing item,onedrive",
  "section": "documentation",
  "tocPath": "Items/Delete",
  "suppressions": [
  ]
}
-->
