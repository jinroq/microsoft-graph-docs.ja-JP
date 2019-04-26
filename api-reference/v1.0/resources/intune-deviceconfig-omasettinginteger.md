---
title: omaSettingInteger リソースの種類
description: OMA 設定の整数の定義。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 0e4896af0e43510eb791f37a72a864a405388e9d
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32569019"
---
# <a name="omasettinginteger-resource-type"></a><span data-ttu-id="24a74-103">omaSettingInteger リソースの種類</span><span class="sxs-lookup"><span data-stu-id="24a74-103">omaSettingInteger resource type</span></span>

> <span data-ttu-id="24a74-104">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="24a74-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="24a74-105">OMA 設定の整数の定義。</span><span class="sxs-lookup"><span data-stu-id="24a74-105">OMA Settings Integer definition.</span></span>


<span data-ttu-id="24a74-106">[omaSetting](../resources/intune-deviceconfig-omasetting.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="24a74-106">Inherits from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>

## <a name="properties"></a><span data-ttu-id="24a74-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="24a74-107">Properties</span></span>
|<span data-ttu-id="24a74-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="24a74-108">Property</span></span>|<span data-ttu-id="24a74-109">型</span><span class="sxs-lookup"><span data-stu-id="24a74-109">Type</span></span>|<span data-ttu-id="24a74-110">説明</span><span class="sxs-lookup"><span data-stu-id="24a74-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="24a74-111">displayName</span><span class="sxs-lookup"><span data-stu-id="24a74-111">displayName</span></span>|<span data-ttu-id="24a74-112">String</span><span class="sxs-lookup"><span data-stu-id="24a74-112">String</span></span>|<span data-ttu-id="24a74-113">表示名。</span><span class="sxs-lookup"><span data-stu-id="24a74-113">Display Name.</span></span> <span data-ttu-id="24a74-114">[omaSetting](../resources/intune-deviceconfig-omasetting.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="24a74-114">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="24a74-115">説明</span><span class="sxs-lookup"><span data-stu-id="24a74-115">description</span></span>|<span data-ttu-id="24a74-116">String</span><span class="sxs-lookup"><span data-stu-id="24a74-116">String</span></span>|<span data-ttu-id="24a74-117">説明。</span><span class="sxs-lookup"><span data-stu-id="24a74-117">Description.</span></span> <span data-ttu-id="24a74-118">[omaSetting](../resources/intune-deviceconfig-omasetting.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="24a74-118">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="24a74-119">omaUri</span><span class="sxs-lookup"><span data-stu-id="24a74-119">omaUri</span></span>|<span data-ttu-id="24a74-120">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="24a74-120">String</span></span>|<span data-ttu-id="24a74-121">OMA。</span><span class="sxs-lookup"><span data-stu-id="24a74-121">OMA.</span></span> <span data-ttu-id="24a74-122">[omaSetting](../resources/intune-deviceconfig-omasetting.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="24a74-122">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="24a74-123">値</span><span class="sxs-lookup"><span data-stu-id="24a74-123">value</span></span>|<span data-ttu-id="24a74-124">Int32</span><span class="sxs-lookup"><span data-stu-id="24a74-124">Int32</span></span>|<span data-ttu-id="24a74-125">値。</span><span class="sxs-lookup"><span data-stu-id="24a74-125">Value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="24a74-126">関係</span><span class="sxs-lookup"><span data-stu-id="24a74-126">Relationships</span></span>
<span data-ttu-id="24a74-127">なし</span><span class="sxs-lookup"><span data-stu-id="24a74-127">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="24a74-128">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="24a74-128">JSON Representation</span></span>
<span data-ttu-id="24a74-129">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="24a74-129">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.omaSettingInteger"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.omaSettingInteger",
  "displayName": "String",
  "description": "String",
  "omaUri": "String",
  "value": 1024
}
```



