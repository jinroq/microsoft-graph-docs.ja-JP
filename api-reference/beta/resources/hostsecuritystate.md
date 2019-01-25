---
title: hostSecurityState リソースの種類
description: " > **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでこれらの API を使用することは、サポートされていません。"
localization_priority: Normal
ms.openlocfilehash: d6f566a2bd42163c570fe837d2419057c62664bb
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29526698"
---
# <a name="hostsecuritystate-resource-type"></a><span data-ttu-id="30ce1-104">hostSecurityState リソースの種類</span><span class="sxs-lookup"><span data-stu-id="30ce1-104">hostSecurityState resource type</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="30ce1-105">ステートフルなホスト (デバイス、コンピューターを含む) について説明します。</span><span class="sxs-lookup"><span data-stu-id="30ce1-105">Contains stateful information about the host (including devices, computers, and so on).</span></span>

## <a name="properties"></a><span data-ttu-id="30ce1-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="30ce1-106">Properties</span></span>

| <span data-ttu-id="30ce1-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="30ce1-107">Property</span></span>   | <span data-ttu-id="30ce1-108">型</span><span class="sxs-lookup"><span data-stu-id="30ce1-108">Type</span></span>|<span data-ttu-id="30ce1-109">説明</span><span class="sxs-lookup"><span data-stu-id="30ce1-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="30ce1-110">fqdn</span><span class="sxs-lookup"><span data-stu-id="30ce1-110">fqdn</span></span>|<span data-ttu-id="30ce1-111">String</span><span class="sxs-lookup"><span data-stu-id="30ce1-111">String</span></span>|<span data-ttu-id="30ce1-112">ホストの FQDN (完全修飾ドメイン名) (machine.company.com など)。</span><span class="sxs-lookup"><span data-stu-id="30ce1-112">Host FQDN (Fully Qualified Domain Name) (for example, machine.company.com).</span></span>|
|<span data-ttu-id="30ce1-113">isAzureAadJoined</span><span class="sxs-lookup"><span data-stu-id="30ce1-113">isAzureAadJoined</span></span>|<span data-ttu-id="30ce1-114">ブール値</span><span class="sxs-lookup"><span data-stu-id="30ce1-114">Boolean</span></span>|<span data-ttu-id="30ce1-115">ホストが Azure Active Directory ドメイン サービスに参加しているドメインである場合は true。</span><span class="sxs-lookup"><span data-stu-id="30ce1-115">True if the host is domain joined to Azure Active Directory Domain Services.</span></span>|
|<span data-ttu-id="30ce1-116">isAzureAadRegistered</span><span class="sxs-lookup"><span data-stu-id="30ce1-116">isAzureAadRegistered</span></span>|<span data-ttu-id="30ce1-117">ブール値</span><span class="sxs-lookup"><span data-stu-id="30ce1-117">Boolean</span></span>|<span data-ttu-id="30ce1-118">Azure Active Directory デバイスの登録 (BYOD - は、完全に管理されているデバイスの企業が) を持つホストが登録されている場合は true。</span><span class="sxs-lookup"><span data-stu-id="30ce1-118">True if the host registered with Azure Active Directory Device Registration (BYOD devices - that is, not fully managed by enterprise).</span></span>|
|<span data-ttu-id="30ce1-119">isHybridAzureDomainJoined</span><span class="sxs-lookup"><span data-stu-id="30ce1-119">isHybridAzureDomainJoined</span></span>|<span data-ttu-id="30ce1-120">ブール値</span><span class="sxs-lookup"><span data-stu-id="30ce1-120">Boolean</span></span>|<span data-ttu-id="30ce1-121">ホストが、オンプレミスの Active Directory ドメインに参加しているドメインである場合は true。</span><span class="sxs-lookup"><span data-stu-id="30ce1-121">True if the host is domain joined to an on-premises Active Directory domain.</span></span>|
|<span data-ttu-id="30ce1-122">あります。</span><span class="sxs-lookup"><span data-stu-id="30ce1-122">netBiosName</span></span>|<span data-ttu-id="30ce1-123">String</span><span class="sxs-lookup"><span data-stu-id="30ce1-123">String</span></span>|<span data-ttu-id="30ce1-124">ローカル ホスト名、DNS ドメインの名前を持たない。</span><span class="sxs-lookup"><span data-stu-id="30ce1-124">The local host name, without the DNS domain name.</span></span>|
|<span data-ttu-id="30ce1-125">I-5.</span><span class="sxs-lookup"><span data-stu-id="30ce1-125">os</span></span>|<span data-ttu-id="30ce1-126">String</span><span class="sxs-lookup"><span data-stu-id="30ce1-126">String</span></span>|<span data-ttu-id="30ce1-127">ホストのオペレーティング ・ システムです。</span><span class="sxs-lookup"><span data-stu-id="30ce1-127">Host Operating System.</span></span> <span data-ttu-id="30ce1-128">(たとえば、Windows10、MacOS、RHEL など)。</span><span class="sxs-lookup"><span data-stu-id="30ce1-128">(For example, Windows10, MacOS, RHEL, etc.).</span></span>|
|<span data-ttu-id="30ce1-129">privateIpAddress</span><span class="sxs-lookup"><span data-stu-id="30ce1-129">privateIpAddress</span></span>|<span data-ttu-id="30ce1-130">String</span><span class="sxs-lookup"><span data-stu-id="30ce1-130">String</span></span>|<span data-ttu-id="30ce1-131">(ルーティングできない) プライベートの IPv4 または IPv6 アドレス ( [RFC 1918](https://tools.ietf.org/html/rfc1918)参照) 時の警告です。</span><span class="sxs-lookup"><span data-stu-id="30ce1-131">Private (not routable) IPv4 or IPv6 address (see [RFC 1918](https://tools.ietf.org/html/rfc1918)) at the time of the alert.</span></span>|
|<span data-ttu-id="30ce1-132">publicIpAddress</span><span class="sxs-lookup"><span data-stu-id="30ce1-132">publicIpAddress</span></span>|<span data-ttu-id="30ce1-133">String</span><span class="sxs-lookup"><span data-stu-id="30ce1-133">String</span></span>|<span data-ttu-id="30ce1-134">公的にルーティング可能な IPv4 アドレスまたは IPv6 アドレス ( [RFC 1918](https://tools.ietf.org/html/rfc1918)参照) 警告の時にします。</span><span class="sxs-lookup"><span data-stu-id="30ce1-134">Publicly routable IPv4 or IPv6 address (see [RFC 1918](https://tools.ietf.org/html/rfc1918)) at time of the alert.</span></span>|
|<span data-ttu-id="30ce1-135">riskScore</span><span class="sxs-lookup"><span data-stu-id="30ce1-135">riskScore</span></span>|<span data-ttu-id="30ce1-136">String</span><span class="sxs-lookup"><span data-stu-id="30ce1-136">String</span></span>|<span data-ttu-id="30ce1-137">ホストのプロバイダーによって生成されると計算されるリスク ・ スコアです。</span><span class="sxs-lookup"><span data-stu-id="30ce1-137">Provider-generated/calculated risk score of the host.</span></span>  <span data-ttu-id="30ce1-138">0 - 1 パーセントに相当する値の範囲をお勧めします。</span><span class="sxs-lookup"><span data-stu-id="30ce1-138">Recommended value range of 0-1, which equates to a percentage.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="30ce1-139">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="30ce1-139">JSON representation</span></span>

<span data-ttu-id="30ce1-140">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="30ce1-140">The following is a JSON representation of the resource.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "hostSecurityState resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/hostsecuritystate.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
