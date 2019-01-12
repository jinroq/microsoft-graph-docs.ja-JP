---
title: omaSettingBase64 リソースの種類
description: OMA 設定の Base64 定義。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 8f1c6a488adf2f39b2c415e31c4919380ebda5ab
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27982569"
---
# <a name="omasettingbase64-resource-type"></a><span data-ttu-id="c9a5b-103">omaSettingBase64 リソースの種類</span><span class="sxs-lookup"><span data-stu-id="c9a5b-103">omaSettingBase64 resource type</span></span>

> <span data-ttu-id="c9a5b-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="c9a5b-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c9a5b-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c9a5b-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="c9a5b-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="c9a5b-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="c9a5b-107">OMA 設定の Base64 定義。</span><span class="sxs-lookup"><span data-stu-id="c9a5b-107">OMA Settings Base64 definition.</span></span>

<span data-ttu-id="c9a5b-108">[omaSetting](../resources/intune-deviceconfig-omasetting.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="c9a5b-108">Inherits from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>

## <a name="properties"></a><span data-ttu-id="c9a5b-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="c9a5b-109">Properties</span></span>
|<span data-ttu-id="c9a5b-110">プロパティ</span><span class="sxs-lookup"><span data-stu-id="c9a5b-110">Property</span></span>|<span data-ttu-id="c9a5b-111">型</span><span class="sxs-lookup"><span data-stu-id="c9a5b-111">Type</span></span>|<span data-ttu-id="c9a5b-112">説明</span><span class="sxs-lookup"><span data-stu-id="c9a5b-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c9a5b-113">displayName</span><span class="sxs-lookup"><span data-stu-id="c9a5b-113">displayName</span></span>|<span data-ttu-id="c9a5b-114">文字列</span><span class="sxs-lookup"><span data-stu-id="c9a5b-114">String</span></span>|<span data-ttu-id="c9a5b-115">表示名。</span><span class="sxs-lookup"><span data-stu-id="c9a5b-115">Display Name.</span></span> <span data-ttu-id="c9a5b-116">[omaSetting](../resources/intune-deviceconfig-omasetting.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="c9a5b-116">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="c9a5b-117">説明</span><span class="sxs-lookup"><span data-stu-id="c9a5b-117">description</span></span>|<span data-ttu-id="c9a5b-118">String</span><span class="sxs-lookup"><span data-stu-id="c9a5b-118">String</span></span>|<span data-ttu-id="c9a5b-119">説明。</span><span class="sxs-lookup"><span data-stu-id="c9a5b-119">Description.</span></span> <span data-ttu-id="c9a5b-120">[omaSetting](../resources/intune-deviceconfig-omasetting.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="c9a5b-120">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="c9a5b-121">omaUri</span><span class="sxs-lookup"><span data-stu-id="c9a5b-121">omaUri</span></span>|<span data-ttu-id="c9a5b-122">文字列</span><span class="sxs-lookup"><span data-stu-id="c9a5b-122">String</span></span>|<span data-ttu-id="c9a5b-123">OMA。</span><span class="sxs-lookup"><span data-stu-id="c9a5b-123">OMA.</span></span> <span data-ttu-id="c9a5b-124">[omaSetting](../resources/intune-deviceconfig-omasetting.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="c9a5b-124">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="c9a5b-125">fileName</span><span class="sxs-lookup"><span data-stu-id="c9a5b-125">fileName</span></span>|<span data-ttu-id="c9a5b-126">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="c9a5b-126">String</span></span>|<span data-ttu-id="c9a5b-127">Value プロパティに関連付けられているファイル名 (\*.cer</span><span class="sxs-lookup"><span data-stu-id="c9a5b-127">File name associated with the Value property (\*.cer</span></span> | <span data-ttu-id="c9a5b-128">\*.crt</span><span class="sxs-lookup"><span data-stu-id="c9a5b-128">\*.crt</span></span> | <span data-ttu-id="c9a5b-129">\*.p7b</span><span class="sxs-lookup"><span data-stu-id="c9a5b-129">\*.p7b</span></span> | <span data-ttu-id="c9a5b-130">\* .bin)。</span><span class="sxs-lookup"><span data-stu-id="c9a5b-130">\*.bin).</span></span>|
|<span data-ttu-id="c9a5b-131">value</span><span class="sxs-lookup"><span data-stu-id="c9a5b-131">value</span></span>|<span data-ttu-id="c9a5b-132">文字列</span><span class="sxs-lookup"><span data-stu-id="c9a5b-132">String</span></span>|<span data-ttu-id="c9a5b-133">値。</span><span class="sxs-lookup"><span data-stu-id="c9a5b-133">Value.</span></span> <span data-ttu-id="c9a5b-134">(Base64 エンコード文字列)</span><span class="sxs-lookup"><span data-stu-id="c9a5b-134">(Base64 encoded string)</span></span>|

## <a name="relationships"></a><span data-ttu-id="c9a5b-135">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="c9a5b-135">Relationships</span></span>
<span data-ttu-id="c9a5b-136">なし</span><span class="sxs-lookup"><span data-stu-id="c9a5b-136">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="c9a5b-137">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="c9a5b-137">JSON Representation</span></span>
<span data-ttu-id="c9a5b-138">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="c9a5b-138">Here is a JSON representation of the resource.</span></span>
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





