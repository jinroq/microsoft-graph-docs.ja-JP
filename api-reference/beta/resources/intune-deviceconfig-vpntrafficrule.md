---
title: vpnTrafficRule リソースの種類
description: VPN トラフィックルールの定義。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 21f174056021e9a9789a2c033383c42ba8f09cc3
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/11/2019
ms.locfileid: "33944559"
---
# <a name="vpntrafficrule-resource-type"></a><span data-ttu-id="22236-103">vpnTrafficRule リソースの種類</span><span class="sxs-lookup"><span data-stu-id="22236-103">vpnTrafficRule resource type</span></span>

> <span data-ttu-id="22236-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="22236-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="22236-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="22236-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="22236-106">VPN トラフィックルールの定義。</span><span class="sxs-lookup"><span data-stu-id="22236-106">VPN Traffic Rule definition.</span></span>

## <a name="properties"></a><span data-ttu-id="22236-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="22236-107">Properties</span></span>
|<span data-ttu-id="22236-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="22236-108">Property</span></span>|<span data-ttu-id="22236-109">型</span><span class="sxs-lookup"><span data-stu-id="22236-109">Type</span></span>|<span data-ttu-id="22236-110">説明</span><span class="sxs-lookup"><span data-stu-id="22236-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="22236-111">name</span><span class="sxs-lookup"><span data-stu-id="22236-111">name</span></span>|<span data-ttu-id="22236-112">String</span><span class="sxs-lookup"><span data-stu-id="22236-112">String</span></span>|<span data-ttu-id="22236-113">拡張子.</span><span class="sxs-lookup"><span data-stu-id="22236-113">Name.</span></span>|
|<span data-ttu-id="22236-114">プロトコル</span><span class="sxs-lookup"><span data-stu-id="22236-114">protocols</span></span>|<span data-ttu-id="22236-115">Int32</span><span class="sxs-lookup"><span data-stu-id="22236-115">Int32</span></span>|<span data-ttu-id="22236-116">プロトコル (0-255)。</span><span class="sxs-lookup"><span data-stu-id="22236-116">Protocols (0-255).</span></span> <span data-ttu-id="22236-117">有効な値は 0 ~ 255</span><span class="sxs-lookup"><span data-stu-id="22236-117">Valid values 0 to 255</span></span>|
|<span data-ttu-id="22236-118">localPortRanges</span><span class="sxs-lookup"><span data-stu-id="22236-118">localPortRanges</span></span>|<span data-ttu-id="22236-119">[numberRange](../resources/intune-deviceconfig-numberrange.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="22236-119">[numberRange](../resources/intune-deviceconfig-numberrange.md) collection</span></span>|<span data-ttu-id="22236-120">プロトコルが TCP または UDP (6 または 17) の場合にのみ、ローカルポート範囲を設定できます。</span><span class="sxs-lookup"><span data-stu-id="22236-120">Local port range can be set only when protocol is either TCP or UDP (6 or 17).</span></span> <span data-ttu-id="22236-121">このコレクションには、最大で 500 個の要素を含めることができます。</span><span class="sxs-lookup"><span data-stu-id="22236-121">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="22236-122">remotePortRanges</span><span class="sxs-lookup"><span data-stu-id="22236-122">remotePortRanges</span></span>|<span data-ttu-id="22236-123">[numberRange](../resources/intune-deviceconfig-numberrange.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="22236-123">[numberRange](../resources/intune-deviceconfig-numberrange.md) collection</span></span>|<span data-ttu-id="22236-124">プロトコルが TCP または UDP (6 または 17) の場合にのみ、リモートポート範囲を設定できます。</span><span class="sxs-lookup"><span data-stu-id="22236-124">Remote port range can be set only when protocol is either TCP or UDP (6 or 17).</span></span> <span data-ttu-id="22236-125">このコレクションには、最大で 500 個の要素を含めることができます。</span><span class="sxs-lookup"><span data-stu-id="22236-125">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="22236-126">localAddressRanges</span><span class="sxs-lookup"><span data-stu-id="22236-126">localAddressRanges</span></span>|<span data-ttu-id="22236-127">[iPv4Range](../resources/intune-shared-ipv4range.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="22236-127">[iPv4Range](../resources/intune-shared-ipv4range.md) collection</span></span>|<span data-ttu-id="22236-128">ローカルアドレス範囲。</span><span class="sxs-lookup"><span data-stu-id="22236-128">Local address range.</span></span> <span data-ttu-id="22236-129">このコレクションには、最大で 500 個の要素を含めることができます。</span><span class="sxs-lookup"><span data-stu-id="22236-129">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="22236-130">remoteAddressRanges</span><span class="sxs-lookup"><span data-stu-id="22236-130">remoteAddressRanges</span></span>|<span data-ttu-id="22236-131">[iPv4Range](../resources/intune-shared-ipv4range.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="22236-131">[iPv4Range](../resources/intune-shared-ipv4range.md) collection</span></span>|<span data-ttu-id="22236-132">リモートアドレス範囲。</span><span class="sxs-lookup"><span data-stu-id="22236-132">Remote address range.</span></span> <span data-ttu-id="22236-133">このコレクションには、最大で 500 個の要素を含めることができます。</span><span class="sxs-lookup"><span data-stu-id="22236-133">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="22236-134">appId</span><span class="sxs-lookup"><span data-stu-id="22236-134">appId</span></span>|<span data-ttu-id="22236-135">String</span><span class="sxs-lookup"><span data-stu-id="22236-135">String</span></span>|<span data-ttu-id="22236-136">アプリ識別子。このトラフィックルールがアプリによってトリガーされた場合。</span><span class="sxs-lookup"><span data-stu-id="22236-136">App identifier, if this traffic rule is triggered by an app.</span></span>|
|<span data-ttu-id="22236-137">appType</span><span class="sxs-lookup"><span data-stu-id="22236-137">appType</span></span>|[<span data-ttu-id="22236-138">vpnTrafficRuleAppType</span><span class="sxs-lookup"><span data-stu-id="22236-138">vpnTrafficRuleAppType</span></span>](../resources/intune-deviceconfig-vpntrafficruleapptype.md)|<span data-ttu-id="22236-139">アプリの種類。このトラフィックルールがアプリによってトリガーされた場合。</span><span class="sxs-lookup"><span data-stu-id="22236-139">App type, if this traffic rule is triggered by an app.</span></span> <span data-ttu-id="22236-140">可能な値は、`none`、`desktop`、`universal` です。</span><span class="sxs-lookup"><span data-stu-id="22236-140">Possible values are: `none`, `desktop`, `universal`.</span></span>|
|<span data-ttu-id="22236-141">routingPolicyType</span><span class="sxs-lookup"><span data-stu-id="22236-141">routingPolicyType</span></span>|[<span data-ttu-id="22236-142">vpnTrafficRuleRoutingPolicyType</span><span class="sxs-lookup"><span data-stu-id="22236-142">vpnTrafficRuleRoutingPolicyType</span></span>](../resources/intune-deviceconfig-vpntrafficruleroutingpolicytype.md)|<span data-ttu-id="22236-143">アプリがトリガーされたときに、このルートに沿った分割トンネリングを有効にするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="22236-143">When app triggered, indicates whether to enable split tunneling along this route.</span></span> <span data-ttu-id="22236-144">可能な値は、`none`、`splitTunnel`、`forceTunnel` です。</span><span class="sxs-lookup"><span data-stu-id="22236-144">Possible values are: `none`, `splitTunnel`, `forceTunnel`.</span></span>|
|<span data-ttu-id="22236-145">差出人</span><span class="sxs-lookup"><span data-stu-id="22236-145">claims</span></span>|<span data-ttu-id="22236-146">String</span><span class="sxs-lookup"><span data-stu-id="22236-146">String</span></span>|<span data-ttu-id="22236-147">このトラフィック規則に関連付けられているクレーム。</span><span class="sxs-lookup"><span data-stu-id="22236-147">Claims associated with this traffic rule.</span></span>|

## <a name="relationships"></a><span data-ttu-id="22236-148">関係</span><span class="sxs-lookup"><span data-stu-id="22236-148">Relationships</span></span>
<span data-ttu-id="22236-149">なし</span><span class="sxs-lookup"><span data-stu-id="22236-149">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="22236-150">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="22236-150">JSON Representation</span></span>
<span data-ttu-id="22236-151">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="22236-151">Here is a JSON representation of the resource.</span></span>
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




