---
title: omaSettingInteger リソースの種類
description: OMA 設定の整数の定義。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: f46398e43f2a7ea224a07b1637deca2c3a6ed067
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27987532"
---
# <a name="omasettinginteger-resource-type"></a><span data-ttu-id="09cbd-103">omaSettingInteger リソースの種類</span><span class="sxs-lookup"><span data-stu-id="09cbd-103">omaSettingInteger resource type</span></span>

> <span data-ttu-id="09cbd-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="09cbd-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="09cbd-105">OMA 設定の整数の定義。</span><span class="sxs-lookup"><span data-stu-id="09cbd-105">OMA Settings Integer definition.</span></span>

<span data-ttu-id="09cbd-106">[omaSetting](../resources/intune-deviceconfig-omasetting.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="09cbd-106">Inherits from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>

## <a name="properties"></a><span data-ttu-id="09cbd-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="09cbd-107">Properties</span></span>
|<span data-ttu-id="09cbd-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="09cbd-108">Property</span></span>|<span data-ttu-id="09cbd-109">種類</span><span class="sxs-lookup"><span data-stu-id="09cbd-109">Type</span></span>|<span data-ttu-id="09cbd-110">説明</span><span class="sxs-lookup"><span data-stu-id="09cbd-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="09cbd-111">displayName</span><span class="sxs-lookup"><span data-stu-id="09cbd-111">displayName</span></span>|<span data-ttu-id="09cbd-112">文字列</span><span class="sxs-lookup"><span data-stu-id="09cbd-112">String</span></span>|<span data-ttu-id="09cbd-113">表示名。</span><span class="sxs-lookup"><span data-stu-id="09cbd-113">Display Name.</span></span> <span data-ttu-id="09cbd-114">[omaSetting](../resources/intune-deviceconfig-omasetting.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="09cbd-114">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="09cbd-115">説明</span><span class="sxs-lookup"><span data-stu-id="09cbd-115">description</span></span>|<span data-ttu-id="09cbd-116">String</span><span class="sxs-lookup"><span data-stu-id="09cbd-116">String</span></span>|<span data-ttu-id="09cbd-117">説明。</span><span class="sxs-lookup"><span data-stu-id="09cbd-117">Description.</span></span> <span data-ttu-id="09cbd-118">[omaSetting](../resources/intune-deviceconfig-omasetting.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="09cbd-118">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="09cbd-119">omaUri</span><span class="sxs-lookup"><span data-stu-id="09cbd-119">omaUri</span></span>|<span data-ttu-id="09cbd-120">文字列</span><span class="sxs-lookup"><span data-stu-id="09cbd-120">String</span></span>|<span data-ttu-id="09cbd-121">OMA。</span><span class="sxs-lookup"><span data-stu-id="09cbd-121">OMA.</span></span> <span data-ttu-id="09cbd-122">[omaSetting](../resources/intune-deviceconfig-omasetting.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="09cbd-122">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="09cbd-123">値</span><span class="sxs-lookup"><span data-stu-id="09cbd-123">value</span></span>|<span data-ttu-id="09cbd-124">Int32</span><span class="sxs-lookup"><span data-stu-id="09cbd-124">Int32</span></span>|<span data-ttu-id="09cbd-125">値。</span><span class="sxs-lookup"><span data-stu-id="09cbd-125">Value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="09cbd-126">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="09cbd-126">Relationships</span></span>
<span data-ttu-id="09cbd-127">なし</span><span class="sxs-lookup"><span data-stu-id="09cbd-127">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="09cbd-128">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="09cbd-128">JSON Representation</span></span>
<span data-ttu-id="09cbd-129">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="09cbd-129">Here is a JSON representation of the resource.</span></span>
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



