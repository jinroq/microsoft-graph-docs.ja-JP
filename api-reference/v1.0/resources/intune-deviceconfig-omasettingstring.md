---
title: omaSettingString リソースの種類
description: OMA 設定の文字列の定義です。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 0b32d5f6942dc5c0284e0ecaa11a27f4df0e99b3
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/26/2019
ms.locfileid: "30259914"
---
# <a name="omasettingstring-resource-type"></a><span data-ttu-id="f23c2-103">omaSettingString リソースの種類</span><span class="sxs-lookup"><span data-stu-id="f23c2-103">omaSettingString resource type</span></span>

> <span data-ttu-id="f23c2-104">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="f23c2-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f23c2-105">OMA 設定の文字列の定義です。</span><span class="sxs-lookup"><span data-stu-id="f23c2-105">OMA Settings String definition.</span></span>


<span data-ttu-id="f23c2-106">[omaSetting](../resources/intune-deviceconfig-omasetting.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="f23c2-106">Inherits from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>

## <a name="properties"></a><span data-ttu-id="f23c2-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="f23c2-107">Properties</span></span>
|<span data-ttu-id="f23c2-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="f23c2-108">Property</span></span>|<span data-ttu-id="f23c2-109">型</span><span class="sxs-lookup"><span data-stu-id="f23c2-109">Type</span></span>|<span data-ttu-id="f23c2-110">説明</span><span class="sxs-lookup"><span data-stu-id="f23c2-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f23c2-111">displayName</span><span class="sxs-lookup"><span data-stu-id="f23c2-111">displayName</span></span>|<span data-ttu-id="f23c2-112">String</span><span class="sxs-lookup"><span data-stu-id="f23c2-112">String</span></span>|<span data-ttu-id="f23c2-113">表示名。</span><span class="sxs-lookup"><span data-stu-id="f23c2-113">Display Name.</span></span> <span data-ttu-id="f23c2-114">[omaSetting](../resources/intune-deviceconfig-omasetting.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="f23c2-114">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="f23c2-115">説明</span><span class="sxs-lookup"><span data-stu-id="f23c2-115">description</span></span>|<span data-ttu-id="f23c2-116">String</span><span class="sxs-lookup"><span data-stu-id="f23c2-116">String</span></span>|<span data-ttu-id="f23c2-117">説明。</span><span class="sxs-lookup"><span data-stu-id="f23c2-117">Description.</span></span> <span data-ttu-id="f23c2-118">[omaSetting](../resources/intune-deviceconfig-omasetting.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="f23c2-118">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="f23c2-119">omaUri</span><span class="sxs-lookup"><span data-stu-id="f23c2-119">omaUri</span></span>|<span data-ttu-id="f23c2-120">文字列</span><span class="sxs-lookup"><span data-stu-id="f23c2-120">String</span></span>|<span data-ttu-id="f23c2-121">OMA。</span><span class="sxs-lookup"><span data-stu-id="f23c2-121">OMA.</span></span> <span data-ttu-id="f23c2-122">[omaSetting](../resources/intune-deviceconfig-omasetting.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="f23c2-122">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="f23c2-123">value</span><span class="sxs-lookup"><span data-stu-id="f23c2-123">value</span></span>|<span data-ttu-id="f23c2-124">文字列</span><span class="sxs-lookup"><span data-stu-id="f23c2-124">String</span></span>|<span data-ttu-id="f23c2-125">値。</span><span class="sxs-lookup"><span data-stu-id="f23c2-125">Value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="f23c2-126">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="f23c2-126">Relationships</span></span>
<span data-ttu-id="f23c2-127">なし</span><span class="sxs-lookup"><span data-stu-id="f23c2-127">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="f23c2-128">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="f23c2-128">JSON Representation</span></span>
<span data-ttu-id="f23c2-129">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="f23c2-129">Here is a JSON representation of the resource.</span></span>
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



