---
author: chackman
ms.author: chackman
title: 次のドライブのアイテム
ms.openlocfilehash: dcfe05e445baa4d01b2968c417648b6b65a17296
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27067597"
---
# <a name="follow-drive-item"></a><span data-ttu-id="34ef2-102">次のドライブのアイテム</span><span class="sxs-lookup"><span data-stu-id="34ef2-102">Follow drive item</span></span>

> <span data-ttu-id="34ef2-103">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="34ef2-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="34ef2-104">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="34ef2-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="34ef2-105">の[driveItem](../resources/driveitem.md)に従います。</span><span class="sxs-lookup"><span data-stu-id="34ef2-105">Follow a [driveItem](../resources/driveitem.md).</span></span>

><span data-ttu-id="34ef2-106">**注:** アイテムのフォローを取り消し、[フォロー取り消しの項目](driveitem-unfollow.md)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="34ef2-106">**Note:** To unfollow an item, see [Unfollow item](driveitem-unfollow.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="34ef2-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="34ef2-107">Permissions</span></span>

<span data-ttu-id="34ef2-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="34ef2-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="34ef2-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="34ef2-110">Permission type</span></span>      | <span data-ttu-id="34ef2-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="34ef2-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="34ef2-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="34ef2-112">Delegated (work or school account)</span></span> | <span data-ttu-id="34ef2-113">Files.Read、Files.ReadWrite、Files.Read.All、Files.ReadWrite.All、Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="34ef2-113">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="34ef2-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="34ef2-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="34ef2-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="34ef2-115">Not supported.</span></span>    |
|<span data-ttu-id="34ef2-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="34ef2-116">Application</span></span> | <span data-ttu-id="34ef2-117">Files.Read.All、Files.ReadWrite.All、Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="34ef2-117">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="34ef2-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="34ef2-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /drives/{drive-id}/items/{item-id}/follow
POST /groups/{group-id/drive/items/{item-id}/follow
POST /me/drive/items/{item-id}/follow
POST /sites/{site-id}/drive/items/{item-id}/follow
POST /users/{user-id}/drive/items/{item-id}/follow
```

## <a name="request-body"></a><span data-ttu-id="34ef2-119">要求本文</span><span class="sxs-lookup"><span data-stu-id="34ef2-119">Request body</span></span>

<span data-ttu-id="34ef2-120">要求の本文は必要ありません。</span><span class="sxs-lookup"><span data-stu-id="34ef2-120">No request body is required.</span></span>

## <a name="response"></a><span data-ttu-id="34ef2-121">応答</span><span class="sxs-lookup"><span data-stu-id="34ef2-121">Response</span></span>

<span data-ttu-id="34ef2-122">このメソッドでは、フォローされている項目については、 [DriveItem](../resources/driveitem.md)を返します。</span><span class="sxs-lookup"><span data-stu-id="34ef2-122">This method returns a [DriveItem](../resources/driveitem.md) for the item being followed.</span></span>

## <a name="example"></a><span data-ttu-id="34ef2-123">使用例</span><span class="sxs-lookup"><span data-stu-id="34ef2-123">Example</span></span>

<span data-ttu-id="34ef2-124">次の使用例は次によって識別される項目は、 `{item-id}`。</span><span class="sxs-lookup"><span data-stu-id="34ef2-124">This example follows an item identified by `{item-id}`.</span></span>

<!-- { "blockType": "request", "name": "follow-item", "scopes": "files.read", "target": "action" } -->

```http
POST /me/drive/items/{item-id}/follow
```

<!-- {
  "type": "#page.annotation",
  "description": "Follow an item.",
  "keywords": "follow item",
  "section": "documentation",
  "tocPath": "Items/Follow"
} -->

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
