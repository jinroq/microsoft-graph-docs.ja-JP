---
title: hostSecurityState リソースの種類
description: ステートフルなホスト (デバイス、コンピューターを含む) について説明します。
localization_priority: Normal
ms.openlocfilehash: 0646547b7f3e31dcf283c1ce423a52b4ae16f013
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27816339"
---
# <a name="hostsecuritystate-resource-type"></a><span data-ttu-id="3dbd0-103">hostSecurityState リソースの種類</span><span class="sxs-lookup"><span data-stu-id="3dbd0-103">hostSecurityState resource type</span></span>

<span data-ttu-id="3dbd0-104">ステートフルなホスト (デバイス、コンピューターを含む) について説明します。</span><span class="sxs-lookup"><span data-stu-id="3dbd0-104">Contains stateful information about the host (including devices, computers, and so on).</span></span>

## <a name="properties"></a><span data-ttu-id="3dbd0-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="3dbd0-105">Properties</span></span>

| <span data-ttu-id="3dbd0-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="3dbd0-106">Property</span></span>   | <span data-ttu-id="3dbd0-107">種類</span><span class="sxs-lookup"><span data-stu-id="3dbd0-107">Type</span></span>|<span data-ttu-id="3dbd0-108">説明</span><span class="sxs-lookup"><span data-stu-id="3dbd0-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="3dbd0-109">fqdn</span><span class="sxs-lookup"><span data-stu-id="3dbd0-109">fqdn</span></span>|<span data-ttu-id="3dbd0-110">String</span><span class="sxs-lookup"><span data-stu-id="3dbd0-110">String</span></span>|<span data-ttu-id="3dbd0-111">FQDN (完全修飾ドメイン名) のホスト (たとえば、 `machine.company.com`)。</span><span class="sxs-lookup"><span data-stu-id="3dbd0-111">Host FQDN (Fully Qualified Domain Name) (for example, `machine.company.com`).</span></span>|
|<span data-ttu-id="3dbd0-112">isAzureAadJoined</span><span class="sxs-lookup"><span data-stu-id="3dbd0-112">isAzureAadJoined</span></span>|<span data-ttu-id="3dbd0-113">ブール型</span><span class="sxs-lookup"><span data-stu-id="3dbd0-113">Boolean</span></span>|<span data-ttu-id="3dbd0-114">ホストが Azure Active Directory ドメイン サービスに参加しているドメインである場合は true。</span><span class="sxs-lookup"><span data-stu-id="3dbd0-114">True if the host is domain joined to Azure Active Directory Domain Services.</span></span>|
|<span data-ttu-id="3dbd0-115">isAzureAadRegistered</span><span class="sxs-lookup"><span data-stu-id="3dbd0-115">isAzureAadRegistered</span></span>|<span data-ttu-id="3dbd0-116">ブール型</span><span class="sxs-lookup"><span data-stu-id="3dbd0-116">Boolean</span></span>|<span data-ttu-id="3dbd0-117">Azure Active Directory デバイスの登録 (BYOD - は、完全に管理されているデバイスの企業が) を持つホストが登録されている場合は true。</span><span class="sxs-lookup"><span data-stu-id="3dbd0-117">True if the host registered with Azure Active Directory Device Registration (BYOD devices - that is, not fully managed by enterprise).</span></span>|
|<span data-ttu-id="3dbd0-118">isHybridAzureDomainJoined</span><span class="sxs-lookup"><span data-stu-id="3dbd0-118">isHybridAzureDomainJoined</span></span>|<span data-ttu-id="3dbd0-119">ブール型</span><span class="sxs-lookup"><span data-stu-id="3dbd0-119">Boolean</span></span>|<span data-ttu-id="3dbd0-120">ホストが、オンプレミスの Active Directory ドメインに参加しているドメインである場合は true。</span><span class="sxs-lookup"><span data-stu-id="3dbd0-120">True if the host is domain joined to an on-premises Active Directory domain.</span></span>|
|<span data-ttu-id="3dbd0-121">あります。</span><span class="sxs-lookup"><span data-stu-id="3dbd0-121">netBiosName</span></span>|<span data-ttu-id="3dbd0-122">String</span><span class="sxs-lookup"><span data-stu-id="3dbd0-122">String</span></span>|<span data-ttu-id="3dbd0-123">ローカル ホスト名、DNS ドメインの名前を持たない。</span><span class="sxs-lookup"><span data-stu-id="3dbd0-123">The local host name, without the DNS domain name.</span></span>|
|<span data-ttu-id="3dbd0-124">os</span><span class="sxs-lookup"><span data-stu-id="3dbd0-124">os</span></span>|<span data-ttu-id="3dbd0-125">String</span><span class="sxs-lookup"><span data-stu-id="3dbd0-125">String</span></span>|<span data-ttu-id="3dbd0-126">ホストのオペレーティング ・ システムです。</span><span class="sxs-lookup"><span data-stu-id="3dbd0-126">Host Operating System.</span></span> <span data-ttu-id="3dbd0-127">(たとえば、Windows10、MacOS、RHEL など)。</span><span class="sxs-lookup"><span data-stu-id="3dbd0-127">(For example, Windows10, MacOS, RHEL, etc.).</span></span>|
|<span data-ttu-id="3dbd0-128">privateIpAddress</span><span class="sxs-lookup"><span data-stu-id="3dbd0-128">privateIpAddress</span></span>|<span data-ttu-id="3dbd0-129">String</span><span class="sxs-lookup"><span data-stu-id="3dbd0-129">String</span></span>|<span data-ttu-id="3dbd0-130">(ルーティングできない) プライベートの IPv4 または IPv6 アドレス ( [RFC 1918](https://tools.ietf.org/html/rfc1918)参照) 時の警告です。</span><span class="sxs-lookup"><span data-stu-id="3dbd0-130">Private (not routable) IPv4 or IPv6 address (see [RFC 1918](https://tools.ietf.org/html/rfc1918)) at the time of the alert.</span></span>|
|<span data-ttu-id="3dbd0-131">publicIpAddress</span><span class="sxs-lookup"><span data-stu-id="3dbd0-131">publicIpAddress</span></span>|<span data-ttu-id="3dbd0-132">String</span><span class="sxs-lookup"><span data-stu-id="3dbd0-132">String</span></span>|<span data-ttu-id="3dbd0-133">公的にルーティング可能な IPv4 アドレスまたは IPv6 アドレス ( [RFC 1918](https://tools.ietf.org/html/rfc1918)参照) 警告の時にします。</span><span class="sxs-lookup"><span data-stu-id="3dbd0-133">Publicly routable IPv4 or IPv6 address (see [RFC 1918](https://tools.ietf.org/html/rfc1918)) at time of the alert.</span></span>|
|<span data-ttu-id="3dbd0-134">riskScore</span><span class="sxs-lookup"><span data-stu-id="3dbd0-134">riskScore</span></span>|<span data-ttu-id="3dbd0-135">String</span><span class="sxs-lookup"><span data-stu-id="3dbd0-135">String</span></span>|<span data-ttu-id="3dbd0-136">ホストのプロバイダーによって生成されると計算されるリスク ・ スコアです。</span><span class="sxs-lookup"><span data-stu-id="3dbd0-136">Provider-generated/calculated risk score of the host.</span></span>  <span data-ttu-id="3dbd0-137">0 - 1 パーセントに相当する値の範囲をお勧めします。</span><span class="sxs-lookup"><span data-stu-id="3dbd0-137">Recommended value range of 0-1, which equates to a percentage.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="3dbd0-138">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="3dbd0-138">JSON representation</span></span>

<span data-ttu-id="3dbd0-139">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="3dbd0-139">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.hostSecurityState"
}-->

```json
{
  "fqdn": "String",
  "isAzureAadJoined": true,
  "isAzureAadRegistered": true,
  "isHybridAzureDomainJoined": true,
  "netBiosName": "String",
  "os": "String",
  "privateIpAddress": "String",
  "publicIpAddress": "String",
  "riskScore": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "hostSecurityState resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
