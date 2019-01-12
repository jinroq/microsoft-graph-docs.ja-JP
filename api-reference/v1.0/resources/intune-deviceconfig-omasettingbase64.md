---
title: omaSettingBase64 リソースの種類
description: OMA 設定の Base64 定義。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 2acf41d36b4a664166dc2b5ceeb17dc0b6db4495
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27949844"
---
# <a name="omasettingbase64-resource-type"></a><span data-ttu-id="4bce1-103">omaSettingBase64 リソースの種類</span><span class="sxs-lookup"><span data-stu-id="4bce1-103">omaSettingBase64 resource type</span></span>

> <span data-ttu-id="4bce1-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="4bce1-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="4bce1-105">OMA 設定の Base64 定義。</span><span class="sxs-lookup"><span data-stu-id="4bce1-105">OMA Settings Base64 definition.</span></span>

<span data-ttu-id="4bce1-106">[omaSetting](../resources/intune-deviceconfig-omasetting.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="4bce1-106">Inherits from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>

## <a name="properties"></a><span data-ttu-id="4bce1-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="4bce1-107">Properties</span></span>
|<span data-ttu-id="4bce1-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="4bce1-108">Property</span></span>|<span data-ttu-id="4bce1-109">種類</span><span class="sxs-lookup"><span data-stu-id="4bce1-109">Type</span></span>|<span data-ttu-id="4bce1-110">説明</span><span class="sxs-lookup"><span data-stu-id="4bce1-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4bce1-111">displayName</span><span class="sxs-lookup"><span data-stu-id="4bce1-111">displayName</span></span>|<span data-ttu-id="4bce1-112">文字列</span><span class="sxs-lookup"><span data-stu-id="4bce1-112">String</span></span>|<span data-ttu-id="4bce1-113">表示名。</span><span class="sxs-lookup"><span data-stu-id="4bce1-113">Display Name.</span></span> <span data-ttu-id="4bce1-114">[omaSetting](../resources/intune-deviceconfig-omasetting.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="4bce1-114">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="4bce1-115">説明</span><span class="sxs-lookup"><span data-stu-id="4bce1-115">description</span></span>|<span data-ttu-id="4bce1-116">String</span><span class="sxs-lookup"><span data-stu-id="4bce1-116">String</span></span>|<span data-ttu-id="4bce1-117">説明。</span><span class="sxs-lookup"><span data-stu-id="4bce1-117">Description.</span></span> <span data-ttu-id="4bce1-118">[omaSetting](../resources/intune-deviceconfig-omasetting.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="4bce1-118">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="4bce1-119">omaUri</span><span class="sxs-lookup"><span data-stu-id="4bce1-119">omaUri</span></span>|<span data-ttu-id="4bce1-120">文字列</span><span class="sxs-lookup"><span data-stu-id="4bce1-120">String</span></span>|<span data-ttu-id="4bce1-121">OMA。</span><span class="sxs-lookup"><span data-stu-id="4bce1-121">OMA.</span></span> <span data-ttu-id="4bce1-122">[omaSetting](../resources/intune-deviceconfig-omasetting.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="4bce1-122">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="4bce1-123">fileName</span><span class="sxs-lookup"><span data-stu-id="4bce1-123">fileName</span></span>|<span data-ttu-id="4bce1-124">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="4bce1-124">String</span></span>|<span data-ttu-id="4bce1-125">Value プロパティに関連付けられているファイル名 (\*.cer</span><span class="sxs-lookup"><span data-stu-id="4bce1-125">File name associated with the Value property (\*.cer</span></span> | <span data-ttu-id="4bce1-126">\*.crt</span><span class="sxs-lookup"><span data-stu-id="4bce1-126">\*.crt</span></span> | <span data-ttu-id="4bce1-127">\*.p7b</span><span class="sxs-lookup"><span data-stu-id="4bce1-127">\*.p7b</span></span> | <span data-ttu-id="4bce1-128">\* .bin)。</span><span class="sxs-lookup"><span data-stu-id="4bce1-128">\*.bin).</span></span>|
|<span data-ttu-id="4bce1-129">value</span><span class="sxs-lookup"><span data-stu-id="4bce1-129">value</span></span>|<span data-ttu-id="4bce1-130">文字列</span><span class="sxs-lookup"><span data-stu-id="4bce1-130">String</span></span>|<span data-ttu-id="4bce1-131">値。</span><span class="sxs-lookup"><span data-stu-id="4bce1-131">Value.</span></span> <span data-ttu-id="4bce1-132">(Base64 エンコード文字列)</span><span class="sxs-lookup"><span data-stu-id="4bce1-132">(Base64 encoded string)</span></span>|

## <a name="relationships"></a><span data-ttu-id="4bce1-133">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="4bce1-133">Relationships</span></span>
<span data-ttu-id="4bce1-134">なし</span><span class="sxs-lookup"><span data-stu-id="4bce1-134">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="4bce1-135">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="4bce1-135">JSON Representation</span></span>
<span data-ttu-id="4bce1-136">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="4bce1-136">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.omaSettingBase64"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.omaSettingBase64",
  "displayName": "String",
  "description": "String",
  "omaUri": "String",
  "fileName": "String",
  "value": "String"
}
```



