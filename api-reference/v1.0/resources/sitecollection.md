---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: SiteCollection
localization_priority: Normal
ms.prod: sharepoint
description: siteCollection リソースは、サイト コレクションの詳細を提供します。
doc_type: resourcePageType
ms.openlocfilehash: 27a534f2f9afe99a1a5abb1aee91b1b53b29566d
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36034161"
---
# <a name="sitecollection-resource"></a><span data-ttu-id="17915-103">SiteCollection リソース</span><span class="sxs-lookup"><span data-stu-id="17915-103">SiteCollection resource</span></span>

<span data-ttu-id="17915-104">**siteCollection** リソースは、サイト コレクションの詳細を提供します。</span><span class="sxs-lookup"><span data-stu-id="17915-104">The **siteCollection** resource provides more information about a site collection.</span></span>

<span data-ttu-id="17915-105">[**サイト**](site.md) リソースが null ではない **siteCollection** プロパティを持つ場合、そのサイトはサイト コレクションのルート サイトです。</span><span class="sxs-lookup"><span data-stu-id="17915-105">If a [**site**](site.md) resource has a non-null **siteCollection** property, then the site is a root site for a site collection.</span></span>

## <a name="json-representation"></a><span data-ttu-id="17915-106">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="17915-106">JSON representation</span></span>

<span data-ttu-id="17915-107">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="17915-107">Here is a JSON representation of the resource.</span></span>

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

## <a name="properties"></a><span data-ttu-id="17915-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="17915-108">Properties</span></span>

| <span data-ttu-id="17915-109">プロパティ名</span><span class="sxs-lookup"><span data-stu-id="17915-109">Property name</span></span>        | <span data-ttu-id="17915-110">種類</span><span class="sxs-lookup"><span data-stu-id="17915-110">Type</span></span>     | <span data-ttu-id="17915-111">説明</span><span class="sxs-lookup"><span data-stu-id="17915-111">Description</span></span>
|:---------------------|:---------|:---------------------------------------------------
| <span data-ttu-id="17915-112">**hostname**</span><span class="sxs-lookup"><span data-stu-id="17915-112">**hostname**</span></span>         | <span data-ttu-id="17915-113">string</span><span class="sxs-lookup"><span data-stu-id="17915-113">string</span></span>   | <span data-ttu-id="17915-p101">サイト コレクションのホスト名です。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="17915-p101">The hostname for the site collection. Read-only.</span></span>
| <span data-ttu-id="17915-116">**root**</span><span class="sxs-lookup"><span data-stu-id="17915-116">**root**</span></span>             | <span data-ttu-id="17915-117">[root][]</span><span class="sxs-lookup"><span data-stu-id="17915-117">[root][]</span></span> | <span data-ttu-id="17915-118">存在する場合は、これが SharePoint のルートサイトコレクションであることを示します。</span><span class="sxs-lookup"><span data-stu-id="17915-118">If present, indicates that this is a root site collection in SharePoint.</span></span> <span data-ttu-id="17915-119">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="17915-119">Read-only.</span></span>

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
