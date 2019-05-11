---
title: omaSettingDateTime リソースの種類
description: OMA 設定の DateTime の定義です。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: d9d58c6fdbba9f4a2fcceaa5d0e2964f0666c571
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/11/2019
ms.locfileid: "33950922"
---
# <a name="omasettingdatetime-resource-type"></a><span data-ttu-id="09a91-103">omaSettingDateTime リソースの種類</span><span class="sxs-lookup"><span data-stu-id="09a91-103">omaSettingDateTime resource type</span></span>

> <span data-ttu-id="09a91-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="09a91-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="09a91-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="09a91-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="09a91-106">OMA 設定の DateTime の定義です。</span><span class="sxs-lookup"><span data-stu-id="09a91-106">OMA Settings DateTime definition.</span></span>


<span data-ttu-id="09a91-107">[omaSetting](../resources/intune-deviceconfig-omasetting.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="09a91-107">Inherits from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>

## <a name="properties"></a><span data-ttu-id="09a91-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="09a91-108">Properties</span></span>
|<span data-ttu-id="09a91-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="09a91-109">Property</span></span>|<span data-ttu-id="09a91-110">型</span><span class="sxs-lookup"><span data-stu-id="09a91-110">Type</span></span>|<span data-ttu-id="09a91-111">説明</span><span class="sxs-lookup"><span data-stu-id="09a91-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="09a91-112">displayName</span><span class="sxs-lookup"><span data-stu-id="09a91-112">displayName</span></span>|<span data-ttu-id="09a91-113">String</span><span class="sxs-lookup"><span data-stu-id="09a91-113">String</span></span>|<span data-ttu-id="09a91-114">表示名。</span><span class="sxs-lookup"><span data-stu-id="09a91-114">Display Name.</span></span> <span data-ttu-id="09a91-115">[omaSetting](../resources/intune-deviceconfig-omasetting.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="09a91-115">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="09a91-116">description</span><span class="sxs-lookup"><span data-stu-id="09a91-116">description</span></span>|<span data-ttu-id="09a91-117">String</span><span class="sxs-lookup"><span data-stu-id="09a91-117">String</span></span>|<span data-ttu-id="09a91-118">説明。</span><span class="sxs-lookup"><span data-stu-id="09a91-118">Description.</span></span> <span data-ttu-id="09a91-119">[omaSetting](../resources/intune-deviceconfig-omasetting.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="09a91-119">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="09a91-120">omaUri</span><span class="sxs-lookup"><span data-stu-id="09a91-120">omaUri</span></span>|<span data-ttu-id="09a91-121">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="09a91-121">String</span></span>|<span data-ttu-id="09a91-122">OMA。</span><span class="sxs-lookup"><span data-stu-id="09a91-122">OMA.</span></span> <span data-ttu-id="09a91-123">[omaSetting](../resources/intune-deviceconfig-omasetting.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="09a91-123">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="09a91-124">値</span><span class="sxs-lookup"><span data-stu-id="09a91-124">value</span></span>|<span data-ttu-id="09a91-125">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="09a91-125">DateTimeOffset</span></span>|<span data-ttu-id="09a91-126">値。</span><span class="sxs-lookup"><span data-stu-id="09a91-126">Value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="09a91-127">関係</span><span class="sxs-lookup"><span data-stu-id="09a91-127">Relationships</span></span>
<span data-ttu-id="09a91-128">なし</span><span class="sxs-lookup"><span data-stu-id="09a91-128">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="09a91-129">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="09a91-129">JSON Representation</span></span>
<span data-ttu-id="09a91-130">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="09a91-130">Here is a JSON representation of the resource.</span></span>
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




