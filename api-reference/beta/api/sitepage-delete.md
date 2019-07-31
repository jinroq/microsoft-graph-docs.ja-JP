---
author: rahmit
description: サイトのサイトページリストから sitePage を削除します。
ms.date: 05/07/2018
title: SharePoint サイトからページを削除する
localization_priority: Normal
ms.prod: sharepoint
doc_type: apiPageType
ms.openlocfilehash: bdf3dacabb99d5dfcfe47dcb954ff1cfd0b62ccb
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35977861"
---
# <a name="delete-page-from-the-site-pages-list-of-a-site"></a><span data-ttu-id="7131b-103">サイトのサイトページリストからページを削除する</span><span class="sxs-lookup"><span data-stu-id="7131b-103">Delete page from the site pages list of a site</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7131b-104">[サイト][]のサイトページ[リスト][]から[sitepage][]を削除します。</span><span class="sxs-lookup"><span data-stu-id="7131b-104">Removes a [sitePage][] from the site pages [list][] in a [site][].</span></span>

[sitePage]: ../resources/sitepage.md
[list]: ../resources/list.md
[サイト]: ../resources/site.md
[site]: ../resources/site.md

## <a name="permissions"></a><span data-ttu-id="7131b-108">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="7131b-108">Permissions</span></span>

<span data-ttu-id="7131b-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="7131b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

><span data-ttu-id="7131b-111">**注:** アイテムを削除するには、削除するアイテムへの書き込みアクセス権がユーザーに付与されている必要があります。</span><span class="sxs-lookup"><span data-stu-id="7131b-111">**Note:** To delete an item, the user must have granted the application write access to the item to be deleted.</span></span>

|<span data-ttu-id="7131b-112">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="7131b-112">Permission type</span></span>      | <span data-ttu-id="7131b-113">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="7131b-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7131b-114">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="7131b-114">Delegated (work or school account)</span></span> | <span data-ttu-id="7131b-115">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7131b-115">Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="7131b-116">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="7131b-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7131b-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="7131b-117">Not supported.</span></span>    |
|<span data-ttu-id="7131b-118">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="7131b-118">Application</span></span> | <span data-ttu-id="7131b-119">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7131b-119">Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="7131b-120">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="7131b-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /sites/{site-id}/pages/{page-id}
```

## <a name="optional-request-headers"></a><span data-ttu-id="7131b-121">オプションの要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="7131b-121">Optional request headers</span></span>

| <span data-ttu-id="7131b-122">名前</span><span class="sxs-lookup"><span data-stu-id="7131b-122">Name</span></span>       | <span data-ttu-id="7131b-123">値</span><span class="sxs-lookup"><span data-stu-id="7131b-123">Value</span></span> | <span data-ttu-id="7131b-124">説明</span><span class="sxs-lookup"><span data-stu-id="7131b-124">Description</span></span>
|:-----------|:------|:--------------------------------------------------------
| <span data-ttu-id="7131b-125">_if-match_</span><span class="sxs-lookup"><span data-stu-id="7131b-125">_if-match_</span></span> | <span data-ttu-id="7131b-126">etag</span><span class="sxs-lookup"><span data-stu-id="7131b-126">etag</span></span>  | <span data-ttu-id="7131b-127">この要求ヘッダーが含まれていて、指定された eTag がアイテムの現在のタグに一致しない場合には、`412 Precondition Failed` 応答が返され、アイテムは削除されません。</span><span class="sxs-lookup"><span data-stu-id="7131b-127">If this request header is included and the eTag provided does not match the current tag on the item, a `412 Precondition Failed` response is returned and the item will not be deleted.</span></span>

## <a name="request-body"></a><span data-ttu-id="7131b-128">要求本文</span><span class="sxs-lookup"><span data-stu-id="7131b-128">Request body</span></span>

<span data-ttu-id="7131b-129">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="7131b-129">Do not supply a request body with this method.</span></span>
<!-- TODO: should we provide a URL to recover/undelete the file, if one exists? -->

## <a name="response"></a><span data-ttu-id="7131b-130">応答</span><span class="sxs-lookup"><span data-stu-id="7131b-130">Response</span></span>

<span data-ttu-id="7131b-131">成功した場合、この呼び出し`204 No Content`は、リソースが削除され、戻り値がないことを示す応答を返します。</span><span class="sxs-lookup"><span data-stu-id="7131b-131">If successful, this call returns a `204 No Content` response to indicate that the resource was deleted and there was nothing to return.</span></span>

## <a name="example"></a><span data-ttu-id="7131b-132">例</span><span class="sxs-lookup"><span data-stu-id="7131b-132">Example</span></span>

<!-- { "blockType": "request", "name": "delete-page", "scopes": "files.readwrite sites.readwrite.all" } -->

##### <a name="request"></a><span data-ttu-id="7131b-133">要求</span><span class="sxs-lookup"><span data-stu-id="7131b-133">Request</span></span>

```http
DELETE /sites/{site-id}/pages/{page-id}
```
##### <a name="response"></a><span data-ttu-id="7131b-134">応答</span><span class="sxs-lookup"><span data-stu-id="7131b-134">Response</span></span>

<!-- { "blockType": "response" } -->

```http
HTTP/1.1 204 No Content
```

<!--
{
  "type": "#page.annotation",
  "description": "Delete a page in the SitePages list in a site.",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Pages/Delete",
  "suppressions": []
}
-->
