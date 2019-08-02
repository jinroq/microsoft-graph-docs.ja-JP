---
title: omaSettingBase64 リソースの種類
description: OMA 設定の Base64 定義。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: a8ab8552205084f41599a37c4a8edf39f329d85d
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36028043"
---
# <a name="omasettingbase64-resource-type"></a><span data-ttu-id="8be48-103">omaSettingBase64 リソースの種類</span><span class="sxs-lookup"><span data-stu-id="8be48-103">omaSettingBase64 resource type</span></span>

> <span data-ttu-id="8be48-104">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="8be48-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8be48-105">OMA 設定の Base64 定義。</span><span class="sxs-lookup"><span data-stu-id="8be48-105">OMA Settings Base64 definition.</span></span>


<span data-ttu-id="8be48-106">[omaSetting](../resources/intune-deviceconfig-omasetting.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="8be48-106">Inherits from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>

## <a name="properties"></a><span data-ttu-id="8be48-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="8be48-107">Properties</span></span>
|<span data-ttu-id="8be48-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="8be48-108">Property</span></span>|<span data-ttu-id="8be48-109">型</span><span class="sxs-lookup"><span data-stu-id="8be48-109">Type</span></span>|<span data-ttu-id="8be48-110">説明</span><span class="sxs-lookup"><span data-stu-id="8be48-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8be48-111">displayName</span><span class="sxs-lookup"><span data-stu-id="8be48-111">displayName</span></span>|<span data-ttu-id="8be48-112">String</span><span class="sxs-lookup"><span data-stu-id="8be48-112">String</span></span>|<span data-ttu-id="8be48-113">表示名。</span><span class="sxs-lookup"><span data-stu-id="8be48-113">Display Name.</span></span> <span data-ttu-id="8be48-114">[omaSetting](../resources/intune-deviceconfig-omasetting.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="8be48-114">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="8be48-115">description</span><span class="sxs-lookup"><span data-stu-id="8be48-115">description</span></span>|<span data-ttu-id="8be48-116">String</span><span class="sxs-lookup"><span data-stu-id="8be48-116">String</span></span>|<span data-ttu-id="8be48-117">説明。</span><span class="sxs-lookup"><span data-stu-id="8be48-117">Description.</span></span> <span data-ttu-id="8be48-118">[omaSetting](../resources/intune-deviceconfig-omasetting.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="8be48-118">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="8be48-119">omaUri</span><span class="sxs-lookup"><span data-stu-id="8be48-119">omaUri</span></span>|<span data-ttu-id="8be48-120">String</span><span class="sxs-lookup"><span data-stu-id="8be48-120">String</span></span>|<span data-ttu-id="8be48-121">OMA。</span><span class="sxs-lookup"><span data-stu-id="8be48-121">OMA.</span></span> <span data-ttu-id="8be48-122">[omaSetting](../resources/intune-deviceconfig-omasetting.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="8be48-122">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="8be48-123">fileName</span><span class="sxs-lookup"><span data-stu-id="8be48-123">fileName</span></span>|<span data-ttu-id="8be48-124">String</span><span class="sxs-lookup"><span data-stu-id="8be48-124">String</span></span>|<span data-ttu-id="8be48-125">Value プロパティに関連付けられているファイル名 (\*.cer</span><span class="sxs-lookup"><span data-stu-id="8be48-125">File name associated with the Value property (\*.cer</span></span> | <span data-ttu-id="8be48-126">\* .crt</span><span class="sxs-lookup"><span data-stu-id="8be48-126">\*.crt</span></span> | <span data-ttu-id="8be48-127">\*. p7b</span><span class="sxs-lookup"><span data-stu-id="8be48-127">\*.p7b</span></span> | <span data-ttu-id="8be48-128">\* .bin)。</span><span class="sxs-lookup"><span data-stu-id="8be48-128">\*.bin).</span></span>|
|<span data-ttu-id="8be48-129">value</span><span class="sxs-lookup"><span data-stu-id="8be48-129">value</span></span>|<span data-ttu-id="8be48-130">文字列</span><span class="sxs-lookup"><span data-stu-id="8be48-130">String</span></span>|<span data-ttu-id="8be48-131">値。</span><span class="sxs-lookup"><span data-stu-id="8be48-131">Value.</span></span> <span data-ttu-id="8be48-132">(Base64 エンコード文字列)</span><span class="sxs-lookup"><span data-stu-id="8be48-132">(Base64 encoded string)</span></span>|

## <a name="relationships"></a><span data-ttu-id="8be48-133">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="8be48-133">Relationships</span></span>
<span data-ttu-id="8be48-134">なし</span><span class="sxs-lookup"><span data-stu-id="8be48-134">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="8be48-135">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="8be48-135">JSON Representation</span></span>
<span data-ttu-id="8be48-136">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="8be48-136">Here is a JSON representation of the resource.</span></span>
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



