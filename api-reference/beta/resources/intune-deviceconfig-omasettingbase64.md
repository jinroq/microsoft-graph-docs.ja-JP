---
title: omaSettingBase64 リソースの種類
description: OMA 設定の Base64 定義。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 6f6eae88e7158d5fd8d09caadda9fee6778182a9
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/21/2019
ms.locfileid: "30166648"
---
# <a name="omasettingbase64-resource-type"></a><span data-ttu-id="bba0b-103">omaSettingBase64 リソースの種類</span><span class="sxs-lookup"><span data-stu-id="bba0b-103">omaSettingBase64 resource type</span></span>

> <span data-ttu-id="bba0b-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="bba0b-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="bba0b-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="bba0b-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bba0b-106">OMA 設定の Base64 定義。</span><span class="sxs-lookup"><span data-stu-id="bba0b-106">OMA Settings Base64 definition.</span></span>


<span data-ttu-id="bba0b-107">[omaSetting](../resources/intune-deviceconfig-omasetting.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="bba0b-107">Inherits from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>

## <a name="properties"></a><span data-ttu-id="bba0b-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="bba0b-108">Properties</span></span>
|<span data-ttu-id="bba0b-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="bba0b-109">Property</span></span>|<span data-ttu-id="bba0b-110">型</span><span class="sxs-lookup"><span data-stu-id="bba0b-110">Type</span></span>|<span data-ttu-id="bba0b-111">説明</span><span class="sxs-lookup"><span data-stu-id="bba0b-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bba0b-112">displayName</span><span class="sxs-lookup"><span data-stu-id="bba0b-112">displayName</span></span>|<span data-ttu-id="bba0b-113">String</span><span class="sxs-lookup"><span data-stu-id="bba0b-113">String</span></span>|<span data-ttu-id="bba0b-114">表示名。</span><span class="sxs-lookup"><span data-stu-id="bba0b-114">Display Name.</span></span> <span data-ttu-id="bba0b-115">[omaSetting](../resources/intune-deviceconfig-omasetting.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="bba0b-115">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="bba0b-116">説明</span><span class="sxs-lookup"><span data-stu-id="bba0b-116">description</span></span>|<span data-ttu-id="bba0b-117">String</span><span class="sxs-lookup"><span data-stu-id="bba0b-117">String</span></span>|<span data-ttu-id="bba0b-118">説明。</span><span class="sxs-lookup"><span data-stu-id="bba0b-118">Description.</span></span> <span data-ttu-id="bba0b-119">[omaSetting](../resources/intune-deviceconfig-omasetting.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="bba0b-119">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="bba0b-120">omaUri</span><span class="sxs-lookup"><span data-stu-id="bba0b-120">omaUri</span></span>|<span data-ttu-id="bba0b-121">文字列</span><span class="sxs-lookup"><span data-stu-id="bba0b-121">String</span></span>|<span data-ttu-id="bba0b-122">OMA。</span><span class="sxs-lookup"><span data-stu-id="bba0b-122">OMA.</span></span> <span data-ttu-id="bba0b-123">[omaSetting](../resources/intune-deviceconfig-omasetting.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="bba0b-123">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="bba0b-124">fileName</span><span class="sxs-lookup"><span data-stu-id="bba0b-124">fileName</span></span>|<span data-ttu-id="bba0b-125">String</span><span class="sxs-lookup"><span data-stu-id="bba0b-125">String</span></span>|<span data-ttu-id="bba0b-126">Value プロパティに関連付けられているファイル名 (\*.cer</span><span class="sxs-lookup"><span data-stu-id="bba0b-126">File name associated with the Value property (\*.cer</span></span> | <span data-ttu-id="bba0b-127">\* .crt</span><span class="sxs-lookup"><span data-stu-id="bba0b-127">\*.crt</span></span> | <span data-ttu-id="bba0b-128">\*. p7b</span><span class="sxs-lookup"><span data-stu-id="bba0b-128">\*.p7b</span></span> | <span data-ttu-id="bba0b-129">\* .bin)。</span><span class="sxs-lookup"><span data-stu-id="bba0b-129">\*.bin).</span></span>|
|<span data-ttu-id="bba0b-130">value</span><span class="sxs-lookup"><span data-stu-id="bba0b-130">value</span></span>|<span data-ttu-id="bba0b-131">文字列</span><span class="sxs-lookup"><span data-stu-id="bba0b-131">String</span></span>|<span data-ttu-id="bba0b-132">値。</span><span class="sxs-lookup"><span data-stu-id="bba0b-132">Value.</span></span> <span data-ttu-id="bba0b-133">(Base64 エンコード文字列)</span><span class="sxs-lookup"><span data-stu-id="bba0b-133">(Base64 encoded string)</span></span>|

## <a name="relationships"></a><span data-ttu-id="bba0b-134">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="bba0b-134">Relationships</span></span>
<span data-ttu-id="bba0b-135">なし</span><span class="sxs-lookup"><span data-stu-id="bba0b-135">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="bba0b-136">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="bba0b-136">JSON Representation</span></span>
<span data-ttu-id="bba0b-137">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="bba0b-137">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.omaSettingBase64"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.omaSettingBase64",
  "displayName": "String",
  "description": "String",
  "omaUri": "String",
  "fileName": "String",
  "value": "String"
}
```




