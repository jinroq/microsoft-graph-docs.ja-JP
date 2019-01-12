---
author: rahmit
ms.author: rahmit
ms.date: 09/10/2018
title: '[発行] ページ'
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 8e59a7aea74e165945757f2513102a66baf64be1
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27920241"
---
# <a name="sitepage-publish"></a><span data-ttu-id="86810-102">sitePage: 発行</span><span class="sxs-lookup"><span data-stu-id="86810-102">sitePage: publish</span></span>

> <span data-ttu-id="86810-103">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="86810-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="86810-104">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="86810-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="86810-105">ページのバージョンをすべてのユーザーが使用可能にする[sitePage][]リソースの最新バージョンを公開します。</span><span class="sxs-lookup"><span data-stu-id="86810-105">Publish the latest version of a [sitePage][] resource, which makes the version of the page available to all users.</span></span> <span data-ttu-id="86810-106">ページがチェック アウトされている場合は、ページをチェックインし、公開します。</span><span class="sxs-lookup"><span data-stu-id="86810-106">If the page is checked out, check in the page and publish it.</span></span> <span data-ttu-id="86810-107">この API の呼び出し元ページがチェック アウトされた場合ページが自動的にチェックインし、公開します。</span><span class="sxs-lookup"><span data-stu-id="86810-107">If the page is checked out to the caller of this API, the page is automatically checked in and then published.</span></span>

[sitePage]: ../resources/sitepage.md

## <a name="permissions"></a><span data-ttu-id="86810-109">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="86810-109">Permissions</span></span>

<span data-ttu-id="86810-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="86810-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="86810-112">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="86810-112">Permission type</span></span>      | <span data-ttu-id="86810-113">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="86810-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="86810-114">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="86810-114">Delegated (work or school account)</span></span> | <span data-ttu-id="86810-115">Files.ReadWrite、Files.ReadWrite.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="86810-115">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="86810-116">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="86810-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="86810-117">Files.ReadWrite、Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="86810-117">Files.ReadWrite, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="86810-118">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="86810-118">Application</span></span> | <span data-ttu-id="86810-119">Files.ReadWrite.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="86810-119">Files.ReadWrite.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="86810-120">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="86810-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /sites/{siteId}/pages/{pageId}/publish
```

## <a name="request-body"></a><span data-ttu-id="86810-121">要求本文</span><span class="sxs-lookup"><span data-stu-id="86810-121">Request body</span></span>

<span data-ttu-id="86810-122">このメッセージには、要求の本体がありません。</span><span class="sxs-lookup"><span data-stu-id="86810-122">This message does not have a request body.</span></span> <span data-ttu-id="86810-123">送信の要求の本文は無視されます。</span><span class="sxs-lookup"><span data-stu-id="86810-123">Any request body sent will be ignored.</span></span>

## <a name="response"></a><span data-ttu-id="86810-124">応答</span><span class="sxs-lookup"><span data-stu-id="86810-124">Response</span></span>

<span data-ttu-id="86810-125">成功すると、API 呼び出しは `204 No Content` を返します。</span><span class="sxs-lookup"><span data-stu-id="86810-125">If successful, the API call returns a `204 No Content`.</span></span>

<!-- { "blockType": "response" } -->

```http
HTTP/1.1 204 No Content
```


<!-- {
  "type": "#page.annotation",
  "description": "Publish a page.",
  "keywords": "publish page",
  "section": "documentation",
  "tocPath": "Pages/Publish"
} -->
