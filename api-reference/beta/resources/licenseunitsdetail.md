---
title: licenseUnitsDetail リソースの種類
description: '**subscribedSku** エンティティの prepaidUnits のプロパティは、**licenseUnitsDetail** 型です。'
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: 4482f9661b41981717422c7c874319fbca7be23d
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35966976"
---
# <a name="licenseunitsdetail-resource-type"></a><span data-ttu-id="b3bc8-103">licenseUnitsDetail リソースの種類</span><span class="sxs-lookup"><span data-stu-id="b3bc8-103">licenseUnitsDetail resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b3bc8-104">**subscribedSku** エンティティの [prepaidUnits](subscribedsku.md) のプロパティは、**licenseUnitsDetail** 型です。</span><span class="sxs-lookup"><span data-stu-id="b3bc8-104">The **prepaidUnits** property of the [subscribedSku](subscribedsku.md) entity is of type **licenseUnitsDetail**.</span></span>

## <a name="properties"></a><span data-ttu-id="b3bc8-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b3bc8-105">Properties</span></span>
| <span data-ttu-id="b3bc8-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b3bc8-106">Property</span></span>     | <span data-ttu-id="b3bc8-107">型</span><span class="sxs-lookup"><span data-stu-id="b3bc8-107">Type</span></span>   |<span data-ttu-id="b3bc8-108">説明</span><span class="sxs-lookup"><span data-stu-id="b3bc8-108">Description</span></span>|
|:-------------|:-----|:----------|
|<span data-ttu-id="b3bc8-109">enabled</span><span class="sxs-lookup"><span data-stu-id="b3bc8-109">enabled</span></span>|<span data-ttu-id="b3bc8-110">Int32</span><span class="sxs-lookup"><span data-stu-id="b3bc8-110">Int32</span></span>| <span data-ttu-id="b3bc8-111">有効になっている単位の数。</span><span class="sxs-lookup"><span data-stu-id="b3bc8-111">The number of units that are enabled.</span></span> |
|<span data-ttu-id="b3bc8-112">suspended</span><span class="sxs-lookup"><span data-stu-id="b3bc8-112">suspended</span></span>|<span data-ttu-id="b3bc8-113">Int32</span><span class="sxs-lookup"><span data-stu-id="b3bc8-113">Int32</span></span>| <span data-ttu-id="b3bc8-114">中断されている単位の数。</span><span class="sxs-lookup"><span data-stu-id="b3bc8-114">The number of units that are suspended.</span></span> |
|<span data-ttu-id="b3bc8-115">warning</span><span class="sxs-lookup"><span data-stu-id="b3bc8-115">warning</span></span>|<span data-ttu-id="b3bc8-116">Int32</span><span class="sxs-lookup"><span data-stu-id="b3bc8-116">Int32</span></span>| <span data-ttu-id="b3bc8-117">警告状態にある単位数。</span><span class="sxs-lookup"><span data-stu-id="b3bc8-117">The number of units that are in warning status.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="b3bc8-118">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="b3bc8-118">JSON representation</span></span>

<span data-ttu-id="b3bc8-119">以下は、リソースの JSON 表記です</span><span class="sxs-lookup"><span data-stu-id="b3bc8-119">Here is a JSON representation of the resource</span></span>

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
  "suppressions": []
}
-->
