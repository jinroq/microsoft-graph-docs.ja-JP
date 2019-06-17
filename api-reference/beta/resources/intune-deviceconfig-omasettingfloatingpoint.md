---
title: omaSettingFloatingPoint リソースの種類
description: OMA 設定の浮動小数点の定義です。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 3507d35f2134b337fcd984104b95eec246c874c7
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/14/2019
ms.locfileid: "34995834"
---
# <a name="omasettingfloatingpoint-resource-type"></a><span data-ttu-id="c520e-103">omaSettingFloatingPoint リソースの種類</span><span class="sxs-lookup"><span data-stu-id="c520e-103">omaSettingFloatingPoint resource type</span></span>

> <span data-ttu-id="c520e-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c520e-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c520e-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="c520e-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c520e-106">OMA 設定の浮動小数点の定義です。</span><span class="sxs-lookup"><span data-stu-id="c520e-106">OMA Settings Floating Point definition.</span></span>


<span data-ttu-id="c520e-107">[omaSetting](../resources/intune-deviceconfig-omasetting.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="c520e-107">Inherits from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>

## <a name="properties"></a><span data-ttu-id="c520e-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="c520e-108">Properties</span></span>
|<span data-ttu-id="c520e-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="c520e-109">Property</span></span>|<span data-ttu-id="c520e-110">型</span><span class="sxs-lookup"><span data-stu-id="c520e-110">Type</span></span>|<span data-ttu-id="c520e-111">説明</span><span class="sxs-lookup"><span data-stu-id="c520e-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c520e-112">displayName</span><span class="sxs-lookup"><span data-stu-id="c520e-112">displayName</span></span>|<span data-ttu-id="c520e-113">String</span><span class="sxs-lookup"><span data-stu-id="c520e-113">String</span></span>|<span data-ttu-id="c520e-114">表示名。</span><span class="sxs-lookup"><span data-stu-id="c520e-114">Display Name.</span></span> <span data-ttu-id="c520e-115">[omaSetting](../resources/intune-deviceconfig-omasetting.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="c520e-115">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="c520e-116">description</span><span class="sxs-lookup"><span data-stu-id="c520e-116">description</span></span>|<span data-ttu-id="c520e-117">String</span><span class="sxs-lookup"><span data-stu-id="c520e-117">String</span></span>|<span data-ttu-id="c520e-118">説明。</span><span class="sxs-lookup"><span data-stu-id="c520e-118">Description.</span></span> <span data-ttu-id="c520e-119">[omaSetting](../resources/intune-deviceconfig-omasetting.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="c520e-119">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="c520e-120">omaUri</span><span class="sxs-lookup"><span data-stu-id="c520e-120">omaUri</span></span>|<span data-ttu-id="c520e-121">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="c520e-121">String</span></span>|<span data-ttu-id="c520e-122">OMA。</span><span class="sxs-lookup"><span data-stu-id="c520e-122">OMA.</span></span> <span data-ttu-id="c520e-123">[omaSetting](../resources/intune-deviceconfig-omasetting.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="c520e-123">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="c520e-124">値</span><span class="sxs-lookup"><span data-stu-id="c520e-124">value</span></span>|<span data-ttu-id="c520e-125">単精度浮動小数点型 (Single)</span><span class="sxs-lookup"><span data-stu-id="c520e-125">Single</span></span>|<span data-ttu-id="c520e-126">値。</span><span class="sxs-lookup"><span data-stu-id="c520e-126">Value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c520e-127">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="c520e-127">Relationships</span></span>
<span data-ttu-id="c520e-128">なし</span><span class="sxs-lookup"><span data-stu-id="c520e-128">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="c520e-129">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="c520e-129">JSON Representation</span></span>
<span data-ttu-id="c520e-130">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="c520e-130">Here is a JSON representation of the resource.</span></span>
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





