---
title: omaSettingFloatingPoint リソースの種類
description: OMA 設定の浮動小数点の定義です。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 122a8fd7ffdef7d314e16bf6154838e09598f7d5
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36031319"
---
# <a name="omasettingfloatingpoint-resource-type"></a><span data-ttu-id="9535c-103">omaSettingFloatingPoint リソースの種類</span><span class="sxs-lookup"><span data-stu-id="9535c-103">omaSettingFloatingPoint resource type</span></span>

> <span data-ttu-id="9535c-104">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="9535c-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9535c-105">OMA 設定の浮動小数点の定義です。</span><span class="sxs-lookup"><span data-stu-id="9535c-105">OMA Settings Floating Point definition.</span></span>


<span data-ttu-id="9535c-106">[omaSetting](../resources/intune-deviceconfig-omasetting.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="9535c-106">Inherits from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>

## <a name="properties"></a><span data-ttu-id="9535c-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="9535c-107">Properties</span></span>
|<span data-ttu-id="9535c-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="9535c-108">Property</span></span>|<span data-ttu-id="9535c-109">型</span><span class="sxs-lookup"><span data-stu-id="9535c-109">Type</span></span>|<span data-ttu-id="9535c-110">説明</span><span class="sxs-lookup"><span data-stu-id="9535c-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9535c-111">displayName</span><span class="sxs-lookup"><span data-stu-id="9535c-111">displayName</span></span>|<span data-ttu-id="9535c-112">String</span><span class="sxs-lookup"><span data-stu-id="9535c-112">String</span></span>|<span data-ttu-id="9535c-113">表示名。</span><span class="sxs-lookup"><span data-stu-id="9535c-113">Display Name.</span></span> <span data-ttu-id="9535c-114">[omaSetting](../resources/intune-deviceconfig-omasetting.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="9535c-114">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="9535c-115">description</span><span class="sxs-lookup"><span data-stu-id="9535c-115">description</span></span>|<span data-ttu-id="9535c-116">String</span><span class="sxs-lookup"><span data-stu-id="9535c-116">String</span></span>|<span data-ttu-id="9535c-117">説明。</span><span class="sxs-lookup"><span data-stu-id="9535c-117">Description.</span></span> <span data-ttu-id="9535c-118">[omaSetting](../resources/intune-deviceconfig-omasetting.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="9535c-118">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="9535c-119">omaUri</span><span class="sxs-lookup"><span data-stu-id="9535c-119">omaUri</span></span>|<span data-ttu-id="9535c-120">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="9535c-120">String</span></span>|<span data-ttu-id="9535c-121">OMA。</span><span class="sxs-lookup"><span data-stu-id="9535c-121">OMA.</span></span> <span data-ttu-id="9535c-122">[omaSetting](../resources/intune-deviceconfig-omasetting.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="9535c-122">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="9535c-123">値</span><span class="sxs-lookup"><span data-stu-id="9535c-123">value</span></span>|<span data-ttu-id="9535c-124">単精度浮動小数点型 (Single)</span><span class="sxs-lookup"><span data-stu-id="9535c-124">Single</span></span>|<span data-ttu-id="9535c-125">値。</span><span class="sxs-lookup"><span data-stu-id="9535c-125">Value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="9535c-126">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="9535c-126">Relationships</span></span>
<span data-ttu-id="9535c-127">なし</span><span class="sxs-lookup"><span data-stu-id="9535c-127">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="9535c-128">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="9535c-128">JSON Representation</span></span>
<span data-ttu-id="9535c-129">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="9535c-129">Here is a JSON representation of the resource.</span></span>
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



