---
author: rahmit
ms.author: rahmit
ms.date: 09/01/2018
title: WebPart
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 9c019da7cb10a8c26faa8d338c54436043f83db8
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32453610"
---
# <a name="webpart-resource"></a><span data-ttu-id="75646-102">webPart リソース</span><span class="sxs-lookup"><span data-stu-id="75646-102">webPart resource</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="75646-103">**webPart**リソースは、[サイトページ](sitepage.md)上の web パーツの種類とレンダリング情報を表します。</span><span class="sxs-lookup"><span data-stu-id="75646-103">The **webPart** resource represents type and rendering information for a web part on a [sitePage](sitepage.md).</span></span>

## <a name="json-representation"></a><span data-ttu-id="75646-104">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="75646-104">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="75646-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="75646-105">Properties</span></span>

| <span data-ttu-id="75646-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="75646-106">Property</span></span>                | <span data-ttu-id="75646-107">型</span><span class="sxs-lookup"><span data-stu-id="75646-107">Type</span></span>             | <span data-ttu-id="75646-108">説明</span><span class="sxs-lookup"><span data-stu-id="75646-108">Description</span></span>
|:------------------------|:-----------------|:----------------------------------
| <span data-ttu-id="75646-109">**type**</span><span class="sxs-lookup"><span data-stu-id="75646-109">**type**</span></span>                | <span data-ttu-id="75646-110">String</span><span class="sxs-lookup"><span data-stu-id="75646-110">String</span></span>           | <span data-ttu-id="75646-111">webPart の種類を指定する一意の識別子。</span><span class="sxs-lookup"><span data-stu-id="75646-111">A unique identifier specifying the webPart type.</span></span> <span data-ttu-id="75646-112">値の取得のみ可能です。</span><span class="sxs-lookup"><span data-stu-id="75646-112">Read-only.</span></span>
| <span data-ttu-id="75646-113">**data**</span><span class="sxs-lookup"><span data-stu-id="75646-113">**data**</span></span>                | <span data-ttu-id="75646-114">[sitepagedata][]</span><span class="sxs-lookup"><span data-stu-id="75646-114">[sitePageData][]</span></span> | <span data-ttu-id="75646-115">webpart に必要なプロパティ (webpart によって異なります)</span><span class="sxs-lookup"><span data-stu-id="75646-115">The required properties for the webPart (varies by webPart)</span></span>

[sitepagedata]: sitepagedata.md
[sitePageData]: sitepagedata.md

## <a name="remarks"></a><span data-ttu-id="75646-117">解説</span><span class="sxs-lookup"><span data-stu-id="75646-117">Remarks</span></span>

<span data-ttu-id="75646-118">Web パーツでは、**データ**の下に必要なプロパティを定義できます。</span><span class="sxs-lookup"><span data-stu-id="75646-118">Web parts can define their own required properties under **data**.</span></span>

<span data-ttu-id="75646-119">ページの詳細については、「 [sitepage](sitepage.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="75646-119">For more information about pages, see [sitePage](sitepage.md).</span></span>
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
