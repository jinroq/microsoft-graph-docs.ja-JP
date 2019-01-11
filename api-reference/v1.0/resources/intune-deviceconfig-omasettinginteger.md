---
title: omaSettingInteger リソースの種類
description: OMA 設定の整数の定義。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: f40d5d225c2b4b99573c482b39f886bcd463e9fe
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27860453"
---
# <a name="omasettinginteger-resource-type"></a><span data-ttu-id="82d32-103">omaSettingInteger リソースの種類</span><span class="sxs-lookup"><span data-stu-id="82d32-103">omaSettingInteger resource type</span></span>

> <span data-ttu-id="82d32-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="82d32-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="82d32-105">OMA 設定の整数の定義。</span><span class="sxs-lookup"><span data-stu-id="82d32-105">OMA Settings Integer definition.</span></span>

<span data-ttu-id="82d32-106">[omaSetting](../resources/intune-deviceconfig-omasetting.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="82d32-106">Inherits from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>

## <a name="properties"></a><span data-ttu-id="82d32-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="82d32-107">Properties</span></span>
|<span data-ttu-id="82d32-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="82d32-108">Property</span></span>|<span data-ttu-id="82d32-109">種類</span><span class="sxs-lookup"><span data-stu-id="82d32-109">Type</span></span>|<span data-ttu-id="82d32-110">説明</span><span class="sxs-lookup"><span data-stu-id="82d32-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="82d32-111">displayName</span><span class="sxs-lookup"><span data-stu-id="82d32-111">displayName</span></span>|<span data-ttu-id="82d32-112">文字列</span><span class="sxs-lookup"><span data-stu-id="82d32-112">String</span></span>|<span data-ttu-id="82d32-113">表示名。</span><span class="sxs-lookup"><span data-stu-id="82d32-113">Display Name.</span></span> <span data-ttu-id="82d32-114">[omaSetting](../resources/intune-deviceconfig-omasetting.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="82d32-114">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="82d32-115">説明</span><span class="sxs-lookup"><span data-stu-id="82d32-115">description</span></span>|<span data-ttu-id="82d32-116">String</span><span class="sxs-lookup"><span data-stu-id="82d32-116">String</span></span>|<span data-ttu-id="82d32-117">説明。</span><span class="sxs-lookup"><span data-stu-id="82d32-117">Description.</span></span> <span data-ttu-id="82d32-118">[omaSetting](../resources/intune-deviceconfig-omasetting.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="82d32-118">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="82d32-119">omaUri</span><span class="sxs-lookup"><span data-stu-id="82d32-119">omaUri</span></span>|<span data-ttu-id="82d32-120">文字列</span><span class="sxs-lookup"><span data-stu-id="82d32-120">String</span></span>|<span data-ttu-id="82d32-121">OMA。</span><span class="sxs-lookup"><span data-stu-id="82d32-121">OMA.</span></span> <span data-ttu-id="82d32-122">[omaSetting](../resources/intune-deviceconfig-omasetting.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="82d32-122">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="82d32-123">値</span><span class="sxs-lookup"><span data-stu-id="82d32-123">value</span></span>|<span data-ttu-id="82d32-124">Int32</span><span class="sxs-lookup"><span data-stu-id="82d32-124">Int32</span></span>|<span data-ttu-id="82d32-125">値。</span><span class="sxs-lookup"><span data-stu-id="82d32-125">Value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="82d32-126">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="82d32-126">Relationships</span></span>
<span data-ttu-id="82d32-127">なし</span><span class="sxs-lookup"><span data-stu-id="82d32-127">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="82d32-128">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="82d32-128">JSON Representation</span></span>
<span data-ttu-id="82d32-129">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="82d32-129">Here is a JSON representation of the resource.</span></span>
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



