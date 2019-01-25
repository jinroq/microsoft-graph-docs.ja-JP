---
title: domainDnsSrvRecord リソースの種類
description: テナント内の特定のドメインの DNS ゾーン ファイルに追加された SRV レコードを表します。DomainDnsRecord エンティティから継承されます。
author: lleonard-msft
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: bdbc2246340d5cd15529dd05101567bc04d1e607
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29524479"
---
# <a name="domaindnssrvrecord-resource-type"></a><span data-ttu-id="a29f2-104">domainDnsSrvRecord リソースの種類</span><span class="sxs-lookup"><span data-stu-id="a29f2-104">domainDnsSrvRecord resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a29f2-p102">テナント内の特定のドメインの DNS ゾーン ファイルに追加された SRV レコードを表します。[DomainDnsRecord](domaindnsrecord.md) エンティティから継承されます。</span><span class="sxs-lookup"><span data-stu-id="a29f2-p102">Represents a SRV record added to the DNS zone file of a particular domain in the tenant. Inherited from [DomainDnsRecord](domaindnsrecord.md) entity.</span></span>

## <a name="methods"></a><span data-ttu-id="a29f2-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="a29f2-107">Methods</span></span>
<span data-ttu-id="a29f2-p103">このリソースへの直接クエリはサポートされていません。ドメイン サービス レコードのクエリを実行する方法の詳細については、[ドメイン](domain.md)のトピックを参照してください。</span><span class="sxs-lookup"><span data-stu-id="a29f2-p103">Direct queries to this resource are not supported. Please see the [domain](domain.md) topic for information on how to query for domain service records.</span></span>

## <a name="properties"></a><span data-ttu-id="a29f2-110">プロパティ</span><span class="sxs-lookup"><span data-stu-id="a29f2-110">Properties</span></span>
| <span data-ttu-id="a29f2-111">プロパティ</span><span class="sxs-lookup"><span data-stu-id="a29f2-111">Property</span></span>     | <span data-ttu-id="a29f2-112">型</span><span class="sxs-lookup"><span data-stu-id="a29f2-112">Type</span></span>   |<span data-ttu-id="a29f2-113">説明</span><span class="sxs-lookup"><span data-stu-id="a29f2-113">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a29f2-114">id</span><span class="sxs-lookup"><span data-stu-id="a29f2-114">id</span></span>|<span data-ttu-id="a29f2-115">String</span><span class="sxs-lookup"><span data-stu-id="a29f2-115">String</span></span>| <span data-ttu-id="a29f2-p104">このエンティティに割り当てられた一意の識別子。null 許容ではありません。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="a29f2-p104">Unique identifier assigned to this entity. Not nullable, Read-only.</span></span>|
|<span data-ttu-id="a29f2-118">isOptional</span><span class="sxs-lookup"><span data-stu-id="a29f2-118">isOptional</span></span>|<span data-ttu-id="a29f2-119">Boolean</span><span class="sxs-lookup"><span data-stu-id="a29f2-119">Boolean</span></span>| <span data-ttu-id="a29f2-120">False の場合、SRV レコードは Microsoft オンライン サービスでドメインを正しく操作するために、DNS ホストで顧客によって構成されている必要があります。</span><span class="sxs-lookup"><span data-stu-id="a29f2-120">If false, the SRV record must be configured by the customer at the DNS host for Microsoft Online Services to operate correctly with the domain.</span></span> |
|<span data-ttu-id="a29f2-121">label</span><span class="sxs-lookup"><span data-stu-id="a29f2-121">label</span></span>|<span data-ttu-id="a29f2-122">文字列</span><span class="sxs-lookup"><span data-stu-id="a29f2-122">String</span></span>| <span data-ttu-id="a29f2-123">DNS ホストで SRV レコードの *name* プロパティを構成する場合に使用される値です。</span><span class="sxs-lookup"><span data-stu-id="a29f2-123">Value used when configuring the *name* property of the SRV record at the DNS host.</span></span> |
|<span data-ttu-id="a29f2-124">nameTarget</span><span class="sxs-lookup"><span data-stu-id="a29f2-124">nameTarget</span></span>|<span data-ttu-id="a29f2-125">String</span><span class="sxs-lookup"><span data-stu-id="a29f2-125">String</span></span>| <span data-ttu-id="a29f2-126">DNS ホストで SRV レコードの *Target* プロパティを構成する場合に使用する値です。</span><span class="sxs-lookup"><span data-stu-id="a29f2-126">Value to use when configuring the *Target* property of the SRV record at the DNS host.</span></span> |
|<span data-ttu-id="a29f2-127">port</span><span class="sxs-lookup"><span data-stu-id="a29f2-127">port</span></span>|<span data-ttu-id="a29f2-128">Int32</span><span class="sxs-lookup"><span data-stu-id="a29f2-128">Int32</span></span>| <span data-ttu-id="a29f2-129">DNS ホストで SRV レコードの *port* プロパティを構成する場合に使用する値です。</span><span class="sxs-lookup"><span data-stu-id="a29f2-129">Value to use when configuring the *port* property of the SRV record at the DNS host.</span></span> |
|<span data-ttu-id="a29f2-130">priority</span><span class="sxs-lookup"><span data-stu-id="a29f2-130">priority</span></span>|<span data-ttu-id="a29f2-131">Int32</span><span class="sxs-lookup"><span data-stu-id="a29f2-131">Int32</span></span>| <span data-ttu-id="a29f2-132">DNS ホストで SRV レコードの *priority* プロパティを構成する場合に使用する値です。</span><span class="sxs-lookup"><span data-stu-id="a29f2-132">Value to use when configuring the *priority* property of the SRV record at the DNS host.</span></span> |
|<span data-ttu-id="a29f2-133">protocol</span><span class="sxs-lookup"><span data-stu-id="a29f2-133">protocol</span></span>|<span data-ttu-id="a29f2-134">String</span><span class="sxs-lookup"><span data-stu-id="a29f2-134">String</span></span>| <span data-ttu-id="a29f2-135">DNS ホストで SRV レコードの *protocol* プロパティを構成する場合に使用する値です。</span><span class="sxs-lookup"><span data-stu-id="a29f2-135">Value to use when configuring the *protocol* property of the SRV record at the DNS host.</span></span> |
|<span data-ttu-id="a29f2-136">recordType</span><span class="sxs-lookup"><span data-stu-id="a29f2-136">recordType</span></span>|<span data-ttu-id="a29f2-137">String</span><span class="sxs-lookup"><span data-stu-id="a29f2-137">String</span></span>|  <span data-ttu-id="a29f2-p105">DNS レコードの種類。この値は常に *Srv* です。キー</span><span class="sxs-lookup"><span data-stu-id="a29f2-p105">Type of DNS record. The value is always *Srv*. Key</span></span> |
|<span data-ttu-id="a29f2-141">service</span><span class="sxs-lookup"><span data-stu-id="a29f2-141">service</span></span>|<span data-ttu-id="a29f2-142">String</span><span class="sxs-lookup"><span data-stu-id="a29f2-142">String</span></span>| <span data-ttu-id="a29f2-143">DNS ホストで SRV レコードの *service* プロパティを構成する場合に使用する値です。</span><span class="sxs-lookup"><span data-stu-id="a29f2-143">Value to use when configuring the *service* property of the SRV record at the DNS host.</span></span> |
|<span data-ttu-id="a29f2-144">supportedService</span><span class="sxs-lookup"><span data-stu-id="a29f2-144">supportedService</span></span>|<span data-ttu-id="a29f2-145">String</span><span class="sxs-lookup"><span data-stu-id="a29f2-145">String</span></span>| <span data-ttu-id="a29f2-146">Microsoft オンライン サービスまたはこの SRV レコードに依存している機能。</span><span class="sxs-lookup"><span data-stu-id="a29f2-146">Microsoft Online Service or feature that has a dependency on this SRV record.</span></span></br></br><span data-ttu-id="a29f2-147">次のいずれかの値を指定できます。**null**、*Email*、*Sharepoint*、*EmailInternalRelayOnly*、*OfficeCommunicationsOnline*、*SharePointDefaultDomain*、*FullRedelegation*、*SharePointPublic*、*OrgIdAuthentication*、*Yammer*、*Intune*</span><span class="sxs-lookup"><span data-stu-id="a29f2-147">Can be one of the following values: **null**, *Email*, *Sharepoint*, *EmailInternalRelayOnly*, *OfficeCommunicationsOnline*, *SharePointDefaultDomain*, *FullRedelegation*, *SharePointPublic*, *OrgIdAuthentication*, *Yammer*, *Intune*</span></span> |
|<span data-ttu-id="a29f2-148">ttl</span><span class="sxs-lookup"><span data-stu-id="a29f2-148">ttl</span></span>|<span data-ttu-id="a29f2-149">Int32</span><span class="sxs-lookup"><span data-stu-id="a29f2-149">Int32</span></span>| <span data-ttu-id="a29f2-p106">DNS ホストで SRV レコードの *Time to Live (TTL)* のプロパティを構成するときに使用する値です。null 許容ではありません</span><span class="sxs-lookup"><span data-stu-id="a29f2-p106">Value to use when configuring the *time-to-live (ttl)* property of the SRV record at the DNS host. Not nullable</span></span> |
|<span data-ttu-id="a29f2-152">weight</span><span class="sxs-lookup"><span data-stu-id="a29f2-152">weight</span></span>|<span data-ttu-id="a29f2-153">Int32</span><span class="sxs-lookup"><span data-stu-id="a29f2-153">Int32</span></span>| <span data-ttu-id="a29f2-154">DNS ホストで SRV レコードの *weight* プロパティを構成する場合に使用する値です。</span><span class="sxs-lookup"><span data-stu-id="a29f2-154">Value to use when configuring the *weight* property of the SRV record at the DNS host.</span></span> |

## <a name="relationships"></a><span data-ttu-id="a29f2-155">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="a29f2-155">Relationships</span></span>
<span data-ttu-id="a29f2-156">なし</span><span class="sxs-lookup"><span data-stu-id="a29f2-156">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="a29f2-157">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="a29f2-157">JSON representation</span></span>
<span data-ttu-id="a29f2-158">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="a29f2-158">Here is a JSON representation of the resource.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "domainDnsSrvRecord resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/domaindnssrvrecord.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
