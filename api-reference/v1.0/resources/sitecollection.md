---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: SiteCollection
ms.openlocfilehash: 6b36f3a0c2d958081f1b5663231a541f2e8a000f
ms.sourcegitcommit: 7aea7a97e36e6d146214de3a90fdbc71628aadba
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/28/2017
---
# <a name="sitecollection-resource"></a><span data-ttu-id="f8f68-102">SiteCollection リソース</span><span class="sxs-lookup"><span data-stu-id="f8f68-102">SiteCollection resource</span></span>

<span data-ttu-id="f8f68-103">**siteCollection** リソースは、サイト コレクションの詳細を提供します。</span><span class="sxs-lookup"><span data-stu-id="f8f68-103">The **siteCollection** resource provides more information about a site collection.</span></span>

<span data-ttu-id="f8f68-104">[**サイト**](site.md) リソースが null ではない **siteCollection** プロパティを持つ場合、そのサイトはサイト コレクションのルート サイトです。</span><span class="sxs-lookup"><span data-stu-id="f8f68-104">If a [**site**](site.md) resource has a non-null **siteCollection** property, then the site is a root site for a site collection.</span></span>

## <a name="json-representation"></a><span data-ttu-id="f8f68-105">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="f8f68-105">JSON representation</span></span>

<span data-ttu-id="f8f68-106">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="f8f68-106">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
  ],
  "@odata.type": "microsoft.graph.siteCollection"
}-->

```json
{
  "hostname": "contoso.sharepoint.com"
}
```

## <a name="properties"></a><span data-ttu-id="f8f68-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="f8f68-107">Properties</span></span>

| <span data-ttu-id="f8f68-108">プロパティ名</span><span class="sxs-lookup"><span data-stu-id="f8f68-108">Property name</span></span> | <span data-ttu-id="f8f68-109">種類</span><span class="sxs-lookup"><span data-stu-id="f8f68-109">Type</span></span>    | <span data-ttu-id="f8f68-110">説明</span><span class="sxs-lookup"><span data-stu-id="f8f68-110">Description</span></span>                                                                                                                  |
|:--------------|:--------|:---------------------------------------------------
| <span data-ttu-id="f8f68-111">**hostname**</span><span class="sxs-lookup"><span data-stu-id="f8f68-111">**hostname**</span></span>  | <span data-ttu-id="f8f68-112">string</span><span class="sxs-lookup"><span data-stu-id="f8f68-112">string</span></span>  | <span data-ttu-id="f8f68-p101">サイト コレクションのホスト名です。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="f8f68-p101">The hostname for the site collection. Read-only.</span></span>


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Facets/SiteCollection"
}-->
