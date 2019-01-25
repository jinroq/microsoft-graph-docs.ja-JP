---
title: educationLinkResource リソースの種類
description: EducationResource のサブクラスです。 このリソースは、リンクとは必要なデータに関連付けられていないことです。
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 09e7c7c5070d6f8f288dbf18d6fb9ce81b456092
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29516960"
---
# <a name="educationlinkresource-resource-type"></a><span data-ttu-id="14417-104">educationLinkResource リソースの種類</span><span class="sxs-lookup"><span data-stu-id="14417-104">educationLinkResource resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="14417-105">[EducationResource](educationresource.md)のサブクラスです。</span><span class="sxs-lookup"><span data-stu-id="14417-105">A subclass of [educationResource](educationresource.md).</span></span> <span data-ttu-id="14417-106">このリソースは、リンクとは必要なデータに関連付けられていないことです。</span><span class="sxs-lookup"><span data-stu-id="14417-106">This resource is a link and does not have any additional data associated with it.</span></span>


## <a name="properties"></a><span data-ttu-id="14417-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="14417-107">Properties</span></span>
| <span data-ttu-id="14417-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="14417-108">Property</span></span>     | <span data-ttu-id="14417-109">型</span><span class="sxs-lookup"><span data-stu-id="14417-109">Type</span></span>   |<span data-ttu-id="14417-110">説明</span><span class="sxs-lookup"><span data-stu-id="14417-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="14417-111">link</span><span class="sxs-lookup"><span data-stu-id="14417-111">link</span></span>|<span data-ttu-id="14417-112">String</span><span class="sxs-lookup"><span data-stu-id="14417-112">String</span></span>|<span data-ttu-id="14417-113">リソースへの URL です。</span><span class="sxs-lookup"><span data-stu-id="14417-113">URL to the resource.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="14417-114">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="14417-114">JSON representation</span></span>

<span data-ttu-id="14417-115">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="14417-115">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationLinkResource"
}-->

```json
{
  "link": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "educationLinkResource resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/educationlinkresource.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
