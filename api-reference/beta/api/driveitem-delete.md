---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: ファイルまたはフォルダーを削除する
ms.openlocfilehash: 13f872033a412791ac7196fbd23fbd679b8bb830
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27067902"
---
# <a name="delete-a-driveitem"></a><span data-ttu-id="a52e5-102">DriveItem を削除する</span><span class="sxs-lookup"><span data-stu-id="a52e5-102">Delete a DriveItem</span></span>

> <span data-ttu-id="a52e5-103">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="a52e5-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a52e5-104">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a52e5-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="a52e5-p102">[DriveItem](../resources/driveitem.md) を、ID またはパスを使用して削除します。このメソッドを使用して項目を削除すると、アイテムは完全に削除されず、ごみ箱に移動するだけであることに注意してください。</span><span class="sxs-lookup"><span data-stu-id="a52e5-p102">Delete a [DriveItem](../resources/driveitem.md) by using its ID or path. Note that deleting items using this method will move the items to the recycle bin instead of permanently deleting the item.</span></span>

## <a name="permissions"></a><span data-ttu-id="a52e5-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="a52e5-107">Permissions</span></span>

<span data-ttu-id="a52e5-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="a52e5-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a52e5-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="a52e5-110">Permission type</span></span>      | <span data-ttu-id="a52e5-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="a52e5-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a52e5-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="a52e5-112">Delegated (work or school account)</span></span> | <span data-ttu-id="a52e5-113">Files.ReadWrite、Files.ReadWrite.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a52e5-113">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="a52e5-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="a52e5-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a52e5-115">Files.ReadWrite、Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a52e5-115">Files.ReadWrite, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="a52e5-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="a52e5-116">Application</span></span> | <span data-ttu-id="a52e5-117">Files.ReadWrite.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a52e5-117">Files.ReadWrite.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="a52e5-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="a52e5-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /drives/{drive-id}/items/{item-id}
DELETE /groups/{group-id}/drive/items/{item-id}
DELETE /me/drive/items/{item-id}
DELETE /sites/{siteId}/drive/items/{itemId}
DELETE /users/{userId}/drive/items/{itemId}
```

## <a name="optional-request-headers"></a><span data-ttu-id="a52e5-119">オプションの要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="a52e5-119">Optional request headers</span></span>

| <span data-ttu-id="a52e5-120">名前</span><span class="sxs-lookup"><span data-stu-id="a52e5-120">Name</span></span>          | <span data-ttu-id="a52e5-121">型</span><span class="sxs-lookup"><span data-stu-id="a52e5-121">Type</span></span>   | <span data-ttu-id="a52e5-122">説明</span><span class="sxs-lookup"><span data-stu-id="a52e5-122">Description</span></span>                                                                                                                                                                                       |
|:--------------|:-------|:--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="a52e5-123">if-match</span><span class="sxs-lookup"><span data-stu-id="a52e5-123">if-match</span></span>      | <span data-ttu-id="a52e5-124">String</span><span class="sxs-lookup"><span data-stu-id="a52e5-124">String</span></span> | <span data-ttu-id="a52e5-125">この要求ヘッダーが含まれていて、指定された eTag (または cTag) が項目の現在のタグに一致しない場合には、`412 Precondition Failed` 応答が返され、項目は削除されません。</span><span class="sxs-lookup"><span data-stu-id="a52e5-125">If this request header is included and the eTag (or cTag) provided does not match the current tag on the item, a `412 Precondition Failed` response is returned and the item will not be deleted.</span></span> |

## <a name="example"></a><span data-ttu-id="a52e5-126">例</span><span class="sxs-lookup"><span data-stu-id="a52e5-126">Example</span></span>

<span data-ttu-id="a52e5-127">以下は、この API を呼び出す方法の例です。</span><span class="sxs-lookup"><span data-stu-id="a52e5-127">Here is an example of how to call this API.</span></span>

<!-- { "blockType": "request", "name": "delete-item", "scopes": "files.readwrite" } -->

```http
DELETE /me/drive/items/{item-id}
```

## <a name="response"></a><span data-ttu-id="a52e5-128">応答</span><span class="sxs-lookup"><span data-stu-id="a52e5-128">Response</span></span>

<span data-ttu-id="a52e5-129">成功した場合、この呼び出しはリソースが削除され返すものがなかったことを示す `204 No Content` 応答を返します。</span><span class="sxs-lookup"><span data-stu-id="a52e5-129">If successful, this call returns a `204 No Content` response to indicate that resource was deleted and there was nothing to return.</span></span>

<!-- { "blockType": "response" } -->

```http
HTTP/1.1 204 No Content
```

### <a name="error-responses"></a><span data-ttu-id="a52e5-130">エラー応答</span><span class="sxs-lookup"><span data-stu-id="a52e5-130">Error responses</span></span>

<span data-ttu-id="a52e5-131">エラーがどのように返されるかについては、「[エラー応答][error-response]」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="a52e5-131">See [Error Responses][error-response] for more info about how errors are returned.</span></span>

[error-response]: /graph/errors

<!-- {
  "type": "#page.annotation",
  "description": "Delete a DriveItem from a drive",
  "keywords": "delete,existing item,onedrive",
  "section": "documentation",
  "tocPath": "Items/Delete"
} -->
