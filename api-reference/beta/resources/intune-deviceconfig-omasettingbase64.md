---
title: omaSettingBase64 リソースの種類
description: OMA 設定の Base64 定義。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: f5b21705d4cabedc24009df794d958c6187af473
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27869819"
---
# <a name="omasettingbase64-resource-type"></a><span data-ttu-id="ecc63-103">omaSettingBase64 リソースの種類</span><span class="sxs-lookup"><span data-stu-id="ecc63-103">omaSettingBase64 resource type</span></span>

> <span data-ttu-id="ecc63-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="ecc63-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ecc63-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ecc63-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="ecc63-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="ecc63-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="ecc63-107">OMA 設定の Base64 定義。</span><span class="sxs-lookup"><span data-stu-id="ecc63-107">OMA Settings Base64 definition.</span></span>

<span data-ttu-id="ecc63-108">[omaSetting](../resources/intune-deviceconfig-omasetting.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="ecc63-108">Inherits from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>

## <a name="properties"></a><span data-ttu-id="ecc63-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="ecc63-109">Properties</span></span>
|<span data-ttu-id="ecc63-110">プロパティ</span><span class="sxs-lookup"><span data-stu-id="ecc63-110">Property</span></span>|<span data-ttu-id="ecc63-111">種類</span><span class="sxs-lookup"><span data-stu-id="ecc63-111">Type</span></span>|<span data-ttu-id="ecc63-112">説明</span><span class="sxs-lookup"><span data-stu-id="ecc63-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ecc63-113">displayName</span><span class="sxs-lookup"><span data-stu-id="ecc63-113">displayName</span></span>|<span data-ttu-id="ecc63-114">文字列</span><span class="sxs-lookup"><span data-stu-id="ecc63-114">String</span></span>|<span data-ttu-id="ecc63-115">表示名。</span><span class="sxs-lookup"><span data-stu-id="ecc63-115">Display Name.</span></span> <span data-ttu-id="ecc63-116">[omaSetting](../resources/intune-deviceconfig-omasetting.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="ecc63-116">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="ecc63-117">説明</span><span class="sxs-lookup"><span data-stu-id="ecc63-117">description</span></span>|<span data-ttu-id="ecc63-118">String</span><span class="sxs-lookup"><span data-stu-id="ecc63-118">String</span></span>|<span data-ttu-id="ecc63-119">説明。</span><span class="sxs-lookup"><span data-stu-id="ecc63-119">Description.</span></span> <span data-ttu-id="ecc63-120">[omaSetting](../resources/intune-deviceconfig-omasetting.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="ecc63-120">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="ecc63-121">omaUri</span><span class="sxs-lookup"><span data-stu-id="ecc63-121">omaUri</span></span>|<span data-ttu-id="ecc63-122">文字列</span><span class="sxs-lookup"><span data-stu-id="ecc63-122">String</span></span>|<span data-ttu-id="ecc63-123">OMA。</span><span class="sxs-lookup"><span data-stu-id="ecc63-123">OMA.</span></span> <span data-ttu-id="ecc63-124">[omaSetting](../resources/intune-deviceconfig-omasetting.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="ecc63-124">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="ecc63-125">fileName</span><span class="sxs-lookup"><span data-stu-id="ecc63-125">fileName</span></span>|<span data-ttu-id="ecc63-126">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="ecc63-126">String</span></span>|<span data-ttu-id="ecc63-127">Value プロパティに関連付けられているファイル名 (\*.cer</span><span class="sxs-lookup"><span data-stu-id="ecc63-127">File name associated with the Value property (\*.cer</span></span> | <span data-ttu-id="ecc63-128">\*.crt</span><span class="sxs-lookup"><span data-stu-id="ecc63-128">\*.crt</span></span> | <span data-ttu-id="ecc63-129">\*.p7b</span><span class="sxs-lookup"><span data-stu-id="ecc63-129">\*.p7b</span></span> | <span data-ttu-id="ecc63-130">\* .bin)。</span><span class="sxs-lookup"><span data-stu-id="ecc63-130">\*.bin).</span></span>|
|<span data-ttu-id="ecc63-131">value</span><span class="sxs-lookup"><span data-stu-id="ecc63-131">value</span></span>|<span data-ttu-id="ecc63-132">文字列</span><span class="sxs-lookup"><span data-stu-id="ecc63-132">String</span></span>|<span data-ttu-id="ecc63-133">値。</span><span class="sxs-lookup"><span data-stu-id="ecc63-133">Value.</span></span> <span data-ttu-id="ecc63-134">(Base64 エンコード文字列)</span><span class="sxs-lookup"><span data-stu-id="ecc63-134">(Base64 encoded string)</span></span>|

## <a name="relationships"></a><span data-ttu-id="ecc63-135">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="ecc63-135">Relationships</span></span>
<span data-ttu-id="ecc63-136">なし</span><span class="sxs-lookup"><span data-stu-id="ecc63-136">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="ecc63-137">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="ecc63-137">JSON Representation</span></span>
<span data-ttu-id="ecc63-138">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="ecc63-138">Here is a JSON representation of the resource.</span></span>
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





