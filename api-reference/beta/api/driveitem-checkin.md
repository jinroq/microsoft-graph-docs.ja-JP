---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: ファイルをチェックインします。
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: fb62dc05c60e26a6d1d6683913eeec0403d1c41c
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27950810"
---
# <a name="check-in-changes-to-a-driveitem-resource"></a><span data-ttu-id="f2d97-102">DriveItem リソースへの変更をチェックインする</span><span class="sxs-lookup"><span data-stu-id="f2d97-102">Check-in changes to a DriveItem resource</span></span>

> <span data-ttu-id="f2d97-103">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="f2d97-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f2d97-104">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f2d97-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="f2d97-105">チェックアウトされた DriveItem リソースをチェックインします。これにより、他のユーザーがドキュメントのバージョンを利用できるようになります。</span><span class="sxs-lookup"><span data-stu-id="f2d97-105">Check-in a checked out DriveItem resource, which makes the version of the document available to others.</span></span>

## <a name="permissions"></a><span data-ttu-id="f2d97-106">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="f2d97-106">Permissions</span></span>

<span data-ttu-id="f2d97-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="f2d97-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f2d97-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="f2d97-109">Permission type</span></span>      | <span data-ttu-id="f2d97-110">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="f2d97-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f2d97-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="f2d97-111">Delegated (work or school account)</span></span> | <span data-ttu-id="f2d97-112">Files.ReadWrite、Files.ReadWrite.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f2d97-112">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="f2d97-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="f2d97-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f2d97-114">Files.ReadWrite、Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f2d97-114">Files.ReadWrite, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="f2d97-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="f2d97-115">Application</span></span> | <span data-ttu-id="f2d97-116">Files.ReadWrite.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f2d97-116">Files.ReadWrite.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="f2d97-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="f2d97-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /drives/{driveId}/items/{itemId}/checkin
POST /groups/{groupId}/drive/items/{itemId}/checkin
POST /me/drive/items/{item-id}/checkin
POST /sites/{siteId}/drive/items/{itemId}/checkin
POST /users/{userId}/drive/items/{itemId}/checkin
```

### <a name="request-body"></a><span data-ttu-id="f2d97-118">要求本文</span><span class="sxs-lookup"><span data-stu-id="f2d97-118">Request body</span></span>

<span data-ttu-id="f2d97-119">要求本文で、次のパラメーターを含む JSON オブジェクトを指定します。</span><span class="sxs-lookup"><span data-stu-id="f2d97-119">In the request body, provide a JSON object with the following parameters.</span></span>


|   <span data-ttu-id="f2d97-120">名前</span><span class="sxs-lookup"><span data-stu-id="f2d97-120">Name</span></span>    | <span data-ttu-id="f2d97-121">値</span><span class="sxs-lookup"><span data-stu-id="f2d97-121">Value</span></span>  |                                                <span data-ttu-id="f2d97-122">説明</span><span class="sxs-lookup"><span data-stu-id="f2d97-122">Description</span></span>                                                |
| :-------- | :----- | :-------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="f2d97-123">checkInAs</span><span class="sxs-lookup"><span data-stu-id="f2d97-123">checkInAs</span></span> | <span data-ttu-id="f2d97-124">文字列</span><span class="sxs-lookup"><span data-stu-id="f2d97-124">string</span></span> | <span data-ttu-id="f2d97-125">省略可能。</span><span class="sxs-lookup"><span data-stu-id="f2d97-125">Optional.</span></span> <span data-ttu-id="f2d97-126">チェックイン操作が完了した後のドキュメントの適切なステータス。</span><span class="sxs-lookup"><span data-stu-id="f2d97-126">The desired status of the document after the check-in operation is complete.</span></span> <span data-ttu-id="f2d97-127">`published` または未設定となります。</span><span class="sxs-lookup"><span data-stu-id="f2d97-127">Can be `published` or unspecified.</span></span> |
| <span data-ttu-id="f2d97-128">comment</span><span class="sxs-lookup"><span data-stu-id="f2d97-128">comment</span></span>   | <span data-ttu-id="f2d97-129">文字列</span><span class="sxs-lookup"><span data-stu-id="f2d97-129">string</span></span> | <span data-ttu-id="f2d97-130">バージョンに関連付けられているチェックイン コメント。</span><span class="sxs-lookup"><span data-stu-id="f2d97-130">A check-in comment that is associated with the version.</span></span>                                                   |

## <a name="example"></a><span data-ttu-id="f2d97-131">例</span><span class="sxs-lookup"><span data-stu-id="f2d97-131">Example</span></span>

<span data-ttu-id="f2d97-132">この例では、`{item-id}` で識別されるファイルをチェックインします。</span><span class="sxs-lookup"><span data-stu-id="f2d97-132">This example checks in a file identified by `{item-id}`.</span></span>

<!-- { "blockType": "request", "name": "checkin-item", "scopes": "files.readwrite", "target": "action" } -->

```http
POST /drives/{drive-id}/items/{item-id}/checkin
Content-Type: application/json

{
  "comment": "Updating the latest guidelines"
}
```

## <a name="response"></a><span data-ttu-id="f2d97-133">応答</span><span class="sxs-lookup"><span data-stu-id="f2d97-133">Response</span></span>

<span data-ttu-id="f2d97-134">成功すると、API 呼び出しは `204 No content` を返します。</span><span class="sxs-lookup"><span data-stu-id="f2d97-134">If successful, the API call returns a `204 No content`.</span></span>

<!-- { "blockType": "response" } -->

```http
HTTP/1.1 204 No content
```

### <a name="remarks"></a><span data-ttu-id="f2d97-135">備考</span><span class="sxs-lookup"><span data-stu-id="f2d97-135">Remarks</span></span>


[item-resource]: ../resources/driveitem.md

<!-- {
  "type": "#page.annotation",
  "description": "Create a copy of an existing item.",
  "keywords": "copy existing item",
  "section": "documentation",
  "tocPath": "Items/Copy"
} -->
