---
author: JeremyKelley
description: DriveItem へのアクセスを削除します。
ms.date: 09/10/2017
title: アイテムへのアクセスを削除する
localization_priority: Normal
doc_type: apiPageType
ms.prod: ''
ms.openlocfilehash: 0cc07dba0263516c0d02179ce81d85f9a6fea806
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/15/2019
ms.locfileid: "36413728"
---
# <a name="delete-a-sharing-permission-from-a-file-or-folder"></a><span data-ttu-id="5395a-103">ファイルまたはフォルダーの共有アクセス許可を削除する</span><span class="sxs-lookup"><span data-stu-id="5395a-103">Delete a sharing permission from a file or folder</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5395a-104">[DriveItem](../resources/driveitem.md) へのアクセスを削除します。</span><span class="sxs-lookup"><span data-stu-id="5395a-104">Remove access to a [DriveItem](../resources/driveitem.md).</span></span>

<span data-ttu-id="5395a-105">継承されて**いない**共有アクセス許可のみを削除することができます。</span><span class="sxs-lookup"><span data-stu-id="5395a-105">Only sharing permissions that are **not** inherited can be deleted.</span></span>
<span data-ttu-id="5395a-106">**InheritedFrom** プロパティは `null` である必要があります。</span><span class="sxs-lookup"><span data-stu-id="5395a-106">The **inheritedFrom** property must be `null`.</span></span>

## <a name="permissions"></a><span data-ttu-id="5395a-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="5395a-107">Permissions</span></span>
<span data-ttu-id="5395a-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="5395a-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5395a-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="5395a-110">Permission type</span></span>      | <span data-ttu-id="5395a-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="5395a-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5395a-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="5395a-112">Delegated (work or school account)</span></span> | <span data-ttu-id="5395a-113">Files.ReadWrite、Files.ReadWrite.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5395a-113">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="5395a-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="5395a-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5395a-115">Files.ReadWrite、Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5395a-115">Files.ReadWrite, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="5395a-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="5395a-116">Application</span></span> | <span data-ttu-id="5395a-117">Files.ReadWrite.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5395a-117">Files.ReadWrite.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="5395a-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="5395a-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
DELETE /drives/{drive-id}/items/{item-id}/permissions/{perm-id}
DELETE /groups/{group-id}/drive/items/{item-id}/permissions/{perm-id}
DELETE /me/drive/items/{item-id}/permissions/{perm-id}
DELETE /sites/{site-id}/drive/items/{item-id}/permissions/{perm-id}
DELETE /users/{user-id}/drive/items/{item-id}/permissions/{perm-id}
```

## <a name="optional-request-headers"></a><span data-ttu-id="5395a-119">オプションの要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="5395a-119">Optional request headers</span></span>

| <span data-ttu-id="5395a-120">名前</span><span class="sxs-lookup"><span data-stu-id="5395a-120">Name</span></span>          | <span data-ttu-id="5395a-121">型</span><span class="sxs-lookup"><span data-stu-id="5395a-121">Type</span></span>   | <span data-ttu-id="5395a-122">説明</span><span class="sxs-lookup"><span data-stu-id="5395a-122">Description</span></span>                                                                                                                                                                                       |
|:--------------|:-------|:--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="5395a-123">if-match</span><span class="sxs-lookup"><span data-stu-id="5395a-123">if-match</span></span>      | <span data-ttu-id="5395a-124">string</span><span class="sxs-lookup"><span data-stu-id="5395a-124">string</span></span> | <span data-ttu-id="5395a-125">この要求ヘッダーが含まれていて、指定された eTag (または cTag) が項目の現在のタグに一致しない場合には、`412 Precondition Failed` 応答が返され、項目は削除されません。</span><span class="sxs-lookup"><span data-stu-id="5395a-125">If this request header is included and the eTag (or cTag) provided does not match the current tag on the item, a `412 Precondition Failed` response is returned and the item will not be deleted.</span></span> |


## <a name="response"></a><span data-ttu-id="5395a-126">応答</span><span class="sxs-lookup"><span data-stu-id="5395a-126">Response</span></span>

<span data-ttu-id="5395a-127">成功した場合、このメソッドは `204 No Content` 応答コードを返します。</span><span class="sxs-lookup"><span data-stu-id="5395a-127">If successful, this method returns `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="5395a-128">例</span><span class="sxs-lookup"><span data-stu-id="5395a-128">Example</span></span>

<span data-ttu-id="5395a-129">この例では、現在のユーザーの OneDrive 内の項目 {item-id} から {perm-id} として識別されるアクセス許可を削除します。</span><span class="sxs-lookup"><span data-stu-id="5395a-129">This example removes the permission identified as {perm-id} from the item {item-id} in the current user's OneDrive.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="5395a-130">プロトコル</span><span class="sxs-lookup"><span data-stu-id="5395a-130">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "delete-permission", "scopes": "files.readwrite" }-->

```http
DELETE https://graph.microsoft.com/beta/me/drive/root/items/{item-id}/permissions/{perm-id}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="5395a-131">C#</span><span class="sxs-lookup"><span data-stu-id="5395a-131">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-permission-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="5395a-132">JavaScript</span><span class="sxs-lookup"><span data-stu-id="5395a-132">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-permission-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="5395a-133">目的-C</span><span class="sxs-lookup"><span data-stu-id="5395a-133">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-permission-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="5395a-134">応答</span><span class="sxs-lookup"><span data-stu-id="5395a-134">Response</span></span>

<!-- { "blockType": "response", "truncated": false } -->

```http
HTTP/1.1 204 No Content
```

## <a name="remarks"></a><span data-ttu-id="5395a-135">注釈</span><span class="sxs-lookup"><span data-stu-id="5395a-135">Remarks</span></span>

* <span data-ttu-id="5395a-136">`personal` (OneDrive Personal) の **driveType** を持つ[ドライブ](../resources/drive.md)は、DriveItem のルートでの作成やアクセス許可の変更を行えません。</span><span class="sxs-lookup"><span data-stu-id="5395a-136">[Drives](../resources/drive.md) with a **driveType** of `personal` (OneDrive Personal) cannot create or modify permissions on the root DriveItem.</span></span> 

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Remove an item's sharing permissions",
  "keywords": "permission, permissions, sharing, remove permissions, delete permissions",
  "section": "documentation",
  "tocPath": "OneDrive/Item/Delete permission",
  "suppressions": [
  ]
}
-->
