---
author: rahmit
ms.author: rahmit
ms.date: 05/07/2018
title: SharePoint サイトからページを削除します。
localization_priority: Normal
ms.openlocfilehash: 1089bd904167f4c86ee1f6becede2824a2b6f2f9
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27815115"
---
# <a name="delete-page-from-the-site-pages-list-of-a-site"></a><span data-ttu-id="2517e-102">サイトのサイトのページのリストからページを削除します。</span><span class="sxs-lookup"><span data-stu-id="2517e-102">Delete page from the site pages list of a site</span></span>

> <span data-ttu-id="2517e-103">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="2517e-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="2517e-104">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="2517e-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="2517e-105">[サイト][]内のサイトのページ[] ボックスの一覧][]から、 [sitePage][]を削除します。</span><span class="sxs-lookup"><span data-stu-id="2517e-105">Removes a [sitePage][] from the site pages [list][] in a [site][].</span></span>

[sitePage]: ../resources/sitepage.md
[list]: ../resources/list.md
[site]: ../resources/site.md

## <a name="permissions"></a><span data-ttu-id="2517e-109">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="2517e-109">Permissions</span></span>

<span data-ttu-id="2517e-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="2517e-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

><span data-ttu-id="2517e-112">**注:** アイテムを削除するには、ユーザーする必要がありますを与え、アプリケーションへの書き込みアクセスを削除する項目。</span><span class="sxs-lookup"><span data-stu-id="2517e-112">**Note:** To delete an item, the user must have granted the application write access to the item to be deleted.</span></span>

|<span data-ttu-id="2517e-113">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="2517e-113">Permission type</span></span>      | <span data-ttu-id="2517e-114">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="2517e-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2517e-115">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="2517e-115">Delegated (work or school account)</span></span> | <span data-ttu-id="2517e-116">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2517e-116">Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="2517e-117">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="2517e-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2517e-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="2517e-118">Not supported.</span></span>    |
|<span data-ttu-id="2517e-119">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="2517e-119">Application</span></span> | <span data-ttu-id="2517e-120">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2517e-120">Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="2517e-121">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="2517e-121">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /sites/{site-id}/pages/{page-id}
```

## <a name="optional-request-headers"></a><span data-ttu-id="2517e-122">オプションの要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="2517e-122">Optional request headers</span></span>

| <span data-ttu-id="2517e-123">名前</span><span class="sxs-lookup"><span data-stu-id="2517e-123">Name</span></span>       | <span data-ttu-id="2517e-124">値</span><span class="sxs-lookup"><span data-stu-id="2517e-124">Value</span></span> | <span data-ttu-id="2517e-125">説明</span><span class="sxs-lookup"><span data-stu-id="2517e-125">Description</span></span>
|:-----------|:------|:--------------------------------------------------------
| <span data-ttu-id="2517e-126">_if-match_</span><span class="sxs-lookup"><span data-stu-id="2517e-126">_if-match_</span></span> | <span data-ttu-id="2517e-127">etag</span><span class="sxs-lookup"><span data-stu-id="2517e-127">etag</span></span>  | <span data-ttu-id="2517e-128">この要求ヘッダーが含まれていて、指定された eTag がアイテムの現在のタグに一致しない場合には、`412 Precondition Failed` 応答が返され、アイテムは削除されません。</span><span class="sxs-lookup"><span data-stu-id="2517e-128">If this request header is included and the eTag provided does not match the current tag on the item, a `412 Precondition Failed` response is returned and the item will not be deleted.</span></span>

## <a name="request-body"></a><span data-ttu-id="2517e-129">要求本文</span><span class="sxs-lookup"><span data-stu-id="2517e-129">Request body</span></span>

<span data-ttu-id="2517e-130">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="2517e-130">Do not supply a request body with this method.</span></span>
<!-- TODO: should we provide a URL to recover/undelete the file, if one exists? -->

## <a name="response"></a><span data-ttu-id="2517e-131">応答</span><span class="sxs-lookup"><span data-stu-id="2517e-131">Response</span></span>

<span data-ttu-id="2517e-132">かどうかは成功すると、この呼び出しが返されます、 `204 No Content` 、リソースが削除された取得するのには何もを使用する必要があることを示すために応答します。</span><span class="sxs-lookup"><span data-stu-id="2517e-132">If successful, this call returns a `204 No Content` response to indicate that the resource was deleted and there was nothing to return.</span></span>

## <a name="example"></a><span data-ttu-id="2517e-133">例</span><span class="sxs-lookup"><span data-stu-id="2517e-133">Example</span></span>

<!-- { "blockType": "request", "name": "delete-page", "scopes": "files.readwrite sites.readwrite.all" } -->

##### <a name="request"></a><span data-ttu-id="2517e-134">要求</span><span class="sxs-lookup"><span data-stu-id="2517e-134">Request</span></span>

```http
DELETE /sites/{site-id}/pages/{page-id}
```
##### <a name="response"></a><span data-ttu-id="2517e-135">応答</span><span class="sxs-lookup"><span data-stu-id="2517e-135">Response</span></span>

<!-- { "blockType": "response" } -->

```http
HTTP/1.1 204 No Content
```

<!-- {
  "type": "#page.annotation",
  "description": "Delete a page in the SitePages list in a site.",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Pages/Delete"
} -->
