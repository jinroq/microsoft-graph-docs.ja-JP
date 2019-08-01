---
title: licenseUnitsDetail リソースの種類
description: '**subscribedSku** エンティティの prepaidUnits のプロパティは、**licenseUnitsDetail** 型です。'
localization_priority: Normal
author: ''
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: b4540cb546c8dae9d519a68b6ace8d030b6c40cd
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36036464"
---
# <a name="licenseunitsdetail-resource-type"></a><span data-ttu-id="e9cef-103">licenseUnitsDetail リソースの種類</span><span class="sxs-lookup"><span data-stu-id="e9cef-103">licenseUnitsDetail resource type</span></span>

<span data-ttu-id="e9cef-104">**subscribedSku** エンティティの [prepaidUnits](subscribedsku.md) のプロパティは、**licenseUnitsDetail** 型です。</span><span class="sxs-lookup"><span data-stu-id="e9cef-104">The **prepaidUnits** property of the [subscribedSku](subscribedsku.md) entity is of type **licenseUnitsDetail**.</span></span>

## <a name="properties"></a><span data-ttu-id="e9cef-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="e9cef-105">Properties</span></span>
| <span data-ttu-id="e9cef-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="e9cef-106">Property</span></span>     | <span data-ttu-id="e9cef-107">型</span><span class="sxs-lookup"><span data-stu-id="e9cef-107">Type</span></span>   |<span data-ttu-id="e9cef-108">説明</span><span class="sxs-lookup"><span data-stu-id="e9cef-108">Description</span></span>|
|:-------------|:-----|:----------|
|<span data-ttu-id="e9cef-109">enabled</span><span class="sxs-lookup"><span data-stu-id="e9cef-109">enabled</span></span>|<span data-ttu-id="e9cef-110">Int32</span><span class="sxs-lookup"><span data-stu-id="e9cef-110">Int32</span></span>| <span data-ttu-id="e9cef-111">有効になっている単位の数。</span><span class="sxs-lookup"><span data-stu-id="e9cef-111">The number of units that are enabled.</span></span> |
|<span data-ttu-id="e9cef-112">suspended</span><span class="sxs-lookup"><span data-stu-id="e9cef-112">suspended</span></span>|<span data-ttu-id="e9cef-113">Int32</span><span class="sxs-lookup"><span data-stu-id="e9cef-113">Int32</span></span>| <span data-ttu-id="e9cef-114">中断されている単位の数。</span><span class="sxs-lookup"><span data-stu-id="e9cef-114">The number of units that are suspended.</span></span> |
|<span data-ttu-id="e9cef-115">warning</span><span class="sxs-lookup"><span data-stu-id="e9cef-115">warning</span></span>|<span data-ttu-id="e9cef-116">Int32</span><span class="sxs-lookup"><span data-stu-id="e9cef-116">Int32</span></span>| <span data-ttu-id="e9cef-117">警告状態にある単位数。</span><span class="sxs-lookup"><span data-stu-id="e9cef-117">The number of units that are in warning status.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="e9cef-118">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="e9cef-118">JSON representation</span></span>

<span data-ttu-id="e9cef-119">以下は、リソースの JSON 表記です</span><span class="sxs-lookup"><span data-stu-id="e9cef-119">Here is a JSON representation of the resource</span></span>

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
