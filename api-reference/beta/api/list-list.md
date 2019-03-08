---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/11/2017
title: サイト内の SharePoint リストを一覧表示する
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: c91d7f8f395faa48965cb8334e1cc9eba78b978c
ms.sourcegitcommit: b877a8dc9aeaf74f975ca495b401ffff001d7699
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/08/2019
ms.locfileid: "30480713"
---
# <a name="enumerate-lists-in-a-site"></a><span data-ttu-id="3bfa3-102">サイト内のリストを列挙する</span><span class="sxs-lookup"><span data-stu-id="3bfa3-102">Enumerate lists in a site</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3bfa3-103">[サイト][]の[リスト][]のコレクションを取得します。</span><span class="sxs-lookup"><span data-stu-id="3bfa3-103">Get the collection of [lists][] for a [site][].</span></span>

[サイト]: ../resources/list.md
[lists]: ../resources/list.md
[リスト]: ../resources/site.md
[site]: ../resources/site.md

## <a name="permissions"></a><span data-ttu-id="3bfa3-106">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="3bfa3-106">Permissions</span></span>

<span data-ttu-id="3bfa3-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="3bfa3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3bfa3-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="3bfa3-109">Permission type</span></span>      | <span data-ttu-id="3bfa3-110">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="3bfa3-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3bfa3-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="3bfa3-111">Delegated (work or school account)</span></span> | <span data-ttu-id="3bfa3-112">Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3bfa3-112">Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="3bfa3-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="3bfa3-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3bfa3-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="3bfa3-114">Not supported.</span></span>    |
|<span data-ttu-id="3bfa3-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="3bfa3-115">Application</span></span> | <span data-ttu-id="3bfa3-116">Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3bfa3-116">Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="3bfa3-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="3bfa3-117">HTTP request</span></span>

```http
GET https://graph.microsoft.com/beta/sites/{site-id}/lists
```

## <a name="example"></a><span data-ttu-id="3bfa3-118">例</span><span class="sxs-lookup"><span data-stu-id="3bfa3-118">Example</span></span>

#### <a name="request"></a><span data-ttu-id="3bfa3-119">要求</span><span class="sxs-lookup"><span data-stu-id="3bfa3-119">Request</span></span>

<!-- { "blockType": "request", "name": "enum-lists", "scopes": "sites.read.all service.sharepoint" } -->

```http
GET https://graph.microsoft.com/beta/sites/{site-id}/lists
```

##### <a name="response"></a><span data-ttu-id="3bfa3-120">応答</span><span class="sxs-lookup"><span data-stu-id="3bfa3-120">Response</span></span>

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

## <a name="remarks"></a><span data-ttu-id="3bfa3-121">注釈</span><span class="sxs-lookup"><span data-stu-id="3bfa3-121">Remarks</span></span>

<span data-ttu-id="3bfa3-122">[system][] ファセットのあるリストは既定では非表示です。</span><span class="sxs-lookup"><span data-stu-id="3bfa3-122">Lists with the [system][] facet are hidden by default.</span></span>
<span data-ttu-id="3bfa3-123">それらを一覧表示するには、`$select` ステートメントに `system` を含めます。</span><span class="sxs-lookup"><span data-stu-id="3bfa3-123">To list them, include `system` in your `$select` statement.</span></span>

[system]: ../resources/systemfacet.md

<!--
{
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Lists/Enumerate",
  "suppressions": [
    "Error: /api-reference/beta/api/list-list.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
