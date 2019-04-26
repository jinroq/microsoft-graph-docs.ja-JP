---
author: rahmit
ms.author: rahmit
ms.date: 09/10/2018
title: ページの発行
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: d9bf699c0038e785a11560ee7326cfb2324345f3
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33335898"
---
# <a name="sitepage-publish"></a><span data-ttu-id="490a5-102">サイトページ: 発行</span><span class="sxs-lookup"><span data-stu-id="490a5-102">sitePage: publish</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="490a5-103">[sitepage][]リソースの最新バージョンを発行します。これにより、すべてのユーザーがページのバージョンを使用できるようになります。</span><span class="sxs-lookup"><span data-stu-id="490a5-103">Publish the latest version of a [sitePage][] resource, which makes the version of the page available to all users.</span></span> <span data-ttu-id="490a5-104">ページがチェックアウトされている場合は、ページをチェックインして発行します。</span><span class="sxs-lookup"><span data-stu-id="490a5-104">If the page is checked out, check in the page and publish it.</span></span> <span data-ttu-id="490a5-105">ページがこの API の呼び出し元にチェックアウトされている場合、ページは自動的にチェックインされてから発行されます。</span><span class="sxs-lookup"><span data-stu-id="490a5-105">If the page is checked out to the caller of this API, the page is automatically checked in and then published.</span></span>

[sitePage]: ../resources/sitepage.md

## <a name="permissions"></a><span data-ttu-id="490a5-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="490a5-107">Permissions</span></span>

<span data-ttu-id="490a5-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="490a5-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="490a5-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="490a5-110">Permission type</span></span>      | <span data-ttu-id="490a5-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="490a5-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="490a5-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="490a5-112">Delegated (work or school account)</span></span> | <span data-ttu-id="490a5-113">Files.ReadWrite、Files.ReadWrite.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="490a5-113">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="490a5-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="490a5-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="490a5-115">Files.ReadWrite、Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="490a5-115">Files.ReadWrite, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="490a5-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="490a5-116">Application</span></span> | <span data-ttu-id="490a5-117">Files.ReadWrite.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="490a5-117">Files.ReadWrite.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="490a5-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="490a5-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /sites/{siteId}/pages/{pageId}/publish
```

## <a name="request-body"></a><span data-ttu-id="490a5-119">要求本文</span><span class="sxs-lookup"><span data-stu-id="490a5-119">Request body</span></span>

<span data-ttu-id="490a5-120">このメッセージには、要求本文がありません。</span><span class="sxs-lookup"><span data-stu-id="490a5-120">This message does not have a request body.</span></span> <span data-ttu-id="490a5-121">送信された要求本文は無視されます。</span><span class="sxs-lookup"><span data-stu-id="490a5-121">Any request body sent will be ignored.</span></span>

## <a name="response"></a><span data-ttu-id="490a5-122">応答</span><span class="sxs-lookup"><span data-stu-id="490a5-122">Response</span></span>

<span data-ttu-id="490a5-123">成功すると、API 呼び出しは `204 No Content` を返します。</span><span class="sxs-lookup"><span data-stu-id="490a5-123">If successful, the API call returns a `204 No Content`.</span></span>

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
