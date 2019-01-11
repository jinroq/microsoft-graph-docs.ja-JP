---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: SiteCollection
localization_priority: Normal
ms.openlocfilehash: a0c55967ed7f7a397e0c8c0a4ce607921dc8a9f0
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27830549"
---
# <a name="sitecollection-resource"></a><span data-ttu-id="b8efe-102">SiteCollection リソース</span><span class="sxs-lookup"><span data-stu-id="b8efe-102">SiteCollection resource</span></span>

> <span data-ttu-id="b8efe-103">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="b8efe-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b8efe-104">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b8efe-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="b8efe-105">**siteCollection** リソースは、サイト コレクションの詳細を提供します。</span><span class="sxs-lookup"><span data-stu-id="b8efe-105">The **siteCollection** resource provides more information about a site collection.</span></span>

<span data-ttu-id="b8efe-106">[**サイト**](site.md) リソースが null ではない **siteCollection** プロパティを持つ場合、そのサイトはサイト コレクションのルート サイトです。</span><span class="sxs-lookup"><span data-stu-id="b8efe-106">If a [**site**](site.md) resource has a non-null **siteCollection** property, then the site is a root site for a site collection.</span></span>

## <a name="json-representation"></a><span data-ttu-id="b8efe-107">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="b8efe-107">JSON representation</span></span>

<span data-ttu-id="b8efe-108">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="b8efe-108">Here is a JSON representation of the resource.</span></span>

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

## <a name="properties"></a><span data-ttu-id="b8efe-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b8efe-109">Properties</span></span>

| <span data-ttu-id="b8efe-110">プロパティ名</span><span class="sxs-lookup"><span data-stu-id="b8efe-110">Property name</span></span>        | <span data-ttu-id="b8efe-111">Type</span><span class="sxs-lookup"><span data-stu-id="b8efe-111">Type</span></span>     | <span data-ttu-id="b8efe-112">説明</span><span class="sxs-lookup"><span data-stu-id="b8efe-112">Description</span></span>
|:---------------------|:---------|:---------------------------------------------------
| <span data-ttu-id="b8efe-113">**hostname**</span><span class="sxs-lookup"><span data-stu-id="b8efe-113">**hostname**</span></span>         | <span data-ttu-id="b8efe-114">文字列</span><span class="sxs-lookup"><span data-stu-id="b8efe-114">string</span></span>   | <span data-ttu-id="b8efe-p102">サイト コレクションのホスト名です。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="b8efe-p102">The hostname for the site collection. Read-only.</span></span>
| <span data-ttu-id="b8efe-117">**dataLocationCode**</span><span class="sxs-lookup"><span data-stu-id="b8efe-117">**dataLocationCode**</span></span> | <span data-ttu-id="b8efe-118">文字列</span><span class="sxs-lookup"><span data-stu-id="b8efe-118">string</span></span>   | <span data-ttu-id="b8efe-119">このサイト コレクションが存在する地域コード。</span><span class="sxs-lookup"><span data-stu-id="b8efe-119">The geographic region code for where this site collection resides.</span></span> <span data-ttu-id="b8efe-120">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="b8efe-120">Read-only.</span></span>
| <span data-ttu-id="b8efe-121">**root**</span><span class="sxs-lookup"><span data-stu-id="b8efe-121">**root**</span></span>             | <span data-ttu-id="b8efe-122">[root][]</span><span class="sxs-lookup"><span data-stu-id="b8efe-122">[root][]</span></span> | <span data-ttu-id="b8efe-123">存在する場合は、SharePoint 内のルート サイト コレクションがあることを示します。</span><span class="sxs-lookup"><span data-stu-id="b8efe-123">If present, indicates that this is a root site collection in SharePoint.</span></span> <span data-ttu-id="b8efe-124">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="b8efe-124">Read-only.</span></span>

[ルート]: root.md
[root]: root.md

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
