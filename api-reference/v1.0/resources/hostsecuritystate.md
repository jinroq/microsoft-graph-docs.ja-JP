---
title: hostsecuritystate リソースの種類
description: ホストに関するステートフルな情報を含みます (デバイス、コンピューターなどを含む)。
localization_priority: Normal
ms.openlocfilehash: 0646547b7f3e31dcf283c1ce423a52b4ae16f013
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32570786"
---
# <a name="hostsecuritystate-resource-type"></a><span data-ttu-id="83ffd-103">hostsecuritystate リソースの種類</span><span class="sxs-lookup"><span data-stu-id="83ffd-103">hostSecurityState resource type</span></span>

<span data-ttu-id="83ffd-104">ホストに関するステートフルな情報を含みます (デバイス、コンピューターなどを含む)。</span><span class="sxs-lookup"><span data-stu-id="83ffd-104">Contains stateful information about the host (including devices, computers, and so on).</span></span>

## <a name="properties"></a><span data-ttu-id="83ffd-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="83ffd-105">Properties</span></span>

| <span data-ttu-id="83ffd-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="83ffd-106">Property</span></span>   | <span data-ttu-id="83ffd-107">型</span><span class="sxs-lookup"><span data-stu-id="83ffd-107">Type</span></span>|<span data-ttu-id="83ffd-108">説明</span><span class="sxs-lookup"><span data-stu-id="83ffd-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="83ffd-109">fqdn</span><span class="sxs-lookup"><span data-stu-id="83ffd-109">fqdn</span></span>|<span data-ttu-id="83ffd-110">String</span><span class="sxs-lookup"><span data-stu-id="83ffd-110">String</span></span>|<span data-ttu-id="83ffd-111">ホストの FQDN (完全修飾ドメイン名) (例: `machine.company.com`)。</span><span class="sxs-lookup"><span data-stu-id="83ffd-111">Host FQDN (Fully Qualified Domain Name) (for example, `machine.company.com`).</span></span>|
|<span data-ttu-id="83ffd-112">isAzureAadJoined</span><span class="sxs-lookup"><span data-stu-id="83ffd-112">isAzureAadJoined</span></span>|<span data-ttu-id="83ffd-113">Boolean</span><span class="sxs-lookup"><span data-stu-id="83ffd-113">Boolean</span></span>|<span data-ttu-id="83ffd-114">ホストが Azure Active Directory ドメインサービスにドメインに参加している場合は True。</span><span class="sxs-lookup"><span data-stu-id="83ffd-114">True if the host is domain joined to Azure Active Directory Domain Services.</span></span>|
|<span data-ttu-id="83ffd-115">isAzureAadRegistered</span><span class="sxs-lookup"><span data-stu-id="83ffd-115">isAzureAadRegistered</span></span>|<span data-ttu-id="83ffd-116">Boolean</span><span class="sxs-lookup"><span data-stu-id="83ffd-116">Boolean</span></span>|<span data-ttu-id="83ffd-117">ホストが Azure Active Directory デバイス登録 (byod devices、enterprise によって完全に管理されていない) に登録されている場合は、True。</span><span class="sxs-lookup"><span data-stu-id="83ffd-117">True if the host registered with Azure Active Directory Device Registration (BYOD devices - that is, not fully managed by enterprise).</span></span>|
|<span data-ttu-id="83ffd-118">isHybridAzureDomainJoined</span><span class="sxs-lookup"><span data-stu-id="83ffd-118">isHybridAzureDomainJoined</span></span>|<span data-ttu-id="83ffd-119">Boolean</span><span class="sxs-lookup"><span data-stu-id="83ffd-119">Boolean</span></span>|<span data-ttu-id="83ffd-120">ホストがオンプレミスの Active Directory ドメインに参加しているドメインである場合は True。</span><span class="sxs-lookup"><span data-stu-id="83ffd-120">True if the host is domain joined to an on-premises Active Directory domain.</span></span>|
|<span data-ttu-id="83ffd-121">netBiosName</span><span class="sxs-lookup"><span data-stu-id="83ffd-121">netBiosName</span></span>|<span data-ttu-id="83ffd-122">String</span><span class="sxs-lookup"><span data-stu-id="83ffd-122">String</span></span>|<span data-ttu-id="83ffd-123">DNS ドメイン名を除いたローカルホスト名。</span><span class="sxs-lookup"><span data-stu-id="83ffd-123">The local host name, without the DNS domain name.</span></span>|
|<span data-ttu-id="83ffd-124">hp-ux</span><span class="sxs-lookup"><span data-stu-id="83ffd-124">os</span></span>|<span data-ttu-id="83ffd-125">String</span><span class="sxs-lookup"><span data-stu-id="83ffd-125">String</span></span>|<span data-ttu-id="83ffd-126">ホストオペレーティングシステム。</span><span class="sxs-lookup"><span data-stu-id="83ffd-126">Host Operating System.</span></span> <span data-ttu-id="83ffd-127">(たとえば、Windows10、MacOS、RHEL など)。</span><span class="sxs-lookup"><span data-stu-id="83ffd-127">(For example, Windows10, MacOS, RHEL, etc.).</span></span>|
|<span data-ttu-id="83ffd-128">privateIpAddress</span><span class="sxs-lookup"><span data-stu-id="83ffd-128">privateIpAddress</span></span>|<span data-ttu-id="83ffd-129">String</span><span class="sxs-lookup"><span data-stu-id="83ffd-129">String</span></span>|<span data-ttu-id="83ffd-130">プライベート (ルーティング可能ではない) IPv4 または IPv6 アドレス ( [RFC 1918](https://tools.ietf.org/html/rfc1918)を参照) 通知時。</span><span class="sxs-lookup"><span data-stu-id="83ffd-130">Private (not routable) IPv4 or IPv6 address (see [RFC 1918](https://tools.ietf.org/html/rfc1918)) at the time of the alert.</span></span>|
|<span data-ttu-id="83ffd-131">publicipaddress</span><span class="sxs-lookup"><span data-stu-id="83ffd-131">publicIpAddress</span></span>|<span data-ttu-id="83ffd-132">String</span><span class="sxs-lookup"><span data-stu-id="83ffd-132">String</span></span>|<span data-ttu-id="83ffd-133">通知時に公開ルーティング可能な IPv4 または IPv6 アドレス ( [RFC 1918](https://tools.ietf.org/html/rfc1918)を参照)。</span><span class="sxs-lookup"><span data-stu-id="83ffd-133">Publicly routable IPv4 or IPv6 address (see [RFC 1918](https://tools.ietf.org/html/rfc1918)) at time of the alert.</span></span>|
|<span data-ttu-id="83ffd-134">riskScore</span><span class="sxs-lookup"><span data-stu-id="83ffd-134">riskScore</span></span>|<span data-ttu-id="83ffd-135">String</span><span class="sxs-lookup"><span data-stu-id="83ffd-135">String</span></span>|<span data-ttu-id="83ffd-136">プロバイダーが生成/計算するホストのリスクスコア。</span><span class="sxs-lookup"><span data-stu-id="83ffd-136">Provider-generated/calculated risk score of the host.</span></span>  <span data-ttu-id="83ffd-137">推奨値の範囲0-1。パーセンテージに相当します。</span><span class="sxs-lookup"><span data-stu-id="83ffd-137">Recommended value range of 0-1, which equates to a percentage.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="83ffd-138">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="83ffd-138">JSON representation</span></span>

<span data-ttu-id="83ffd-139">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="83ffd-139">The following is a JSON representation of the resource.</span></span>

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
