---
title: vpnTrafficRule リソースの種類
description: VPN トラフィックの規則の定義です。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 4b7a4a1841850c0276e50068b9e9c7d1ce69e765
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27840223"
---
# <a name="vpntrafficrule-resource-type"></a><span data-ttu-id="636f0-103">vpnTrafficRule リソースの種類</span><span class="sxs-lookup"><span data-stu-id="636f0-103">vpnTrafficRule resource type</span></span>

> <span data-ttu-id="636f0-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="636f0-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="636f0-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="636f0-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="636f0-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="636f0-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="636f0-107">VPN トラフィックの規則の定義です。</span><span class="sxs-lookup"><span data-stu-id="636f0-107">VPN Traffic Rule definition.</span></span>
## <a name="properties"></a><span data-ttu-id="636f0-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="636f0-108">Properties</span></span>
|<span data-ttu-id="636f0-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="636f0-109">Property</span></span>|<span data-ttu-id="636f0-110">種類</span><span class="sxs-lookup"><span data-stu-id="636f0-110">Type</span></span>|<span data-ttu-id="636f0-111">説明</span><span class="sxs-lookup"><span data-stu-id="636f0-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="636f0-112">名前</span><span class="sxs-lookup"><span data-stu-id="636f0-112">name</span></span>|<span data-ttu-id="636f0-113">String</span><span class="sxs-lookup"><span data-stu-id="636f0-113">String</span></span>|<span data-ttu-id="636f0-114">名前です。</span><span class="sxs-lookup"><span data-stu-id="636f0-114">Name.</span></span>|
|<span data-ttu-id="636f0-115">プロトコル</span><span class="sxs-lookup"><span data-stu-id="636f0-115">protocols</span></span>|<span data-ttu-id="636f0-116">Int32</span><span class="sxs-lookup"><span data-stu-id="636f0-116">Int32</span></span>|<span data-ttu-id="636f0-117">(0 ~ 255) のプロトコル。</span><span class="sxs-lookup"><span data-stu-id="636f0-117">Protocols (0-255).</span></span> <span data-ttu-id="636f0-118">0 から 255 までの有効な値</span><span class="sxs-lookup"><span data-stu-id="636f0-118">Valid values 0 to 255</span></span>|
|<span data-ttu-id="636f0-119">localPortRanges</span><span class="sxs-lookup"><span data-stu-id="636f0-119">localPortRanges</span></span>|<span data-ttu-id="636f0-120">[numberRange](../resources/intune-deviceconfig-numberrange.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="636f0-120">[numberRange](../resources/intune-deviceconfig-numberrange.md) collection</span></span>|<span data-ttu-id="636f0-121">プロトコルが TCP または UDP 6 (17) である場合にのみ、ローカル ポートの範囲を設定できます。</span><span class="sxs-lookup"><span data-stu-id="636f0-121">Local port range can be set only when protocol is either TCP or UDP (6 or 17).</span></span> <span data-ttu-id="636f0-122">このコレクションには、最大で 500 個の要素を含めることができます。</span><span class="sxs-lookup"><span data-stu-id="636f0-122">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="636f0-123">remotePortRanges</span><span class="sxs-lookup"><span data-stu-id="636f0-123">remotePortRanges</span></span>|<span data-ttu-id="636f0-124">[numberRange](../resources/intune-deviceconfig-numberrange.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="636f0-124">[numberRange](../resources/intune-deviceconfig-numberrange.md) collection</span></span>|<span data-ttu-id="636f0-125">プロトコルが TCP または UDP 6 (17) である場合にのみ、リモート ポートの範囲を設定できます。</span><span class="sxs-lookup"><span data-stu-id="636f0-125">Remote port range can be set only when protocol is either TCP or UDP (6 or 17).</span></span> <span data-ttu-id="636f0-126">このコレクションには、最大で 500 個の要素を含めることができます。</span><span class="sxs-lookup"><span data-stu-id="636f0-126">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="636f0-127">localAddressRanges</span><span class="sxs-lookup"><span data-stu-id="636f0-127">localAddressRanges</span></span>|<span data-ttu-id="636f0-128">[iPv4Range](../resources/intune-shared-ipv4range.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="636f0-128">[iPv4Range](../resources/intune-shared-ipv4range.md) collection</span></span>|<span data-ttu-id="636f0-129">ローカル アドレスの範囲です。</span><span class="sxs-lookup"><span data-stu-id="636f0-129">Local address range.</span></span> <span data-ttu-id="636f0-130">このコレクションには、最大で 500 個の要素を含めることができます。</span><span class="sxs-lookup"><span data-stu-id="636f0-130">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="636f0-131">remoteAddressRanges</span><span class="sxs-lookup"><span data-stu-id="636f0-131">remoteAddressRanges</span></span>|<span data-ttu-id="636f0-132">[iPv4Range](../resources/intune-shared-ipv4range.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="636f0-132">[iPv4Range](../resources/intune-shared-ipv4range.md) collection</span></span>|<span data-ttu-id="636f0-133">リモート アドレスの範囲です。</span><span class="sxs-lookup"><span data-stu-id="636f0-133">Remote address range.</span></span> <span data-ttu-id="636f0-134">このコレクションには、最大で 500 個の要素を含めることができます。</span><span class="sxs-lookup"><span data-stu-id="636f0-134">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="636f0-135">appId</span><span class="sxs-lookup"><span data-stu-id="636f0-135">appId</span></span>|<span data-ttu-id="636f0-136">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="636f0-136">String</span></span>|<span data-ttu-id="636f0-137">アプリケーション識別子、アプリケーションでこのトラフィック ルールがトリガーされる場合です。</span><span class="sxs-lookup"><span data-stu-id="636f0-137">App identifier, if this traffic rule is triggered by an app.</span></span>|
|<span data-ttu-id="636f0-138">appType</span><span class="sxs-lookup"><span data-stu-id="636f0-138">appType</span></span>|[<span data-ttu-id="636f0-139">vpnTrafficRuleAppType</span><span class="sxs-lookup"><span data-stu-id="636f0-139">vpnTrafficRuleAppType</span></span>](../resources/intune-deviceconfig-vpntrafficruleapptype.md)|<span data-ttu-id="636f0-140">アプリケーションの種類、アプリケーションでこのトラフィック ルールがトリガーされる場合。</span><span class="sxs-lookup"><span data-stu-id="636f0-140">App type, if this traffic rule is triggered by an app.</span></span> <span data-ttu-id="636f0-141">可能な値は、`none`、`desktop`、`universal` です。</span><span class="sxs-lookup"><span data-stu-id="636f0-141">Possible values are: `none`, `desktop`, `universal`.</span></span>|
|<span data-ttu-id="636f0-142">routingPolicyType</span><span class="sxs-lookup"><span data-stu-id="636f0-142">routingPolicyType</span></span>|[<span data-ttu-id="636f0-143">vpnTrafficRuleRoutingPolicyType</span><span class="sxs-lookup"><span data-stu-id="636f0-143">vpnTrafficRuleRoutingPolicyType</span></span>](../resources/intune-deviceconfig-vpntrafficruleroutingpolicytype.md)|<span data-ttu-id="636f0-144">いつトリガーされると、アプリケーションでは、このルートの分割トンネリングを有効にするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="636f0-144">When app triggered, indicates whether to enable split tunneling along this route.</span></span> <span data-ttu-id="636f0-145">可能な値は、`none`、`splitTunnel`、`forceTunnel` です。</span><span class="sxs-lookup"><span data-stu-id="636f0-145">Possible values are: `none`, `splitTunnel`, `forceTunnel`.</span></span>|
|<span data-ttu-id="636f0-146">クレーム</span><span class="sxs-lookup"><span data-stu-id="636f0-146">claims</span></span>|<span data-ttu-id="636f0-147">String</span><span class="sxs-lookup"><span data-stu-id="636f0-147">String</span></span>|<span data-ttu-id="636f0-148">このトラフィックの規則に関連付けられている請求します。</span><span class="sxs-lookup"><span data-stu-id="636f0-148">Claims associated with this traffic rule.</span></span>|

## <a name="relationships"></a><span data-ttu-id="636f0-149">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="636f0-149">Relationships</span></span>
<span data-ttu-id="636f0-150">なし</span><span class="sxs-lookup"><span data-stu-id="636f0-150">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="636f0-151">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="636f0-151">JSON Representation</span></span>
<span data-ttu-id="636f0-152">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="636f0-152">Here is a JSON representation of the resource.</span></span>
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





