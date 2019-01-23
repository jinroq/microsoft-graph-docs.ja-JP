---
title: omaSettingBase64 リソースの種類
description: OMA 設定の Base64 定義。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 5f5885a81e68dbea4e5f6f1c8cae456144785338
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29413921"
---
# <a name="omasettingbase64-resource-type"></a><span data-ttu-id="bc843-103">omaSettingBase64 リソースの種類</span><span class="sxs-lookup"><span data-stu-id="bc843-103">omaSettingBase64 resource type</span></span>

> <span data-ttu-id="bc843-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="bc843-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="bc843-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="bc843-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="bc843-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="bc843-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bc843-107">OMA 設定の Base64 定義。</span><span class="sxs-lookup"><span data-stu-id="bc843-107">OMA Settings Base64 definition.</span></span>


<span data-ttu-id="bc843-108">[omaSetting](../resources/intune-deviceconfig-omasetting.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="bc843-108">Inherits from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>

## <a name="properties"></a><span data-ttu-id="bc843-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="bc843-109">Properties</span></span>
|<span data-ttu-id="bc843-110">プロパティ</span><span class="sxs-lookup"><span data-stu-id="bc843-110">Property</span></span>|<span data-ttu-id="bc843-111">型</span><span class="sxs-lookup"><span data-stu-id="bc843-111">Type</span></span>|<span data-ttu-id="bc843-112">説明</span><span class="sxs-lookup"><span data-stu-id="bc843-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bc843-113">displayName</span><span class="sxs-lookup"><span data-stu-id="bc843-113">displayName</span></span>|<span data-ttu-id="bc843-114">文字列</span><span class="sxs-lookup"><span data-stu-id="bc843-114">String</span></span>|<span data-ttu-id="bc843-115">表示名。</span><span class="sxs-lookup"><span data-stu-id="bc843-115">Display Name.</span></span> <span data-ttu-id="bc843-116">[omaSetting](../resources/intune-deviceconfig-omasetting.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="bc843-116">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="bc843-117">説明</span><span class="sxs-lookup"><span data-stu-id="bc843-117">description</span></span>|<span data-ttu-id="bc843-118">String</span><span class="sxs-lookup"><span data-stu-id="bc843-118">String</span></span>|<span data-ttu-id="bc843-119">説明。</span><span class="sxs-lookup"><span data-stu-id="bc843-119">Description.</span></span> <span data-ttu-id="bc843-120">[omaSetting](../resources/intune-deviceconfig-omasetting.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="bc843-120">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="bc843-121">omaUri</span><span class="sxs-lookup"><span data-stu-id="bc843-121">omaUri</span></span>|<span data-ttu-id="bc843-122">文字列</span><span class="sxs-lookup"><span data-stu-id="bc843-122">String</span></span>|<span data-ttu-id="bc843-123">OMA。</span><span class="sxs-lookup"><span data-stu-id="bc843-123">OMA.</span></span> <span data-ttu-id="bc843-124">[omaSetting](../resources/intune-deviceconfig-omasetting.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="bc843-124">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="bc843-125">fileName</span><span class="sxs-lookup"><span data-stu-id="bc843-125">fileName</span></span>|<span data-ttu-id="bc843-126">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="bc843-126">String</span></span>|<span data-ttu-id="bc843-127">Value プロパティに関連付けられているファイル名 (\*.cer</span><span class="sxs-lookup"><span data-stu-id="bc843-127">File name associated with the Value property (\*.cer</span></span> | <span data-ttu-id="bc843-128">\*.crt</span><span class="sxs-lookup"><span data-stu-id="bc843-128">\*.crt</span></span> | <span data-ttu-id="bc843-129">\*.p7b</span><span class="sxs-lookup"><span data-stu-id="bc843-129">\*.p7b</span></span> | <span data-ttu-id="bc843-130">\* .bin)。</span><span class="sxs-lookup"><span data-stu-id="bc843-130">\*.bin).</span></span>|
|<span data-ttu-id="bc843-131">value</span><span class="sxs-lookup"><span data-stu-id="bc843-131">value</span></span>|<span data-ttu-id="bc843-132">文字列</span><span class="sxs-lookup"><span data-stu-id="bc843-132">String</span></span>|<span data-ttu-id="bc843-133">値。</span><span class="sxs-lookup"><span data-stu-id="bc843-133">Value.</span></span> <span data-ttu-id="bc843-134">(Base64 エンコード文字列)</span><span class="sxs-lookup"><span data-stu-id="bc843-134">(Base64 encoded string)</span></span>|

## <a name="relationships"></a><span data-ttu-id="bc843-135">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="bc843-135">Relationships</span></span>
<span data-ttu-id="bc843-136">なし</span><span class="sxs-lookup"><span data-stu-id="bc843-136">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="bc843-137">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="bc843-137">JSON Representation</span></span>
<span data-ttu-id="bc843-138">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="bc843-138">Here is a JSON representation of the resource.</span></span>
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




