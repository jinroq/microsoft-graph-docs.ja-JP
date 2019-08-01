---
title: omaSettingInteger リソースの種類
description: OMA 設定の整数の定義。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: f80f8583907a25646643fdd5770d6bce5adcb4b3
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36028022"
---
# <a name="omasettinginteger-resource-type"></a><span data-ttu-id="e0d9f-103">omaSettingInteger リソースの種類</span><span class="sxs-lookup"><span data-stu-id="e0d9f-103">omaSettingInteger resource type</span></span>

> <span data-ttu-id="e0d9f-104">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="e0d9f-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e0d9f-105">OMA 設定の整数の定義。</span><span class="sxs-lookup"><span data-stu-id="e0d9f-105">OMA Settings Integer definition.</span></span>


<span data-ttu-id="e0d9f-106">[omaSetting](../resources/intune-deviceconfig-omasetting.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="e0d9f-106">Inherits from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>

## <a name="properties"></a><span data-ttu-id="e0d9f-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="e0d9f-107">Properties</span></span>
|<span data-ttu-id="e0d9f-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="e0d9f-108">Property</span></span>|<span data-ttu-id="e0d9f-109">型</span><span class="sxs-lookup"><span data-stu-id="e0d9f-109">Type</span></span>|<span data-ttu-id="e0d9f-110">説明</span><span class="sxs-lookup"><span data-stu-id="e0d9f-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e0d9f-111">displayName</span><span class="sxs-lookup"><span data-stu-id="e0d9f-111">displayName</span></span>|<span data-ttu-id="e0d9f-112">String</span><span class="sxs-lookup"><span data-stu-id="e0d9f-112">String</span></span>|<span data-ttu-id="e0d9f-113">表示名。</span><span class="sxs-lookup"><span data-stu-id="e0d9f-113">Display Name.</span></span> <span data-ttu-id="e0d9f-114">[omaSetting](../resources/intune-deviceconfig-omasetting.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="e0d9f-114">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="e0d9f-115">description</span><span class="sxs-lookup"><span data-stu-id="e0d9f-115">description</span></span>|<span data-ttu-id="e0d9f-116">String</span><span class="sxs-lookup"><span data-stu-id="e0d9f-116">String</span></span>|<span data-ttu-id="e0d9f-117">説明。</span><span class="sxs-lookup"><span data-stu-id="e0d9f-117">Description.</span></span> <span data-ttu-id="e0d9f-118">[omaSetting](../resources/intune-deviceconfig-omasetting.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="e0d9f-118">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="e0d9f-119">omaUri</span><span class="sxs-lookup"><span data-stu-id="e0d9f-119">omaUri</span></span>|<span data-ttu-id="e0d9f-120">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="e0d9f-120">String</span></span>|<span data-ttu-id="e0d9f-121">OMA。</span><span class="sxs-lookup"><span data-stu-id="e0d9f-121">OMA.</span></span> <span data-ttu-id="e0d9f-122">[omaSetting](../resources/intune-deviceconfig-omasetting.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="e0d9f-122">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="e0d9f-123">値</span><span class="sxs-lookup"><span data-stu-id="e0d9f-123">value</span></span>|<span data-ttu-id="e0d9f-124">Int32</span><span class="sxs-lookup"><span data-stu-id="e0d9f-124">Int32</span></span>|<span data-ttu-id="e0d9f-125">値。</span><span class="sxs-lookup"><span data-stu-id="e0d9f-125">Value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e0d9f-126">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="e0d9f-126">Relationships</span></span>
<span data-ttu-id="e0d9f-127">なし</span><span class="sxs-lookup"><span data-stu-id="e0d9f-127">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="e0d9f-128">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="e0d9f-128">JSON Representation</span></span>
<span data-ttu-id="e0d9f-129">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="e0d9f-129">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.omaSettingInteger"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.omaSettingInteger",
  "displayName": "String",
  "description": "String",
  "omaUri": "String",
  "value": 1024
}
```



