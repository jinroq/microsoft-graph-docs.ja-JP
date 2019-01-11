---
author: rahmit
ms.author: rahmit
ms.date: 09/01/2018
title: WebPart
localization_priority: Normal
ms.openlocfilehash: f7293b986b5e6d77d0601cffb6b60edc5dfd2dd7
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27856029"
---
# <a name="webpart-resource"></a><span data-ttu-id="ff0f2-102">web パーツ リソース</span><span class="sxs-lookup"><span data-stu-id="ff0f2-102">webPart resource</span></span>

> <span data-ttu-id="ff0f2-103">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="ff0f2-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ff0f2-104">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ff0f2-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="ff0f2-105">**Web パーツ**リソースは、型との[sitePage](sitepage.md)上の web パーツのレンダリング情報を表します。</span><span class="sxs-lookup"><span data-stu-id="ff0f2-105">The **webPart** resource represents type and rendering information for a web part on a [sitePage](sitepage.md).</span></span>

## <a name="json-representation"></a><span data-ttu-id="ff0f2-106">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="ff0f2-106">JSON representation</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [  ],
  "@odata.type": "microsoft.graph.webPart"
}-->

```json
{
  "type": "string (guid)",
  "data": {
    "instanceId": "string (guid) (optional)"
  }
}
```

## <a name="properties"></a><span data-ttu-id="ff0f2-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="ff0f2-107">Properties</span></span>

| <span data-ttu-id="ff0f2-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="ff0f2-108">Property</span></span>                | <span data-ttu-id="ff0f2-109">種類</span><span class="sxs-lookup"><span data-stu-id="ff0f2-109">Type</span></span>             | <span data-ttu-id="ff0f2-110">説明</span><span class="sxs-lookup"><span data-stu-id="ff0f2-110">Description</span></span>
|:------------------------|:-----------------|:----------------------------------
| <span data-ttu-id="ff0f2-111">**type**</span><span class="sxs-lookup"><span data-stu-id="ff0f2-111">**type**</span></span>                | <span data-ttu-id="ff0f2-112">String</span><span class="sxs-lookup"><span data-stu-id="ff0f2-112">String</span></span>           | <span data-ttu-id="ff0f2-113">Web パーツの種類を指定する一意の識別子です。</span><span class="sxs-lookup"><span data-stu-id="ff0f2-113">A unique identifier specifying the webPart type.</span></span> <span data-ttu-id="ff0f2-114">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="ff0f2-114">Read-only.</span></span>
| <span data-ttu-id="ff0f2-115">**data**</span><span class="sxs-lookup"><span data-stu-id="ff0f2-115">**data**</span></span>                | <span data-ttu-id="ff0f2-116">[sitePageData][]</span><span class="sxs-lookup"><span data-stu-id="ff0f2-116">[sitePageData][]</span></span> | <span data-ttu-id="ff0f2-117">Web パーツ (web パーツによって異なります) に必要なプロパティ</span><span class="sxs-lookup"><span data-stu-id="ff0f2-117">The required properties for the webPart (varies by webPart)</span></span>

[sitePageData]: sitepagedata.md

## <a name="remarks"></a><span data-ttu-id="ff0f2-119">解説</span><span class="sxs-lookup"><span data-stu-id="ff0f2-119">Remarks</span></span>

<span data-ttu-id="ff0f2-120">Web パーツは、[**データ**の独自の必要なプロパティを定義できます。</span><span class="sxs-lookup"><span data-stu-id="ff0f2-120">Web parts can define their own required properties under **data**.</span></span>

<span data-ttu-id="ff0f2-121">ページの詳細については、 [sitePage](sitepage.md)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="ff0f2-121">For more information about pages, see [sitePage](sitepage.md).</span></span>
<!-- {
  "type": "#page.annotation",
  "description": "Defines a control resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Control"
} -->
