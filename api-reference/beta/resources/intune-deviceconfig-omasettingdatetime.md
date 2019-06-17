---
title: omaSettingDateTime リソースの種類
description: OMA 設定の DateTime の定義です。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 4686e3354e53dc0ad2502673bbf44866135d577d
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/14/2019
ms.locfileid: "34993740"
---
# <a name="omasettingdatetime-resource-type"></a><span data-ttu-id="410c8-103">omaSettingDateTime リソースの種類</span><span class="sxs-lookup"><span data-stu-id="410c8-103">omaSettingDateTime resource type</span></span>

> <span data-ttu-id="410c8-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="410c8-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="410c8-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="410c8-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="410c8-106">OMA 設定の DateTime の定義です。</span><span class="sxs-lookup"><span data-stu-id="410c8-106">OMA Settings DateTime definition.</span></span>


<span data-ttu-id="410c8-107">[omaSetting](../resources/intune-deviceconfig-omasetting.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="410c8-107">Inherits from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>

## <a name="properties"></a><span data-ttu-id="410c8-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="410c8-108">Properties</span></span>
|<span data-ttu-id="410c8-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="410c8-109">Property</span></span>|<span data-ttu-id="410c8-110">型</span><span class="sxs-lookup"><span data-stu-id="410c8-110">Type</span></span>|<span data-ttu-id="410c8-111">説明</span><span class="sxs-lookup"><span data-stu-id="410c8-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="410c8-112">displayName</span><span class="sxs-lookup"><span data-stu-id="410c8-112">displayName</span></span>|<span data-ttu-id="410c8-113">String</span><span class="sxs-lookup"><span data-stu-id="410c8-113">String</span></span>|<span data-ttu-id="410c8-114">表示名。</span><span class="sxs-lookup"><span data-stu-id="410c8-114">Display Name.</span></span> <span data-ttu-id="410c8-115">[omaSetting](../resources/intune-deviceconfig-omasetting.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="410c8-115">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="410c8-116">description</span><span class="sxs-lookup"><span data-stu-id="410c8-116">description</span></span>|<span data-ttu-id="410c8-117">String</span><span class="sxs-lookup"><span data-stu-id="410c8-117">String</span></span>|<span data-ttu-id="410c8-118">説明。</span><span class="sxs-lookup"><span data-stu-id="410c8-118">Description.</span></span> <span data-ttu-id="410c8-119">[omaSetting](../resources/intune-deviceconfig-omasetting.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="410c8-119">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="410c8-120">omaUri</span><span class="sxs-lookup"><span data-stu-id="410c8-120">omaUri</span></span>|<span data-ttu-id="410c8-121">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="410c8-121">String</span></span>|<span data-ttu-id="410c8-122">OMA。</span><span class="sxs-lookup"><span data-stu-id="410c8-122">OMA.</span></span> <span data-ttu-id="410c8-123">[omaSetting](../resources/intune-deviceconfig-omasetting.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="410c8-123">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="410c8-124">値</span><span class="sxs-lookup"><span data-stu-id="410c8-124">value</span></span>|<span data-ttu-id="410c8-125">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="410c8-125">DateTimeOffset</span></span>|<span data-ttu-id="410c8-126">値。</span><span class="sxs-lookup"><span data-stu-id="410c8-126">Value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="410c8-127">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="410c8-127">Relationships</span></span>
<span data-ttu-id="410c8-128">なし</span><span class="sxs-lookup"><span data-stu-id="410c8-128">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="410c8-129">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="410c8-129">JSON Representation</span></span>
<span data-ttu-id="410c8-130">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="410c8-130">Here is a JSON representation of the resource.</span></span>
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





