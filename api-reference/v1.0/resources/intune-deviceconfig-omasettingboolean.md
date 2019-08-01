---
title: omaSettingBoolean リソースの種類
description: OMA 設定のブール定義。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 9c0ecb59f45a83cc98c6ff060b46ba0c620dc9cf
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36031340"
---
# <a name="omasettingboolean-resource-type"></a><span data-ttu-id="812e5-103">omaSettingBoolean リソースの種類</span><span class="sxs-lookup"><span data-stu-id="812e5-103">omaSettingBoolean resource type</span></span>

> <span data-ttu-id="812e5-104">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="812e5-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="812e5-105">OMA 設定のブール定義。</span><span class="sxs-lookup"><span data-stu-id="812e5-105">OMA Settings Boolean definition.</span></span>


<span data-ttu-id="812e5-106">[omaSetting](../resources/intune-deviceconfig-omasetting.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="812e5-106">Inherits from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>

## <a name="properties"></a><span data-ttu-id="812e5-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="812e5-107">Properties</span></span>
|<span data-ttu-id="812e5-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="812e5-108">Property</span></span>|<span data-ttu-id="812e5-109">型</span><span class="sxs-lookup"><span data-stu-id="812e5-109">Type</span></span>|<span data-ttu-id="812e5-110">説明</span><span class="sxs-lookup"><span data-stu-id="812e5-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="812e5-111">displayName</span><span class="sxs-lookup"><span data-stu-id="812e5-111">displayName</span></span>|<span data-ttu-id="812e5-112">String</span><span class="sxs-lookup"><span data-stu-id="812e5-112">String</span></span>|<span data-ttu-id="812e5-113">表示名。</span><span class="sxs-lookup"><span data-stu-id="812e5-113">Display Name.</span></span> <span data-ttu-id="812e5-114">[omaSetting](../resources/intune-deviceconfig-omasetting.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="812e5-114">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="812e5-115">description</span><span class="sxs-lookup"><span data-stu-id="812e5-115">description</span></span>|<span data-ttu-id="812e5-116">String</span><span class="sxs-lookup"><span data-stu-id="812e5-116">String</span></span>|<span data-ttu-id="812e5-117">説明。</span><span class="sxs-lookup"><span data-stu-id="812e5-117">Description.</span></span> <span data-ttu-id="812e5-118">[omaSetting](../resources/intune-deviceconfig-omasetting.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="812e5-118">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="812e5-119">omaUri</span><span class="sxs-lookup"><span data-stu-id="812e5-119">omaUri</span></span>|<span data-ttu-id="812e5-120">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="812e5-120">String</span></span>|<span data-ttu-id="812e5-121">OMA。</span><span class="sxs-lookup"><span data-stu-id="812e5-121">OMA.</span></span> <span data-ttu-id="812e5-122">[omaSetting](../resources/intune-deviceconfig-omasetting.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="812e5-122">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="812e5-123">value</span><span class="sxs-lookup"><span data-stu-id="812e5-123">value</span></span>|<span data-ttu-id="812e5-124">ブール型 (Boolean)</span><span class="sxs-lookup"><span data-stu-id="812e5-124">Boolean</span></span>|<span data-ttu-id="812e5-125">値。</span><span class="sxs-lookup"><span data-stu-id="812e5-125">Value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="812e5-126">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="812e5-126">Relationships</span></span>
<span data-ttu-id="812e5-127">なし</span><span class="sxs-lookup"><span data-stu-id="812e5-127">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="812e5-128">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="812e5-128">JSON Representation</span></span>
<span data-ttu-id="812e5-129">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="812e5-129">Here is a JSON representation of the resource.</span></span>
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



