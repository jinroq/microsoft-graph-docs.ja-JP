---
title: omaSettingBoolean リソースの種類
description: OMA 設定のブール定義。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 1d202997cdf0c1325e887337842513cc30dd2941
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32549539"
---
# <a name="omasettingboolean-resource-type"></a><span data-ttu-id="2cd66-103">omaSettingBoolean リソースの種類</span><span class="sxs-lookup"><span data-stu-id="2cd66-103">omaSettingBoolean resource type</span></span>

> <span data-ttu-id="2cd66-104">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="2cd66-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2cd66-105">OMA 設定のブール定義。</span><span class="sxs-lookup"><span data-stu-id="2cd66-105">OMA Settings Boolean definition.</span></span>


<span data-ttu-id="2cd66-106">[omaSetting](../resources/intune-deviceconfig-omasetting.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="2cd66-106">Inherits from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>

## <a name="properties"></a><span data-ttu-id="2cd66-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="2cd66-107">Properties</span></span>
|<span data-ttu-id="2cd66-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="2cd66-108">Property</span></span>|<span data-ttu-id="2cd66-109">型</span><span class="sxs-lookup"><span data-stu-id="2cd66-109">Type</span></span>|<span data-ttu-id="2cd66-110">説明</span><span class="sxs-lookup"><span data-stu-id="2cd66-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2cd66-111">displayName</span><span class="sxs-lookup"><span data-stu-id="2cd66-111">displayName</span></span>|<span data-ttu-id="2cd66-112">String</span><span class="sxs-lookup"><span data-stu-id="2cd66-112">String</span></span>|<span data-ttu-id="2cd66-113">表示名。</span><span class="sxs-lookup"><span data-stu-id="2cd66-113">Display Name.</span></span> <span data-ttu-id="2cd66-114">[omaSetting](../resources/intune-deviceconfig-omasetting.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="2cd66-114">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="2cd66-115">description</span><span class="sxs-lookup"><span data-stu-id="2cd66-115">description</span></span>|<span data-ttu-id="2cd66-116">String</span><span class="sxs-lookup"><span data-stu-id="2cd66-116">String</span></span>|<span data-ttu-id="2cd66-117">説明。</span><span class="sxs-lookup"><span data-stu-id="2cd66-117">Description.</span></span> <span data-ttu-id="2cd66-118">[omaSetting](../resources/intune-deviceconfig-omasetting.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="2cd66-118">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="2cd66-119">omaUri</span><span class="sxs-lookup"><span data-stu-id="2cd66-119">omaUri</span></span>|<span data-ttu-id="2cd66-120">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="2cd66-120">String</span></span>|<span data-ttu-id="2cd66-121">OMA。</span><span class="sxs-lookup"><span data-stu-id="2cd66-121">OMA.</span></span> <span data-ttu-id="2cd66-122">[omaSetting](../resources/intune-deviceconfig-omasetting.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="2cd66-122">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="2cd66-123">value</span><span class="sxs-lookup"><span data-stu-id="2cd66-123">value</span></span>|<span data-ttu-id="2cd66-124">ブール型 (Boolean)</span><span class="sxs-lookup"><span data-stu-id="2cd66-124">Boolean</span></span>|<span data-ttu-id="2cd66-125">値。</span><span class="sxs-lookup"><span data-stu-id="2cd66-125">Value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="2cd66-126">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="2cd66-126">Relationships</span></span>
<span data-ttu-id="2cd66-127">なし</span><span class="sxs-lookup"><span data-stu-id="2cd66-127">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="2cd66-128">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="2cd66-128">JSON Representation</span></span>
<span data-ttu-id="2cd66-129">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="2cd66-129">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.omaSettingBoolean"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.omaSettingBoolean",
  "displayName": "String",
  "description": "String",
  "omaUri": "String",
  "value": true
}
```



