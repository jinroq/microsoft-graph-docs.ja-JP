---
author: rgregg
ms.author: rgregg
ms.date: 09/11/2017
title: サイト内の SharePoint リストを一覧表示する
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: fa13fc93dcfcfc807671082be43a7c4b4eafd63d
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27957873"
---
# <a name="enumerate-lists-in-a-site"></a><span data-ttu-id="ae187-102">サイト内のリストを列挙する</span><span class="sxs-lookup"><span data-stu-id="ae187-102">Enumerate lists in a site</span></span>

> <span data-ttu-id="ae187-103">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="ae187-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ae187-104">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ae187-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="ae187-105">[サイト][]の[リスト][]のコレクションを取得します。</span><span class="sxs-lookup"><span data-stu-id="ae187-105">Get the collection of [lists][] for a [site][].</span></span>

[サイト]: ../resources/list.md
[lists]: ../resources/list.md
[site]: ../resources/site.md

## <a name="permissions"></a><span data-ttu-id="ae187-108">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="ae187-108">Permissions</span></span>

<span data-ttu-id="ae187-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="ae187-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ae187-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="ae187-111">Permission type</span></span>      | <span data-ttu-id="ae187-112">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="ae187-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ae187-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="ae187-113">Delegated (work or school account)</span></span> | <span data-ttu-id="ae187-114">Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ae187-114">Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="ae187-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="ae187-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ae187-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ae187-116">Not supported.</span></span>    |
|<span data-ttu-id="ae187-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="ae187-117">Application</span></span> | <span data-ttu-id="ae187-118">Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ae187-118">Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="ae187-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="ae187-119">HTTP request</span></span>

```http
GET https://graph.microsoft.com/beta/sites/{site-id}/lists
```

## <a name="example"></a><span data-ttu-id="ae187-120">例</span><span class="sxs-lookup"><span data-stu-id="ae187-120">Example</span></span>

#### <a name="request"></a><span data-ttu-id="ae187-121">要求</span><span class="sxs-lookup"><span data-stu-id="ae187-121">Request</span></span>

<!-- { "blockType": "request", "name": "enum-lists", "scopes": "sites.read.all service.sharepoint" } -->

```http
GET https://graph.microsoft.com/beta/sites/{site-id}/lists
```

##### <a name="response"></a><span data-ttu-id="ae187-122">応答</span><span class="sxs-lookup"><span data-stu-id="ae187-122">Response</span></span>

<!-- { "blockType": "response", "@type": "microsoft.graph.list", "isCollection": true, "truncated": true } -->

```json
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "id": "b57af081-936c-4803-a120-d94887b03864",
      "name": "Documents",
      "createdDateTime": "2016-08-30T08:32:00Z",
      "lastModifiedDateTime": "2016-08-30T08:32:00Z",
      "list": {
        "hidden": false,
        "template": "documentLibrary"
       }
    },
    {
      "id": "1234-112-112-4",
      "name": "MicroFeed",
      "createdDateTime": "2016-08-30T08:32:00Z",
      "lastModifiedDateTime": "2016-08-30T08:32:00Z",
      "list": {
        "hidden": false,
        "template": "genericList"
       }
    }
  ]
}
```

## <a name="remarks"></a><span data-ttu-id="ae187-123">注釈</span><span class="sxs-lookup"><span data-stu-id="ae187-123">Remarks</span></span>

<span data-ttu-id="ae187-124">[system][] ファセットのあるリストは既定では非表示です。</span><span class="sxs-lookup"><span data-stu-id="ae187-124">Lists with the [system][] facet are hidden by default.</span></span>
<span data-ttu-id="ae187-125">それらを一覧表示するには、`$select` ステートメントに `system` を含めます。</span><span class="sxs-lookup"><span data-stu-id="ae187-125">To list them, include `system` in your `$select` statement.</span></span>

[system]: ../resources/systemfacet.md

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Lists/Enumerate"
} -->
