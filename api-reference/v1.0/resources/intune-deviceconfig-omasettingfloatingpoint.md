---
title: omaSettingFloatingPoint リソースの種類
description: OMA 設定の浮動小数点の定義です。
author: tfitzmac
ms.openlocfilehash: efed2112f85ee0600fcbe499616a7f3e787beb59
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27360754"
---
# <a name="omasettingfloatingpoint-resource-type"></a><span data-ttu-id="98576-103">omaSettingFloatingPoint リソースの種類</span><span class="sxs-lookup"><span data-stu-id="98576-103">omaSettingFloatingPoint resource type</span></span>

> <span data-ttu-id="98576-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="98576-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="98576-105">OMA 設定の浮動小数点の定義です。</span><span class="sxs-lookup"><span data-stu-id="98576-105">OMA Settings Floating Point definition.</span></span>

<span data-ttu-id="98576-106">[omaSetting](../resources/intune-deviceconfig-omasetting.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="98576-106">Inherits from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>

## <a name="properties"></a><span data-ttu-id="98576-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="98576-107">Properties</span></span>
|<span data-ttu-id="98576-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="98576-108">Property</span></span>|<span data-ttu-id="98576-109">種類</span><span class="sxs-lookup"><span data-stu-id="98576-109">Type</span></span>|<span data-ttu-id="98576-110">説明</span><span class="sxs-lookup"><span data-stu-id="98576-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="98576-111">displayName</span><span class="sxs-lookup"><span data-stu-id="98576-111">displayName</span></span>|<span data-ttu-id="98576-112">文字列</span><span class="sxs-lookup"><span data-stu-id="98576-112">String</span></span>|<span data-ttu-id="98576-113">表示名。</span><span class="sxs-lookup"><span data-stu-id="98576-113">Display Name.</span></span> <span data-ttu-id="98576-114">[omaSetting](../resources/intune-deviceconfig-omasetting.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="98576-114">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="98576-115">説明</span><span class="sxs-lookup"><span data-stu-id="98576-115">description</span></span>|<span data-ttu-id="98576-116">String</span><span class="sxs-lookup"><span data-stu-id="98576-116">String</span></span>|<span data-ttu-id="98576-117">説明。</span><span class="sxs-lookup"><span data-stu-id="98576-117">Description.</span></span> <span data-ttu-id="98576-118">[omaSetting](../resources/intune-deviceconfig-omasetting.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="98576-118">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="98576-119">omaUri</span><span class="sxs-lookup"><span data-stu-id="98576-119">omaUri</span></span>|<span data-ttu-id="98576-120">文字列</span><span class="sxs-lookup"><span data-stu-id="98576-120">String</span></span>|<span data-ttu-id="98576-121">OMA。</span><span class="sxs-lookup"><span data-stu-id="98576-121">OMA.</span></span> <span data-ttu-id="98576-122">[omaSetting](../resources/intune-deviceconfig-omasetting.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="98576-122">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="98576-123">値</span><span class="sxs-lookup"><span data-stu-id="98576-123">value</span></span>|<span data-ttu-id="98576-124">単精度浮動小数点型 (Single)</span><span class="sxs-lookup"><span data-stu-id="98576-124">Single</span></span>|<span data-ttu-id="98576-125">値。</span><span class="sxs-lookup"><span data-stu-id="98576-125">Value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="98576-126">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="98576-126">Relationships</span></span>
<span data-ttu-id="98576-127">なし</span><span class="sxs-lookup"><span data-stu-id="98576-127">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="98576-128">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="98576-128">JSON Representation</span></span>
<span data-ttu-id="98576-129">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="98576-129">Here is a JSON representation of the resource.</span></span>
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


