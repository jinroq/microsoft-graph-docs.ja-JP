---
title: hostSecurityState リソースの種類
description: " > **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。"
localization_priority: Normal
ms.openlocfilehash: 1ae1436dd9771d34c37542eb756f81a4f8f0306a
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27853376"
---
# <a name="hostsecuritystate-resource-type"></a><span data-ttu-id="88564-104">hostSecurityState リソースの種類</span><span class="sxs-lookup"><span data-stu-id="88564-104">hostSecurityState resource type</span></span>

 > <span data-ttu-id="88564-105">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="88564-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="88564-106">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="88564-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="88564-107">ステートフルなホスト (デバイス、コンピューターを含む) について説明します。</span><span class="sxs-lookup"><span data-stu-id="88564-107">Contains stateful information about the host (including devices, computers, and so on).</span></span>

## <a name="properties"></a><span data-ttu-id="88564-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="88564-108">Properties</span></span>

| <span data-ttu-id="88564-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="88564-109">Property</span></span>   | <span data-ttu-id="88564-110">種類</span><span class="sxs-lookup"><span data-stu-id="88564-110">Type</span></span>|<span data-ttu-id="88564-111">説明</span><span class="sxs-lookup"><span data-stu-id="88564-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="88564-112">fqdn</span><span class="sxs-lookup"><span data-stu-id="88564-112">fqdn</span></span>|<span data-ttu-id="88564-113">String</span><span class="sxs-lookup"><span data-stu-id="88564-113">String</span></span>|<span data-ttu-id="88564-114">ホストの FQDN (完全修飾ドメイン名) (machine.company.com など)。</span><span class="sxs-lookup"><span data-stu-id="88564-114">Host FQDN (Fully Qualified Domain Name) (for example, machine.company.com).</span></span>|
|<span data-ttu-id="88564-115">isAzureAadJoined</span><span class="sxs-lookup"><span data-stu-id="88564-115">isAzureAadJoined</span></span>|<span data-ttu-id="88564-116">ブール型</span><span class="sxs-lookup"><span data-stu-id="88564-116">Boolean</span></span>|<span data-ttu-id="88564-117">ホストが Azure Active Directory ドメイン サービスに参加しているドメインである場合は true。</span><span class="sxs-lookup"><span data-stu-id="88564-117">True if the host is domain joined to Azure Active Directory Domain Services.</span></span>|
|<span data-ttu-id="88564-118">isAzureAadRegistered</span><span class="sxs-lookup"><span data-stu-id="88564-118">isAzureAadRegistered</span></span>|<span data-ttu-id="88564-119">ブール型</span><span class="sxs-lookup"><span data-stu-id="88564-119">Boolean</span></span>|<span data-ttu-id="88564-120">Azure Active Directory デバイスの登録 (BYOD - は、完全に管理されているデバイスの企業が) を持つホストが登録されている場合は true。</span><span class="sxs-lookup"><span data-stu-id="88564-120">True if the host registered with Azure Active Directory Device Registration (BYOD devices - that is, not fully managed by enterprise).</span></span>|
|<span data-ttu-id="88564-121">isHybridAzureDomainJoined</span><span class="sxs-lookup"><span data-stu-id="88564-121">isHybridAzureDomainJoined</span></span>|<span data-ttu-id="88564-122">ブール型</span><span class="sxs-lookup"><span data-stu-id="88564-122">Boolean</span></span>|<span data-ttu-id="88564-123">ホストが、オンプレミスの Active Directory ドメインに参加しているドメインである場合は true。</span><span class="sxs-lookup"><span data-stu-id="88564-123">True if the host is domain joined to an on-premises Active Directory domain.</span></span>|
|<span data-ttu-id="88564-124">あります。</span><span class="sxs-lookup"><span data-stu-id="88564-124">netBiosName</span></span>|<span data-ttu-id="88564-125">String</span><span class="sxs-lookup"><span data-stu-id="88564-125">String</span></span>|<span data-ttu-id="88564-126">ローカル ホスト名、DNS ドメインの名前を持たない。</span><span class="sxs-lookup"><span data-stu-id="88564-126">The local host name, without the DNS domain name.</span></span>|
|<span data-ttu-id="88564-127">os</span><span class="sxs-lookup"><span data-stu-id="88564-127">os</span></span>|<span data-ttu-id="88564-128">String</span><span class="sxs-lookup"><span data-stu-id="88564-128">String</span></span>|<span data-ttu-id="88564-129">ホストのオペレーティング ・ システムです。</span><span class="sxs-lookup"><span data-stu-id="88564-129">Host Operating System.</span></span> <span data-ttu-id="88564-130">(たとえば、Windows10、MacOS、RHEL など)。</span><span class="sxs-lookup"><span data-stu-id="88564-130">(For example, Windows10, MacOS, RHEL, etc.).</span></span>|
|<span data-ttu-id="88564-131">privateIpAddress</span><span class="sxs-lookup"><span data-stu-id="88564-131">privateIpAddress</span></span>|<span data-ttu-id="88564-132">String</span><span class="sxs-lookup"><span data-stu-id="88564-132">String</span></span>|<span data-ttu-id="88564-133">(ルーティングできない) プライベートの IPv4 または IPv6 アドレス ( [RFC 1918](https://tools.ietf.org/html/rfc1918)参照) 時の警告です。</span><span class="sxs-lookup"><span data-stu-id="88564-133">Private (not routable) IPv4 or IPv6 address (see [RFC 1918](https://tools.ietf.org/html/rfc1918)) at the time of the alert.</span></span>|
|<span data-ttu-id="88564-134">publicIpAddress</span><span class="sxs-lookup"><span data-stu-id="88564-134">publicIpAddress</span></span>|<span data-ttu-id="88564-135">String</span><span class="sxs-lookup"><span data-stu-id="88564-135">String</span></span>|<span data-ttu-id="88564-136">公的にルーティング可能な IPv4 アドレスまたは IPv6 アドレス ( [RFC 1918](https://tools.ietf.org/html/rfc1918)参照) 警告の時にします。</span><span class="sxs-lookup"><span data-stu-id="88564-136">Publicly routable IPv4 or IPv6 address (see [RFC 1918](https://tools.ietf.org/html/rfc1918)) at time of the alert.</span></span>|
|<span data-ttu-id="88564-137">riskScore</span><span class="sxs-lookup"><span data-stu-id="88564-137">riskScore</span></span>|<span data-ttu-id="88564-138">String</span><span class="sxs-lookup"><span data-stu-id="88564-138">String</span></span>|<span data-ttu-id="88564-139">ホストのプロバイダーによって生成されると計算されるリスク ・ スコアです。</span><span class="sxs-lookup"><span data-stu-id="88564-139">Provider-generated/calculated risk score of the host.</span></span>  <span data-ttu-id="88564-140">0 - 1 パーセントに相当する値の範囲をお勧めします。</span><span class="sxs-lookup"><span data-stu-id="88564-140">Recommended value range of 0-1, which equates to a percentage.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="88564-141">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="88564-141">JSON representation</span></span>

<span data-ttu-id="88564-142">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="88564-142">The following is a JSON representation of the resource.</span></span>

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
