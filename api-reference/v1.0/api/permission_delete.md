---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: "アイテムへのアクセスの削除"
ms.openlocfilehash: cf573b49edc326ca221545657b29b1f2e86ba417
ms.sourcegitcommit: 7aea7a97e36e6d146214de3a90fdbc71628aadba
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/28/2017
---
# <a name="delete-a-sharing-permission-from-a-file-or-folder"></a><span data-ttu-id="fb02d-102">ファイルまたはフォルダーの共有アクセス許可を削除する</span><span class="sxs-lookup"><span data-stu-id="fb02d-102">Delete a sharing permission from a file or folder</span></span>

<span data-ttu-id="fb02d-103">[DriveItem](../resources/driveitem.md) へのアクセスを削除します。</span><span class="sxs-lookup"><span data-stu-id="fb02d-103">Remove access to a [DriveItem](../resources/driveitem.md).</span></span>

<span data-ttu-id="fb02d-104">継承されて**いない**共有アクセス許可のみを削除することができます。</span><span class="sxs-lookup"><span data-stu-id="fb02d-104">Only Permissions that are not inherited can be deleted.</span></span>
<span data-ttu-id="fb02d-105">**InheritedFrom** プロパティは `null` である必要があります。</span><span class="sxs-lookup"><span data-stu-id="fb02d-105">The **inheritedFrom** property must be `null`.</span></span>

## <a name="permissions"></a><span data-ttu-id="fb02d-106">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="fb02d-106">Permissions</span></span>

<span data-ttu-id="fb02d-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="fb02d-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="fb02d-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="fb02d-109">Permission type</span></span>      | <span data-ttu-id="fb02d-110">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="fb02d-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="fb02d-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="fb02d-111">Delegated (work or school account)</span></span> | <span data-ttu-id="fb02d-112">Files.ReadWrite、Files.ReadWrite.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fb02d-112">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="fb02d-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="fb02d-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="fb02d-114">Files.ReadWrite、Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fb02d-114">Files.ReadWrite, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="fb02d-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="fb02d-115">Application</span></span> | <span data-ttu-id="fb02d-116">Files.ReadWrite.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fb02d-116">Files.ReadWrite.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="fb02d-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="fb02d-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /drives/{drive-id}/items/{item-id}/permissions/{perm-id}
DELETE /groups/{group-id}/drive/items/{item-id}/permissions/{perm-id}
DELETE /me/drive/items/{item-id}/permissions/{perm-id}
DELETE /sites/{site-id}/drive/items/{item-id}/permissions/{perm-id}
DELETE /users/{user-id}/drive/items/{item-id}/permissions/{perm-id}
```

## <a name="optional-request-headers"></a><span data-ttu-id="fb02d-118">オプションの要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="fb02d-118">Optional request headers</span></span>

| <span data-ttu-id="fb02d-119">名前</span><span class="sxs-lookup"><span data-stu-id="fb02d-119">Name</span></span>          | <span data-ttu-id="fb02d-120">型</span><span class="sxs-lookup"><span data-stu-id="fb02d-120">Type</span></span>   | <span data-ttu-id="fb02d-121">説明</span><span class="sxs-lookup"><span data-stu-id="fb02d-121">Description</span></span>                                                                                                                                                                                       |
|:--------------|:-------|:--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="fb02d-122">if-match</span><span class="sxs-lookup"><span data-stu-id="fb02d-122">if-match</span></span>      | <span data-ttu-id="fb02d-123">string</span><span class="sxs-lookup"><span data-stu-id="fb02d-123">string</span></span> | <span data-ttu-id="fb02d-124">この要求ヘッダーが含まれていて、指定された eTag (または cTag) が項目の現在のタグに一致しない場合には、`412 Precondition Failed` 応答が返され、項目は削除されません。</span><span class="sxs-lookup"><span data-stu-id="fb02d-124">If this request header is included and the eTag (or cTag) provided does not match the current tag on the item, a `412 Precondition Failed` response is returned and the item will not be deleted.</span></span> |

## <a name="response"></a><span data-ttu-id="fb02d-125">応答</span><span class="sxs-lookup"><span data-stu-id="fb02d-125">Response</span></span>

<span data-ttu-id="fb02d-126">成功した場合、このメソッドは `204 No Content` 応答コードを返します。</span><span class="sxs-lookup"><span data-stu-id="fb02d-126">If successful, this method returns `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="fb02d-127">例</span><span class="sxs-lookup"><span data-stu-id="fb02d-127">Example</span></span>

<span data-ttu-id="fb02d-128">この例では、現在のユーザーの OneDrive のアイテム {item-id} から {perm-id} として識別されたアクセス許可を削除します。</span><span class="sxs-lookup"><span data-stu-id="fb02d-128">This example removes the permission identified as {perm-id} from the item {item-id} in the current user's OneDrive.</span></span>

<!-- { "blockType": "request", "name": "delete-permission", "scopes": "files.readwrite" }-->

```http
DELETE /me/drive/root/items/{item-id}/permissions/{perm-id}
```

### <a name="response"></a><span data-ttu-id="fb02d-129">応答</span><span class="sxs-lookup"><span data-stu-id="fb02d-129">Response</span></span>

<!-- { "blockType": "response", "truncated": false } -->

```http
HTTP/1.1 204 No Content
```

## <a name="remarks"></a><span data-ttu-id="fb02d-130">注釈</span><span class="sxs-lookup"><span data-stu-id="fb02d-130">Remarks</span></span>

* <span data-ttu-id="fb02d-131">`personal` (OneDrive Personal) の **driveType** を持つ[ドライブ](../resources/drive.md)は、DriveItem のルートでの作成やアクセス許可の変更を行えません。</span><span class="sxs-lookup"><span data-stu-id="fb02d-131">[Drives](../resources/drive.md) with a **driveType** of `personal` (OneDrive Personal) cannot create or modify permissions on the root DriveItem.</span></span> 

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Remove an item's sharing permissions",
  "keywords": "permission, permissions, sharing, remove permissions, delete permissions",
  "section": "documentation",
  "tocPath": "Sharing/Remove permissions"
} -->
