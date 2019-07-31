---
author: rahmit
description: WebPart リソースは、サイトページ上の web パーツの種類とレンダリング情報を表します。
ms.date: 09/01/2018
title: WebPart
localization_priority: Normal
ms.prod: sharepoint
doc_type: resourcePageType
ms.openlocfilehash: 71626440abe9eb63af3419b3e65c4351ae442dea
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36007355"
---
# <a name="webpart-resource"></a><span data-ttu-id="e64d5-103">webPart リソース</span><span class="sxs-lookup"><span data-stu-id="e64d5-103">webPart resource</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e64d5-104">**WebPart**リソースは、[サイトページ](sitepage.md)上の web パーツの種類とレンダリング情報を表します。</span><span class="sxs-lookup"><span data-stu-id="e64d5-104">The **webPart** resource represents type and rendering information for a web part on a [sitePage](sitepage.md).</span></span>

## <a name="json-representation"></a><span data-ttu-id="e64d5-105">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="e64d5-105">JSON representation</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [  ],
  "@odata.type": "microsoft.graph.webPart"
}-->

```json
{
  "type": "string (identifier)",
  "data": {"@odata.type":"microsoft.graph.sitePageData"}
}
```

## <a name="properties"></a><span data-ttu-id="e64d5-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="e64d5-106">Properties</span></span>

| <span data-ttu-id="e64d5-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="e64d5-107">Property</span></span>                | <span data-ttu-id="e64d5-108">型</span><span class="sxs-lookup"><span data-stu-id="e64d5-108">Type</span></span>             | <span data-ttu-id="e64d5-109">説明</span><span class="sxs-lookup"><span data-stu-id="e64d5-109">Description</span></span>
|:------------------------|:-----------------|:----------------------------------
| <span data-ttu-id="e64d5-110">**type**</span><span class="sxs-lookup"><span data-stu-id="e64d5-110">**type**</span></span>                | <span data-ttu-id="e64d5-111">String</span><span class="sxs-lookup"><span data-stu-id="e64d5-111">String</span></span>           | <span data-ttu-id="e64d5-112">WebPart の種類を指定する一意の識別子。</span><span class="sxs-lookup"><span data-stu-id="e64d5-112">A unique identifier specifying the webPart type.</span></span> <span data-ttu-id="e64d5-113">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="e64d5-113">Read-only.</span></span>
| <span data-ttu-id="e64d5-114">**data**</span><span class="sxs-lookup"><span data-stu-id="e64d5-114">**data**</span></span>                | <span data-ttu-id="e64d5-115">[sitePageData][]</span><span class="sxs-lookup"><span data-stu-id="e64d5-115">[sitePageData][]</span></span> | <span data-ttu-id="e64d5-116">WebPart に必要なプロパティ (webPart によって異なります)</span><span class="sxs-lookup"><span data-stu-id="e64d5-116">The required properties for the webPart (varies by webPart)</span></span>

[sitePageData]: sitepagedata.md

## <a name="remarks"></a><span data-ttu-id="e64d5-118">解説</span><span class="sxs-lookup"><span data-stu-id="e64d5-118">Remarks</span></span>

<span data-ttu-id="e64d5-119">Web パーツでは、**データ**の下に必要なプロパティを定義できます。</span><span class="sxs-lookup"><span data-stu-id="e64d5-119">Web parts can define their own required properties under **data**.</span></span>

<span data-ttu-id="e64d5-120">ページの詳細については、「 [Sitepage](sitepage.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="e64d5-120">For more information about pages, see [sitePage](sitepage.md).</span></span>
<!--
{
  "type": "#page.annotation",
  "description": "Defines a control resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Control",
  "suppressions": []
}
-->
