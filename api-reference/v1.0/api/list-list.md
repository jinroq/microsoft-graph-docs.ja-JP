---
author: rgregg
ms.author: rgregg
ms.date: 09/11/2017
title: サイト内の SharePoint リストを一覧表示する
ms.openlocfilehash: 4171947eb2a7ac6be18ba385de39c5befd762f26
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27023260"
---
# <a name="enumerate-lists-in-a-site"></a><span data-ttu-id="be674-102">サイト内のリストを列挙する</span><span class="sxs-lookup"><span data-stu-id="be674-102">Enumerate lists in a site</span></span>

<span data-ttu-id="be674-103">[サイト][]の[リスト][]のコレクションを取得します。</span><span class="sxs-lookup"><span data-stu-id="be674-103">Get the collection of [lists][] for a [site][].</span></span>

[サイト]: ../resources/list.md
[lists]: ../resources/list.md
[site]: ../resources/site.md

## <a name="permissions"></a><span data-ttu-id="be674-106">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="be674-106">Permissions</span></span>

<span data-ttu-id="be674-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="be674-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="be674-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="be674-109">Permission type</span></span>      | <span data-ttu-id="be674-110">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="be674-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="be674-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="be674-111">Delegated (work or school account)</span></span> | <span data-ttu-id="be674-112">Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="be674-112">Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="be674-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="be674-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="be674-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="be674-114">Not supported.</span></span>    |
|<span data-ttu-id="be674-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="be674-115">Application</span></span> | <span data-ttu-id="be674-116">Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="be674-116">Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="be674-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="be674-117">HTTP request</span></span>

```http
GET https://graph.microsoft.com/v1.0/sites/{site-id}/lists
```

## <a name="example"></a><span data-ttu-id="be674-118">例</span><span class="sxs-lookup"><span data-stu-id="be674-118">Example</span></span>

#### <a name="request"></a><span data-ttu-id="be674-119">要求</span><span class="sxs-lookup"><span data-stu-id="be674-119">Request</span></span>

<!-- { "blockType": "request", "name": "enum-lists", "scopes": "sites.read.all", "tags": "service.sharepoint" } -->

```http
GET https://graph.microsoft.com/v1.0/sites/{site-id}/lists
```

##### <a name="response"></a><span data-ttu-id="be674-120">応答</span><span class="sxs-lookup"><span data-stu-id="be674-120">Response</span></span>

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

## <a name="remarks"></a><span data-ttu-id="be674-121">注釈</span><span class="sxs-lookup"><span data-stu-id="be674-121">Remarks</span></span>

<span data-ttu-id="be674-122">[system][] ファセットのあるリストは既定では非表示です。</span><span class="sxs-lookup"><span data-stu-id="be674-122">Lists with the [system][] facet are hidden by default.</span></span>
<span data-ttu-id="be674-123">それらを一覧表示するには、`$select` ステートメントに `system` を含めます。</span><span class="sxs-lookup"><span data-stu-id="be674-123">To list them, include `system` in your `$select` statement.</span></span>

[system]: ../resources/systemfacet.md

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Lists/Enumerate"
} -->