---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: ファイルをチェック アウト
ms.openlocfilehash: c8b7cd9231150d9898ea21a15c4745791137cdba
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27067900"
---
# <a name="check-out-a-driveitem-resource"></a><span data-ttu-id="fe183-102">DriveItem リソースをチェックアウトする</span><span class="sxs-lookup"><span data-stu-id="fe183-102">Check-out a DriveItem resource</span></span>

> <span data-ttu-id="fe183-103">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="fe183-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="fe183-104">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="fe183-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="fe183-105">driveItem リソースをチェックアウトして、他者がドキュメントを編集できないようにします。また、ドキュメントが[チェックイン](driveitem-checkin.md)されるまで、変更内容が表示されないようにします。</span><span class="sxs-lookup"><span data-stu-id="fe183-105">Check-out a driveItem resource to prevent others from editing the document, and your changes from being visible until the documented is [checked-in](driveitem-checkin.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="fe183-106">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="fe183-106">Permissions</span></span>

<span data-ttu-id="fe183-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="fe183-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fe183-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="fe183-109">Permission type</span></span>      | <span data-ttu-id="fe183-110">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="fe183-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="fe183-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="fe183-111">Delegated (work or school account)</span></span> | <span data-ttu-id="fe183-112">Files.ReadWrite、Files.ReadWrite.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fe183-112">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="fe183-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="fe183-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="fe183-114">Files.ReadWrite、Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fe183-114">Files.ReadWrite, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="fe183-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="fe183-115">Application</span></span> | <span data-ttu-id="fe183-116">Files.ReadWrite.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fe183-116">Files.ReadWrite.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="fe183-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="fe183-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /drives/{driveId}/items/{itemId}/checkout
POST /groups/{groupId}/drive/items/{itemId}/checkout
POST /me/drive/items/{item-id}/checkout
POST /sites/{siteId}/drive/items/{itemId}/checkout
POST /users/{userId}/drive/items/{itemId}/checkout
```

### <a name="request-body"></a><span data-ttu-id="fe183-118">要求本文</span><span class="sxs-lookup"><span data-stu-id="fe183-118">Request body</span></span>

<span data-ttu-id="fe183-119">要求の本文は必要ありません。</span><span class="sxs-lookup"><span data-stu-id="fe183-119">No request body is required.</span></span>

## <a name="example"></a><span data-ttu-id="fe183-120">例</span><span class="sxs-lookup"><span data-stu-id="fe183-120">Example</span></span>

<span data-ttu-id="fe183-121">この例では、`{item-id}` で識別されるファイルをチェックアウトします。</span><span class="sxs-lookup"><span data-stu-id="fe183-121">This example checks out a file identified by `{item-id}`.</span></span>

<!-- { "blockType": "request", "name": "checkout-item", "scopes": "files.readwrite", "target": "action" } -->

```http
POST /drives/{drive-id}/items/{item-id}/checkout
```

## <a name="response"></a><span data-ttu-id="fe183-122">応答</span><span class="sxs-lookup"><span data-stu-id="fe183-122">Response</span></span>

<span data-ttu-id="fe183-123">成功すると、API 呼び出しは `204 No content` を返します。</span><span class="sxs-lookup"><span data-stu-id="fe183-123">If successful, the API call returns a `204 No content`.</span></span>

<!-- { "blockType": "response" } -->

```http
HTTP/1.1 204 No content
```

### <a name="remarks"></a><span data-ttu-id="fe183-124">備考</span><span class="sxs-lookup"><span data-stu-id="fe183-124">Remarks</span></span>


[item-resource]: ../resources/driveitem.md

<!-- {
  "type": "#page.annotation",
  "description": "Create a copy of an existing item.",
  "keywords": "copy existing item",
  "section": "documentation",
  "tocPath": "Items/Copy"
} -->
