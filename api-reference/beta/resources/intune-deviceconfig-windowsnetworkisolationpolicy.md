---
title: windowsNetworkIsolationPolicy リソースの種類
description: Windows ネットワークの分離のポリシー
ms.openlocfilehash: 89c7db0453c76f6ec5016a4701bf357e27c579bc
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27069949"
---
# <a name="windowsnetworkisolationpolicy-resource-type"></a><span data-ttu-id="0a008-103">windowsNetworkIsolationPolicy リソースの種類</span><span class="sxs-lookup"><span data-stu-id="0a008-103">windowsNetworkIsolationPolicy resource type</span></span>

> <span data-ttu-id="0a008-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="0a008-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="0a008-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="0a008-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="0a008-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="0a008-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="0a008-107">Windows ネットワークの分離のポリシー</span><span class="sxs-lookup"><span data-stu-id="0a008-107">Windows Network Isolation Policy</span></span>
## <a name="properties"></a><span data-ttu-id="0a008-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="0a008-108">Properties</span></span>
|<span data-ttu-id="0a008-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="0a008-109">Property</span></span>|<span data-ttu-id="0a008-110">型</span><span class="sxs-lookup"><span data-stu-id="0a008-110">Type</span></span>|<span data-ttu-id="0a008-111">説明</span><span class="sxs-lookup"><span data-stu-id="0a008-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0a008-112">enterpriseNetworkDomainNames</span><span class="sxs-lookup"><span data-stu-id="0a008-112">enterpriseNetworkDomainNames</span></span>|<span data-ttu-id="0a008-113">String コレクション</span><span class="sxs-lookup"><span data-stu-id="0a008-113">String collection</span></span>|<span data-ttu-id="0a008-114">これは、エンタープライズの境界を構成するドメインのリストです。</span><span class="sxs-lookup"><span data-stu-id="0a008-114">This is the list of domains that comprise the boundaries of the enterprise.</span></span> <span data-ttu-id="0a008-115">デバイスに送信されるこれらのドメインの 1 つのデータはエンタープライズ データと見なされ、保護します。</span><span class="sxs-lookup"><span data-stu-id="0a008-115">Data from one of these domains that is sent to a device will be considered enterprise data and protected.</span></span> <span data-ttu-id="0a008-116">これらの場所は安全なエンタープライズ ・ データを共有する先と見なされます。</span><span class="sxs-lookup"><span data-stu-id="0a008-116">These locations will be considered a safe destination for enterprise data to be shared to.</span></span>|
|<span data-ttu-id="0a008-117">enterpriseCloudResources</span><span class="sxs-lookup"><span data-stu-id="0a008-117">enterpriseCloudResources</span></span>|<span data-ttu-id="0a008-118">[proxiedDomain](../resources/intune-shared-proxieddomain.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="0a008-118">[proxiedDomain](../resources/intune-shared-proxieddomain.md) collection</span></span>|<span data-ttu-id="0a008-119">保護する必要のあるクラウドでホストされているエンタープライズ リソースのドメインの一覧が含まれています。</span><span class="sxs-lookup"><span data-stu-id="0a008-119">Contains a list of enterprise resource domains hosted in the cloud that need to be protected.</span></span> <span data-ttu-id="0a008-120">これらのリソースへの接続は、エンタープライズ データと見なされます。</span><span class="sxs-lookup"><span data-stu-id="0a008-120">Connections to these resources are considered enterprise data.</span></span> <span data-ttu-id="0a008-121">プロキシがクラウド リソースとペアリング済みの場合、クラウド リソースへのトラフィックは、指定されたプロキシ サーバー (ポート 80) を介してエンタープライズ ネットワーク経由でルーティングされます。</span><span class="sxs-lookup"><span data-stu-id="0a008-121">If a proxy is paired with a cloud resource, traffic to the cloud resource will be routed through the enterprise network via the denoted proxy server (on Port 80).</span></span> <span data-ttu-id="0a008-122">EnterpriseInternalProxyServers ポリシーを使用してこの目的に使用されるプロキシ サーバーを構成することもする必要があります。</span><span class="sxs-lookup"><span data-stu-id="0a008-122">A proxy server used for this purpose must also be configured using the EnterpriseInternalProxyServers policy.</span></span> <span data-ttu-id="0a008-123">このコレクションには、最大で 500 個の要素を含めることができます。</span><span class="sxs-lookup"><span data-stu-id="0a008-123">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="0a008-124">enterpriseIPRanges</span><span class="sxs-lookup"><span data-stu-id="0a008-124">enterpriseIPRanges</span></span>|<span data-ttu-id="0a008-125">[ipRange](../resources/intune-shared-iprange.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="0a008-125">[ipRange](../resources/intune-shared-iprange.md) collection</span></span>|<span data-ttu-id="0a008-126">エンタープライズ ネットワーク内のコンピューターを定義するエンタープライズ IP の範囲を設定します。</span><span class="sxs-lookup"><span data-stu-id="0a008-126">Sets the enterprise IP ranges that define the computers in the enterprise network.</span></span> <span data-ttu-id="0a008-127">これらのコンピューターからのデータはエンタープライズの一部と見なされ、保護されます。</span><span class="sxs-lookup"><span data-stu-id="0a008-127">Data that comes from those computers will be considered part of the enterprise and protected.</span></span> <span data-ttu-id="0a008-128">これらの場所は安全なエンタープライズ ・ データを共有する先と見なされます。</span><span class="sxs-lookup"><span data-stu-id="0a008-128">These locations will be considered a safe destination for enterprise data to be shared to.</span></span> <span data-ttu-id="0a008-129">このコレクションには、最大で 500 個の要素を含めることができます。</span><span class="sxs-lookup"><span data-stu-id="0a008-129">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="0a008-130">enterpriseInternalProxyServers</span><span class="sxs-lookup"><span data-stu-id="0a008-130">enterpriseInternalProxyServers</span></span>|<span data-ttu-id="0a008-131">String コレクション</span><span class="sxs-lookup"><span data-stu-id="0a008-131">String collection</span></span>|<span data-ttu-id="0a008-132">これは、内部プロキシ サーバーのコンマ区切りのリストです。</span><span class="sxs-lookup"><span data-stu-id="0a008-132">This is the comma-separated list of internal proxy servers.</span></span> <span data-ttu-id="0a008-133">例: "157.54.14.28, 157.54.11.118, 10.202.14.167, 157.53.14.163, 157.69.210.59"。</span><span class="sxs-lookup"><span data-stu-id="0a008-133">For example, "157.54.14.28, 157.54.11.118, 10.202.14.167, 157.53.14.163, 157.69.210.59".</span></span> <span data-ttu-id="0a008-134">これらのプロキシは、管理者により、インターネット上の特定のリソースに接続するように構成されています。</span><span class="sxs-lookup"><span data-stu-id="0a008-134">These proxies have been configured by the admin to connect to specific resources on the Internet.</span></span> <span data-ttu-id="0a008-135">それらはエンタープライズ ネットワークの場所にあると見なされます。</span><span class="sxs-lookup"><span data-stu-id="0a008-135">They are considered to be enterprise network locations.</span></span> <span data-ttu-id="0a008-136">プロキシは、一致したクラウド リソースのこれらのプロキシを経由するトラフィックを強制的に EnterpriseCloudResources のポリシーを構成する際に活用できるのみ。</span><span class="sxs-lookup"><span data-stu-id="0a008-136">The proxies are only leveraged in configuring the EnterpriseCloudResources policy to force traffic to the matched cloud resources through these proxies.</span></span>|
|<span data-ttu-id="0a008-137">enterpriseIPRangesAreAuthoritative</span><span class="sxs-lookup"><span data-stu-id="0a008-137">enterpriseIPRangesAreAuthoritative</span></span>|<span data-ttu-id="0a008-138">Boolean</span><span class="sxs-lookup"><span data-stu-id="0a008-138">Boolean</span></span>|<span data-ttu-id="0a008-139">構成済みのリストを承諾し、ヒューリスティックを使用した他のサブネットの検索を行わないよう、クライアントに指示するブール値。</span><span class="sxs-lookup"><span data-stu-id="0a008-139">Boolean value that tells the client to accept the configured list and not to use heuristics to attempt to find other subnets.</span></span> <span data-ttu-id="0a008-140">既定では false を指定します。</span><span class="sxs-lookup"><span data-stu-id="0a008-140">Default is false.</span></span>|
|<span data-ttu-id="0a008-141">enterpriseProxyServers</span><span class="sxs-lookup"><span data-stu-id="0a008-141">enterpriseProxyServers</span></span>|<span data-ttu-id="0a008-142">String コレクション</span><span class="sxs-lookup"><span data-stu-id="0a008-142">String collection</span></span>|<span data-ttu-id="0a008-143">これは、プロキシ サーバーのリストです。</span><span class="sxs-lookup"><span data-stu-id="0a008-143">This is a list of proxy servers.</span></span> <span data-ttu-id="0a008-144">任意のサーバー一覧とは見なされません非エンタープライズです。</span><span class="sxs-lookup"><span data-stu-id="0a008-144">Any server not on this list is considered non-enterprise.</span></span>|
|<span data-ttu-id="0a008-145">enterpriseProxyServersAreAuthoritative</span><span class="sxs-lookup"><span data-stu-id="0a008-145">enterpriseProxyServersAreAuthoritative</span></span>|<span data-ttu-id="0a008-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="0a008-146">Boolean</span></span>|<span data-ttu-id="0a008-147">プロキシの構成済みリストを承諾し、他の作業プロキシの検出を試みないよう、クライアントに指示するブール値。</span><span class="sxs-lookup"><span data-stu-id="0a008-147">Boolean value that tells the client to accept the configured list of proxies and not try to detect other work proxies.</span></span> <span data-ttu-id="0a008-148">既定値は false です</span><span class="sxs-lookup"><span data-stu-id="0a008-148">Default is false</span></span>|
|<span data-ttu-id="0a008-149">neutralDomainResources</span><span class="sxs-lookup"><span data-stu-id="0a008-149">neutralDomainResources</span></span>|<span data-ttu-id="0a008-150">String コレクション</span><span class="sxs-lookup"><span data-stu-id="0a008-150">String collection</span></span>|<span data-ttu-id="0a008-151">作業時間またはリソースの個人に使用できるドメイン名のリストです。</span><span class="sxs-lookup"><span data-stu-id="0a008-151">List of domain names that can used for work or personal resource.</span></span>|

## <a name="relationships"></a><span data-ttu-id="0a008-152">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="0a008-152">Relationships</span></span>
<span data-ttu-id="0a008-153">なし</span><span class="sxs-lookup"><span data-stu-id="0a008-153">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="0a008-154">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="0a008-154">JSON Representation</span></span>
<span data-ttu-id="0a008-155">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="0a008-155">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsNetworkIsolationPolicy"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsNetworkIsolationPolicy",
  "enterpriseNetworkDomainNames": [
    "String"
  ],
  "enterpriseCloudResources": [
    {
      "@odata.type": "microsoft.graph.proxiedDomain",
      "ipAddressOrFQDN": "String",
      "proxy": "String"
    }
  ],
  "enterpriseIPRanges": [
    {
      "@odata.type": "microsoft.graph.iPv6Range",
      "lowerAddress": "String",
      "upperAddress": "String"
    }
  ],
  "enterpriseInternalProxyServers": [
    "String"
  ],
  "enterpriseIPRangesAreAuthoritative": true,
  "enterpriseProxyServers": [
    "String"
  ],
  "enterpriseProxyServersAreAuthoritative": true,
  "neutralDomainResources": [
    "String"
  ]
}
```





