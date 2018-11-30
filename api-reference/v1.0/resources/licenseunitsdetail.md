---
title: licenseUnitsDetail リソースの種類
description: subscribedSku エンティティの **prepaidUnits** のプロパティは、**licenseUnitsDetail** 型です。
ms.openlocfilehash: e8cf5253676dab8a4b31c3ab33faa0af3ddfd527
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27020381"
---
# <a name="licenseunitsdetail-resource-type"></a><span data-ttu-id="76468-103">licenseUnitsDetail リソースの種類</span><span class="sxs-lookup"><span data-stu-id="76468-103">licenseUnitsDetail resource type</span></span>

<span data-ttu-id="76468-104">[subscribedSku](subscribedsku.md) エンティティの **prepaidUnits** のプロパティは、**licenseUnitsDetail** 型です。</span><span class="sxs-lookup"><span data-stu-id="76468-104">The **prepaidUnits** property of the [subscribedSku](subscribedsku.md) entity is of type **licenseUnitsDetail**.</span></span>

## <a name="properties"></a><span data-ttu-id="76468-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="76468-105">Properties</span></span>
| <span data-ttu-id="76468-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="76468-106">Property</span></span>     | <span data-ttu-id="76468-107">型</span><span class="sxs-lookup"><span data-stu-id="76468-107">Type</span></span>   |<span data-ttu-id="76468-108">説明</span><span class="sxs-lookup"><span data-stu-id="76468-108">Description</span></span>|
|:-------------|:-----|:----------|
|<span data-ttu-id="76468-109">enabled</span><span class="sxs-lookup"><span data-stu-id="76468-109">enabled</span></span>|<span data-ttu-id="76468-110">Int32</span><span class="sxs-lookup"><span data-stu-id="76468-110">Int32</span></span>| <span data-ttu-id="76468-111">有効になっている単位の数です。</span><span class="sxs-lookup"><span data-stu-id="76468-111">The number of units that are enabled.</span></span> |
|<span data-ttu-id="76468-112">suspended</span><span class="sxs-lookup"><span data-stu-id="76468-112">suspended</span></span>|<span data-ttu-id="76468-113">Int32</span><span class="sxs-lookup"><span data-stu-id="76468-113">Int32</span></span>| <span data-ttu-id="76468-114">利用停止中の単位の数です。</span><span class="sxs-lookup"><span data-stu-id="76468-114">The number of units that are suspended.</span></span> |
|<span data-ttu-id="76468-115">warning</span><span class="sxs-lookup"><span data-stu-id="76468-115">warning</span></span>|<span data-ttu-id="76468-116">Int32</span><span class="sxs-lookup"><span data-stu-id="76468-116">Int32</span></span>| <span data-ttu-id="76468-117">警告ステータスのユニットの数です。</span><span class="sxs-lookup"><span data-stu-id="76468-117">The number of units that are in warning status.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="76468-118">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="76468-118">JSON representation</span></span>

<span data-ttu-id="76468-119">以下は、リソースの JSON 表記です</span><span class="sxs-lookup"><span data-stu-id="76468-119">Here is a JSON representation of the resource</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "licenseUnitsDetail resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
