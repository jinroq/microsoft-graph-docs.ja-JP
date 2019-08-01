---
title: omaSettingDateTime リソースの種類
description: OMA 設定の DateTime の定義です。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 71347ecd4a566409d1043c788df70601ffc70a2a
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36028029"
---
# <a name="omasettingdatetime-resource-type"></a><span data-ttu-id="f9d54-103">omaSettingDateTime リソースの種類</span><span class="sxs-lookup"><span data-stu-id="f9d54-103">omaSettingDateTime resource type</span></span>

> <span data-ttu-id="f9d54-104">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="f9d54-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f9d54-105">OMA 設定の DateTime の定義です。</span><span class="sxs-lookup"><span data-stu-id="f9d54-105">OMA Settings DateTime definition.</span></span>


<span data-ttu-id="f9d54-106">[omaSetting](../resources/intune-deviceconfig-omasetting.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="f9d54-106">Inherits from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>

## <a name="properties"></a><span data-ttu-id="f9d54-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="f9d54-107">Properties</span></span>
|<span data-ttu-id="f9d54-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="f9d54-108">Property</span></span>|<span data-ttu-id="f9d54-109">型</span><span class="sxs-lookup"><span data-stu-id="f9d54-109">Type</span></span>|<span data-ttu-id="f9d54-110">説明</span><span class="sxs-lookup"><span data-stu-id="f9d54-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f9d54-111">displayName</span><span class="sxs-lookup"><span data-stu-id="f9d54-111">displayName</span></span>|<span data-ttu-id="f9d54-112">String</span><span class="sxs-lookup"><span data-stu-id="f9d54-112">String</span></span>|<span data-ttu-id="f9d54-113">表示名。</span><span class="sxs-lookup"><span data-stu-id="f9d54-113">Display Name.</span></span> <span data-ttu-id="f9d54-114">[omaSetting](../resources/intune-deviceconfig-omasetting.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="f9d54-114">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="f9d54-115">description</span><span class="sxs-lookup"><span data-stu-id="f9d54-115">description</span></span>|<span data-ttu-id="f9d54-116">String</span><span class="sxs-lookup"><span data-stu-id="f9d54-116">String</span></span>|<span data-ttu-id="f9d54-117">説明。</span><span class="sxs-lookup"><span data-stu-id="f9d54-117">Description.</span></span> <span data-ttu-id="f9d54-118">[omaSetting](../resources/intune-deviceconfig-omasetting.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="f9d54-118">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="f9d54-119">omaUri</span><span class="sxs-lookup"><span data-stu-id="f9d54-119">omaUri</span></span>|<span data-ttu-id="f9d54-120">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="f9d54-120">String</span></span>|<span data-ttu-id="f9d54-121">OMA。</span><span class="sxs-lookup"><span data-stu-id="f9d54-121">OMA.</span></span> <span data-ttu-id="f9d54-122">[omaSetting](../resources/intune-deviceconfig-omasetting.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="f9d54-122">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="f9d54-123">値</span><span class="sxs-lookup"><span data-stu-id="f9d54-123">value</span></span>|<span data-ttu-id="f9d54-124">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f9d54-124">DateTimeOffset</span></span>|<span data-ttu-id="f9d54-125">値。</span><span class="sxs-lookup"><span data-stu-id="f9d54-125">Value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="f9d54-126">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="f9d54-126">Relationships</span></span>
<span data-ttu-id="f9d54-127">なし</span><span class="sxs-lookup"><span data-stu-id="f9d54-127">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="f9d54-128">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="f9d54-128">JSON Representation</span></span>
<span data-ttu-id="f9d54-129">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="f9d54-129">Here is a JSON representation of the resource.</span></span>
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



