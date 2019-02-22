---
title: omaSettingDateTime リソースの種類
description: OMA 設定の DateTime の定義です。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 283b41018ad89b157c679c8b532c869d350b9182
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/21/2019
ms.locfileid: "30144465"
---
# <a name="omasettingdatetime-resource-type"></a><span data-ttu-id="2465f-103">omaSettingDateTime リソースの種類</span><span class="sxs-lookup"><span data-stu-id="2465f-103">omaSettingDateTime resource type</span></span>

> <span data-ttu-id="2465f-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="2465f-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2465f-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="2465f-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2465f-106">OMA 設定の DateTime の定義です。</span><span class="sxs-lookup"><span data-stu-id="2465f-106">OMA Settings DateTime definition.</span></span>


<span data-ttu-id="2465f-107">[omaSetting](../resources/intune-deviceconfig-omasetting.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="2465f-107">Inherits from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>

## <a name="properties"></a><span data-ttu-id="2465f-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="2465f-108">Properties</span></span>
|<span data-ttu-id="2465f-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="2465f-109">Property</span></span>|<span data-ttu-id="2465f-110">型</span><span class="sxs-lookup"><span data-stu-id="2465f-110">Type</span></span>|<span data-ttu-id="2465f-111">説明</span><span class="sxs-lookup"><span data-stu-id="2465f-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2465f-112">displayName</span><span class="sxs-lookup"><span data-stu-id="2465f-112">displayName</span></span>|<span data-ttu-id="2465f-113">String</span><span class="sxs-lookup"><span data-stu-id="2465f-113">String</span></span>|<span data-ttu-id="2465f-114">表示名。</span><span class="sxs-lookup"><span data-stu-id="2465f-114">Display Name.</span></span> <span data-ttu-id="2465f-115">[omaSetting](../resources/intune-deviceconfig-omasetting.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="2465f-115">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="2465f-116">説明</span><span class="sxs-lookup"><span data-stu-id="2465f-116">description</span></span>|<span data-ttu-id="2465f-117">String</span><span class="sxs-lookup"><span data-stu-id="2465f-117">String</span></span>|<span data-ttu-id="2465f-118">説明。</span><span class="sxs-lookup"><span data-stu-id="2465f-118">Description.</span></span> <span data-ttu-id="2465f-119">[omaSetting](../resources/intune-deviceconfig-omasetting.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="2465f-119">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="2465f-120">omaUri</span><span class="sxs-lookup"><span data-stu-id="2465f-120">omaUri</span></span>|<span data-ttu-id="2465f-121">文字列</span><span class="sxs-lookup"><span data-stu-id="2465f-121">String</span></span>|<span data-ttu-id="2465f-122">OMA。</span><span class="sxs-lookup"><span data-stu-id="2465f-122">OMA.</span></span> <span data-ttu-id="2465f-123">[omaSetting](../resources/intune-deviceconfig-omasetting.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="2465f-123">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="2465f-124">値</span><span class="sxs-lookup"><span data-stu-id="2465f-124">value</span></span>|<span data-ttu-id="2465f-125">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2465f-125">DateTimeOffset</span></span>|<span data-ttu-id="2465f-126">値。</span><span class="sxs-lookup"><span data-stu-id="2465f-126">Value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="2465f-127">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="2465f-127">Relationships</span></span>
<span data-ttu-id="2465f-128">なし</span><span class="sxs-lookup"><span data-stu-id="2465f-128">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="2465f-129">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="2465f-129">JSON Representation</span></span>
<span data-ttu-id="2465f-130">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="2465f-130">Here is a JSON representation of the resource.</span></span>
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




