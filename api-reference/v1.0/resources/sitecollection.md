---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: SiteCollection
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 6fb5f05a1dbdf7485957bb4bf04db06432f17da4
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27916986"
---
# <a name="sitecollection-resource"></a><span data-ttu-id="a061e-102">SiteCollection リソース</span><span class="sxs-lookup"><span data-stu-id="a061e-102">SiteCollection resource</span></span>

<span data-ttu-id="a061e-103">**siteCollection** リソースは、サイト コレクションの詳細を提供します。</span><span class="sxs-lookup"><span data-stu-id="a061e-103">The **siteCollection** resource provides more information about a site collection.</span></span>

<span data-ttu-id="a061e-104">[**サイト**](site.md) リソースが null ではない **siteCollection** プロパティを持つ場合、そのサイトはサイト コレクションのルート サイトです。</span><span class="sxs-lookup"><span data-stu-id="a061e-104">If a [**site**](site.md) resource has a non-null **siteCollection** property, then the site is a root site for a site collection.</span></span>

## <a name="json-representation"></a><span data-ttu-id="a061e-105">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="a061e-105">JSON representation</span></span>

<span data-ttu-id="a061e-106">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="a061e-106">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
  ],
  "@odata.type": "microsoft.graph.siteCollection"
}-->

```json
{
  "hostname": "contoso.sharepoint.com",
  "root": { "@odata.type": "microsoft.graph.root" }
}
```

## <a name="properties"></a><span data-ttu-id="a061e-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="a061e-107">Properties</span></span>

| <span data-ttu-id="a061e-108">プロパティ名</span><span class="sxs-lookup"><span data-stu-id="a061e-108">Property name</span></span>        | <span data-ttu-id="a061e-109">種類</span><span class="sxs-lookup"><span data-stu-id="a061e-109">Type</span></span>     | <span data-ttu-id="a061e-110">説明</span><span class="sxs-lookup"><span data-stu-id="a061e-110">Description</span></span>
|:---------------------|:---------|:---------------------------------------------------
| <span data-ttu-id="a061e-111">**hostname**</span><span class="sxs-lookup"><span data-stu-id="a061e-111">**hostname**</span></span>         | <span data-ttu-id="a061e-112">string</span><span class="sxs-lookup"><span data-stu-id="a061e-112">string</span></span>   | <span data-ttu-id="a061e-p101">サイト コレクションのホスト名です。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="a061e-p101">The hostname for the site collection. Read-only.</span></span>
| <span data-ttu-id="a061e-115">**root**</span><span class="sxs-lookup"><span data-stu-id="a061e-115">**root**</span></span>             | <span data-ttu-id="a061e-116">[root][]</span><span class="sxs-lookup"><span data-stu-id="a061e-116">[root][]</span></span> | <span data-ttu-id="a061e-117">存在する場合は、SharePoint 内のルート サイト コレクションがあることを示します。</span><span class="sxs-lookup"><span data-stu-id="a061e-117">If present, indicates that this is a root site collection in SharePoint.</span></span> <span data-ttu-id="a061e-118">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="a061e-118">Read-only.</span></span>

[ルート]: root.md
[root]: root.md

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Facets/SiteCollection"
}-->
