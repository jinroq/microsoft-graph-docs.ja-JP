---
title: licenseUnitsDetail リソースの種類
description: subscribedSku エンティティの prepaidUnits のプロパティは、licenseUnitsDetail 型です。
localization_priority: Normal
ms.openlocfilehash: a5eacb79dfca97b992e2f8584761aaa45beccd76
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29511318"
---
# <a name="licenseunitsdetail-resource-type"></a><span data-ttu-id="b5be2-103">licenseUnitsDetail リソースの種類</span><span class="sxs-lookup"><span data-stu-id="b5be2-103">licenseUnitsDetail resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b5be2-104">[subscribedSku](subscribedsku.md) エンティティの **prepaidUnits** のプロパティは、**licenseUnitsDetail** 型です。</span><span class="sxs-lookup"><span data-stu-id="b5be2-104">The **prepaidUnits** property of the [subscribedSku](subscribedsku.md) entity is of type **licenseUnitsDetail**.</span></span>

## <a name="properties"></a><span data-ttu-id="b5be2-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b5be2-105">Properties</span></span>
| <span data-ttu-id="b5be2-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b5be2-106">Property</span></span>     | <span data-ttu-id="b5be2-107">型</span><span class="sxs-lookup"><span data-stu-id="b5be2-107">Type</span></span>   |<span data-ttu-id="b5be2-108">説明</span><span class="sxs-lookup"><span data-stu-id="b5be2-108">Description</span></span>|
|:-------------|:-----|:----------|
|<span data-ttu-id="b5be2-109">enabled</span><span class="sxs-lookup"><span data-stu-id="b5be2-109">enabled</span></span>|<span data-ttu-id="b5be2-110">Int32</span><span class="sxs-lookup"><span data-stu-id="b5be2-110">Int32</span></span>| <span data-ttu-id="b5be2-111">有効になっている単位の数です。</span><span class="sxs-lookup"><span data-stu-id="b5be2-111">The number of units that are enabled.</span></span> |
|<span data-ttu-id="b5be2-112">suspended</span><span class="sxs-lookup"><span data-stu-id="b5be2-112">suspended</span></span>|<span data-ttu-id="b5be2-113">Int32</span><span class="sxs-lookup"><span data-stu-id="b5be2-113">Int32</span></span>| <span data-ttu-id="b5be2-114">利用停止中の単位の数です。</span><span class="sxs-lookup"><span data-stu-id="b5be2-114">The number of units that are suspended.</span></span> |
|<span data-ttu-id="b5be2-115">warning</span><span class="sxs-lookup"><span data-stu-id="b5be2-115">warning</span></span>|<span data-ttu-id="b5be2-116">Int32</span><span class="sxs-lookup"><span data-stu-id="b5be2-116">Int32</span></span>| <span data-ttu-id="b5be2-117">警告ステータスのユニットの数です。</span><span class="sxs-lookup"><span data-stu-id="b5be2-117">The number of units that are in warning status.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="b5be2-118">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="b5be2-118">JSON representation</span></span>

<span data-ttu-id="b5be2-119">以下は、リソースの JSON 表記です</span><span class="sxs-lookup"><span data-stu-id="b5be2-119">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.licenseUnitsDetail"
}-->

```json
{
  "enabled": 1024,
  "suspended": 1024,
  "warning": 1024
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "licenseUnitsDetail resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/licenseunitsdetail.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
