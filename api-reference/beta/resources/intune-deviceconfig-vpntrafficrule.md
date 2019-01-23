---
title: vpnTrafficRule リソースの種類
description: VPN トラフィックの規則の定義です。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 5b28d26356eea113f267c4eb0499f9600671f114
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29415286"
---
# <a name="vpntrafficrule-resource-type"></a><span data-ttu-id="29e21-103">vpnTrafficRule リソースの種類</span><span class="sxs-lookup"><span data-stu-id="29e21-103">vpnTrafficRule resource type</span></span>

> <span data-ttu-id="29e21-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="29e21-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="29e21-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="29e21-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="29e21-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="29e21-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="29e21-107">VPN トラフィックの規則の定義です。</span><span class="sxs-lookup"><span data-stu-id="29e21-107">VPN Traffic Rule definition.</span></span>

## <a name="properties"></a><span data-ttu-id="29e21-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="29e21-108">Properties</span></span>
|<span data-ttu-id="29e21-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="29e21-109">Property</span></span>|<span data-ttu-id="29e21-110">型</span><span class="sxs-lookup"><span data-stu-id="29e21-110">Type</span></span>|<span data-ttu-id="29e21-111">説明</span><span class="sxs-lookup"><span data-stu-id="29e21-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="29e21-112">name</span><span class="sxs-lookup"><span data-stu-id="29e21-112">name</span></span>|<span data-ttu-id="29e21-113">String</span><span class="sxs-lookup"><span data-stu-id="29e21-113">String</span></span>|<span data-ttu-id="29e21-114">名前です。</span><span class="sxs-lookup"><span data-stu-id="29e21-114">Name.</span></span>|
|<span data-ttu-id="29e21-115">プロトコル</span><span class="sxs-lookup"><span data-stu-id="29e21-115">protocols</span></span>|<span data-ttu-id="29e21-116">Int32</span><span class="sxs-lookup"><span data-stu-id="29e21-116">Int32</span></span>|<span data-ttu-id="29e21-117">(0 ~ 255) のプロトコル。</span><span class="sxs-lookup"><span data-stu-id="29e21-117">Protocols (0-255).</span></span> <span data-ttu-id="29e21-118">0 から 255 までの有効な値</span><span class="sxs-lookup"><span data-stu-id="29e21-118">Valid values 0 to 255</span></span>|
|<span data-ttu-id="29e21-119">localPortRanges</span><span class="sxs-lookup"><span data-stu-id="29e21-119">localPortRanges</span></span>|<span data-ttu-id="29e21-120">[numberRange](../resources/intune-deviceconfig-numberrange.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="29e21-120">[numberRange](../resources/intune-deviceconfig-numberrange.md) collection</span></span>|<span data-ttu-id="29e21-121">プロトコルが TCP または UDP 6 (17) である場合にのみ、ローカル ポートの範囲を設定できます。</span><span class="sxs-lookup"><span data-stu-id="29e21-121">Local port range can be set only when protocol is either TCP or UDP (6 or 17).</span></span> <span data-ttu-id="29e21-122">このコレクションには、最大で 500 個の要素を含めることができます。</span><span class="sxs-lookup"><span data-stu-id="29e21-122">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="29e21-123">remotePortRanges</span><span class="sxs-lookup"><span data-stu-id="29e21-123">remotePortRanges</span></span>|<span data-ttu-id="29e21-124">[numberRange](../resources/intune-deviceconfig-numberrange.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="29e21-124">[numberRange](../resources/intune-deviceconfig-numberrange.md) collection</span></span>|<span data-ttu-id="29e21-125">プロトコルが TCP または UDP 6 (17) である場合にのみ、リモート ポートの範囲を設定できます。</span><span class="sxs-lookup"><span data-stu-id="29e21-125">Remote port range can be set only when protocol is either TCP or UDP (6 or 17).</span></span> <span data-ttu-id="29e21-126">このコレクションには、最大で 500 個の要素を含めることができます。</span><span class="sxs-lookup"><span data-stu-id="29e21-126">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="29e21-127">localAddressRanges</span><span class="sxs-lookup"><span data-stu-id="29e21-127">localAddressRanges</span></span>|<span data-ttu-id="29e21-128">[iPv4Range](../resources/intune-shared-ipv4range.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="29e21-128">[iPv4Range](../resources/intune-shared-ipv4range.md) collection</span></span>|<span data-ttu-id="29e21-129">ローカル アドレスの範囲です。</span><span class="sxs-lookup"><span data-stu-id="29e21-129">Local address range.</span></span> <span data-ttu-id="29e21-130">このコレクションには、最大で 500 個の要素を含めることができます。</span><span class="sxs-lookup"><span data-stu-id="29e21-130">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="29e21-131">remoteAddressRanges</span><span class="sxs-lookup"><span data-stu-id="29e21-131">remoteAddressRanges</span></span>|<span data-ttu-id="29e21-132">[iPv4Range](../resources/intune-shared-ipv4range.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="29e21-132">[iPv4Range](../resources/intune-shared-ipv4range.md) collection</span></span>|<span data-ttu-id="29e21-133">リモート アドレスの範囲です。</span><span class="sxs-lookup"><span data-stu-id="29e21-133">Remote address range.</span></span> <span data-ttu-id="29e21-134">このコレクションには、最大で 500 個の要素を含めることができます。</span><span class="sxs-lookup"><span data-stu-id="29e21-134">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="29e21-135">appId</span><span class="sxs-lookup"><span data-stu-id="29e21-135">appId</span></span>|<span data-ttu-id="29e21-136">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="29e21-136">String</span></span>|<span data-ttu-id="29e21-137">アプリケーション識別子、アプリケーションでこのトラフィック ルールがトリガーされる場合です。</span><span class="sxs-lookup"><span data-stu-id="29e21-137">App identifier, if this traffic rule is triggered by an app.</span></span>|
|<span data-ttu-id="29e21-138">appType</span><span class="sxs-lookup"><span data-stu-id="29e21-138">appType</span></span>|[<span data-ttu-id="29e21-139">vpnTrafficRuleAppType</span><span class="sxs-lookup"><span data-stu-id="29e21-139">vpnTrafficRuleAppType</span></span>](../resources/intune-deviceconfig-vpntrafficruleapptype.md)|<span data-ttu-id="29e21-140">アプリケーションの種類、アプリケーションでこのトラフィック ルールがトリガーされる場合。</span><span class="sxs-lookup"><span data-stu-id="29e21-140">App type, if this traffic rule is triggered by an app.</span></span> <span data-ttu-id="29e21-141">可能な値は、`none`、`desktop`、`universal` です。</span><span class="sxs-lookup"><span data-stu-id="29e21-141">Possible values are: `none`, `desktop`, `universal`.</span></span>|
|<span data-ttu-id="29e21-142">routingPolicyType</span><span class="sxs-lookup"><span data-stu-id="29e21-142">routingPolicyType</span></span>|[<span data-ttu-id="29e21-143">vpnTrafficRuleRoutingPolicyType</span><span class="sxs-lookup"><span data-stu-id="29e21-143">vpnTrafficRuleRoutingPolicyType</span></span>](../resources/intune-deviceconfig-vpntrafficruleroutingpolicytype.md)|<span data-ttu-id="29e21-144">いつトリガーされると、アプリケーションでは、このルートの分割トンネリングを有効にするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="29e21-144">When app triggered, indicates whether to enable split tunneling along this route.</span></span> <span data-ttu-id="29e21-145">可能な値は、`none`、`splitTunnel`、`forceTunnel` です。</span><span class="sxs-lookup"><span data-stu-id="29e21-145">Possible values are: `none`, `splitTunnel`, `forceTunnel`.</span></span>|
|<span data-ttu-id="29e21-146">クレーム</span><span class="sxs-lookup"><span data-stu-id="29e21-146">claims</span></span>|<span data-ttu-id="29e21-147">String</span><span class="sxs-lookup"><span data-stu-id="29e21-147">String</span></span>|<span data-ttu-id="29e21-148">このトラフィックの規則に関連付けられている請求します。</span><span class="sxs-lookup"><span data-stu-id="29e21-148">Claims associated with this traffic rule.</span></span>|

## <a name="relationships"></a><span data-ttu-id="29e21-149">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="29e21-149">Relationships</span></span>
<span data-ttu-id="29e21-150">なし</span><span class="sxs-lookup"><span data-stu-id="29e21-150">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="29e21-151">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="29e21-151">JSON Representation</span></span>
<span data-ttu-id="29e21-152">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="29e21-152">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.vpnTrafficRule"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.vpnTrafficRule",
  "name": "String",
  "protocols": 1024,
  "localPortRanges": [
    {
      "@odata.type": "microsoft.graph.numberRange",
      "lowerNumber": 1024,
      "upperNumber": 1024
    }
  ],
  "remotePortRanges": [
    {
      "@odata.type": "microsoft.graph.numberRange",
      "lowerNumber": 1024,
      "upperNumber": 1024
    }
  ],
  "localAddressRanges": [
    {
      "@odata.type": "microsoft.graph.iPv4Range",
      "lowerAddress": "String",
      "upperAddress": "String"
    }
  ],
  "remoteAddressRanges": [
    {
      "@odata.type": "microsoft.graph.iPv4Range",
      "lowerAddress": "String",
      "upperAddress": "String"
    }
  ],
  "appId": "String",
  "appType": "String",
  "routingPolicyType": "String",
  "claims": "String"
}
```




