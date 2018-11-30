---
title: domainDnsSrvRecord リソースの種類
description: テナント内の特定のドメインの DNS ゾーン ファイルに追加された SRV レコードを表します。DomainDnsRecord エンティティから継承されます。
ms.openlocfilehash: 9eba2c74dd26d1c9431b1cabe3d5b283ee7a406d
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27073803"
---
# <a name="domaindnssrvrecord-resource-type"></a><span data-ttu-id="dda22-104">domainDnsSrvRecord リソースの種類</span><span class="sxs-lookup"><span data-stu-id="dda22-104">domainDnsSrvRecord resource type</span></span>

> <span data-ttu-id="dda22-105">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="dda22-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="dda22-106">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="dda22-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="dda22-p103">テナント内の特定のドメインの DNS ゾーン ファイルに追加された SRV レコードを表します。[DomainDnsRecord](domaindnsrecord.md) エンティティから継承されます。</span><span class="sxs-lookup"><span data-stu-id="dda22-p103">Represents a SRV record added to the DNS zone file of a particular domain in the tenant. Inherited from [DomainDnsRecord](domaindnsrecord.md) entity.</span></span>

## <a name="methods"></a><span data-ttu-id="dda22-109">メソッド</span><span class="sxs-lookup"><span data-stu-id="dda22-109">Methods</span></span>
<span data-ttu-id="dda22-p104">このリソースへの直接クエリはサポートされていません。ドメイン サービス レコードのクエリを実行する方法の詳細については、[ドメイン](domain.md)のトピックを参照してください。</span><span class="sxs-lookup"><span data-stu-id="dda22-p104">Direct queries to this resource are not supported. Please see the [domain](domain.md) topic for information on how to query for domain service records.</span></span>

## <a name="properties"></a><span data-ttu-id="dda22-112">プロパティ</span><span class="sxs-lookup"><span data-stu-id="dda22-112">Properties</span></span>
| <span data-ttu-id="dda22-113">プロパティ</span><span class="sxs-lookup"><span data-stu-id="dda22-113">Property</span></span>     | <span data-ttu-id="dda22-114">型</span><span class="sxs-lookup"><span data-stu-id="dda22-114">Type</span></span>   |<span data-ttu-id="dda22-115">説明</span><span class="sxs-lookup"><span data-stu-id="dda22-115">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="dda22-116">id</span><span class="sxs-lookup"><span data-stu-id="dda22-116">id</span></span>|<span data-ttu-id="dda22-117">String</span><span class="sxs-lookup"><span data-stu-id="dda22-117">String</span></span>| <span data-ttu-id="dda22-p105">このエンティティに割り当てられた一意の識別子。null 許容ではありません。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="dda22-p105">Unique identifier assigned to this entity. Not nullable, Read-only.</span></span>|
|<span data-ttu-id="dda22-120">isOptional</span><span class="sxs-lookup"><span data-stu-id="dda22-120">isOptional</span></span>|<span data-ttu-id="dda22-121">Boolean</span><span class="sxs-lookup"><span data-stu-id="dda22-121">Boolean</span></span>| <span data-ttu-id="dda22-122">False の場合、SRV レコードは Microsoft オンライン サービスでドメインを正しく操作するために、DNS ホストで顧客によって構成されている必要があります。</span><span class="sxs-lookup"><span data-stu-id="dda22-122">If false, the SRV record must be configured by the customer at the DNS host for Microsoft Online Services to operate correctly with the domain.</span></span> |
|<span data-ttu-id="dda22-123">label</span><span class="sxs-lookup"><span data-stu-id="dda22-123">label</span></span>|<span data-ttu-id="dda22-124">String</span><span class="sxs-lookup"><span data-stu-id="dda22-124">String</span></span>| <span data-ttu-id="dda22-125">DNS ホストで SRV レコードの *name* プロパティを構成する場合に使用される値です。</span><span class="sxs-lookup"><span data-stu-id="dda22-125">Value used when configuring the *name* property of the SRV record at the DNS host.</span></span> |
|<span data-ttu-id="dda22-126">nameTarget</span><span class="sxs-lookup"><span data-stu-id="dda22-126">nameTarget</span></span>|<span data-ttu-id="dda22-127">String</span><span class="sxs-lookup"><span data-stu-id="dda22-127">String</span></span>| <span data-ttu-id="dda22-128">DNS ホストで SRV レコードの *Target* プロパティを構成する場合に使用する値です。</span><span class="sxs-lookup"><span data-stu-id="dda22-128">Value to use when configuring the *Target* property of the SRV record at the DNS host.</span></span> |
|<span data-ttu-id="dda22-129">port</span><span class="sxs-lookup"><span data-stu-id="dda22-129">port</span></span>|<span data-ttu-id="dda22-130">Int32</span><span class="sxs-lookup"><span data-stu-id="dda22-130">Int32</span></span>| <span data-ttu-id="dda22-131">DNS ホストで SRV レコードの *port* プロパティを構成する場合に使用する値です。</span><span class="sxs-lookup"><span data-stu-id="dda22-131">Value to use when configuring the *port* property of the SRV record at the DNS host.</span></span> |
|<span data-ttu-id="dda22-132">priority</span><span class="sxs-lookup"><span data-stu-id="dda22-132">priority</span></span>|<span data-ttu-id="dda22-133">Int32</span><span class="sxs-lookup"><span data-stu-id="dda22-133">Int32</span></span>| <span data-ttu-id="dda22-134">DNS ホストで SRV レコードの *priority* プロパティを構成する場合に使用する値です。</span><span class="sxs-lookup"><span data-stu-id="dda22-134">Value to use when configuring the *priority* property of the SRV record at the DNS host.</span></span> |
|<span data-ttu-id="dda22-135">protocol</span><span class="sxs-lookup"><span data-stu-id="dda22-135">protocol</span></span>|<span data-ttu-id="dda22-136">String</span><span class="sxs-lookup"><span data-stu-id="dda22-136">String</span></span>| <span data-ttu-id="dda22-137">DNS ホストで SRV レコードの *protocol* プロパティを構成する場合に使用する値です。</span><span class="sxs-lookup"><span data-stu-id="dda22-137">Value to use when configuring the *protocol* property of the SRV record at the DNS host.</span></span> |
|<span data-ttu-id="dda22-138">recordType</span><span class="sxs-lookup"><span data-stu-id="dda22-138">recordType</span></span>|<span data-ttu-id="dda22-139">String</span><span class="sxs-lookup"><span data-stu-id="dda22-139">String</span></span>|  <span data-ttu-id="dda22-p106">DNS レコードの種類。この値は常に *Srv* です。キー</span><span class="sxs-lookup"><span data-stu-id="dda22-p106">Type of DNS record. The value is always *Srv*. Key</span></span> |
|<span data-ttu-id="dda22-143">service</span><span class="sxs-lookup"><span data-stu-id="dda22-143">service</span></span>|<span data-ttu-id="dda22-144">String</span><span class="sxs-lookup"><span data-stu-id="dda22-144">String</span></span>| <span data-ttu-id="dda22-145">DNS ホストで SRV レコードの *service* プロパティを構成する場合に使用する値です。</span><span class="sxs-lookup"><span data-stu-id="dda22-145">Value to use when configuring the *service* property of the SRV record at the DNS host.</span></span> |
|<span data-ttu-id="dda22-146">supportedService</span><span class="sxs-lookup"><span data-stu-id="dda22-146">supportedService</span></span>|<span data-ttu-id="dda22-147">String</span><span class="sxs-lookup"><span data-stu-id="dda22-147">String</span></span>| <span data-ttu-id="dda22-148">Microsoft オンライン サービスまたはこの SRV レコードに依存している機能。</span><span class="sxs-lookup"><span data-stu-id="dda22-148">Microsoft Online Service or feature that has a dependency on this SRV record.</span></span></br></br><span data-ttu-id="dda22-149">次のいずれかの値を指定できます。**null**、*Email*、*Sharepoint*、*EmailInternalRelayOnly*、*OfficeCommunicationsOnline*、*SharePointDefaultDomain*、*FullRedelegation*、*SharePointPublic*、*OrgIdAuthentication*、*Yammer*、*Intune*</span><span class="sxs-lookup"><span data-stu-id="dda22-149">Can be one of the following values: **null**, *Email*, *Sharepoint*, *EmailInternalRelayOnly*, *OfficeCommunicationsOnline*, *SharePointDefaultDomain*, *FullRedelegation*, *SharePointPublic*, *OrgIdAuthentication*, *Yammer*, *Intune*</span></span> |
|<span data-ttu-id="dda22-150">ttl</span><span class="sxs-lookup"><span data-stu-id="dda22-150">ttl</span></span>|<span data-ttu-id="dda22-151">Int32</span><span class="sxs-lookup"><span data-stu-id="dda22-151">Int32</span></span>| <span data-ttu-id="dda22-p107">DNS ホストで SRV レコードの *Time to Live (TTL)* のプロパティを構成するときに使用する値です。null 許容ではありません</span><span class="sxs-lookup"><span data-stu-id="dda22-p107">Value to use when configuring the *time-to-live (ttl)* property of the SRV record at the DNS host. Not nullable</span></span> |
|<span data-ttu-id="dda22-154">weight</span><span class="sxs-lookup"><span data-stu-id="dda22-154">weight</span></span>|<span data-ttu-id="dda22-155">Int32</span><span class="sxs-lookup"><span data-stu-id="dda22-155">Int32</span></span>| <span data-ttu-id="dda22-156">DNS ホストで SRV レコードの *weight* プロパティを構成する場合に使用する値です。</span><span class="sxs-lookup"><span data-stu-id="dda22-156">Value to use when configuring the *weight* property of the SRV record at the DNS host.</span></span> |

## <a name="relationships"></a><span data-ttu-id="dda22-157">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="dda22-157">Relationships</span></span>
<span data-ttu-id="dda22-158">なし</span><span class="sxs-lookup"><span data-stu-id="dda22-158">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="dda22-159">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="dda22-159">JSON representation</span></span>
<span data-ttu-id="dda22-160">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="dda22-160">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.domainDnsSrvRecord"
}-->

```json
{
  "canonicalName": "String",
  "id": "String (identifier)",
  "isOptional": true,
  "label": "String",
  "nameTarget": "String",
  "port": 1024,
  "priority": 1024,
  "protocol": "String",
  "recordType": "String",
  "service": "String",
  "supportedService": "String",
  "ttl": 1024,
  "weight": 1024
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "domainDnsSrvRecord resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->