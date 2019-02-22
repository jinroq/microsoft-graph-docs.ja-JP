---
title: windowsNetworkIsolationPolicy リソースの種類
description: Windows ネットワーク分離ポリシー
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: e98d14d68ff5b936a9baf0a0065d0080f275a2ac
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/21/2019
ms.locfileid: "30158241"
---
# <a name="windowsnetworkisolationpolicy-resource-type"></a><span data-ttu-id="f7c08-103">windowsNetworkIsolationPolicy リソースの種類</span><span class="sxs-lookup"><span data-stu-id="f7c08-103">windowsNetworkIsolationPolicy resource type</span></span>

> <span data-ttu-id="f7c08-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f7c08-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f7c08-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="f7c08-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f7c08-106">Windows ネットワーク分離ポリシー</span><span class="sxs-lookup"><span data-stu-id="f7c08-106">Windows Network Isolation Policy</span></span>

## <a name="properties"></a><span data-ttu-id="f7c08-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="f7c08-107">Properties</span></span>
|<span data-ttu-id="f7c08-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="f7c08-108">Property</span></span>|<span data-ttu-id="f7c08-109">型</span><span class="sxs-lookup"><span data-stu-id="f7c08-109">Type</span></span>|<span data-ttu-id="f7c08-110">説明</span><span class="sxs-lookup"><span data-stu-id="f7c08-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f7c08-111">enterpriseNetworkDomainNames</span><span class="sxs-lookup"><span data-stu-id="f7c08-111">enterpriseNetworkDomainNames</span></span>|<span data-ttu-id="f7c08-112">String collection</span><span class="sxs-lookup"><span data-stu-id="f7c08-112">String collection</span></span>|<span data-ttu-id="f7c08-113">これは、エンタープライズの境界を構成するドメインのリストです。</span><span class="sxs-lookup"><span data-stu-id="f7c08-113">This is the list of domains that comprise the boundaries of the enterprise.</span></span> <span data-ttu-id="f7c08-114">デバイスに送信されるこれらのドメインのいずれかのデータは、エンタープライズデータとして保護されています。</span><span class="sxs-lookup"><span data-stu-id="f7c08-114">Data from one of these domains that is sent to a device will be considered enterprise data and protected.</span></span> <span data-ttu-id="f7c08-115">これらの場所は、エンタープライズデータの共有先として安全であると見なされます。</span><span class="sxs-lookup"><span data-stu-id="f7c08-115">These locations will be considered a safe destination for enterprise data to be shared to.</span></span>|
|<span data-ttu-id="f7c08-116">enterpriseCloudResources</span><span class="sxs-lookup"><span data-stu-id="f7c08-116">enterpriseCloudResources</span></span>|<span data-ttu-id="f7c08-117">[proxiedDomain](../resources/intune-shared-proxieddomain.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="f7c08-117">[proxiedDomain](../resources/intune-shared-proxieddomain.md) collection</span></span>|<span data-ttu-id="f7c08-118">クラウドでホストされている、保護する必要があるエンタープライズリソースドメインの一覧が含まれています。</span><span class="sxs-lookup"><span data-stu-id="f7c08-118">Contains a list of enterprise resource domains hosted in the cloud that need to be protected.</span></span> <span data-ttu-id="f7c08-119">これらのリソースへの接続は、エンタープライズ データと見なされます。</span><span class="sxs-lookup"><span data-stu-id="f7c08-119">Connections to these resources are considered enterprise data.</span></span> <span data-ttu-id="f7c08-120">プロキシがクラウド リソースとペアリング済みの場合、クラウド リソースへのトラフィックは、指定されたプロキシ サーバー (ポート 80) を介してエンタープライズ ネットワーク経由でルーティングされます。</span><span class="sxs-lookup"><span data-stu-id="f7c08-120">If a proxy is paired with a cloud resource, traffic to the cloud resource will be routed through the enterprise network via the denoted proxy server (on Port 80).</span></span> <span data-ttu-id="f7c08-121">この目的で使用されるプロキシサーバーも、enterpriseinternalproxyservers ポリシーを使用して構成する必要があります。</span><span class="sxs-lookup"><span data-stu-id="f7c08-121">A proxy server used for this purpose must also be configured using the EnterpriseInternalProxyServers policy.</span></span> <span data-ttu-id="f7c08-122">このコレクションには、最大で 500 個の要素を含めることができます。</span><span class="sxs-lookup"><span data-stu-id="f7c08-122">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="f7c08-123">enterpriseIPRanges</span><span class="sxs-lookup"><span data-stu-id="f7c08-123">enterpriseIPRanges</span></span>|<span data-ttu-id="f7c08-124">[ipRange](../resources/intune-shared-iprange.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="f7c08-124">[ipRange](../resources/intune-shared-iprange.md) collection</span></span>|<span data-ttu-id="f7c08-125">エンタープライズ ネットワーク内のコンピューターを定義するエンタープライズ IP の範囲を設定します。</span><span class="sxs-lookup"><span data-stu-id="f7c08-125">Sets the enterprise IP ranges that define the computers in the enterprise network.</span></span> <span data-ttu-id="f7c08-126">これらのコンピューターからのデータはエンタープライズの一部と見なされ、保護されます。</span><span class="sxs-lookup"><span data-stu-id="f7c08-126">Data that comes from those computers will be considered part of the enterprise and protected.</span></span> <span data-ttu-id="f7c08-127">これらの場所は、エンタープライズデータの共有先として安全であると見なされます。</span><span class="sxs-lookup"><span data-stu-id="f7c08-127">These locations will be considered a safe destination for enterprise data to be shared to.</span></span> <span data-ttu-id="f7c08-128">このコレクションには、最大で 500 個の要素を含めることができます。</span><span class="sxs-lookup"><span data-stu-id="f7c08-128">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="f7c08-129">enterpriseInternalProxyServers</span><span class="sxs-lookup"><span data-stu-id="f7c08-129">enterpriseInternalProxyServers</span></span>|<span data-ttu-id="f7c08-130">String collection</span><span class="sxs-lookup"><span data-stu-id="f7c08-130">String collection</span></span>|<span data-ttu-id="f7c08-131">これは、内部プロキシ サーバーのコンマ区切りのリストです。</span><span class="sxs-lookup"><span data-stu-id="f7c08-131">This is the comma-separated list of internal proxy servers.</span></span> <span data-ttu-id="f7c08-132">例: "157.54.14.28, 157.54.11.118, 10.202.14.167, 157.53.14.163, 157.69.210.59"。</span><span class="sxs-lookup"><span data-stu-id="f7c08-132">For example, "157.54.14.28, 157.54.11.118, 10.202.14.167, 157.53.14.163, 157.69.210.59".</span></span> <span data-ttu-id="f7c08-133">これらのプロキシは、管理者により、インターネット上の特定のリソースに接続するように構成されています。</span><span class="sxs-lookup"><span data-stu-id="f7c08-133">These proxies have been configured by the admin to connect to specific resources on the Internet.</span></span> <span data-ttu-id="f7c08-134">それらはエンタープライズ ネットワークの場所にあると見なされます。</span><span class="sxs-lookup"><span data-stu-id="f7c08-134">They are considered to be enterprise network locations.</span></span> <span data-ttu-id="f7c08-135">プロキシは、EnterpriseCloudResources ポリシーを構成する場合にのみ使用され、これらのプロキシを介して一致するクラウドリソースにトラフィックを強制します。</span><span class="sxs-lookup"><span data-stu-id="f7c08-135">The proxies are only leveraged in configuring the EnterpriseCloudResources policy to force traffic to the matched cloud resources through these proxies.</span></span>|
|<span data-ttu-id="f7c08-136">enterpriseIPRangesAreAuthoritative</span><span class="sxs-lookup"><span data-stu-id="f7c08-136">enterpriseIPRangesAreAuthoritative</span></span>|<span data-ttu-id="f7c08-137">Boolean</span><span class="sxs-lookup"><span data-stu-id="f7c08-137">Boolean</span></span>|<span data-ttu-id="f7c08-138">構成済みのリストを承諾し、ヒューリスティックを使用した他のサブネットの検索を行わないよう、クライアントに指示するブール値。</span><span class="sxs-lookup"><span data-stu-id="f7c08-138">Boolean value that tells the client to accept the configured list and not to use heuristics to attempt to find other subnets.</span></span> <span data-ttu-id="f7c08-139">既定値は false です。</span><span class="sxs-lookup"><span data-stu-id="f7c08-139">Default is false.</span></span>|
|<span data-ttu-id="f7c08-140">enterpriseProxyServers</span><span class="sxs-lookup"><span data-stu-id="f7c08-140">enterpriseProxyServers</span></span>|<span data-ttu-id="f7c08-141">String collection</span><span class="sxs-lookup"><span data-stu-id="f7c08-141">String collection</span></span>|<span data-ttu-id="f7c08-142">これは、プロキシ サーバーのリストです。</span><span class="sxs-lookup"><span data-stu-id="f7c08-142">This is a list of proxy servers.</span></span> <span data-ttu-id="f7c08-143">この一覧にないサーバーは、非エンタープライズとみなされます。</span><span class="sxs-lookup"><span data-stu-id="f7c08-143">Any server not on this list is considered non-enterprise.</span></span>|
|<span data-ttu-id="f7c08-144">enterpriseProxyServersAreAuthoritative</span><span class="sxs-lookup"><span data-stu-id="f7c08-144">enterpriseProxyServersAreAuthoritative</span></span>|<span data-ttu-id="f7c08-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="f7c08-145">Boolean</span></span>|<span data-ttu-id="f7c08-146">プロキシの構成済みリストを承諾し、他の作業プロキシの検出を試みないよう、クライアントに指示するブール値。</span><span class="sxs-lookup"><span data-stu-id="f7c08-146">Boolean value that tells the client to accept the configured list of proxies and not try to detect other work proxies.</span></span> <span data-ttu-id="f7c08-147">既定値は false です</span><span class="sxs-lookup"><span data-stu-id="f7c08-147">Default is false</span></span>|
|<span data-ttu-id="f7c08-148">neutralDomainResources</span><span class="sxs-lookup"><span data-stu-id="f7c08-148">neutralDomainResources</span></span>|<span data-ttu-id="f7c08-149">String collection</span><span class="sxs-lookup"><span data-stu-id="f7c08-149">String collection</span></span>|<span data-ttu-id="f7c08-150">作業または個人のリソースに使用できるドメイン名のリスト。</span><span class="sxs-lookup"><span data-stu-id="f7c08-150">List of domain names that can used for work or personal resource.</span></span>|

## <a name="relationships"></a><span data-ttu-id="f7c08-151">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="f7c08-151">Relationships</span></span>
<span data-ttu-id="f7c08-152">なし</span><span class="sxs-lookup"><span data-stu-id="f7c08-152">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="f7c08-153">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="f7c08-153">JSON Representation</span></span>
<span data-ttu-id="f7c08-154">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="f7c08-154">Here is a JSON representation of the resource.</span></span>
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




