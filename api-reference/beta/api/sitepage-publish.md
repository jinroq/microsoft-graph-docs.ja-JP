---
author: rahmit
ms.author: rahmit
ms.date: 09/10/2018
title: '[発行] ページ'
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 5a00a69542c2b59b1b268433b08656c87d194feb
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29507531"
---
# <a name="sitepage-publish"></a><span data-ttu-id="085eb-102">sitePage: 発行</span><span class="sxs-lookup"><span data-stu-id="085eb-102">sitePage: publish</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="085eb-103">ページのバージョンをすべてのユーザーが使用可能にする[sitePage][]リソースの最新バージョンを公開します。</span><span class="sxs-lookup"><span data-stu-id="085eb-103">Publish the latest version of a [sitePage][] resource, which makes the version of the page available to all users.</span></span> <span data-ttu-id="085eb-104">ページがチェック アウトされている場合は、ページをチェックインし、公開します。</span><span class="sxs-lookup"><span data-stu-id="085eb-104">If the page is checked out, check in the page and publish it.</span></span> <span data-ttu-id="085eb-105">この API の呼び出し元ページがチェック アウトされた場合ページが自動的にチェックインし、公開します。</span><span class="sxs-lookup"><span data-stu-id="085eb-105">If the page is checked out to the caller of this API, the page is automatically checked in and then published.</span></span>

[sitePage]: ../resources/sitepage.md

## <a name="permissions"></a><span data-ttu-id="085eb-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="085eb-107">Permissions</span></span>

<span data-ttu-id="085eb-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="085eb-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="085eb-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="085eb-110">Permission type</span></span>      | <span data-ttu-id="085eb-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="085eb-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="085eb-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="085eb-112">Delegated (work or school account)</span></span> | <span data-ttu-id="085eb-113">Files.ReadWrite、Files.ReadWrite.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="085eb-113">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="085eb-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="085eb-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="085eb-115">Files.ReadWrite、Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="085eb-115">Files.ReadWrite, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="085eb-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="085eb-116">Application</span></span> | <span data-ttu-id="085eb-117">Files.ReadWrite.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="085eb-117">Files.ReadWrite.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="085eb-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="085eb-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /sites/{siteId}/pages/{pageId}/publish
```

## <a name="request-body"></a><span data-ttu-id="085eb-119">要求本文</span><span class="sxs-lookup"><span data-stu-id="085eb-119">Request body</span></span>

<span data-ttu-id="085eb-120">このメッセージには、要求の本体がありません。</span><span class="sxs-lookup"><span data-stu-id="085eb-120">This message does not have a request body.</span></span> <span data-ttu-id="085eb-121">送信の要求の本文は無視されます。</span><span class="sxs-lookup"><span data-stu-id="085eb-121">Any request body sent will be ignored.</span></span>

## <a name="response"></a><span data-ttu-id="085eb-122">応答</span><span class="sxs-lookup"><span data-stu-id="085eb-122">Response</span></span>

<span data-ttu-id="085eb-123">成功すると、API 呼び出しは `204 No Content` を返します。</span><span class="sxs-lookup"><span data-stu-id="085eb-123">If successful, the API call returns a `204 No Content`.</span></span>

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
  "suppressions": [
    "Error: /api-reference/beta/api/sitepage-publish.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
