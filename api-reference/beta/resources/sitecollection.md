---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: SiteCollection
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: e9525882b08aaae5500ce23a4b54e95d0b0e0d65
ms.sourcegitcommit: b877a8dc9aeaf74f975ca495b401ffff001d7699
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/08/2019
ms.locfileid: "30481805"
---
# <a name="sitecollection-resource"></a><span data-ttu-id="2abb7-102">SiteCollection リソース</span><span class="sxs-lookup"><span data-stu-id="2abb7-102">SiteCollection resource</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2abb7-103">**siteCollection** リソースは、サイト コレクションの詳細を提供します。</span><span class="sxs-lookup"><span data-stu-id="2abb7-103">The **siteCollection** resource provides more information about a site collection.</span></span>

<span data-ttu-id="2abb7-104">[**サイト**](site.md) リソースが null ではない **siteCollection** プロパティを持つ場合、そのサイトはサイト コレクションのルート サイトです。</span><span class="sxs-lookup"><span data-stu-id="2abb7-104">If a [**site**](site.md) resource has a non-null **siteCollection** property, then the site is a root site for a site collection.</span></span>

## <a name="json-representation"></a><span data-ttu-id="2abb7-105">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="2abb7-105">JSON representation</span></span>

<span data-ttu-id="2abb7-106">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="2abb7-106">Here is a JSON representation of the resource.</span></span>

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

## <a name="properties"></a><span data-ttu-id="2abb7-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="2abb7-107">Properties</span></span>

| <span data-ttu-id="2abb7-108">プロパティ名</span><span class="sxs-lookup"><span data-stu-id="2abb7-108">Property name</span></span>        | <span data-ttu-id="2abb7-109">種類</span><span class="sxs-lookup"><span data-stu-id="2abb7-109">Type</span></span>     | <span data-ttu-id="2abb7-110">説明</span><span class="sxs-lookup"><span data-stu-id="2abb7-110">Description</span></span>
|:---------------------|:---------|:---------------------------------------------------
| <span data-ttu-id="2abb7-111">**hostname**</span><span class="sxs-lookup"><span data-stu-id="2abb7-111">**hostname**</span></span>         | <span data-ttu-id="2abb7-112">string</span><span class="sxs-lookup"><span data-stu-id="2abb7-112">string</span></span>   | <span data-ttu-id="2abb7-p101">サイト コレクションのホスト名です。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="2abb7-p101">The hostname for the site collection. Read-only.</span></span>
| <span data-ttu-id="2abb7-115">**dataLocationCode**</span><span class="sxs-lookup"><span data-stu-id="2abb7-115">**dataLocationCode**</span></span> | <span data-ttu-id="2abb7-116">string</span><span class="sxs-lookup"><span data-stu-id="2abb7-116">string</span></span>   | <span data-ttu-id="2abb7-117">このサイトコレクションが存在する地域の地域コード。</span><span class="sxs-lookup"><span data-stu-id="2abb7-117">The geographic region code for where this site collection resides.</span></span> <span data-ttu-id="2abb7-118">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="2abb7-118">Read-only.</span></span>
| <span data-ttu-id="2abb7-119">**root**</span><span class="sxs-lookup"><span data-stu-id="2abb7-119">**root**</span></span>             | <span data-ttu-id="2abb7-120">[root][]</span><span class="sxs-lookup"><span data-stu-id="2abb7-120">[root][]</span></span> | <span data-ttu-id="2abb7-121">存在する場合は、これが SharePoint のルートサイトコレクションであることを示します。</span><span class="sxs-lookup"><span data-stu-id="2abb7-121">If present, indicates that this is a root site collection in SharePoint.</span></span> <span data-ttu-id="2abb7-122">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="2abb7-122">Read-only.</span></span>

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
  "suppressions": [
    "Error: /api-reference/beta/resources/sitecollection.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
