---
author: rahmit
ms.author: rahmit
ms.date: 09/01/2018
title: WebPart
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 03b5f1007d8dbe6587da736cdf0ac0fdc1ed8a55
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33345793"
---
# <a name="webpart-resource"></a><span data-ttu-id="cef09-102">webPart リソース</span><span class="sxs-lookup"><span data-stu-id="cef09-102">webPart resource</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="cef09-103">**webPart**リソースは、[サイトページ](sitepage.md)上の web パーツの種類とレンダリング情報を表します。</span><span class="sxs-lookup"><span data-stu-id="cef09-103">The **webPart** resource represents type and rendering information for a web part on a [sitePage](sitepage.md).</span></span>

## <a name="json-representation"></a><span data-ttu-id="cef09-104">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="cef09-104">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="cef09-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="cef09-105">Properties</span></span>

| <span data-ttu-id="cef09-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="cef09-106">Property</span></span>                | <span data-ttu-id="cef09-107">型</span><span class="sxs-lookup"><span data-stu-id="cef09-107">Type</span></span>             | <span data-ttu-id="cef09-108">説明</span><span class="sxs-lookup"><span data-stu-id="cef09-108">Description</span></span>
|:------------------------|:-----------------|:----------------------------------
| <span data-ttu-id="cef09-109">**type**</span><span class="sxs-lookup"><span data-stu-id="cef09-109">**type**</span></span>                | <span data-ttu-id="cef09-110">String</span><span class="sxs-lookup"><span data-stu-id="cef09-110">String</span></span>           | <span data-ttu-id="cef09-111">webPart の種類を指定する一意の識別子。</span><span class="sxs-lookup"><span data-stu-id="cef09-111">A unique identifier specifying the webPart type.</span></span> <span data-ttu-id="cef09-112">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="cef09-112">Read-only.</span></span>
| <span data-ttu-id="cef09-113">**data**</span><span class="sxs-lookup"><span data-stu-id="cef09-113">**data**</span></span>                | <span data-ttu-id="cef09-114">[sitepagedata][]</span><span class="sxs-lookup"><span data-stu-id="cef09-114">[sitePageData][]</span></span> | <span data-ttu-id="cef09-115">webpart に必要なプロパティ (webpart によって異なります)</span><span class="sxs-lookup"><span data-stu-id="cef09-115">The required properties for the webPart (varies by webPart)</span></span>

[sitepagedata]: sitepagedata.md
[sitePageData]: sitepagedata.md

## <a name="remarks"></a><span data-ttu-id="cef09-117">注釈</span><span class="sxs-lookup"><span data-stu-id="cef09-117">Remarks</span></span>

<span data-ttu-id="cef09-118">Web パーツでは、**データ**の下に必要なプロパティを定義できます。</span><span class="sxs-lookup"><span data-stu-id="cef09-118">Web parts can define their own required properties under **data**.</span></span>

<span data-ttu-id="cef09-119">ページの詳細については、「 [sitepage](sitepage.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="cef09-119">For more information about pages, see [sitePage](sitepage.md).</span></span>
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
