---
title: omaSettingDateTime リソースの種類
description: OMA 設定の DateTime の定義です。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 20bc82e88480dca1df727e299e62c4274002176f
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/26/2019
ms.locfileid: "30260915"
---
# <a name="omasettingdatetime-resource-type"></a><span data-ttu-id="7f987-103">omaSettingDateTime リソースの種類</span><span class="sxs-lookup"><span data-stu-id="7f987-103">omaSettingDateTime resource type</span></span>

> <span data-ttu-id="7f987-104">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="7f987-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7f987-105">OMA 設定の DateTime の定義です。</span><span class="sxs-lookup"><span data-stu-id="7f987-105">OMA Settings DateTime definition.</span></span>


<span data-ttu-id="7f987-106">[omaSetting](../resources/intune-deviceconfig-omasetting.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="7f987-106">Inherits from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>

## <a name="properties"></a><span data-ttu-id="7f987-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="7f987-107">Properties</span></span>
|<span data-ttu-id="7f987-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="7f987-108">Property</span></span>|<span data-ttu-id="7f987-109">型</span><span class="sxs-lookup"><span data-stu-id="7f987-109">Type</span></span>|<span data-ttu-id="7f987-110">説明</span><span class="sxs-lookup"><span data-stu-id="7f987-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7f987-111">displayName</span><span class="sxs-lookup"><span data-stu-id="7f987-111">displayName</span></span>|<span data-ttu-id="7f987-112">String</span><span class="sxs-lookup"><span data-stu-id="7f987-112">String</span></span>|<span data-ttu-id="7f987-113">表示名。</span><span class="sxs-lookup"><span data-stu-id="7f987-113">Display Name.</span></span> <span data-ttu-id="7f987-114">[omaSetting](../resources/intune-deviceconfig-omasetting.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="7f987-114">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="7f987-115">説明</span><span class="sxs-lookup"><span data-stu-id="7f987-115">description</span></span>|<span data-ttu-id="7f987-116">String</span><span class="sxs-lookup"><span data-stu-id="7f987-116">String</span></span>|<span data-ttu-id="7f987-117">説明。</span><span class="sxs-lookup"><span data-stu-id="7f987-117">Description.</span></span> <span data-ttu-id="7f987-118">[omaSetting](../resources/intune-deviceconfig-omasetting.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="7f987-118">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="7f987-119">omaUri</span><span class="sxs-lookup"><span data-stu-id="7f987-119">omaUri</span></span>|<span data-ttu-id="7f987-120">文字列</span><span class="sxs-lookup"><span data-stu-id="7f987-120">String</span></span>|<span data-ttu-id="7f987-121">OMA。</span><span class="sxs-lookup"><span data-stu-id="7f987-121">OMA.</span></span> <span data-ttu-id="7f987-122">[omaSetting](../resources/intune-deviceconfig-omasetting.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="7f987-122">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="7f987-123">値</span><span class="sxs-lookup"><span data-stu-id="7f987-123">value</span></span>|<span data-ttu-id="7f987-124">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7f987-124">DateTimeOffset</span></span>|<span data-ttu-id="7f987-125">値。</span><span class="sxs-lookup"><span data-stu-id="7f987-125">Value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="7f987-126">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="7f987-126">Relationships</span></span>
<span data-ttu-id="7f987-127">なし</span><span class="sxs-lookup"><span data-stu-id="7f987-127">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="7f987-128">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="7f987-128">JSON Representation</span></span>
<span data-ttu-id="7f987-129">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="7f987-129">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.omaSettingDateTime"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.omaSettingDateTime",
  "displayName": "String",
  "description": "String",
  "omaUri": "String",
  "value": "String (timestamp)"
}
```



