---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: アイテムへのアクセスの削除
ms.openlocfilehash: 726818b14a694380e46bfd38280e4cba9effb67d
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27071641"
---
# <a name="delete-a-sharing-permission-from-a-file-or-folder"></a><span data-ttu-id="6ed95-102">ファイルまたはフォルダーの共有アクセス許可を削除する</span><span class="sxs-lookup"><span data-stu-id="6ed95-102">Delete a sharing permission from a file or folder</span></span>

> <span data-ttu-id="6ed95-103">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="6ed95-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="6ed95-104">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="6ed95-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="6ed95-105">[DriveItem](../resources/driveitem.md) へのアクセスを削除します。</span><span class="sxs-lookup"><span data-stu-id="6ed95-105">Remove access to a [DriveItem](../resources/driveitem.md).</span></span>

<span data-ttu-id="6ed95-106">継承されて**いない**共有アクセス許可のみを削除することができます。</span><span class="sxs-lookup"><span data-stu-id="6ed95-106">Only sharing permissions that are **not** inherited can be deleted.</span></span>
<span data-ttu-id="6ed95-107">**InheritedFrom** プロパティは `null` である必要があります。</span><span class="sxs-lookup"><span data-stu-id="6ed95-107">The **inheritedFrom** property must be `null`.</span></span>

## <a name="permissions"></a><span data-ttu-id="6ed95-108">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="6ed95-108">Permissions</span></span>
<span data-ttu-id="6ed95-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="6ed95-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6ed95-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="6ed95-111">Permission type</span></span>      | <span data-ttu-id="6ed95-112">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="6ed95-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6ed95-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="6ed95-113">Delegated (work or school account)</span></span> | <span data-ttu-id="6ed95-114">Files.ReadWrite、Files.ReadWrite.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6ed95-114">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="6ed95-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="6ed95-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6ed95-116">Files.ReadWrite、Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6ed95-116">Files.ReadWrite, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="6ed95-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="6ed95-117">Application</span></span> | <span data-ttu-id="6ed95-118">Files.ReadWrite.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6ed95-118">Files.ReadWrite.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="6ed95-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="6ed95-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
DELETE /drives/{drive-id}/items/{item-id}/permissions/{perm-id}
DELETE /groups/{group-id}/drive/items/{item-id}/permissions/{perm-id}
DELETE /me/drive/items/{item-id}/permissions/{perm-id}
DELETE /sites/{site-id}/drive/items/{item-id}/permissions/{perm-id}
DELETE /users/{user-id}/drive/items/{item-id}/permissions/{perm-id}
```

## <a name="optional-request-headers"></a><span data-ttu-id="6ed95-120">オプションの要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="6ed95-120">Optional request headers</span></span>

| <span data-ttu-id="6ed95-121">名前</span><span class="sxs-lookup"><span data-stu-id="6ed95-121">Name</span></span>          | <span data-ttu-id="6ed95-122">型</span><span class="sxs-lookup"><span data-stu-id="6ed95-122">Type</span></span>   | <span data-ttu-id="6ed95-123">説明</span><span class="sxs-lookup"><span data-stu-id="6ed95-123">Description</span></span>                                                                                                                                                                                       |
|:--------------|:-------|:--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="6ed95-124">if-match</span><span class="sxs-lookup"><span data-stu-id="6ed95-124">if-match</span></span>      | <span data-ttu-id="6ed95-125">文字列</span><span class="sxs-lookup"><span data-stu-id="6ed95-125">string</span></span> | <span data-ttu-id="6ed95-126">この要求ヘッダーが含まれていて、指定された eTag (または cTag) が項目の現在のタグに一致しない場合には、`412 Precondition Failed` 応答が返され、項目は削除されません。</span><span class="sxs-lookup"><span data-stu-id="6ed95-126">If this request header is included and the eTag (or cTag) provided does not match the current tag on the item, a `412 Precondition Failed` response is returned and the item will not be deleted.</span></span> |


## <a name="response"></a><span data-ttu-id="6ed95-127">応答</span><span class="sxs-lookup"><span data-stu-id="6ed95-127">Response</span></span>

<span data-ttu-id="6ed95-128">成功した場合、このメソッドは `204 No Content` 応答コードを返します。</span><span class="sxs-lookup"><span data-stu-id="6ed95-128">If successful, this method returns `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="6ed95-129">例</span><span class="sxs-lookup"><span data-stu-id="6ed95-129">Example</span></span>

<span data-ttu-id="6ed95-130">この例では、現在のユーザーの OneDrive 内の項目 {item-id} から {perm-id} として識別されるアクセス許可を削除します。</span><span class="sxs-lookup"><span data-stu-id="6ed95-130">This example removes the permission identified as {perm-id} from the item {item-id} in the current user's OneDrive.</span></span>

<!-- { "blockType": "request", "name": "delete-permission", "scopes": "files.readwrite" }-->

```http
DELETE https://graph.microsoft.com/beta/me/drive/root/items/{item-id}/permissions/{perm-id}
```

### <a name="response"></a><span data-ttu-id="6ed95-131">応答</span><span class="sxs-lookup"><span data-stu-id="6ed95-131">Response</span></span>

<!-- { "blockType": "response", "truncated": false } -->

```http
HTTP/1.1 204 No Content
```

## <a name="remarks"></a><span data-ttu-id="6ed95-132">注釈</span><span class="sxs-lookup"><span data-stu-id="6ed95-132">Remarks</span></span>

* <span data-ttu-id="6ed95-133">`personal` (OneDrive Personal) の **driveType** を持つ[ドライブ](../resources/drive.md)は、DriveItem のルートでの作成やアクセス許可の変更を行えません。</span><span class="sxs-lookup"><span data-stu-id="6ed95-133">[Drives](../resources/drive.md) with a **driveType** of `personal` (OneDrive Personal) cannot create or modify permissions on the root DriveItem.</span></span> 

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Remove an item's sharing permissions",
  "keywords": "permission, permissions, sharing, remove permissions, delete permissions",
  "section": "documentation",
  "tocPath": "OneDrive/Item/Delete permission"
}-->
