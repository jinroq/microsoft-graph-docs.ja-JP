---
title: windowsNetworkIsolationPolicy リソースの種類
description: Windows ネットワークの分離のポリシー
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 5bb427d519cf1f981997b70242095af22bf705df
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27940163"
---
# <a name="windowsnetworkisolationpolicy-resource-type"></a><span data-ttu-id="13d36-103">windowsNetworkIsolationPolicy リソースの種類</span><span class="sxs-lookup"><span data-stu-id="13d36-103">windowsNetworkIsolationPolicy resource type</span></span>

> <span data-ttu-id="13d36-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="13d36-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="13d36-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="13d36-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="13d36-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="13d36-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="13d36-107">Windows ネットワークの分離のポリシー</span><span class="sxs-lookup"><span data-stu-id="13d36-107">Windows Network Isolation Policy</span></span>
## <a name="properties"></a><span data-ttu-id="13d36-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="13d36-108">Properties</span></span>
|<span data-ttu-id="13d36-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="13d36-109">Property</span></span>|<span data-ttu-id="13d36-110">種類</span><span class="sxs-lookup"><span data-stu-id="13d36-110">Type</span></span>|<span data-ttu-id="13d36-111">説明</span><span class="sxs-lookup"><span data-stu-id="13d36-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="13d36-112">enterpriseNetworkDomainNames</span><span class="sxs-lookup"><span data-stu-id="13d36-112">enterpriseNetworkDomainNames</span></span>|<span data-ttu-id="13d36-113">String コレクション</span><span class="sxs-lookup"><span data-stu-id="13d36-113">String collection</span></span>|<span data-ttu-id="13d36-114">これは、エンタープライズの境界を構成するドメインのリストです。</span><span class="sxs-lookup"><span data-stu-id="13d36-114">This is the list of domains that comprise the boundaries of the enterprise.</span></span> <span data-ttu-id="13d36-115">デバイスに送信されるこれらのドメインの 1 つのデータはエンタープライズ データと見なされ、保護します。</span><span class="sxs-lookup"><span data-stu-id="13d36-115">Data from one of these domains that is sent to a device will be considered enterprise data and protected.</span></span> <span data-ttu-id="13d36-116">これらの場所は安全なエンタープライズ ・ データを共有する先と見なされます。</span><span class="sxs-lookup"><span data-stu-id="13d36-116">These locations will be considered a safe destination for enterprise data to be shared to.</span></span>|
|<span data-ttu-id="13d36-117">enterpriseCloudResources</span><span class="sxs-lookup"><span data-stu-id="13d36-117">enterpriseCloudResources</span></span>|<span data-ttu-id="13d36-118">[proxiedDomain](../resources/intune-shared-proxieddomain.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="13d36-118">[proxiedDomain](../resources/intune-shared-proxieddomain.md) collection</span></span>|<span data-ttu-id="13d36-119">保護する必要のあるクラウドでホストされているエンタープライズ リソースのドメインの一覧が含まれています。</span><span class="sxs-lookup"><span data-stu-id="13d36-119">Contains a list of enterprise resource domains hosted in the cloud that need to be protected.</span></span> <span data-ttu-id="13d36-120">これらのリソースへの接続は、エンタープライズ データと見なされます。</span><span class="sxs-lookup"><span data-stu-id="13d36-120">Connections to these resources are considered enterprise data.</span></span> <span data-ttu-id="13d36-121">プロキシがクラウド リソースとペアリング済みの場合、クラウド リソースへのトラフィックは、指定されたプロキシ サーバー (ポート 80) を介してエンタープライズ ネットワーク経由でルーティングされます。</span><span class="sxs-lookup"><span data-stu-id="13d36-121">If a proxy is paired with a cloud resource, traffic to the cloud resource will be routed through the enterprise network via the denoted proxy server (on Port 80).</span></span> <span data-ttu-id="13d36-122">EnterpriseInternalProxyServers ポリシーを使用してこの目的に使用されるプロキシ サーバーを構成することもする必要があります。</span><span class="sxs-lookup"><span data-stu-id="13d36-122">A proxy server used for this purpose must also be configured using the EnterpriseInternalProxyServers policy.</span></span> <span data-ttu-id="13d36-123">このコレクションには、最大で 500 個の要素を含めることができます。</span><span class="sxs-lookup"><span data-stu-id="13d36-123">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="13d36-124">enterpriseIPRanges</span><span class="sxs-lookup"><span data-stu-id="13d36-124">enterpriseIPRanges</span></span>|<span data-ttu-id="13d36-125">[ipRange](../resources/intune-shared-iprange.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="13d36-125">[ipRange](../resources/intune-shared-iprange.md) collection</span></span>|<span data-ttu-id="13d36-126">エンタープライズ ネットワーク内のコンピューターを定義するエンタープライズ IP の範囲を設定します。</span><span class="sxs-lookup"><span data-stu-id="13d36-126">Sets the enterprise IP ranges that define the computers in the enterprise network.</span></span> <span data-ttu-id="13d36-127">これらのコンピューターからのデータはエンタープライズの一部と見なされ、保護されます。</span><span class="sxs-lookup"><span data-stu-id="13d36-127">Data that comes from those computers will be considered part of the enterprise and protected.</span></span> <span data-ttu-id="13d36-128">これらの場所は安全なエンタープライズ ・ データを共有する先と見なされます。</span><span class="sxs-lookup"><span data-stu-id="13d36-128">These locations will be considered a safe destination for enterprise data to be shared to.</span></span> <span data-ttu-id="13d36-129">このコレクションには、最大で 500 個の要素を含めることができます。</span><span class="sxs-lookup"><span data-stu-id="13d36-129">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="13d36-130">enterpriseInternalProxyServers</span><span class="sxs-lookup"><span data-stu-id="13d36-130">enterpriseInternalProxyServers</span></span>|<span data-ttu-id="13d36-131">String コレクション</span><span class="sxs-lookup"><span data-stu-id="13d36-131">String collection</span></span>|<span data-ttu-id="13d36-132">これは、内部プロキシ サーバーのコンマ区切りのリストです。</span><span class="sxs-lookup"><span data-stu-id="13d36-132">This is the comma-separated list of internal proxy servers.</span></span> <span data-ttu-id="13d36-133">例: "157.54.14.28, 157.54.11.118, 10.202.14.167, 157.53.14.163, 157.69.210.59"。</span><span class="sxs-lookup"><span data-stu-id="13d36-133">For example, "157.54.14.28, 157.54.11.118, 10.202.14.167, 157.53.14.163, 157.69.210.59".</span></span> <span data-ttu-id="13d36-134">これらのプロキシは、管理者により、インターネット上の特定のリソースに接続するように構成されています。</span><span class="sxs-lookup"><span data-stu-id="13d36-134">These proxies have been configured by the admin to connect to specific resources on the Internet.</span></span> <span data-ttu-id="13d36-135">それらはエンタープライズ ネットワークの場所にあると見なされます。</span><span class="sxs-lookup"><span data-stu-id="13d36-135">They are considered to be enterprise network locations.</span></span> <span data-ttu-id="13d36-136">プロキシは、一致したクラウド リソースのこれらのプロキシを経由するトラフィックを強制的に EnterpriseCloudResources のポリシーを構成する際に活用できるのみ。</span><span class="sxs-lookup"><span data-stu-id="13d36-136">The proxies are only leveraged in configuring the EnterpriseCloudResources policy to force traffic to the matched cloud resources through these proxies.</span></span>|
|<span data-ttu-id="13d36-137">enterpriseIPRangesAreAuthoritative</span><span class="sxs-lookup"><span data-stu-id="13d36-137">enterpriseIPRangesAreAuthoritative</span></span>|<span data-ttu-id="13d36-138">Boolean</span><span class="sxs-lookup"><span data-stu-id="13d36-138">Boolean</span></span>|<span data-ttu-id="13d36-139">構成済みのリストを承諾し、ヒューリスティックを使用した他のサブネットの検索を行わないよう、クライアントに指示するブール値。</span><span class="sxs-lookup"><span data-stu-id="13d36-139">Boolean value that tells the client to accept the configured list and not to use heuristics to attempt to find other subnets.</span></span> <span data-ttu-id="13d36-140">既定では false を指定します。</span><span class="sxs-lookup"><span data-stu-id="13d36-140">Default is false.</span></span>|
|<span data-ttu-id="13d36-141">enterpriseProxyServers</span><span class="sxs-lookup"><span data-stu-id="13d36-141">enterpriseProxyServers</span></span>|<span data-ttu-id="13d36-142">String コレクション</span><span class="sxs-lookup"><span data-stu-id="13d36-142">String collection</span></span>|<span data-ttu-id="13d36-143">これは、プロキシ サーバーのリストです。</span><span class="sxs-lookup"><span data-stu-id="13d36-143">This is a list of proxy servers.</span></span> <span data-ttu-id="13d36-144">任意のサーバー一覧とは見なされません非エンタープライズです。</span><span class="sxs-lookup"><span data-stu-id="13d36-144">Any server not on this list is considered non-enterprise.</span></span>|
|<span data-ttu-id="13d36-145">enterpriseProxyServersAreAuthoritative</span><span class="sxs-lookup"><span data-stu-id="13d36-145">enterpriseProxyServersAreAuthoritative</span></span>|<span data-ttu-id="13d36-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="13d36-146">Boolean</span></span>|<span data-ttu-id="13d36-147">プロキシの構成済みリストを承諾し、他の作業プロキシの検出を試みないよう、クライアントに指示するブール値。</span><span class="sxs-lookup"><span data-stu-id="13d36-147">Boolean value that tells the client to accept the configured list of proxies and not try to detect other work proxies.</span></span> <span data-ttu-id="13d36-148">既定値は false です</span><span class="sxs-lookup"><span data-stu-id="13d36-148">Default is false</span></span>|
|<span data-ttu-id="13d36-149">neutralDomainResources</span><span class="sxs-lookup"><span data-stu-id="13d36-149">neutralDomainResources</span></span>|<span data-ttu-id="13d36-150">String コレクション</span><span class="sxs-lookup"><span data-stu-id="13d36-150">String collection</span></span>|<span data-ttu-id="13d36-151">作業時間またはリソースの個人に使用できるドメイン名のリストです。</span><span class="sxs-lookup"><span data-stu-id="13d36-151">List of domain names that can used for work or personal resource.</span></span>|

## <a name="relationships"></a><span data-ttu-id="13d36-152">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="13d36-152">Relationships</span></span>
<span data-ttu-id="13d36-153">なし</span><span class="sxs-lookup"><span data-stu-id="13d36-153">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="13d36-154">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="13d36-154">JSON Representation</span></span>
<span data-ttu-id="13d36-155">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="13d36-155">Here is a JSON representation of the resource.</span></span>
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





