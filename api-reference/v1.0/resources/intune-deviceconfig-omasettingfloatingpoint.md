---
title: omaSettingFloatingPoint リソースの種類
description: OMA 設定の浮動小数点の定義です。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 4720d635eeb119a2e1cacc741ab9c96f8ac55d4f
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32568998"
---
# <a name="omasettingfloatingpoint-resource-type"></a><span data-ttu-id="68f27-103">omaSettingFloatingPoint リソースの種類</span><span class="sxs-lookup"><span data-stu-id="68f27-103">omaSettingFloatingPoint resource type</span></span>

> <span data-ttu-id="68f27-104">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="68f27-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="68f27-105">OMA 設定の浮動小数点の定義です。</span><span class="sxs-lookup"><span data-stu-id="68f27-105">OMA Settings Floating Point definition.</span></span>


<span data-ttu-id="68f27-106">[omaSetting](../resources/intune-deviceconfig-omasetting.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="68f27-106">Inherits from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>

## <a name="properties"></a><span data-ttu-id="68f27-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="68f27-107">Properties</span></span>
|<span data-ttu-id="68f27-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="68f27-108">Property</span></span>|<span data-ttu-id="68f27-109">型</span><span class="sxs-lookup"><span data-stu-id="68f27-109">Type</span></span>|<span data-ttu-id="68f27-110">説明</span><span class="sxs-lookup"><span data-stu-id="68f27-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="68f27-111">displayName</span><span class="sxs-lookup"><span data-stu-id="68f27-111">displayName</span></span>|<span data-ttu-id="68f27-112">String</span><span class="sxs-lookup"><span data-stu-id="68f27-112">String</span></span>|<span data-ttu-id="68f27-113">表示名。</span><span class="sxs-lookup"><span data-stu-id="68f27-113">Display Name.</span></span> <span data-ttu-id="68f27-114">[omaSetting](../resources/intune-deviceconfig-omasetting.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="68f27-114">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="68f27-115">説明</span><span class="sxs-lookup"><span data-stu-id="68f27-115">description</span></span>|<span data-ttu-id="68f27-116">String</span><span class="sxs-lookup"><span data-stu-id="68f27-116">String</span></span>|<span data-ttu-id="68f27-117">説明。</span><span class="sxs-lookup"><span data-stu-id="68f27-117">Description.</span></span> <span data-ttu-id="68f27-118">[omaSetting](../resources/intune-deviceconfig-omasetting.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="68f27-118">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="68f27-119">omaUri</span><span class="sxs-lookup"><span data-stu-id="68f27-119">omaUri</span></span>|<span data-ttu-id="68f27-120">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="68f27-120">String</span></span>|<span data-ttu-id="68f27-121">OMA。</span><span class="sxs-lookup"><span data-stu-id="68f27-121">OMA.</span></span> <span data-ttu-id="68f27-122">[omaSetting](../resources/intune-deviceconfig-omasetting.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="68f27-122">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="68f27-123">値</span><span class="sxs-lookup"><span data-stu-id="68f27-123">value</span></span>|<span data-ttu-id="68f27-124">単精度浮動小数点型 (Single)</span><span class="sxs-lookup"><span data-stu-id="68f27-124">Single</span></span>|<span data-ttu-id="68f27-125">値。</span><span class="sxs-lookup"><span data-stu-id="68f27-125">Value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="68f27-126">関係</span><span class="sxs-lookup"><span data-stu-id="68f27-126">Relationships</span></span>
<span data-ttu-id="68f27-127">なし</span><span class="sxs-lookup"><span data-stu-id="68f27-127">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="68f27-128">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="68f27-128">JSON Representation</span></span>
<span data-ttu-id="68f27-129">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="68f27-129">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.omaSettingFloatingPoint"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.omaSettingFloatingPoint",
  "displayName": "String",
  "description": "String",
  "omaUri": "String",
  "value": "<Unknown Primitive Type Edm.Single>"
}
```



