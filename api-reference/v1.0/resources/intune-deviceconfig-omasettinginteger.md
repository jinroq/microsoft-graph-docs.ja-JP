---
title: omaSettingInteger リソースの種類
description: OMA 設定の整数の定義。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 0e4896af0e43510eb791f37a72a864a405388e9d
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/26/2019
ms.locfileid: "30253555"
---
# <a name="omasettinginteger-resource-type"></a><span data-ttu-id="4dc1e-103">omaSettingInteger リソースの種類</span><span class="sxs-lookup"><span data-stu-id="4dc1e-103">omaSettingInteger resource type</span></span>

> <span data-ttu-id="4dc1e-104">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="4dc1e-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4dc1e-105">OMA 設定の整数の定義。</span><span class="sxs-lookup"><span data-stu-id="4dc1e-105">OMA Settings Integer definition.</span></span>


<span data-ttu-id="4dc1e-106">[omaSetting](../resources/intune-deviceconfig-omasetting.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="4dc1e-106">Inherits from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>

## <a name="properties"></a><span data-ttu-id="4dc1e-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="4dc1e-107">Properties</span></span>
|<span data-ttu-id="4dc1e-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="4dc1e-108">Property</span></span>|<span data-ttu-id="4dc1e-109">型</span><span class="sxs-lookup"><span data-stu-id="4dc1e-109">Type</span></span>|<span data-ttu-id="4dc1e-110">説明</span><span class="sxs-lookup"><span data-stu-id="4dc1e-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4dc1e-111">displayName</span><span class="sxs-lookup"><span data-stu-id="4dc1e-111">displayName</span></span>|<span data-ttu-id="4dc1e-112">String</span><span class="sxs-lookup"><span data-stu-id="4dc1e-112">String</span></span>|<span data-ttu-id="4dc1e-113">表示名。</span><span class="sxs-lookup"><span data-stu-id="4dc1e-113">Display Name.</span></span> <span data-ttu-id="4dc1e-114">[omaSetting](../resources/intune-deviceconfig-omasetting.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="4dc1e-114">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="4dc1e-115">説明</span><span class="sxs-lookup"><span data-stu-id="4dc1e-115">description</span></span>|<span data-ttu-id="4dc1e-116">String</span><span class="sxs-lookup"><span data-stu-id="4dc1e-116">String</span></span>|<span data-ttu-id="4dc1e-117">説明。</span><span class="sxs-lookup"><span data-stu-id="4dc1e-117">Description.</span></span> <span data-ttu-id="4dc1e-118">[omaSetting](../resources/intune-deviceconfig-omasetting.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="4dc1e-118">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="4dc1e-119">omaUri</span><span class="sxs-lookup"><span data-stu-id="4dc1e-119">omaUri</span></span>|<span data-ttu-id="4dc1e-120">文字列</span><span class="sxs-lookup"><span data-stu-id="4dc1e-120">String</span></span>|<span data-ttu-id="4dc1e-121">OMA。</span><span class="sxs-lookup"><span data-stu-id="4dc1e-121">OMA.</span></span> <span data-ttu-id="4dc1e-122">[omaSetting](../resources/intune-deviceconfig-omasetting.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="4dc1e-122">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="4dc1e-123">値</span><span class="sxs-lookup"><span data-stu-id="4dc1e-123">value</span></span>|<span data-ttu-id="4dc1e-124">Int32</span><span class="sxs-lookup"><span data-stu-id="4dc1e-124">Int32</span></span>|<span data-ttu-id="4dc1e-125">値。</span><span class="sxs-lookup"><span data-stu-id="4dc1e-125">Value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="4dc1e-126">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="4dc1e-126">Relationships</span></span>
<span data-ttu-id="4dc1e-127">なし</span><span class="sxs-lookup"><span data-stu-id="4dc1e-127">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="4dc1e-128">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="4dc1e-128">JSON Representation</span></span>
<span data-ttu-id="4dc1e-129">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="4dc1e-129">Here is a JSON representation of the resource.</span></span>
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



