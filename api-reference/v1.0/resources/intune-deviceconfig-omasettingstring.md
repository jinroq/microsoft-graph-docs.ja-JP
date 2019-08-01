---
title: omaSettingString リソースの種類
description: OMA 設定の文字列の定義です。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 30802cc391958fabec4540fc3256f7c67ec094c7
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36031305"
---
# <a name="omasettingstring-resource-type"></a><span data-ttu-id="e4102-103">omaSettingString リソースの種類</span><span class="sxs-lookup"><span data-stu-id="e4102-103">omaSettingString resource type</span></span>

> <span data-ttu-id="e4102-104">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="e4102-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e4102-105">OMA 設定の文字列の定義です。</span><span class="sxs-lookup"><span data-stu-id="e4102-105">OMA Settings String definition.</span></span>


<span data-ttu-id="e4102-106">[omaSetting](../resources/intune-deviceconfig-omasetting.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="e4102-106">Inherits from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>

## <a name="properties"></a><span data-ttu-id="e4102-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="e4102-107">Properties</span></span>
|<span data-ttu-id="e4102-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="e4102-108">Property</span></span>|<span data-ttu-id="e4102-109">型</span><span class="sxs-lookup"><span data-stu-id="e4102-109">Type</span></span>|<span data-ttu-id="e4102-110">説明</span><span class="sxs-lookup"><span data-stu-id="e4102-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e4102-111">displayName</span><span class="sxs-lookup"><span data-stu-id="e4102-111">displayName</span></span>|<span data-ttu-id="e4102-112">String</span><span class="sxs-lookup"><span data-stu-id="e4102-112">String</span></span>|<span data-ttu-id="e4102-113">表示名。</span><span class="sxs-lookup"><span data-stu-id="e4102-113">Display Name.</span></span> <span data-ttu-id="e4102-114">[omaSetting](../resources/intune-deviceconfig-omasetting.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="e4102-114">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="e4102-115">description</span><span class="sxs-lookup"><span data-stu-id="e4102-115">description</span></span>|<span data-ttu-id="e4102-116">String</span><span class="sxs-lookup"><span data-stu-id="e4102-116">String</span></span>|<span data-ttu-id="e4102-117">説明。</span><span class="sxs-lookup"><span data-stu-id="e4102-117">Description.</span></span> <span data-ttu-id="e4102-118">[omaSetting](../resources/intune-deviceconfig-omasetting.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="e4102-118">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="e4102-119">omaUri</span><span class="sxs-lookup"><span data-stu-id="e4102-119">omaUri</span></span>|<span data-ttu-id="e4102-120">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="e4102-120">String</span></span>|<span data-ttu-id="e4102-121">OMA。</span><span class="sxs-lookup"><span data-stu-id="e4102-121">OMA.</span></span> <span data-ttu-id="e4102-122">[omaSetting](../resources/intune-deviceconfig-omasetting.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="e4102-122">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="e4102-123">value</span><span class="sxs-lookup"><span data-stu-id="e4102-123">value</span></span>|<span data-ttu-id="e4102-124">文字列</span><span class="sxs-lookup"><span data-stu-id="e4102-124">String</span></span>|<span data-ttu-id="e4102-125">値。</span><span class="sxs-lookup"><span data-stu-id="e4102-125">Value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e4102-126">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="e4102-126">Relationships</span></span>
<span data-ttu-id="e4102-127">なし</span><span class="sxs-lookup"><span data-stu-id="e4102-127">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="e4102-128">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="e4102-128">JSON Representation</span></span>
<span data-ttu-id="e4102-129">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="e4102-129">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.omaSettingString"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.omaSettingString",
  "displayName": "String",
  "description": "String",
  "omaUri": "String",
  "value": "String"
}
```



