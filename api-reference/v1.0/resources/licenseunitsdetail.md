---
title: licenseUnitsDetail リソースの種類
description: '**subscribedSku** エンティティの prepaidUnits のプロパティは、**licenseUnitsDetail** 型です。'
localization_priority: Normal
ms.openlocfilehash: 8c2a4e995c7e1afa63b7f9daea6b61cbaf974958
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32519908"
---
# <a name="licenseunitsdetail-resource-type"></a><span data-ttu-id="f3a01-103">licenseUnitsDetail リソースの種類</span><span class="sxs-lookup"><span data-stu-id="f3a01-103">licenseUnitsDetail resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f3a01-104">**subscribedSku** エンティティの [prepaidUnits](subscribedsku.md) のプロパティは、**licenseUnitsDetail** 型です。</span><span class="sxs-lookup"><span data-stu-id="f3a01-104">The **prepaidUnits** property of the [subscribedSku](subscribedsku.md) entity is of type **licenseUnitsDetail**.</span></span>

## <a name="properties"></a><span data-ttu-id="f3a01-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="f3a01-105">Properties</span></span>
| <span data-ttu-id="f3a01-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="f3a01-106">Property</span></span>     | <span data-ttu-id="f3a01-107">型</span><span class="sxs-lookup"><span data-stu-id="f3a01-107">Type</span></span>   |<span data-ttu-id="f3a01-108">説明</span><span class="sxs-lookup"><span data-stu-id="f3a01-108">Description</span></span>|
|:-------------|:-----|:----------|
|<span data-ttu-id="f3a01-109">enabled</span><span class="sxs-lookup"><span data-stu-id="f3a01-109">enabled</span></span>|<span data-ttu-id="f3a01-110">Int32</span><span class="sxs-lookup"><span data-stu-id="f3a01-110">Int32</span></span>| <span data-ttu-id="f3a01-111">有効になっている単位の数。</span><span class="sxs-lookup"><span data-stu-id="f3a01-111">The number of units that are enabled.</span></span> |
|<span data-ttu-id="f3a01-112">suspended</span><span class="sxs-lookup"><span data-stu-id="f3a01-112">suspended</span></span>|<span data-ttu-id="f3a01-113">Int32</span><span class="sxs-lookup"><span data-stu-id="f3a01-113">Int32</span></span>| <span data-ttu-id="f3a01-114">中断されている単位の数。</span><span class="sxs-lookup"><span data-stu-id="f3a01-114">The number of units that are suspended.</span></span> |
|<span data-ttu-id="f3a01-115">warning</span><span class="sxs-lookup"><span data-stu-id="f3a01-115">warning</span></span>|<span data-ttu-id="f3a01-116">Int32</span><span class="sxs-lookup"><span data-stu-id="f3a01-116">Int32</span></span>| <span data-ttu-id="f3a01-117">警告状態にある単位数。</span><span class="sxs-lookup"><span data-stu-id="f3a01-117">The number of units that are in warning status.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="f3a01-118">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="f3a01-118">JSON representation</span></span>

<span data-ttu-id="f3a01-119">以下は、リソースの JSON 表記です</span><span class="sxs-lookup"><span data-stu-id="f3a01-119">Here is a JSON representation of the resource</span></span>

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
