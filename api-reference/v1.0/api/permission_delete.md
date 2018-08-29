---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: アイテムへのアクセスの削除
ms.openlocfilehash: 011345afb9789b0ff2927704a1e678f39656a719
ms.sourcegitcommit: abf4b739257e3ffd9d045f783ec595d846172590
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/21/2018
ms.locfileid: "23268621"
---
# <a name="delete-a-sharing-permission-from-a-file-or-folder"></a><span data-ttu-id="8552a-102">ファイルまたはフォルダーの共有アクセス許可を削除する</span><span class="sxs-lookup"><span data-stu-id="8552a-102">Delete a sharing permission from a file or folder</span></span>

<span data-ttu-id="8552a-103">[DriveItem](../resources/driveitem.md) へのアクセスを削除します。</span><span class="sxs-lookup"><span data-stu-id="8552a-103">Remove access to a [DriveItem](../resources/driveitem.md).</span></span>

<span data-ttu-id="8552a-104">継承されて**いない**共有アクセス許可のみを削除することができます。</span><span class="sxs-lookup"><span data-stu-id="8552a-104">Only sharing permissions that are **not** inherited can be deleted.</span></span>
<span data-ttu-id="8552a-105">**InheritedFrom** プロパティは `null` である必要があります。</span><span class="sxs-lookup"><span data-stu-id="8552a-105">The **inheritedFrom** property must be `null`.</span></span>

## <a name="permissions"></a><span data-ttu-id="8552a-106">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="8552a-106">Permissions</span></span>

<span data-ttu-id="8552a-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="8552a-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="8552a-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="8552a-109">Permission type</span></span>      | <span data-ttu-id="8552a-110">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="8552a-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8552a-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="8552a-111">Delegated (work or school account)</span></span> | <span data-ttu-id="8552a-112">Files.ReadWrite、Files.ReadWrite.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8552a-112">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="8552a-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="8552a-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8552a-114">Files.ReadWrite、Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8552a-114">Files.ReadWrite, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="8552a-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="8552a-115">Application</span></span> | <span data-ttu-id="8552a-116">Files.ReadWrite.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8552a-116">Files.ReadWrite.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="8552a-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="8552a-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /drives/{drive-id}/items/{item-id}/permissions/{perm-id}
DELETE /groups/{group-id}/drive/items/{item-id}/permissions/{perm-id}
DELETE /me/drive/items/{item-id}/permissions/{perm-id}
DELETE /sites/{site-id}/drive/items/{item-id}/permissions/{perm-id}
DELETE /users/{user-id}/drive/items/{item-id}/permissions/{perm-id}
```

## <a name="optional-request-headers"></a><span data-ttu-id="8552a-118">オプションの要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="8552a-118">Optional request headers</span></span>

| <span data-ttu-id="8552a-119">名前</span><span class="sxs-lookup"><span data-stu-id="8552a-119">Name</span></span>          | <span data-ttu-id="8552a-120">型</span><span class="sxs-lookup"><span data-stu-id="8552a-120">Type</span></span>   | <span data-ttu-id="8552a-121">説明</span><span class="sxs-lookup"><span data-stu-id="8552a-121">Description</span></span>                                                                                                                                                                                       |
|:--------------|:-------|:--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="8552a-122">if-match</span><span class="sxs-lookup"><span data-stu-id="8552a-122">if-match</span></span>      | <span data-ttu-id="8552a-123">文字列</span><span class="sxs-lookup"><span data-stu-id="8552a-123">string</span></span> | <span data-ttu-id="8552a-124">この要求ヘッダーが含まれていて、指定された eTag (または cTag) が項目の現在のタグに一致しない場合には、`412 Precondition Failed` 応答が返され、項目は削除されません。</span><span class="sxs-lookup"><span data-stu-id="8552a-124">If this request header is included and the eTag (or cTag) provided does not match the current tag on the item, a `412 Precondition Failed` response is returned and the item will not be deleted.</span></span> |

## <a name="response"></a><span data-ttu-id="8552a-125">応答</span><span class="sxs-lookup"><span data-stu-id="8552a-125">Response</span></span>

<span data-ttu-id="8552a-126">成功した場合、このメソッドは `204 No Content` 応答コードを返します。</span><span class="sxs-lookup"><span data-stu-id="8552a-126">If successful, this method returns `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="8552a-127">例</span><span class="sxs-lookup"><span data-stu-id="8552a-127">Example</span></span>

<span data-ttu-id="8552a-128">この例では、現在のユーザーの OneDrive 内の項目 {item-id} から {perm-id} として識別されるアクセス許可を削除します。</span><span class="sxs-lookup"><span data-stu-id="8552a-128">This example removes the permission identified as {perm-id} from the item {item-id} in the current user's OneDrive.</span></span>

<!-- { "blockType": "request", "name": "delete-permission", "scopes": "files.readwrite", "tags": "service.graph" }-->

```http
DELETE /me/drive/items/{item-id}/permissions/{perm-id}
```

### <a name="response"></a><span data-ttu-id="8552a-129">応答</span><span class="sxs-lookup"><span data-stu-id="8552a-129">Response</span></span>

<!-- { "blockType": "response", "truncated": false } -->

```http
HTTP/1.1 204 No Content
```

## <a name="remarks"></a><span data-ttu-id="8552a-130">注釈</span><span class="sxs-lookup"><span data-stu-id="8552a-130">Remarks</span></span>

* <span data-ttu-id="8552a-131">(OneDrive Personal) の **driveType** を持つ[ドライブ](../resources/drive.md)は、DriveItem のルートでの作成やアクセス許可の変更を行えません。`personal`</span><span class="sxs-lookup"><span data-stu-id="8552a-131">[Drives](../resources/drive.md) with a **driveType** of `personal` (OneDrive Personal) cannot create or modify permissions on the root DriveItem.</span></span> 

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Remove an item's sharing permissions",
  "keywords": "permission, permissions, sharing, remove permissions, delete permissions",
  "section": "documentation",
  "tocPath": "Sharing/Remove permissions"
} -->
