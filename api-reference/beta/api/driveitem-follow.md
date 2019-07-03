---
author: chackman
ms.author: chackman
title: ドライブアイテムをフォローする
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 1dc7cdd1f863687773236fee927b6c5a37cf82ea
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/02/2019
ms.locfileid: "35436425"
---
# <a name="follow-drive-item"></a><span data-ttu-id="db5ed-102">ドライブアイテムをフォローする</span><span class="sxs-lookup"><span data-stu-id="db5ed-102">Follow drive item</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="db5ed-103">[ドライブ項目](../resources/driveitem.md)をフォローします。</span><span class="sxs-lookup"><span data-stu-id="db5ed-103">Follow a [driveItem](../resources/driveitem.md).</span></span>

><span data-ttu-id="db5ed-104">**注:** アイテムのフォローを取り消したい場合は、「[アイテムをフォロー](driveitem-unfollow.md)取り消し」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="db5ed-104">**Note:** To unfollow an item, see [Unfollow item](driveitem-unfollow.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="db5ed-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="db5ed-105">Permissions</span></span>

<span data-ttu-id="db5ed-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="db5ed-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="db5ed-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="db5ed-108">Permission type</span></span>      | <span data-ttu-id="db5ed-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="db5ed-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="db5ed-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="db5ed-110">Delegated (work or school account)</span></span> | <span data-ttu-id="db5ed-111">Files.Read、Files.ReadWrite、Files.Read.All、Files.ReadWrite.All、Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="db5ed-111">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="db5ed-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="db5ed-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="db5ed-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="db5ed-113">Not supported.</span></span>    |
|<span data-ttu-id="db5ed-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="db5ed-114">Application</span></span> | <span data-ttu-id="db5ed-115">Files.Read.All、Files.ReadWrite.All、Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="db5ed-115">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="db5ed-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="db5ed-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /drives/{drive-id}/items/{item-id}/follow
POST /groups/{group-id/drive/items/{item-id}/follow
POST /me/drive/items/{item-id}/follow
POST /sites/{site-id}/drive/items/{item-id}/follow
POST /users/{user-id}/drive/items/{item-id}/follow
```

## <a name="request-body"></a><span data-ttu-id="db5ed-117">要求本文</span><span class="sxs-lookup"><span data-stu-id="db5ed-117">Request body</span></span>

<span data-ttu-id="db5ed-118">要求の本文は必要ありません。</span><span class="sxs-lookup"><span data-stu-id="db5ed-118">No request body is required.</span></span>

## <a name="response"></a><span data-ttu-id="db5ed-119">応答</span><span class="sxs-lookup"><span data-stu-id="db5ed-119">Response</span></span>

<span data-ttu-id="db5ed-120">このメソッドは、フォローされているアイテムの[ドライブ項目](../resources/driveitem.md)を返します。</span><span class="sxs-lookup"><span data-stu-id="db5ed-120">This method returns a [DriveItem](../resources/driveitem.md) for the item being followed.</span></span>

## <a name="example"></a><span data-ttu-id="db5ed-121">例</span><span class="sxs-lookup"><span data-stu-id="db5ed-121">Example</span></span>

<span data-ttu-id="db5ed-122">この例では、で`{item-id}`識別されるアイテムをフォローします。</span><span class="sxs-lookup"><span data-stu-id="db5ed-122">This example follows an item identified by `{item-id}`.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="db5ed-123">プロトコル</span><span class="sxs-lookup"><span data-stu-id="db5ed-123">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "follow-item", "scopes": "files.read", "target": "action" } -->

```http
POST /me/drive/items/{item-id}/follow
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="db5ed-124">C#</span><span class="sxs-lookup"><span data-stu-id="db5ed-124">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/follow-item-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="db5ed-125">Javascript</span><span class="sxs-lookup"><span data-stu-id="db5ed-125">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/follow-item-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="db5ed-126">目的-C</span><span class="sxs-lookup"><span data-stu-id="db5ed-126">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/follow-item-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<!--
{
  "type": "#page.annotation",
  "description": "Follow an item.",
  "keywords": "follow item",
  "section": "documentation",
  "tocPath": "Items/Follow",
  "suppressions": [
  ]
}
-->

<!-- { "blockType": "response", "@odata.type": "microsoft.graph.driveItem", "truncated": true } -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "id": "1312abc!1231",
  "name": "March Proposal.docx",
  "size": 19121,
  "lastModifiedDateTime": "2017-12-12T10:40:59Z"
}
```
