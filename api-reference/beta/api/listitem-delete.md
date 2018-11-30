---
author: rgregg
ms.author: rgregg
ms.date: 09/11/2017
title: SharePoint リストからエントリを削除する
ms.openlocfilehash: d0b39a7c0ca69d3bfdd0edb256ac20711dfe5efc
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27072048"
---
# <a name="delete-an-item-from-a-list"></a><span data-ttu-id="08cbd-102">リストからアイテムを削除する</span><span class="sxs-lookup"><span data-stu-id="08cbd-102">Delete an item from a list</span></span>

> <span data-ttu-id="08cbd-103">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="08cbd-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="08cbd-104">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="08cbd-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="08cbd-105">[list][] からアイテムを削除します。</span><span class="sxs-lookup"><span data-stu-id="08cbd-105">Removes an item from a [list][].</span></span>

[list]: ../resources/list.md

## <a name="permissions"></a><span data-ttu-id="08cbd-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="08cbd-107">Permissions</span></span>

<span data-ttu-id="08cbd-108">アイテムを削除するには、削除するアイテムへの書き込みアクセス権がユーザーに付与されている必要があります。</span><span class="sxs-lookup"><span data-stu-id="08cbd-108">To delete an item, the user must have granted the application write access to the item to be deleted.</span></span>

<span data-ttu-id="08cbd-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="08cbd-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="08cbd-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="08cbd-111">Permission type</span></span>      | <span data-ttu-id="08cbd-112">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="08cbd-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="08cbd-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="08cbd-113">Delegated (work or school account)</span></span> | <span data-ttu-id="08cbd-114">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="08cbd-114">Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="08cbd-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="08cbd-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="08cbd-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="08cbd-116">Not supported.</span></span>    |
|<span data-ttu-id="08cbd-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="08cbd-117">Application</span></span> | <span data-ttu-id="08cbd-118">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="08cbd-118">Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="08cbd-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="08cbd-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE https://graph.microsoft.com/beta/sites/{site-id}/lists/{list-id}/items/{item-id}
```

## <a name="optional-request-headers"></a><span data-ttu-id="08cbd-120">オプションの要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="08cbd-120">Optional request headers</span></span>

| <span data-ttu-id="08cbd-121">名前</span><span class="sxs-lookup"><span data-stu-id="08cbd-121">Name</span></span>       | <span data-ttu-id="08cbd-122">値</span><span class="sxs-lookup"><span data-stu-id="08cbd-122">Value</span></span> | <span data-ttu-id="08cbd-123">説明</span><span class="sxs-lookup"><span data-stu-id="08cbd-123">Description</span></span>
|:-----------|:------|:--------------------------------------------------------
| <span data-ttu-id="08cbd-124">_if-match_</span><span class="sxs-lookup"><span data-stu-id="08cbd-124">_if-match_</span></span> | <span data-ttu-id="08cbd-125">etag</span><span class="sxs-lookup"><span data-stu-id="08cbd-125">etag</span></span>  | <span data-ttu-id="08cbd-126">この要求ヘッダーが含まれていて、指定された eTag がアイテムの現在のタグに一致しない場合には、`412 Precondition Failed` 応答が返され、アイテムは削除されません。</span><span class="sxs-lookup"><span data-stu-id="08cbd-126">If this request header is included and the eTag provided does not match the current tag on the item, a `412 Precondition Failed` response is returned and the item will not be deleted.</span></span>

## <a name="request-body"></a><span data-ttu-id="08cbd-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="08cbd-127">Request body</span></span>

<span data-ttu-id="08cbd-128">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="08cbd-128">Do not supply a request body with this method.</span></span>

## <a name="example"></a><span data-ttu-id="08cbd-129">例</span><span class="sxs-lookup"><span data-stu-id="08cbd-129">Example</span></span>

<!-- { "blockType": "request", "name": "delete-item", "scopes": "files.readwrite" } -->

```http
DELETE https://graph.microsoft.com/beta/sites/{site-id}/lists/{list-id}/items/{item-id}
```

## <a name="response"></a><span data-ttu-id="08cbd-130">応答</span><span class="sxs-lookup"><span data-stu-id="08cbd-130">Response</span></span>

<span data-ttu-id="08cbd-131">成功した場合、この呼び出しはリソースが削除され返すものがなかったことを示す `204 No Content` 応答を返します。</span><span class="sxs-lookup"><span data-stu-id="08cbd-131">If successful, this call returns a `204 No Content` response to indicate that resource was deleted and there was nothing to return.</span></span>

<!-- { "blockType": "response" } -->

```http
HTTP/1.1 204 No Content
```

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "ListItem/Delete"
} -->
