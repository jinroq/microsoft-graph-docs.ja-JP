---
title: omaSettingBase64 リソースの種類
description: OMA 設定の Base64 定義。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: f5fd4df9b5deb49745d337632cfe103fdaad0581
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36011429"
---
# <a name="omasettingbase64-resource-type"></a><span data-ttu-id="7dbad-103">omaSettingBase64 リソースの種類</span><span class="sxs-lookup"><span data-stu-id="7dbad-103">omaSettingBase64 resource type</span></span>

> <span data-ttu-id="7dbad-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="7dbad-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7dbad-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="7dbad-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7dbad-106">OMA 設定の Base64 定義。</span><span class="sxs-lookup"><span data-stu-id="7dbad-106">OMA Settings Base64 definition.</span></span>


<span data-ttu-id="7dbad-107">[omaSetting](../resources/intune-deviceconfig-omasetting.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="7dbad-107">Inherits from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>

## <a name="properties"></a><span data-ttu-id="7dbad-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="7dbad-108">Properties</span></span>
|<span data-ttu-id="7dbad-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="7dbad-109">Property</span></span>|<span data-ttu-id="7dbad-110">型</span><span class="sxs-lookup"><span data-stu-id="7dbad-110">Type</span></span>|<span data-ttu-id="7dbad-111">説明</span><span class="sxs-lookup"><span data-stu-id="7dbad-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7dbad-112">displayName</span><span class="sxs-lookup"><span data-stu-id="7dbad-112">displayName</span></span>|<span data-ttu-id="7dbad-113">String</span><span class="sxs-lookup"><span data-stu-id="7dbad-113">String</span></span>|<span data-ttu-id="7dbad-114">表示名。</span><span class="sxs-lookup"><span data-stu-id="7dbad-114">Display Name.</span></span> <span data-ttu-id="7dbad-115">[omaSetting](../resources/intune-deviceconfig-omasetting.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="7dbad-115">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="7dbad-116">description</span><span class="sxs-lookup"><span data-stu-id="7dbad-116">description</span></span>|<span data-ttu-id="7dbad-117">String</span><span class="sxs-lookup"><span data-stu-id="7dbad-117">String</span></span>|<span data-ttu-id="7dbad-118">説明。</span><span class="sxs-lookup"><span data-stu-id="7dbad-118">Description.</span></span> <span data-ttu-id="7dbad-119">[omaSetting](../resources/intune-deviceconfig-omasetting.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="7dbad-119">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="7dbad-120">omaUri</span><span class="sxs-lookup"><span data-stu-id="7dbad-120">omaUri</span></span>|<span data-ttu-id="7dbad-121">String</span><span class="sxs-lookup"><span data-stu-id="7dbad-121">String</span></span>|<span data-ttu-id="7dbad-122">OMA。</span><span class="sxs-lookup"><span data-stu-id="7dbad-122">OMA.</span></span> <span data-ttu-id="7dbad-123">[omaSetting](../resources/intune-deviceconfig-omasetting.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="7dbad-123">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="7dbad-124">fileName</span><span class="sxs-lookup"><span data-stu-id="7dbad-124">fileName</span></span>|<span data-ttu-id="7dbad-125">String</span><span class="sxs-lookup"><span data-stu-id="7dbad-125">String</span></span>|<span data-ttu-id="7dbad-126">Value プロパティに関連付けられているファイル名 (\*.cer</span><span class="sxs-lookup"><span data-stu-id="7dbad-126">File name associated with the Value property (\*.cer</span></span> | <span data-ttu-id="7dbad-127">\* .crt</span><span class="sxs-lookup"><span data-stu-id="7dbad-127">\*.crt</span></span> | <span data-ttu-id="7dbad-128">\*. p7b</span><span class="sxs-lookup"><span data-stu-id="7dbad-128">\*.p7b</span></span> | <span data-ttu-id="7dbad-129">\* .bin)。</span><span class="sxs-lookup"><span data-stu-id="7dbad-129">\*.bin).</span></span>|
|<span data-ttu-id="7dbad-130">value</span><span class="sxs-lookup"><span data-stu-id="7dbad-130">value</span></span>|<span data-ttu-id="7dbad-131">文字列</span><span class="sxs-lookup"><span data-stu-id="7dbad-131">String</span></span>|<span data-ttu-id="7dbad-132">値。</span><span class="sxs-lookup"><span data-stu-id="7dbad-132">Value.</span></span> <span data-ttu-id="7dbad-133">(Base64 エンコード文字列)</span><span class="sxs-lookup"><span data-stu-id="7dbad-133">(Base64 encoded string)</span></span>|

## <a name="relationships"></a><span data-ttu-id="7dbad-134">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="7dbad-134">Relationships</span></span>
<span data-ttu-id="7dbad-135">なし</span><span class="sxs-lookup"><span data-stu-id="7dbad-135">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="7dbad-136">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="7dbad-136">JSON Representation</span></span>
<span data-ttu-id="7dbad-137">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="7dbad-137">Here is a JSON representation of the resource.</span></span>
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





