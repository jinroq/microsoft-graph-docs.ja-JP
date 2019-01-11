---
title: domainDnsSrvRecord リソースの種類
description: テナント内の特定のドメインの DNS ゾーン ファイルに追加された SRV レコードを表します。DomainDnsRecord エンティティから継承されます。
author: lleonard-msft
localization_priority: Normal
ms.openlocfilehash: 655dc6fcbccdcb6e1794c94d97dd8e7fc4837f04
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27835792"
---
# <a name="domaindnssrvrecord-resource-type"></a><span data-ttu-id="b53e6-104">domainDnsSrvRecord リソースの種類</span><span class="sxs-lookup"><span data-stu-id="b53e6-104">domainDnsSrvRecord resource type</span></span>

<span data-ttu-id="b53e6-p102">テナント内の特定のドメインの DNS ゾーン ファイルに追加された SRV レコードを表します。[DomainDnsRecord](domaindnsrecord.md) エンティティから継承されます。</span><span class="sxs-lookup"><span data-stu-id="b53e6-p102">Represents a SRV record added to the DNS zone file of a particular domain in the tenant. Inherited from [DomainDnsRecord](domaindnsrecord.md) entity.</span></span>

## <a name="methods"></a><span data-ttu-id="b53e6-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="b53e6-107">Methods</span></span>
<span data-ttu-id="b53e6-p103">このリソースへの直接クエリはサポートされていません。ドメイン サービス レコードのクエリを実行する方法の詳細については、[ドメイン](domain.md)のトピックを参照してください。</span><span class="sxs-lookup"><span data-stu-id="b53e6-p103">Direct queries to this resource are not supported. Please see the [domain](domain.md) topic for information on how to query for domain service records.</span></span>

## <a name="properties"></a><span data-ttu-id="b53e6-110">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b53e6-110">Properties</span></span>
| <span data-ttu-id="b53e6-111">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b53e6-111">Property</span></span>     | <span data-ttu-id="b53e6-112">種類</span><span class="sxs-lookup"><span data-stu-id="b53e6-112">Type</span></span>   |<span data-ttu-id="b53e6-113">説明</span><span class="sxs-lookup"><span data-stu-id="b53e6-113">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b53e6-114">ID</span><span class="sxs-lookup"><span data-stu-id="b53e6-114">id</span></span>|<span data-ttu-id="b53e6-115">String</span><span class="sxs-lookup"><span data-stu-id="b53e6-115">String</span></span>| <span data-ttu-id="b53e6-p104">このエンティティに割り当てられた一意の識別子。null 許容ではありません。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="b53e6-p104">Unique identifier assigned to this entity. Not nullable, Read-only.</span></span>|
|<span data-ttu-id="b53e6-118">isOptional</span><span class="sxs-lookup"><span data-stu-id="b53e6-118">isOptional</span></span>|<span data-ttu-id="b53e6-119">Boolean</span><span class="sxs-lookup"><span data-stu-id="b53e6-119">Boolean</span></span>| <span data-ttu-id="b53e6-120">False の場合、SRV レコードは Microsoft オンライン サービスでドメインを正しく操作するために、DNS ホストで顧客によって構成されている必要があります。</span><span class="sxs-lookup"><span data-stu-id="b53e6-120">If false, the SRV record must be configured by the customer at the DNS host for Microsoft Online Services to operate correctly with the domain.</span></span> |
|<span data-ttu-id="b53e6-121">label</span><span class="sxs-lookup"><span data-stu-id="b53e6-121">label</span></span>|<span data-ttu-id="b53e6-122">String</span><span class="sxs-lookup"><span data-stu-id="b53e6-122">String</span></span>| <span data-ttu-id="b53e6-123">DNS ホストで SRV レコードの *name* プロパティを構成する場合に使用される値です。</span><span class="sxs-lookup"><span data-stu-id="b53e6-123">Value used when configuring the *name* property of the SRV record at the DNS host.</span></span> |
|<span data-ttu-id="b53e6-124">nameTarget</span><span class="sxs-lookup"><span data-stu-id="b53e6-124">nameTarget</span></span>|<span data-ttu-id="b53e6-125">String</span><span class="sxs-lookup"><span data-stu-id="b53e6-125">String</span></span>| <span data-ttu-id="b53e6-126">DNS ホストで SRV レコードの *Target* プロパティを構成する場合に使用する値です。</span><span class="sxs-lookup"><span data-stu-id="b53e6-126">Value to use when configuring the *Target* property of the SRV record at the DNS host.</span></span> |
|<span data-ttu-id="b53e6-127">port</span><span class="sxs-lookup"><span data-stu-id="b53e6-127">port</span></span>|<span data-ttu-id="b53e6-128">Int32</span><span class="sxs-lookup"><span data-stu-id="b53e6-128">Int32</span></span>| <span data-ttu-id="b53e6-129">DNS ホストで SRV レコードの *port* プロパティを構成する場合に使用する値です。</span><span class="sxs-lookup"><span data-stu-id="b53e6-129">Value to use when configuring the *port* property of the SRV record at the DNS host.</span></span> |
|<span data-ttu-id="b53e6-130">priority</span><span class="sxs-lookup"><span data-stu-id="b53e6-130">priority</span></span>|<span data-ttu-id="b53e6-131">Int32</span><span class="sxs-lookup"><span data-stu-id="b53e6-131">Int32</span></span>| <span data-ttu-id="b53e6-132">DNS ホストで SRV レコードの *priority* プロパティを構成する場合に使用する値です。</span><span class="sxs-lookup"><span data-stu-id="b53e6-132">Value to use when configuring the *priority* property of the SRV record at the DNS host.</span></span> |
|<span data-ttu-id="b53e6-133">protocol</span><span class="sxs-lookup"><span data-stu-id="b53e6-133">protocol</span></span>|<span data-ttu-id="b53e6-134">String</span><span class="sxs-lookup"><span data-stu-id="b53e6-134">String</span></span>| <span data-ttu-id="b53e6-135">DNS ホストで SRV レコードの *protocol* プロパティを構成する場合に使用する値です。</span><span class="sxs-lookup"><span data-stu-id="b53e6-135">Value to use when configuring the *protocol* property of the SRV record at the DNS host.</span></span> |
|<span data-ttu-id="b53e6-136">recordType</span><span class="sxs-lookup"><span data-stu-id="b53e6-136">recordType</span></span>|<span data-ttu-id="b53e6-137">String</span><span class="sxs-lookup"><span data-stu-id="b53e6-137">String</span></span>|  <span data-ttu-id="b53e6-p105">DNS レコードの種類。この値は常に *Srv* です。キー</span><span class="sxs-lookup"><span data-stu-id="b53e6-p105">Type of DNS record. The value is always *Srv*. Key</span></span> |
|<span data-ttu-id="b53e6-141">service</span><span class="sxs-lookup"><span data-stu-id="b53e6-141">service</span></span>|<span data-ttu-id="b53e6-142">String</span><span class="sxs-lookup"><span data-stu-id="b53e6-142">String</span></span>| <span data-ttu-id="b53e6-143">DNS ホストで SRV レコードの *service* プロパティを構成する場合に使用する値です。</span><span class="sxs-lookup"><span data-stu-id="b53e6-143">Value to use when configuring the *service* property of the SRV record at the DNS host.</span></span> |
|<span data-ttu-id="b53e6-144">supportedService</span><span class="sxs-lookup"><span data-stu-id="b53e6-144">supportedService</span></span>|<span data-ttu-id="b53e6-145">String</span><span class="sxs-lookup"><span data-stu-id="b53e6-145">String</span></span>| <span data-ttu-id="b53e6-146">Microsoft オンライン サービスまたはこの SRV レコードに依存している機能。</span><span class="sxs-lookup"><span data-stu-id="b53e6-146">Microsoft Online Service or feature that has a dependency on this SRV record.</span></span></br></br><span data-ttu-id="b53e6-147">次のいずれかの値を指定できます。**null**、*Email*、*Sharepoint*、*EmailInternalRelayOnly*、*OfficeCommunicationsOnline*、*SharePointDefaultDomain*、*FullRedelegation*、*SharePointPublic*、*OrgIdAuthentication*、*Yammer*、*Intune*</span><span class="sxs-lookup"><span data-stu-id="b53e6-147">Can be one of the following values: **null**, *Email*, *Sharepoint*, *EmailInternalRelayOnly*, *OfficeCommunicationsOnline*, *SharePointDefaultDomain*, *FullRedelegation*, *SharePointPublic*, *OrgIdAuthentication*, *Yammer*, *Intune*</span></span> |
|<span data-ttu-id="b53e6-148">ttl</span><span class="sxs-lookup"><span data-stu-id="b53e6-148">ttl</span></span>|<span data-ttu-id="b53e6-149">Int32</span><span class="sxs-lookup"><span data-stu-id="b53e6-149">Int32</span></span>| <span data-ttu-id="b53e6-p106">DNS ホストで SRV レコードの *Time to Live (TTL)* のプロパティを構成するときに使用する値です。null 許容ではありません</span><span class="sxs-lookup"><span data-stu-id="b53e6-p106">Value to use when configuring the *time-to-live (ttl)* property of the SRV record at the DNS host. Not nullable</span></span> |
|<span data-ttu-id="b53e6-152">weight</span><span class="sxs-lookup"><span data-stu-id="b53e6-152">weight</span></span>|<span data-ttu-id="b53e6-153">Int32</span><span class="sxs-lookup"><span data-stu-id="b53e6-153">Int32</span></span>| <span data-ttu-id="b53e6-154">DNS ホストで SRV レコードの *weight* プロパティを構成する場合に使用する値です。</span><span class="sxs-lookup"><span data-stu-id="b53e6-154">Value to use when configuring the *weight* property of the SRV record at the DNS host.</span></span> |

## <a name="relationships"></a><span data-ttu-id="b53e6-155">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="b53e6-155">Relationships</span></span>
<span data-ttu-id="b53e6-156">なし</span><span class="sxs-lookup"><span data-stu-id="b53e6-156">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="b53e6-157">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="b53e6-157">JSON representation</span></span>
<span data-ttu-id="b53e6-158">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="b53e6-158">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.domainDnsRecord",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.domainDnsSrvRecord"
}-->

```json
{
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
