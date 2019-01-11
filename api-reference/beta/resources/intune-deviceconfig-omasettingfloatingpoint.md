---
title: omaSettingFloatingPoint リソースの種類
description: OMA 設定の浮動小数点の定義です。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 21419d857699f6eec4b59f6ea33a96e6b7f8c730
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27829387"
---
# <a name="omasettingfloatingpoint-resource-type"></a><span data-ttu-id="7eaba-103">omaSettingFloatingPoint リソースの種類</span><span class="sxs-lookup"><span data-stu-id="7eaba-103">omaSettingFloatingPoint resource type</span></span>

> <span data-ttu-id="7eaba-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="7eaba-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="7eaba-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="7eaba-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="7eaba-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="7eaba-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="7eaba-107">OMA 設定の浮動小数点の定義です。</span><span class="sxs-lookup"><span data-stu-id="7eaba-107">OMA Settings Floating Point definition.</span></span>

<span data-ttu-id="7eaba-108">[omaSetting](../resources/intune-deviceconfig-omasetting.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="7eaba-108">Inherits from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>

## <a name="properties"></a><span data-ttu-id="7eaba-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="7eaba-109">Properties</span></span>
|<span data-ttu-id="7eaba-110">プロパティ</span><span class="sxs-lookup"><span data-stu-id="7eaba-110">Property</span></span>|<span data-ttu-id="7eaba-111">種類</span><span class="sxs-lookup"><span data-stu-id="7eaba-111">Type</span></span>|<span data-ttu-id="7eaba-112">説明</span><span class="sxs-lookup"><span data-stu-id="7eaba-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7eaba-113">displayName</span><span class="sxs-lookup"><span data-stu-id="7eaba-113">displayName</span></span>|<span data-ttu-id="7eaba-114">文字列</span><span class="sxs-lookup"><span data-stu-id="7eaba-114">String</span></span>|<span data-ttu-id="7eaba-115">表示名。</span><span class="sxs-lookup"><span data-stu-id="7eaba-115">Display Name.</span></span> <span data-ttu-id="7eaba-116">[omaSetting](../resources/intune-deviceconfig-omasetting.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="7eaba-116">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="7eaba-117">説明</span><span class="sxs-lookup"><span data-stu-id="7eaba-117">description</span></span>|<span data-ttu-id="7eaba-118">String</span><span class="sxs-lookup"><span data-stu-id="7eaba-118">String</span></span>|<span data-ttu-id="7eaba-119">説明。</span><span class="sxs-lookup"><span data-stu-id="7eaba-119">Description.</span></span> <span data-ttu-id="7eaba-120">[omaSetting](../resources/intune-deviceconfig-omasetting.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="7eaba-120">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="7eaba-121">omaUri</span><span class="sxs-lookup"><span data-stu-id="7eaba-121">omaUri</span></span>|<span data-ttu-id="7eaba-122">文字列</span><span class="sxs-lookup"><span data-stu-id="7eaba-122">String</span></span>|<span data-ttu-id="7eaba-123">OMA。</span><span class="sxs-lookup"><span data-stu-id="7eaba-123">OMA.</span></span> <span data-ttu-id="7eaba-124">[omaSetting](../resources/intune-deviceconfig-omasetting.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="7eaba-124">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="7eaba-125">値</span><span class="sxs-lookup"><span data-stu-id="7eaba-125">value</span></span>|<span data-ttu-id="7eaba-126">単精度浮動小数点型 (Single)</span><span class="sxs-lookup"><span data-stu-id="7eaba-126">Single</span></span>|<span data-ttu-id="7eaba-127">値。</span><span class="sxs-lookup"><span data-stu-id="7eaba-127">Value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="7eaba-128">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="7eaba-128">Relationships</span></span>
<span data-ttu-id="7eaba-129">なし</span><span class="sxs-lookup"><span data-stu-id="7eaba-129">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="7eaba-130">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="7eaba-130">JSON Representation</span></span>
<span data-ttu-id="7eaba-131">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="7eaba-131">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.omaSettingFloatingPoint"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.omaSettingFloatingPoint",
  "displayName": "String",
  "description": "String",
  "omaUri": "String",
  "value": "<Unknown Primitive Type Edm.Single>"
}
```





