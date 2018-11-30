---
title: omaSettingBase64 リソースの種類
description: OMA 設定の Base64 定義。
ms.openlocfilehash: eebe9730c36ab4bc7e48aa765ecd3959897c6c12
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27069939"
---
# <a name="omasettingbase64-resource-type"></a><span data-ttu-id="9c291-103">omaSettingBase64 リソースの種類</span><span class="sxs-lookup"><span data-stu-id="9c291-103">omaSettingBase64 resource type</span></span>

> <span data-ttu-id="9c291-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="9c291-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="9c291-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="9c291-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="9c291-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="9c291-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="9c291-107">OMA 設定の Base64 定義。</span><span class="sxs-lookup"><span data-stu-id="9c291-107">OMA Settings Base64 definition.</span></span>

<span data-ttu-id="9c291-108">[omaSetting](../resources/intune-deviceconfig-omasetting.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="9c291-108">Inherits from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>

## <a name="properties"></a><span data-ttu-id="9c291-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="9c291-109">Properties</span></span>
|<span data-ttu-id="9c291-110">プロパティ</span><span class="sxs-lookup"><span data-stu-id="9c291-110">Property</span></span>|<span data-ttu-id="9c291-111">型</span><span class="sxs-lookup"><span data-stu-id="9c291-111">Type</span></span>|<span data-ttu-id="9c291-112">説明</span><span class="sxs-lookup"><span data-stu-id="9c291-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9c291-113">displayName</span><span class="sxs-lookup"><span data-stu-id="9c291-113">displayName</span></span>|<span data-ttu-id="9c291-114">文字列</span><span class="sxs-lookup"><span data-stu-id="9c291-114">String</span></span>|<span data-ttu-id="9c291-115">表示名。</span><span class="sxs-lookup"><span data-stu-id="9c291-115">Display Name.</span></span> <span data-ttu-id="9c291-116">[omaSetting](../resources/intune-deviceconfig-omasetting.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="9c291-116">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="9c291-117">説明</span><span class="sxs-lookup"><span data-stu-id="9c291-117">description</span></span>|<span data-ttu-id="9c291-118">String</span><span class="sxs-lookup"><span data-stu-id="9c291-118">String</span></span>|<span data-ttu-id="9c291-119">説明。</span><span class="sxs-lookup"><span data-stu-id="9c291-119">Description.</span></span> <span data-ttu-id="9c291-120">[omaSetting](../resources/intune-deviceconfig-omasetting.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="9c291-120">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="9c291-121">omaUri</span><span class="sxs-lookup"><span data-stu-id="9c291-121">omaUri</span></span>|<span data-ttu-id="9c291-122">文字列</span><span class="sxs-lookup"><span data-stu-id="9c291-122">String</span></span>|<span data-ttu-id="9c291-123">OMA。</span><span class="sxs-lookup"><span data-stu-id="9c291-123">OMA.</span></span> <span data-ttu-id="9c291-124">[omaSetting](../resources/intune-deviceconfig-omasetting.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="9c291-124">Inherited from [omaSetting](../resources/intune-deviceconfig-omasetting.md)</span></span>|
|<span data-ttu-id="9c291-125">fileName</span><span class="sxs-lookup"><span data-stu-id="9c291-125">fileName</span></span>|<span data-ttu-id="9c291-126">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="9c291-126">String</span></span>|<span data-ttu-id="9c291-127">Value プロパティに関連付けられているファイル名 (\*.cer</span><span class="sxs-lookup"><span data-stu-id="9c291-127">File name associated with the Value property (\*.cer</span></span> | <span data-ttu-id="9c291-128">\*.crt</span><span class="sxs-lookup"><span data-stu-id="9c291-128">\*.crt</span></span> | <span data-ttu-id="9c291-129">\*.p7b</span><span class="sxs-lookup"><span data-stu-id="9c291-129">\*.p7b</span></span> | <span data-ttu-id="9c291-130">\* .bin)。</span><span class="sxs-lookup"><span data-stu-id="9c291-130">\*.bin).</span></span>|
|<span data-ttu-id="9c291-131">value</span><span class="sxs-lookup"><span data-stu-id="9c291-131">value</span></span>|<span data-ttu-id="9c291-132">文字列</span><span class="sxs-lookup"><span data-stu-id="9c291-132">String</span></span>|<span data-ttu-id="9c291-133">値。</span><span class="sxs-lookup"><span data-stu-id="9c291-133">Value.</span></span> <span data-ttu-id="9c291-134">(Base64 エンコード文字列)</span><span class="sxs-lookup"><span data-stu-id="9c291-134">(Base64 encoded string)</span></span>|

## <a name="relationships"></a><span data-ttu-id="9c291-135">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="9c291-135">Relationships</span></span>
<span data-ttu-id="9c291-136">なし</span><span class="sxs-lookup"><span data-stu-id="9c291-136">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="9c291-137">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="9c291-137">JSON Representation</span></span>
<span data-ttu-id="9c291-138">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="9c291-138">Here is a JSON representation of the resource.</span></span>
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





