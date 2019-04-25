---
author: rahmit
ms.author: rahmit
ms.date: 05/07/2018
title: SharePoint サイトからページを削除する
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: f855942288556fdf07e2b3af78408976c34eb052
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32537115"
---
# <a name="delete-page-from-the-site-pages-list-of-a-site"></a><span data-ttu-id="80e52-102">サイトのサイトページリストからページを削除する</span><span class="sxs-lookup"><span data-stu-id="80e52-102">Delete page from the site pages list of a site</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="80e52-103">[サイト][]のサイトページ[リスト][]から[sitepage][]を削除します。</span><span class="sxs-lookup"><span data-stu-id="80e52-103">Removes a [sitePage][] from the site pages [list][] in a [site][].</span></span>

[sitePage]: ../resources/sitepage.md
[list]: ../resources/list.md
[サイト]: ../resources/site.md
[site]: ../resources/site.md

## <a name="permissions"></a><span data-ttu-id="80e52-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="80e52-107">Permissions</span></span>

<span data-ttu-id="80e52-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="80e52-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

><span data-ttu-id="80e52-110">**注:** アイテムを削除するには、削除するアイテムへの書き込みアクセス権がユーザーに付与されている必要があります。</span><span class="sxs-lookup"><span data-stu-id="80e52-110">**Note:** To delete an item, the user must have granted the application write access to the item to be deleted.</span></span>

|<span data-ttu-id="80e52-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="80e52-111">Permission type</span></span>      | <span data-ttu-id="80e52-112">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="80e52-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="80e52-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="80e52-113">Delegated (work or school account)</span></span> | <span data-ttu-id="80e52-114">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="80e52-114">Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="80e52-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="80e52-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="80e52-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="80e52-116">Not supported.</span></span>    |
|<span data-ttu-id="80e52-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="80e52-117">Application</span></span> | <span data-ttu-id="80e52-118">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="80e52-118">Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="80e52-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="80e52-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /sites/{site-id}/pages/{page-id}
```

## <a name="optional-request-headers"></a><span data-ttu-id="80e52-120">オプションの要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="80e52-120">Optional request headers</span></span>

| <span data-ttu-id="80e52-121">名前</span><span class="sxs-lookup"><span data-stu-id="80e52-121">Name</span></span>       | <span data-ttu-id="80e52-122">値</span><span class="sxs-lookup"><span data-stu-id="80e52-122">Value</span></span> | <span data-ttu-id="80e52-123">説明</span><span class="sxs-lookup"><span data-stu-id="80e52-123">Description</span></span>
|:-----------|:------|:--------------------------------------------------------
| <span data-ttu-id="80e52-124">_if-match_</span><span class="sxs-lookup"><span data-stu-id="80e52-124">_if-match_</span></span> | <span data-ttu-id="80e52-125">etag</span><span class="sxs-lookup"><span data-stu-id="80e52-125">etag</span></span>  | <span data-ttu-id="80e52-126">この要求ヘッダーが含まれていて、指定された eTag がアイテムの現在のタグに一致しない場合には、`412 Precondition Failed` 応答が返され、アイテムは削除されません。</span><span class="sxs-lookup"><span data-stu-id="80e52-126">If this request header is included and the eTag provided does not match the current tag on the item, a `412 Precondition Failed` response is returned and the item will not be deleted.</span></span>

## <a name="request-body"></a><span data-ttu-id="80e52-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="80e52-127">Request body</span></span>

<span data-ttu-id="80e52-128">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="80e52-128">Do not supply a request body with this method.</span></span>
<!-- TODO: should we provide a URL to recover/undelete the file, if one exists? -->

## <a name="response"></a><span data-ttu-id="80e52-129">応答</span><span class="sxs-lookup"><span data-stu-id="80e52-129">Response</span></span>

<span data-ttu-id="80e52-130">成功した場合、この呼び出し`204 No Content`は、リソースが削除され、戻り値がないことを示す応答を返します。</span><span class="sxs-lookup"><span data-stu-id="80e52-130">If successful, this call returns a `204 No Content` response to indicate that the resource was deleted and there was nothing to return.</span></span>

## <a name="example"></a><span data-ttu-id="80e52-131">例</span><span class="sxs-lookup"><span data-stu-id="80e52-131">Example</span></span>

<!-- { "blockType": "request", "name": "delete-page", "scopes": "files.readwrite sites.readwrite.all" } -->

##### <a name="request"></a><span data-ttu-id="80e52-132">要求</span><span class="sxs-lookup"><span data-stu-id="80e52-132">Request</span></span>

```http
DELETE /sites/{site-id}/pages/{page-id}
```
##### <a name="response"></a><span data-ttu-id="80e52-133">応答</span><span class="sxs-lookup"><span data-stu-id="80e52-133">Response</span></span>

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
  "suppressions": [
    "Error: /api-reference/beta/api/sitepage-delete.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
