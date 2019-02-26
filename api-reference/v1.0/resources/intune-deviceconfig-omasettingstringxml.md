---
title: omaSettingStringXml リソースの種類
description: OMA 設定文字列の XML 定義です。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: b4f95201a725969fa125cdf949874686b9155fc3
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/26/2019
ms.locfileid: "30252428"
---
# <a name="omasettingstringxml-resource-type"></a><span data-ttu-id="4b72e-103">omaSettingStringXml リソースの種類</span><span class="sxs-lookup"><span data-stu-id="4b72e-103">omaSettingStringXml resource type</span></span>

> <span data-ttu-id="4b72e-104">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="4b72e-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4b72e-105">OMA 設定文字列の XML 定義です。</span><span class="sxs-lookup"><span data-stu-id="4b72e-105">OMA Settings StringXML definition.</span></span>


<span data-ttu-id="4b72e-106">[omaSetting](../resources/intune-deviceconfig-omasetting.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="4b72e-106">Inherits from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>

## <a name="properties"></a><span data-ttu-id="4b72e-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="4b72e-107">Properties</span></span>
|<span data-ttu-id="4b72e-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="4b72e-108">Property</span></span>|<span data-ttu-id="4b72e-109">型</span><span class="sxs-lookup"><span data-stu-id="4b72e-109">Type</span></span>|<span data-ttu-id="4b72e-110">説明</span><span class="sxs-lookup"><span data-stu-id="4b72e-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4b72e-111">displayName</span><span class="sxs-lookup"><span data-stu-id="4b72e-111">displayName</span></span>|<span data-ttu-id="4b72e-112">String</span><span class="sxs-lookup"><span data-stu-id="4b72e-112">String</span></span>|<span data-ttu-id="4b72e-113">表示名。</span><span class="sxs-lookup"><span data-stu-id="4b72e-113">Display Name.</span></span> <span data-ttu-id="4b72e-114">[omaSetting](../resources/intune-deviceconfig-omasetting.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="4b72e-114">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="4b72e-115">説明</span><span class="sxs-lookup"><span data-stu-id="4b72e-115">description</span></span>|<span data-ttu-id="4b72e-116">String</span><span class="sxs-lookup"><span data-stu-id="4b72e-116">String</span></span>|<span data-ttu-id="4b72e-117">説明。</span><span class="sxs-lookup"><span data-stu-id="4b72e-117">Description.</span></span> <span data-ttu-id="4b72e-118">[omaSetting](../resources/intune-deviceconfig-omasetting.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="4b72e-118">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="4b72e-119">omaUri</span><span class="sxs-lookup"><span data-stu-id="4b72e-119">omaUri</span></span>|<span data-ttu-id="4b72e-120">文字列</span><span class="sxs-lookup"><span data-stu-id="4b72e-120">String</span></span>|<span data-ttu-id="4b72e-121">OMA。</span><span class="sxs-lookup"><span data-stu-id="4b72e-121">OMA.</span></span> <span data-ttu-id="4b72e-122">[omaSetting](../resources/intune-deviceconfig-omasetting.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="4b72e-122">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="4b72e-123">fileName</span><span class="sxs-lookup"><span data-stu-id="4b72e-123">fileName</span></span>|<span data-ttu-id="4b72e-124">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="4b72e-124">String</span></span>|<span data-ttu-id="4b72e-125">Value プロパティに関連付けられているファイル名 (\*.xml)。</span><span class="sxs-lookup"><span data-stu-id="4b72e-125">File name associated with the Value property (\*.xml).</span></span>|
|<span data-ttu-id="4b72e-126">value</span><span class="sxs-lookup"><span data-stu-id="4b72e-126">value</span></span>|<span data-ttu-id="4b72e-127">バイナリ型 (Binary)</span><span class="sxs-lookup"><span data-stu-id="4b72e-127">Binary</span></span>|<span data-ttu-id="4b72e-128">値。</span><span class="sxs-lookup"><span data-stu-id="4b72e-128">Value.</span></span> <span data-ttu-id="4b72e-129">(UTF8 でエンコードされたバイト配列)</span><span class="sxs-lookup"><span data-stu-id="4b72e-129">(UTF8 encoded byte array)</span></span>|

## <a name="relationships"></a><span data-ttu-id="4b72e-130">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="4b72e-130">Relationships</span></span>
<span data-ttu-id="4b72e-131">なし</span><span class="sxs-lookup"><span data-stu-id="4b72e-131">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="4b72e-132">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="4b72e-132">JSON Representation</span></span>
<span data-ttu-id="4b72e-133">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="4b72e-133">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.omaSettingStringXml"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.omaSettingStringXml",
  "displayName": "String",
  "description": "String",
  "omaUri": "String",
  "fileName": "String",
  "value": "binary"
}
```



