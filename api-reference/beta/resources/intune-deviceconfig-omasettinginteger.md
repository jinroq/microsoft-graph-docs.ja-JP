---
title: omaSettingInteger リソースの種類
description: OMA 設定の整数の定義。
author: tfitzmac
ms.openlocfilehash: 27d38d1e1fe035ef95203ca1e636dedf7a05f103
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27363607"
---
# <a name="omasettinginteger-resource-type"></a><span data-ttu-id="220a3-103">omaSettingInteger リソースの種類</span><span class="sxs-lookup"><span data-stu-id="220a3-103">omaSettingInteger resource type</span></span>

> <span data-ttu-id="220a3-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="220a3-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="220a3-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="220a3-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="220a3-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="220a3-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="220a3-107">OMA 設定の整数の定義。</span><span class="sxs-lookup"><span data-stu-id="220a3-107">OMA Settings Integer definition.</span></span>

<span data-ttu-id="220a3-108">[omaSetting](../resources/intune-deviceconfig-omasetting.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="220a3-108">Inherits from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>

## <a name="properties"></a><span data-ttu-id="220a3-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="220a3-109">Properties</span></span>
|<span data-ttu-id="220a3-110">プロパティ</span><span class="sxs-lookup"><span data-stu-id="220a3-110">Property</span></span>|<span data-ttu-id="220a3-111">種類</span><span class="sxs-lookup"><span data-stu-id="220a3-111">Type</span></span>|<span data-ttu-id="220a3-112">説明</span><span class="sxs-lookup"><span data-stu-id="220a3-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="220a3-113">displayName</span><span class="sxs-lookup"><span data-stu-id="220a3-113">displayName</span></span>|<span data-ttu-id="220a3-114">文字列</span><span class="sxs-lookup"><span data-stu-id="220a3-114">String</span></span>|<span data-ttu-id="220a3-115">表示名。</span><span class="sxs-lookup"><span data-stu-id="220a3-115">Display Name.</span></span> <span data-ttu-id="220a3-116">[omaSetting](../resources/intune-deviceconfig-omasetting.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="220a3-116">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="220a3-117">説明</span><span class="sxs-lookup"><span data-stu-id="220a3-117">description</span></span>|<span data-ttu-id="220a3-118">String</span><span class="sxs-lookup"><span data-stu-id="220a3-118">String</span></span>|<span data-ttu-id="220a3-119">説明。</span><span class="sxs-lookup"><span data-stu-id="220a3-119">Description.</span></span> <span data-ttu-id="220a3-120">[omaSetting](../resources/intune-deviceconfig-omasetting.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="220a3-120">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="220a3-121">omaUri</span><span class="sxs-lookup"><span data-stu-id="220a3-121">omaUri</span></span>|<span data-ttu-id="220a3-122">文字列</span><span class="sxs-lookup"><span data-stu-id="220a3-122">String</span></span>|<span data-ttu-id="220a3-123">OMA。</span><span class="sxs-lookup"><span data-stu-id="220a3-123">OMA.</span></span> <span data-ttu-id="220a3-124">[omaSetting](../resources/intune-deviceconfig-omasetting.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="220a3-124">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="220a3-125">値</span><span class="sxs-lookup"><span data-stu-id="220a3-125">value</span></span>|<span data-ttu-id="220a3-126">Int32</span><span class="sxs-lookup"><span data-stu-id="220a3-126">Int32</span></span>|<span data-ttu-id="220a3-127">値。</span><span class="sxs-lookup"><span data-stu-id="220a3-127">Value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="220a3-128">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="220a3-128">Relationships</span></span>
<span data-ttu-id="220a3-129">なし</span><span class="sxs-lookup"><span data-stu-id="220a3-129">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="220a3-130">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="220a3-130">JSON Representation</span></span>
<span data-ttu-id="220a3-131">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="220a3-131">Here is a JSON representation of the resource.</span></span>
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





