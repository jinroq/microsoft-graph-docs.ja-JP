---
title: vpnTrafficRule リソースの種類
description: VPN トラフィックルールの定義。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: fd004341928260187518966e2356f59faff57898
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/21/2019
ms.locfileid: "30139943"
---
# <a name="vpntrafficrule-resource-type"></a><span data-ttu-id="7be01-103">vpnTrafficRule リソースの種類</span><span class="sxs-lookup"><span data-stu-id="7be01-103">vpnTrafficRule resource type</span></span>

> <span data-ttu-id="7be01-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="7be01-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7be01-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="7be01-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7be01-106">VPN トラフィックルールの定義。</span><span class="sxs-lookup"><span data-stu-id="7be01-106">VPN Traffic Rule definition.</span></span>

## <a name="properties"></a><span data-ttu-id="7be01-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="7be01-107">Properties</span></span>
|<span data-ttu-id="7be01-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="7be01-108">Property</span></span>|<span data-ttu-id="7be01-109">型</span><span class="sxs-lookup"><span data-stu-id="7be01-109">Type</span></span>|<span data-ttu-id="7be01-110">説明</span><span class="sxs-lookup"><span data-stu-id="7be01-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7be01-111">name</span><span class="sxs-lookup"><span data-stu-id="7be01-111">name</span></span>|<span data-ttu-id="7be01-112">String</span><span class="sxs-lookup"><span data-stu-id="7be01-112">String</span></span>|<span data-ttu-id="7be01-113">拡張子.</span><span class="sxs-lookup"><span data-stu-id="7be01-113">Name.</span></span>|
|<span data-ttu-id="7be01-114">プロトコル</span><span class="sxs-lookup"><span data-stu-id="7be01-114">protocols</span></span>|<span data-ttu-id="7be01-115">Int32</span><span class="sxs-lookup"><span data-stu-id="7be01-115">Int32</span></span>|<span data-ttu-id="7be01-116">プロトコル (0-255)。</span><span class="sxs-lookup"><span data-stu-id="7be01-116">Protocols (0-255).</span></span> <span data-ttu-id="7be01-117">有効な値は 0 ~ 255</span><span class="sxs-lookup"><span data-stu-id="7be01-117">Valid values 0 to 255</span></span>|
|<span data-ttu-id="7be01-118">localPortRanges</span><span class="sxs-lookup"><span data-stu-id="7be01-118">localPortRanges</span></span>|<span data-ttu-id="7be01-119">[numberRange](../resources/intune-deviceconfig-numberrange.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="7be01-119">[numberRange](../resources/intune-deviceconfig-numberrange.md) collection</span></span>|<span data-ttu-id="7be01-120">プロトコルが TCP または UDP (6 または 17) の場合にのみ、ローカルポート範囲を設定できます。</span><span class="sxs-lookup"><span data-stu-id="7be01-120">Local port range can be set only when protocol is either TCP or UDP (6 or 17).</span></span> <span data-ttu-id="7be01-121">このコレクションには、最大で 500 個の要素を含めることができます。</span><span class="sxs-lookup"><span data-stu-id="7be01-121">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="7be01-122">remotePortRanges</span><span class="sxs-lookup"><span data-stu-id="7be01-122">remotePortRanges</span></span>|<span data-ttu-id="7be01-123">[numberRange](../resources/intune-deviceconfig-numberrange.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="7be01-123">[numberRange](../resources/intune-deviceconfig-numberrange.md) collection</span></span>|<span data-ttu-id="7be01-124">プロトコルが TCP または UDP (6 または 17) の場合にのみ、リモートポート範囲を設定できます。</span><span class="sxs-lookup"><span data-stu-id="7be01-124">Remote port range can be set only when protocol is either TCP or UDP (6 or 17).</span></span> <span data-ttu-id="7be01-125">このコレクションには、最大で 500 個の要素を含めることができます。</span><span class="sxs-lookup"><span data-stu-id="7be01-125">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="7be01-126">localaddressranges</span><span class="sxs-lookup"><span data-stu-id="7be01-126">localAddressRanges</span></span>|<span data-ttu-id="7be01-127">[iPv4Range](../resources/intune-shared-ipv4range.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="7be01-127">[iPv4Range](../resources/intune-shared-ipv4range.md) collection</span></span>|<span data-ttu-id="7be01-128">ローカルアドレス範囲。</span><span class="sxs-lookup"><span data-stu-id="7be01-128">Local address range.</span></span> <span data-ttu-id="7be01-129">このコレクションには、最大で 500 個の要素を含めることができます。</span><span class="sxs-lookup"><span data-stu-id="7be01-129">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="7be01-130">remoteaddressranges</span><span class="sxs-lookup"><span data-stu-id="7be01-130">remoteAddressRanges</span></span>|<span data-ttu-id="7be01-131">[iPv4Range](../resources/intune-shared-ipv4range.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="7be01-131">[iPv4Range](../resources/intune-shared-ipv4range.md) collection</span></span>|<span data-ttu-id="7be01-132">リモートアドレス範囲。</span><span class="sxs-lookup"><span data-stu-id="7be01-132">Remote address range.</span></span> <span data-ttu-id="7be01-133">このコレクションには、最大で 500 個の要素を含めることができます。</span><span class="sxs-lookup"><span data-stu-id="7be01-133">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="7be01-134">appId</span><span class="sxs-lookup"><span data-stu-id="7be01-134">appId</span></span>|<span data-ttu-id="7be01-135">String</span><span class="sxs-lookup"><span data-stu-id="7be01-135">String</span></span>|<span data-ttu-id="7be01-136">アプリ識別子。このトラフィックルールがアプリによってトリガーされた場合。</span><span class="sxs-lookup"><span data-stu-id="7be01-136">App identifier, if this traffic rule is triggered by an app.</span></span>|
|<span data-ttu-id="7be01-137">appType</span><span class="sxs-lookup"><span data-stu-id="7be01-137">appType</span></span>|[<span data-ttu-id="7be01-138">vpnTrafficRuleAppType</span><span class="sxs-lookup"><span data-stu-id="7be01-138">vpnTrafficRuleAppType</span></span>](../resources/intune-deviceconfig-vpntrafficruleapptype.md)|<span data-ttu-id="7be01-139">アプリの種類。このトラフィックルールがアプリによってトリガーされた場合。</span><span class="sxs-lookup"><span data-stu-id="7be01-139">App type, if this traffic rule is triggered by an app.</span></span> <span data-ttu-id="7be01-140">可能な値は `none`、`desktop`、`universal` です。</span><span class="sxs-lookup"><span data-stu-id="7be01-140">Possible values are: `none`, `desktop`, `universal`.</span></span>|
|<span data-ttu-id="7be01-141">routingPolicyType</span><span class="sxs-lookup"><span data-stu-id="7be01-141">routingPolicyType</span></span>|[<span data-ttu-id="7be01-142">vpnTrafficRuleRoutingPolicyType</span><span class="sxs-lookup"><span data-stu-id="7be01-142">vpnTrafficRuleRoutingPolicyType</span></span>](../resources/intune-deviceconfig-vpntrafficruleroutingpolicytype.md)|<span data-ttu-id="7be01-143">アプリがトリガーされたときに、このルートに沿った分割トンネリングを有効にするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="7be01-143">When app triggered, indicates whether to enable split tunneling along this route.</span></span> <span data-ttu-id="7be01-144">可能な値は `none`、`splitTunnel`、`forceTunnel` です。</span><span class="sxs-lookup"><span data-stu-id="7be01-144">Possible values are: `none`, `splitTunnel`, `forceTunnel`.</span></span>|
|<span data-ttu-id="7be01-145">クレーム</span><span class="sxs-lookup"><span data-stu-id="7be01-145">claims</span></span>|<span data-ttu-id="7be01-146">String</span><span class="sxs-lookup"><span data-stu-id="7be01-146">String</span></span>|<span data-ttu-id="7be01-147">このトラフィック規則に関連付けられているクレーム。</span><span class="sxs-lookup"><span data-stu-id="7be01-147">Claims associated with this traffic rule.</span></span>|

## <a name="relationships"></a><span data-ttu-id="7be01-148">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="7be01-148">Relationships</span></span>
<span data-ttu-id="7be01-149">なし</span><span class="sxs-lookup"><span data-stu-id="7be01-149">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="7be01-150">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="7be01-150">JSON Representation</span></span>
<span data-ttu-id="7be01-151">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="7be01-151">Here is a JSON representation of the resource.</span></span>
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




