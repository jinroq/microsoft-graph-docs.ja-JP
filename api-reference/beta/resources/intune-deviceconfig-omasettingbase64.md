---
title: omaSettingBase64 リソースの種類
description: OMA 設定の Base64 定義。
author: tfitzmac
ms.openlocfilehash: ee25db94cc1426194166a7c66b9a8a626d62c3e4
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27304075"
---
# <a name="omasettingbase64-resource-type"></a><span data-ttu-id="01355-103">omaSettingBase64 リソースの種類</span><span class="sxs-lookup"><span data-stu-id="01355-103">omaSettingBase64 resource type</span></span>

> <span data-ttu-id="01355-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="01355-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="01355-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="01355-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="01355-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="01355-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="01355-107">OMA 設定の Base64 定義。</span><span class="sxs-lookup"><span data-stu-id="01355-107">OMA Settings Base64 definition.</span></span>

<span data-ttu-id="01355-108">[omaSetting](../resources/intune-deviceconfig-omasetting.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="01355-108">Inherits from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>

## <a name="properties"></a><span data-ttu-id="01355-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="01355-109">Properties</span></span>
|<span data-ttu-id="01355-110">プロパティ</span><span class="sxs-lookup"><span data-stu-id="01355-110">Property</span></span>|<span data-ttu-id="01355-111">種類</span><span class="sxs-lookup"><span data-stu-id="01355-111">Type</span></span>|<span data-ttu-id="01355-112">説明</span><span class="sxs-lookup"><span data-stu-id="01355-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="01355-113">displayName</span><span class="sxs-lookup"><span data-stu-id="01355-113">displayName</span></span>|<span data-ttu-id="01355-114">文字列</span><span class="sxs-lookup"><span data-stu-id="01355-114">String</span></span>|<span data-ttu-id="01355-115">表示名。</span><span class="sxs-lookup"><span data-stu-id="01355-115">Display Name.</span></span> <span data-ttu-id="01355-116">[omaSetting](../resources/intune-deviceconfig-omasetting.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="01355-116">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="01355-117">説明</span><span class="sxs-lookup"><span data-stu-id="01355-117">description</span></span>|<span data-ttu-id="01355-118">String</span><span class="sxs-lookup"><span data-stu-id="01355-118">String</span></span>|<span data-ttu-id="01355-119">説明。</span><span class="sxs-lookup"><span data-stu-id="01355-119">Description.</span></span> <span data-ttu-id="01355-120">[omaSetting](../resources/intune-deviceconfig-omasetting.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="01355-120">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="01355-121">omaUri</span><span class="sxs-lookup"><span data-stu-id="01355-121">omaUri</span></span>|<span data-ttu-id="01355-122">文字列</span><span class="sxs-lookup"><span data-stu-id="01355-122">String</span></span>|<span data-ttu-id="01355-123">OMA。</span><span class="sxs-lookup"><span data-stu-id="01355-123">OMA.</span></span> <span data-ttu-id="01355-124">[omaSetting](../resources/intune-deviceconfig-omasetting.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="01355-124">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="01355-125">fileName</span><span class="sxs-lookup"><span data-stu-id="01355-125">fileName</span></span>|<span data-ttu-id="01355-126">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="01355-126">String</span></span>|<span data-ttu-id="01355-127">Value プロパティに関連付けられているファイル名 (\*.cer</span><span class="sxs-lookup"><span data-stu-id="01355-127">File name associated with the Value property (\*.cer</span></span> | <span data-ttu-id="01355-128">\*.crt</span><span class="sxs-lookup"><span data-stu-id="01355-128">\*.crt</span></span> | <span data-ttu-id="01355-129">\*.p7b</span><span class="sxs-lookup"><span data-stu-id="01355-129">\*.p7b</span></span> | <span data-ttu-id="01355-130">\* .bin)。</span><span class="sxs-lookup"><span data-stu-id="01355-130">\*.bin).</span></span>|
|<span data-ttu-id="01355-131">value</span><span class="sxs-lookup"><span data-stu-id="01355-131">value</span></span>|<span data-ttu-id="01355-132">文字列</span><span class="sxs-lookup"><span data-stu-id="01355-132">String</span></span>|<span data-ttu-id="01355-133">値。</span><span class="sxs-lookup"><span data-stu-id="01355-133">Value.</span></span> <span data-ttu-id="01355-134">(Base64 エンコード文字列)</span><span class="sxs-lookup"><span data-stu-id="01355-134">(Base64 encoded string)</span></span>|

## <a name="relationships"></a><span data-ttu-id="01355-135">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="01355-135">Relationships</span></span>
<span data-ttu-id="01355-136">なし</span><span class="sxs-lookup"><span data-stu-id="01355-136">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="01355-137">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="01355-137">JSON Representation</span></span>
<span data-ttu-id="01355-138">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="01355-138">Here is a JSON representation of the resource.</span></span>
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





