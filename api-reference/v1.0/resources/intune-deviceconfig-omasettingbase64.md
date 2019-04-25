---
title: omaSettingBase64 リソースの種類
description: OMA 設定の Base64 定義。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 678c6e78070a7aae185a041962083b7908ef1cc1
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32549402"
---
# <a name="omasettingbase64-resource-type"></a><span data-ttu-id="cf9f7-103">omaSettingBase64 リソースの種類</span><span class="sxs-lookup"><span data-stu-id="cf9f7-103">omaSettingBase64 resource type</span></span>

> <span data-ttu-id="cf9f7-104">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="cf9f7-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="cf9f7-105">OMA 設定の Base64 定義。</span><span class="sxs-lookup"><span data-stu-id="cf9f7-105">OMA Settings Base64 definition.</span></span>


<span data-ttu-id="cf9f7-106">[omaSetting](../resources/intune-deviceconfig-omasetting.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="cf9f7-106">Inherits from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>

## <a name="properties"></a><span data-ttu-id="cf9f7-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="cf9f7-107">Properties</span></span>
|<span data-ttu-id="cf9f7-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="cf9f7-108">Property</span></span>|<span data-ttu-id="cf9f7-109">型</span><span class="sxs-lookup"><span data-stu-id="cf9f7-109">Type</span></span>|<span data-ttu-id="cf9f7-110">説明</span><span class="sxs-lookup"><span data-stu-id="cf9f7-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cf9f7-111">displayName</span><span class="sxs-lookup"><span data-stu-id="cf9f7-111">displayName</span></span>|<span data-ttu-id="cf9f7-112">String</span><span class="sxs-lookup"><span data-stu-id="cf9f7-112">String</span></span>|<span data-ttu-id="cf9f7-113">表示名。</span><span class="sxs-lookup"><span data-stu-id="cf9f7-113">Display Name.</span></span> <span data-ttu-id="cf9f7-114">[omaSetting](../resources/intune-deviceconfig-omasetting.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="cf9f7-114">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="cf9f7-115">description</span><span class="sxs-lookup"><span data-stu-id="cf9f7-115">description</span></span>|<span data-ttu-id="cf9f7-116">String</span><span class="sxs-lookup"><span data-stu-id="cf9f7-116">String</span></span>|<span data-ttu-id="cf9f7-117">説明。</span><span class="sxs-lookup"><span data-stu-id="cf9f7-117">Description.</span></span> <span data-ttu-id="cf9f7-118">[omaSetting](../resources/intune-deviceconfig-omasetting.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="cf9f7-118">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="cf9f7-119">omaUri</span><span class="sxs-lookup"><span data-stu-id="cf9f7-119">omaUri</span></span>|<span data-ttu-id="cf9f7-120">String</span><span class="sxs-lookup"><span data-stu-id="cf9f7-120">String</span></span>|<span data-ttu-id="cf9f7-121">OMA。</span><span class="sxs-lookup"><span data-stu-id="cf9f7-121">OMA.</span></span> <span data-ttu-id="cf9f7-122">[omaSetting](../resources/intune-deviceconfig-omasetting.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="cf9f7-122">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="cf9f7-123">fileName</span><span class="sxs-lookup"><span data-stu-id="cf9f7-123">fileName</span></span>|<span data-ttu-id="cf9f7-124">String</span><span class="sxs-lookup"><span data-stu-id="cf9f7-124">String</span></span>|<span data-ttu-id="cf9f7-125">Value プロパティに関連付けられているファイル名 (\*.cer</span><span class="sxs-lookup"><span data-stu-id="cf9f7-125">File name associated with the Value property (\*.cer</span></span> | <span data-ttu-id="cf9f7-126">\* .crt</span><span class="sxs-lookup"><span data-stu-id="cf9f7-126">\*.crt</span></span> | <span data-ttu-id="cf9f7-127">\*. p7b</span><span class="sxs-lookup"><span data-stu-id="cf9f7-127">\*.p7b</span></span> | <span data-ttu-id="cf9f7-128">\* .bin)。</span><span class="sxs-lookup"><span data-stu-id="cf9f7-128">\*.bin).</span></span>|
|<span data-ttu-id="cf9f7-129">value</span><span class="sxs-lookup"><span data-stu-id="cf9f7-129">value</span></span>|<span data-ttu-id="cf9f7-130">文字列</span><span class="sxs-lookup"><span data-stu-id="cf9f7-130">String</span></span>|<span data-ttu-id="cf9f7-131">値。</span><span class="sxs-lookup"><span data-stu-id="cf9f7-131">Value.</span></span> <span data-ttu-id="cf9f7-132">(Base64 エンコード文字列)</span><span class="sxs-lookup"><span data-stu-id="cf9f7-132">(Base64 encoded string)</span></span>|

## <a name="relationships"></a><span data-ttu-id="cf9f7-133">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="cf9f7-133">Relationships</span></span>
<span data-ttu-id="cf9f7-134">なし</span><span class="sxs-lookup"><span data-stu-id="cf9f7-134">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="cf9f7-135">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="cf9f7-135">JSON Representation</span></span>
<span data-ttu-id="cf9f7-136">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="cf9f7-136">Here is a JSON representation of the resource.</span></span>
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



