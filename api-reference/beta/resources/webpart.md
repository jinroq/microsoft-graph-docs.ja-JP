---
author: rahmit
ms.author: rahmit
ms.date: 09/01/2018
title: WebPart
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 9c019da7cb10a8c26faa8d338c54436043f83db8
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29510240"
---
# <a name="webpart-resource"></a><span data-ttu-id="69606-102">web パーツ リソース</span><span class="sxs-lookup"><span data-stu-id="69606-102">webPart resource</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="69606-103">**Web パーツ**リソースは、型との[sitePage](sitepage.md)上の web パーツのレンダリング情報を表します。</span><span class="sxs-lookup"><span data-stu-id="69606-103">The **webPart** resource represents type and rendering information for a web part on a [sitePage](sitepage.md).</span></span>

## <a name="json-representation"></a><span data-ttu-id="69606-104">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="69606-104">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="69606-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="69606-105">Properties</span></span>

| <span data-ttu-id="69606-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="69606-106">Property</span></span>                | <span data-ttu-id="69606-107">型</span><span class="sxs-lookup"><span data-stu-id="69606-107">Type</span></span>             | <span data-ttu-id="69606-108">説明</span><span class="sxs-lookup"><span data-stu-id="69606-108">Description</span></span>
|:------------------------|:-----------------|:----------------------------------
| <span data-ttu-id="69606-109">**type**</span><span class="sxs-lookup"><span data-stu-id="69606-109">**type**</span></span>                | <span data-ttu-id="69606-110">String</span><span class="sxs-lookup"><span data-stu-id="69606-110">String</span></span>           | <span data-ttu-id="69606-111">Web パーツの種類を指定する一意の識別子です。</span><span class="sxs-lookup"><span data-stu-id="69606-111">A unique identifier specifying the webPart type.</span></span> <span data-ttu-id="69606-112">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="69606-112">Read-only.</span></span>
| <span data-ttu-id="69606-113">**data**</span><span class="sxs-lookup"><span data-stu-id="69606-113">**data**</span></span>                | <span data-ttu-id="69606-114">[sitePageData][]</span><span class="sxs-lookup"><span data-stu-id="69606-114">[sitePageData][]</span></span> | <span data-ttu-id="69606-115">Web パーツ (web パーツによって異なります) に必要なプロパティ</span><span class="sxs-lookup"><span data-stu-id="69606-115">The required properties for the webPart (varies by webPart)</span></span>

[sitePageData]: sitepagedata.md

## <a name="remarks"></a><span data-ttu-id="69606-117">解説</span><span class="sxs-lookup"><span data-stu-id="69606-117">Remarks</span></span>

<span data-ttu-id="69606-118">Web パーツは、[**データ**の独自の必要なプロパティを定義できます。</span><span class="sxs-lookup"><span data-stu-id="69606-118">Web parts can define their own required properties under **data**.</span></span>

<span data-ttu-id="69606-119">ページの詳細については、 [sitePage](sitepage.md)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="69606-119">For more information about pages, see [sitePage](sitepage.md).</span></span>
<!--
{
  "type": "#page.annotation",
  "description": "Defines a control resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Control",
  "suppressions": [
    "Error: /api-reference/beta/resources/webpart.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
