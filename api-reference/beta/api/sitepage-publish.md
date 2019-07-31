---
author: rahmit
description: SitePage リソースの最新バージョンを発行します。これにより、すべてのユーザーがページのバージョンを使用できるようになります。 ページがチェックアウトされている場合は、ページをチェックインして発行します。 ページがこの API の呼び出し元にチェックアウトされている場合、ページは自動的にチェックインされてから発行されます。
ms.date: 09/10/2018
title: ページの発行
localization_priority: Normal
ms.prod: sharepoint
doc_type: apiPageType
ms.openlocfilehash: 5f4404b33a54979271750d4074a9c6da235966ea
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35991213"
---
# <a name="sitepage-publish"></a><span data-ttu-id="6f6ef-105">サイトページ: 発行</span><span class="sxs-lookup"><span data-stu-id="6f6ef-105">sitePage: publish</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6f6ef-106">[Sitepage][]リソースの最新バージョンを発行します。これにより、すべてのユーザーがページのバージョンを使用できるようになります。</span><span class="sxs-lookup"><span data-stu-id="6f6ef-106">Publish the latest version of a [sitePage][] resource, which makes the version of the page available to all users.</span></span> <span data-ttu-id="6f6ef-107">ページがチェックアウトされている場合は、ページをチェックインして発行します。</span><span class="sxs-lookup"><span data-stu-id="6f6ef-107">If the page is checked out, check in the page and publish it.</span></span> <span data-ttu-id="6f6ef-108">ページがこの API の呼び出し元にチェックアウトされている場合、ページは自動的にチェックインされてから発行されます。</span><span class="sxs-lookup"><span data-stu-id="6f6ef-108">If the page is checked out to the caller of this API, the page is automatically checked in and then published.</span></span>

[sitePage]: ../resources/sitepage.md

## <a name="permissions"></a><span data-ttu-id="6f6ef-110">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="6f6ef-110">Permissions</span></span>

<span data-ttu-id="6f6ef-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="6f6ef-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6f6ef-113">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="6f6ef-113">Permission type</span></span>      | <span data-ttu-id="6f6ef-114">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="6f6ef-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6f6ef-115">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="6f6ef-115">Delegated (work or school account)</span></span> | <span data-ttu-id="6f6ef-116">Files.ReadWrite、Files.ReadWrite.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6f6ef-116">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="6f6ef-117">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="6f6ef-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6f6ef-118">Files.ReadWrite、Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6f6ef-118">Files.ReadWrite, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="6f6ef-119">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="6f6ef-119">Application</span></span> | <span data-ttu-id="6f6ef-120">Files.ReadWrite.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6f6ef-120">Files.ReadWrite.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="6f6ef-121">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="6f6ef-121">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /sites/{siteId}/pages/{pageId}/publish
```

## <a name="request-body"></a><span data-ttu-id="6f6ef-122">要求本文</span><span class="sxs-lookup"><span data-stu-id="6f6ef-122">Request body</span></span>

<span data-ttu-id="6f6ef-123">このメッセージには、要求本文がありません。</span><span class="sxs-lookup"><span data-stu-id="6f6ef-123">This message does not have a request body.</span></span> <span data-ttu-id="6f6ef-124">送信された要求本文は無視されます。</span><span class="sxs-lookup"><span data-stu-id="6f6ef-124">Any request body sent will be ignored.</span></span>

## <a name="response"></a><span data-ttu-id="6f6ef-125">応答</span><span class="sxs-lookup"><span data-stu-id="6f6ef-125">Response</span></span>

<span data-ttu-id="6f6ef-126">成功すると、API 呼び出しは `204 No Content` を返します。</span><span class="sxs-lookup"><span data-stu-id="6f6ef-126">If successful, the API call returns a `204 No Content`.</span></span>

<!-- { "blockType": "response" } -->

```http
HTTP/1.1 204 No Content
```


<!--
{
  "type": "#page.annotation",
  "description": "Publish a page.",
  "keywords": "publish page",
  "section": "documentation",
  "tocPath": "Pages/Publish",
  "suppressions": []
}
-->
