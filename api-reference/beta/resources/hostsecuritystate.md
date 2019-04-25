---
title: hostsecuritystate リソースの種類
description: " > **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでこれらの API を使用することは、サポートされていません。"
localization_priority: Normal
ms.openlocfilehash: d6f566a2bd42163c570fe837d2419057c62664bb
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32547411"
---
# <a name="hostsecuritystate-resource-type"></a><span data-ttu-id="63788-104">hostsecuritystate リソースの種類</span><span class="sxs-lookup"><span data-stu-id="63788-104">hostSecurityState resource type</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="63788-105">ホストに関するステートフルな情報を含みます (デバイス、コンピューターなどを含む)。</span><span class="sxs-lookup"><span data-stu-id="63788-105">Contains stateful information about the host (including devices, computers, and so on).</span></span>

## <a name="properties"></a><span data-ttu-id="63788-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="63788-106">Properties</span></span>

| <span data-ttu-id="63788-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="63788-107">Property</span></span>   | <span data-ttu-id="63788-108">型</span><span class="sxs-lookup"><span data-stu-id="63788-108">Type</span></span>|<span data-ttu-id="63788-109">説明</span><span class="sxs-lookup"><span data-stu-id="63788-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="63788-110">fqdn</span><span class="sxs-lookup"><span data-stu-id="63788-110">fqdn</span></span>|<span data-ttu-id="63788-111">String</span><span class="sxs-lookup"><span data-stu-id="63788-111">String</span></span>|<span data-ttu-id="63788-112">ホストの FQDN (完全修飾ドメイン名) (たとえば、machine.company.com)。</span><span class="sxs-lookup"><span data-stu-id="63788-112">Host FQDN (Fully Qualified Domain Name) (for example, machine.company.com).</span></span>|
|<span data-ttu-id="63788-113">isAzureAadJoined</span><span class="sxs-lookup"><span data-stu-id="63788-113">isAzureAadJoined</span></span>|<span data-ttu-id="63788-114">ブール値</span><span class="sxs-lookup"><span data-stu-id="63788-114">Boolean</span></span>|<span data-ttu-id="63788-115">ホストが Azure Active Directory ドメインサービスにドメインに参加している場合は True。</span><span class="sxs-lookup"><span data-stu-id="63788-115">True if the host is domain joined to Azure Active Directory Domain Services.</span></span>|
|<span data-ttu-id="63788-116">isAzureAadRegistered</span><span class="sxs-lookup"><span data-stu-id="63788-116">isAzureAadRegistered</span></span>|<span data-ttu-id="63788-117">ブール値</span><span class="sxs-lookup"><span data-stu-id="63788-117">Boolean</span></span>|<span data-ttu-id="63788-118">ホストが Azure Active Directory デバイス登録 (byod devices、enterprise によって完全に管理されていない) に登録されている場合は、True。</span><span class="sxs-lookup"><span data-stu-id="63788-118">True if the host registered with Azure Active Directory Device Registration (BYOD devices - that is, not fully managed by enterprise).</span></span>|
|<span data-ttu-id="63788-119">isHybridAzureDomainJoined</span><span class="sxs-lookup"><span data-stu-id="63788-119">isHybridAzureDomainJoined</span></span>|<span data-ttu-id="63788-120">ブール値</span><span class="sxs-lookup"><span data-stu-id="63788-120">Boolean</span></span>|<span data-ttu-id="63788-121">ホストがオンプレミスの Active Directory ドメインに参加しているドメインである場合は True。</span><span class="sxs-lookup"><span data-stu-id="63788-121">True if the host is domain joined to an on-premises Active Directory domain.</span></span>|
|<span data-ttu-id="63788-122">netBiosName</span><span class="sxs-lookup"><span data-stu-id="63788-122">netBiosName</span></span>|<span data-ttu-id="63788-123">String</span><span class="sxs-lookup"><span data-stu-id="63788-123">String</span></span>|<span data-ttu-id="63788-124">DNS ドメイン名を除いたローカルホスト名。</span><span class="sxs-lookup"><span data-stu-id="63788-124">The local host name, without the DNS domain name.</span></span>|
|<span data-ttu-id="63788-125">hp-ux</span><span class="sxs-lookup"><span data-stu-id="63788-125">os</span></span>|<span data-ttu-id="63788-126">String</span><span class="sxs-lookup"><span data-stu-id="63788-126">String</span></span>|<span data-ttu-id="63788-127">ホストオペレーティングシステム。</span><span class="sxs-lookup"><span data-stu-id="63788-127">Host Operating System.</span></span> <span data-ttu-id="63788-128">(たとえば、Windows10、MacOS、RHEL など)。</span><span class="sxs-lookup"><span data-stu-id="63788-128">(For example, Windows10, MacOS, RHEL, etc.).</span></span>|
|<span data-ttu-id="63788-129">privateIpAddress</span><span class="sxs-lookup"><span data-stu-id="63788-129">privateIpAddress</span></span>|<span data-ttu-id="63788-130">String</span><span class="sxs-lookup"><span data-stu-id="63788-130">String</span></span>|<span data-ttu-id="63788-131">プライベート (ルーティング可能ではない) IPv4 または IPv6 アドレス ( [RFC 1918](https://tools.ietf.org/html/rfc1918)を参照) 通知時。</span><span class="sxs-lookup"><span data-stu-id="63788-131">Private (not routable) IPv4 or IPv6 address (see [RFC 1918](https://tools.ietf.org/html/rfc1918)) at the time of the alert.</span></span>|
|<span data-ttu-id="63788-132">publicipaddress</span><span class="sxs-lookup"><span data-stu-id="63788-132">publicIpAddress</span></span>|<span data-ttu-id="63788-133">String</span><span class="sxs-lookup"><span data-stu-id="63788-133">String</span></span>|<span data-ttu-id="63788-134">通知時に公開ルーティング可能な IPv4 または IPv6 アドレス ( [RFC 1918](https://tools.ietf.org/html/rfc1918)を参照)。</span><span class="sxs-lookup"><span data-stu-id="63788-134">Publicly routable IPv4 or IPv6 address (see [RFC 1918](https://tools.ietf.org/html/rfc1918)) at time of the alert.</span></span>|
|<span data-ttu-id="63788-135">riskScore</span><span class="sxs-lookup"><span data-stu-id="63788-135">riskScore</span></span>|<span data-ttu-id="63788-136">String</span><span class="sxs-lookup"><span data-stu-id="63788-136">String</span></span>|<span data-ttu-id="63788-137">プロバイダーが生成/計算するホストのリスクスコア。</span><span class="sxs-lookup"><span data-stu-id="63788-137">Provider-generated/calculated risk score of the host.</span></span>  <span data-ttu-id="63788-138">推奨値の範囲0-1。パーセンテージに相当します。</span><span class="sxs-lookup"><span data-stu-id="63788-138">Recommended value range of 0-1, which equates to a percentage.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="63788-139">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="63788-139">JSON representation</span></span>

<span data-ttu-id="63788-140">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="63788-140">The following is a JSON representation of the resource.</span></span>

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
