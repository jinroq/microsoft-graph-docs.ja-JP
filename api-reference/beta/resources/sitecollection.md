---
author: JeremyKelley
description: siteCollection リソースは、サイト コレクションの詳細を提供します。
ms.date: 09/10/2017
title: SiteCollection
localization_priority: Normal
ms.prod: sharepoint
doc_type: resourcePageType
ms.openlocfilehash: 0989306be8fa8e456d2718079aec069097cab035
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36008293"
---
# <a name="sitecollection-resource"></a><span data-ttu-id="eb16b-103">SiteCollection リソース</span><span class="sxs-lookup"><span data-stu-id="eb16b-103">SiteCollection resource</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="eb16b-104">**siteCollection** リソースは、サイト コレクションの詳細を提供します。</span><span class="sxs-lookup"><span data-stu-id="eb16b-104">The **siteCollection** resource provides more information about a site collection.</span></span>

<span data-ttu-id="eb16b-105">[**サイト**](site.md) リソースが null ではない **siteCollection** プロパティを持つ場合、そのサイトはサイト コレクションのルート サイトです。</span><span class="sxs-lookup"><span data-stu-id="eb16b-105">If a [**site**](site.md) resource has a non-null **siteCollection** property, then the site is a root site for a site collection.</span></span>

## <a name="json-representation"></a><span data-ttu-id="eb16b-106">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="eb16b-106">JSON representation</span></span>

<span data-ttu-id="eb16b-107">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="eb16b-107">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "dataLocationCode", "root"
  ],
  "@odata.type": "microsoft.graph.siteCollection"
}-->

```json
{
  "hostname": "contoso.sharepoint.com",
  "dataLocationCode": "EUR",
  "root": { "@odata.type": "microsoft.graph.root" }
}
```

## <a name="properties"></a><span data-ttu-id="eb16b-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="eb16b-108">Properties</span></span>

| <span data-ttu-id="eb16b-109">プロパティ名</span><span class="sxs-lookup"><span data-stu-id="eb16b-109">Property name</span></span>        | <span data-ttu-id="eb16b-110">種類</span><span class="sxs-lookup"><span data-stu-id="eb16b-110">Type</span></span>     | <span data-ttu-id="eb16b-111">説明</span><span class="sxs-lookup"><span data-stu-id="eb16b-111">Description</span></span>
|:---------------------|:---------|:---------------------------------------------------
| <span data-ttu-id="eb16b-112">**hostname**</span><span class="sxs-lookup"><span data-stu-id="eb16b-112">**hostname**</span></span>         | <span data-ttu-id="eb16b-113">string</span><span class="sxs-lookup"><span data-stu-id="eb16b-113">string</span></span>   | <span data-ttu-id="eb16b-p101">サイト コレクションのホスト名です。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="eb16b-p101">The hostname for the site collection. Read-only.</span></span>
| <span data-ttu-id="eb16b-116">**dataLocationCode**</span><span class="sxs-lookup"><span data-stu-id="eb16b-116">**dataLocationCode**</span></span> | <span data-ttu-id="eb16b-117">string</span><span class="sxs-lookup"><span data-stu-id="eb16b-117">string</span></span>   | <span data-ttu-id="eb16b-118">このサイトコレクションが存在する地域の地域コード。</span><span class="sxs-lookup"><span data-stu-id="eb16b-118">The geographic region code for where this site collection resides.</span></span> <span data-ttu-id="eb16b-119">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="eb16b-119">Read-only.</span></span>
| <span data-ttu-id="eb16b-120">**root**</span><span class="sxs-lookup"><span data-stu-id="eb16b-120">**root**</span></span>             | <span data-ttu-id="eb16b-121">[root][]</span><span class="sxs-lookup"><span data-stu-id="eb16b-121">[root][]</span></span> | <span data-ttu-id="eb16b-122">存在する場合は、これが SharePoint のルートサイトコレクションであることを示します。</span><span class="sxs-lookup"><span data-stu-id="eb16b-122">If present, indicates that this is a root site collection in SharePoint.</span></span> <span data-ttu-id="eb16b-123">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="eb16b-123">Read-only.</span></span>

[root]: root.md

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
