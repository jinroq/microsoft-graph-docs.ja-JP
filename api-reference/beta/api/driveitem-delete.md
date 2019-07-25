---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: ファイルまたはフォルダーを削除する
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: d4b3222e25d715b64ead1a91c1d3b21e033b2ca6
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35861259"
---
# <a name="delete-a-driveitem"></a><span data-ttu-id="938e9-102">DriveItem を削除する</span><span class="sxs-lookup"><span data-stu-id="938e9-102">Delete a DriveItem</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="938e9-p101">[DriveItem](../resources/driveitem.md) を、ID またはパスを使用して削除します。このメソッドを使用して項目を削除すると、アイテムは完全に削除されず、ごみ箱に移動するだけであることに注意してください。</span><span class="sxs-lookup"><span data-stu-id="938e9-p101">Delete a [DriveItem](../resources/driveitem.md) by using its ID or path. Note that deleting items using this method will move the items to the recycle bin instead of permanently deleting the item.</span></span>

## <a name="permissions"></a><span data-ttu-id="938e9-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="938e9-105">Permissions</span></span>

<span data-ttu-id="938e9-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="938e9-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="938e9-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="938e9-108">Permission type</span></span>      | <span data-ttu-id="938e9-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="938e9-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="938e9-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="938e9-110">Delegated (work or school account)</span></span> | <span data-ttu-id="938e9-111">Files.ReadWrite、Files.ReadWrite.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="938e9-111">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="938e9-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="938e9-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="938e9-113">Files.ReadWrite、Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="938e9-113">Files.ReadWrite, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="938e9-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="938e9-114">Application</span></span> | <span data-ttu-id="938e9-115">Files.ReadWrite.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="938e9-115">Files.ReadWrite.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="938e9-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="938e9-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /drives/{drive-id}/items/{item-id}
DELETE /groups/{group-id}/drive/items/{item-id}
DELETE /me/drive/items/{item-id}
DELETE /sites/{siteId}/drive/items/{itemId}
DELETE /users/{userId}/drive/items/{itemId}
```

## <a name="optional-request-headers"></a><span data-ttu-id="938e9-117">オプションの要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="938e9-117">Optional request headers</span></span>

| <span data-ttu-id="938e9-118">名前</span><span class="sxs-lookup"><span data-stu-id="938e9-118">Name</span></span>          | <span data-ttu-id="938e9-119">型</span><span class="sxs-lookup"><span data-stu-id="938e9-119">Type</span></span>   | <span data-ttu-id="938e9-120">説明</span><span class="sxs-lookup"><span data-stu-id="938e9-120">Description</span></span>                                                                                                                                                                                       |
|:--------------|:-------|:--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="938e9-121">if-match</span><span class="sxs-lookup"><span data-stu-id="938e9-121">if-match</span></span>      | <span data-ttu-id="938e9-122">String</span><span class="sxs-lookup"><span data-stu-id="938e9-122">String</span></span> | <span data-ttu-id="938e9-123">この要求ヘッダーが含まれていて、指定された eTag (または cTag) が項目の現在のタグに一致しない場合には、`412 Precondition Failed` 応答が返され、項目は削除されません。</span><span class="sxs-lookup"><span data-stu-id="938e9-123">If this request header is included and the eTag (or cTag) provided does not match the current tag on the item, a `412 Precondition Failed` response is returned and the item will not be deleted.</span></span> |

## <a name="example"></a><span data-ttu-id="938e9-124">例</span><span class="sxs-lookup"><span data-stu-id="938e9-124">Example</span></span>

<span data-ttu-id="938e9-125">以下は、この API を呼び出す方法の例です。</span><span class="sxs-lookup"><span data-stu-id="938e9-125">Here is an example of how to call this API.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="938e9-126">プロトコル</span><span class="sxs-lookup"><span data-stu-id="938e9-126">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "delete-drive-item", "scopes": "files.readwrite" } -->

```http
DELETE /me/drive/items/{item-id}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="938e9-127">C#</span><span class="sxs-lookup"><span data-stu-id="938e9-127">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-drive-item-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="938e9-128">Javascript</span><span class="sxs-lookup"><span data-stu-id="938e9-128">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-drive-item-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="938e9-129">目的-C</span><span class="sxs-lookup"><span data-stu-id="938e9-129">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-drive-item-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="938e9-130">Java</span><span class="sxs-lookup"><span data-stu-id="938e9-130">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-drive-item-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


## <a name="response"></a><span data-ttu-id="938e9-131">応答</span><span class="sxs-lookup"><span data-stu-id="938e9-131">Response</span></span>

<span data-ttu-id="938e9-132">成功した場合、この呼び出しはリソースが削除され返すものがなかったことを示す `204 No Content` 応答を返します。</span><span class="sxs-lookup"><span data-stu-id="938e9-132">If successful, this call returns a `204 No Content` response to indicate that resource was deleted and there was nothing to return.</span></span>

<!-- { "blockType": "response" } -->

```http
HTTP/1.1 204 No Content
```

### <a name="error-responses"></a><span data-ttu-id="938e9-133">エラー応答</span><span class="sxs-lookup"><span data-stu-id="938e9-133">Error responses</span></span>

<span data-ttu-id="938e9-134">エラーがどのように返されるかについては、「[エラー応答][error-response]」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="938e9-134">See [Error Responses][error-response] for more info about how errors are returned.</span></span>

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
