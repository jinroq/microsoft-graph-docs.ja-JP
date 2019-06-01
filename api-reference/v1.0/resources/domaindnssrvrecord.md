---
title: domainDnsSrvRecord リソースの種類
description: テナント内の特定のドメインの DNS ゾーンファイルに追加される SRV レコードを表します。 DomainDnsRecord エンティティから継承されます。
author: davidmu1
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 1e7563d90a92e319ceec5a5ca11d7edb4f267c5b
ms.sourcegitcommit: 33f1cf5b3b79bfba6a06b52d34e558a6ba327d21
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2019
ms.locfileid: "34657666"
---
# <a name="domaindnssrvrecord-resource-type"></a><span data-ttu-id="b4bfa-104">domainDnsSrvRecord リソースの種類</span><span class="sxs-lookup"><span data-stu-id="b4bfa-104">domainDnsSrvRecord resource type</span></span>

<span data-ttu-id="b4bfa-105">テナント内の特定のドメインの DNS ゾーンファイルに追加される SRV レコードを表します。</span><span class="sxs-lookup"><span data-stu-id="b4bfa-105">Represents a SRV record added to the DNS zone file of a particular domain in the tenant.</span></span> <span data-ttu-id="b4bfa-106">[Domaindnsrecord](domaindnsrecord.md)エンティティから継承されます。</span><span class="sxs-lookup"><span data-stu-id="b4bfa-106">Inherited from [DomainDnsRecord](domaindnsrecord.md) entity.</span></span>

## <a name="methods"></a><span data-ttu-id="b4bfa-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="b4bfa-107">Methods</span></span>
<span data-ttu-id="b4bfa-108">このリソースへの直接クエリはサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b4bfa-108">Direct queries to this resource are not supported.</span></span> <span data-ttu-id="b4bfa-109">ドメインサービスレコードを照会する方法については、「 [domain](domain.md) 」のトピックを参照してください。</span><span class="sxs-lookup"><span data-stu-id="b4bfa-109">Please see the [domain](domain.md) topic for information on how to query for domain service records.</span></span>

## <a name="properties"></a><span data-ttu-id="b4bfa-110">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b4bfa-110">Properties</span></span>
| <span data-ttu-id="b4bfa-111">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b4bfa-111">Property</span></span>     | <span data-ttu-id="b4bfa-112">型</span><span class="sxs-lookup"><span data-stu-id="b4bfa-112">Type</span></span>   |<span data-ttu-id="b4bfa-113">説明</span><span class="sxs-lookup"><span data-stu-id="b4bfa-113">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b4bfa-114">id</span><span class="sxs-lookup"><span data-stu-id="b4bfa-114">id</span></span>|<span data-ttu-id="b4bfa-115">String</span><span class="sxs-lookup"><span data-stu-id="b4bfa-115">String</span></span>| <span data-ttu-id="b4bfa-116">このエンティティに割り当てられている一意の識別子。</span><span class="sxs-lookup"><span data-stu-id="b4bfa-116">Unique identifier assigned to this entity.</span></span> <span data-ttu-id="b4bfa-117">Null 許容ではありません。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="b4bfa-117">Not nullable, Read-only.</span></span>|
|<span data-ttu-id="b4bfa-118">isOptional</span><span class="sxs-lookup"><span data-stu-id="b4bfa-118">isOptional</span></span>|<span data-ttu-id="b4bfa-119">Boolean</span><span class="sxs-lookup"><span data-stu-id="b4bfa-119">Boolean</span></span>| <span data-ttu-id="b4bfa-120">False の場合、SRV レコードは、Microsoft Online Services がドメインで正常に動作するように、DNS ホストで顧客によって構成されている必要があります。</span><span class="sxs-lookup"><span data-stu-id="b4bfa-120">If false, the SRV record must be configured by the customer at the DNS host for Microsoft Online Services to operate correctly with the domain.</span></span> |
|<span data-ttu-id="b4bfa-121">label</span><span class="sxs-lookup"><span data-stu-id="b4bfa-121">label</span></span>|<span data-ttu-id="b4bfa-122">String</span><span class="sxs-lookup"><span data-stu-id="b4bfa-122">String</span></span>| <span data-ttu-id="b4bfa-123">DNS ホストで SRV レコードの*name*プロパティを構成する場合に使用される値です。</span><span class="sxs-lookup"><span data-stu-id="b4bfa-123">Value used when configuring the *name* property of the SRV record at the DNS host.</span></span> |
|<span data-ttu-id="b4bfa-124">nameTarget</span><span class="sxs-lookup"><span data-stu-id="b4bfa-124">nameTarget</span></span>|<span data-ttu-id="b4bfa-125">String</span><span class="sxs-lookup"><span data-stu-id="b4bfa-125">String</span></span>| <span data-ttu-id="b4bfa-126">DNS ホストで SRV レコードの*Target*プロパティを構成する場合に使用する値です。</span><span class="sxs-lookup"><span data-stu-id="b4bfa-126">Value to use when configuring the *Target* property of the SRV record at the DNS host.</span></span> |
|<span data-ttu-id="b4bfa-127">ポート</span><span class="sxs-lookup"><span data-stu-id="b4bfa-127">port</span></span>|<span data-ttu-id="b4bfa-128">Int32</span><span class="sxs-lookup"><span data-stu-id="b4bfa-128">Int32</span></span>| <span data-ttu-id="b4bfa-129">DNS ホストで SRV レコードの*port*プロパティを構成する場合に使用する値です。</span><span class="sxs-lookup"><span data-stu-id="b4bfa-129">Value to use when configuring the *port* property of the SRV record at the DNS host.</span></span> |
|<span data-ttu-id="b4bfa-130">priority</span><span class="sxs-lookup"><span data-stu-id="b4bfa-130">priority</span></span>|<span data-ttu-id="b4bfa-131">Int32</span><span class="sxs-lookup"><span data-stu-id="b4bfa-131">Int32</span></span>| <span data-ttu-id="b4bfa-132">DNS ホストで SRV レコードの*priority*プロパティを構成する場合に使用する値です。</span><span class="sxs-lookup"><span data-stu-id="b4bfa-132">Value to use when configuring the *priority* property of the SRV record at the DNS host.</span></span> |
|<span data-ttu-id="b4bfa-133">プロトコール</span><span class="sxs-lookup"><span data-stu-id="b4bfa-133">protocol</span></span>|<span data-ttu-id="b4bfa-134">String</span><span class="sxs-lookup"><span data-stu-id="b4bfa-134">String</span></span>| <span data-ttu-id="b4bfa-135">DNS ホストで SRV レコードの*protocol*プロパティを構成する場合に使用する値です。</span><span class="sxs-lookup"><span data-stu-id="b4bfa-135">Value to use when configuring the *protocol* property of the SRV record at the DNS host.</span></span> |
|<span data-ttu-id="b4bfa-136">recordType</span><span class="sxs-lookup"><span data-stu-id="b4bfa-136">recordType</span></span>|<span data-ttu-id="b4bfa-137">String</span><span class="sxs-lookup"><span data-stu-id="b4bfa-137">String</span></span>|  <span data-ttu-id="b4bfa-138">DNS レコードの種類。</span><span class="sxs-lookup"><span data-stu-id="b4bfa-138">Type of DNS record.</span></span> <span data-ttu-id="b4bfa-139">値は常に*Srv*です。</span><span class="sxs-lookup"><span data-stu-id="b4bfa-139">The value is always *Srv*.</span></span> <span data-ttu-id="b4bfa-140">Key</span><span class="sxs-lookup"><span data-stu-id="b4bfa-140">Key</span></span> |
|<span data-ttu-id="b4bfa-141">service</span><span class="sxs-lookup"><span data-stu-id="b4bfa-141">service</span></span>|<span data-ttu-id="b4bfa-142">String</span><span class="sxs-lookup"><span data-stu-id="b4bfa-142">String</span></span>| <span data-ttu-id="b4bfa-143">DNS ホストで SRV レコードの*service*プロパティを構成する場合に使用する値です。</span><span class="sxs-lookup"><span data-stu-id="b4bfa-143">Value to use when configuring the *service* property of the SRV record at the DNS host.</span></span> |
|<span data-ttu-id="b4bfa-144">supportedService</span><span class="sxs-lookup"><span data-stu-id="b4bfa-144">supportedService</span></span>|<span data-ttu-id="b4bfa-145">String</span><span class="sxs-lookup"><span data-stu-id="b4bfa-145">String</span></span>| <span data-ttu-id="b4bfa-146">この SRV レコードに依存している Microsoft Online サービスまたは機能。</span><span class="sxs-lookup"><span data-stu-id="b4bfa-146">Microsoft Online Service or feature that has a dependency on this SRV record.</span></span></br></br><span data-ttu-id="b4bfa-147">**Null**、 *Email*、 *Sharepoint*、 *emailinternalrelayonly*、 *OfficeCommunicationsOnline*、 *sharepointdefaultdomain*、 *fullredelegation*、sharepointpublic のいずれかの値を使用できます。 \*\*、 *Orgidauthentication*、 *Yammer*、 *Intune*</span><span class="sxs-lookup"><span data-stu-id="b4bfa-147">Can be one of the following values: **null**, *Email*, *Sharepoint*, *EmailInternalRelayOnly*, *OfficeCommunicationsOnline*, *SharePointDefaultDomain*, *FullRedelegation*, *SharePointPublic*, *OrgIdAuthentication*, *Yammer*, *Intune*</span></span> |
|<span data-ttu-id="b4bfa-148">ttl</span><span class="sxs-lookup"><span data-stu-id="b4bfa-148">ttl</span></span>|<span data-ttu-id="b4bfa-149">Int32</span><span class="sxs-lookup"><span data-stu-id="b4bfa-149">Int32</span></span>| <span data-ttu-id="b4bfa-150">DNS ホストで SRV レコードの*タイムツーリブ (ttl)* プロパティを構成する場合に使用する値です。</span><span class="sxs-lookup"><span data-stu-id="b4bfa-150">Value to use when configuring the *time-to-live (ttl)* property of the SRV record at the DNS host.</span></span> <span data-ttu-id="b4bfa-151">Null 許容ではない</span><span class="sxs-lookup"><span data-stu-id="b4bfa-151">Not nullable</span></span> |
|<span data-ttu-id="b4bfa-152">weight</span><span class="sxs-lookup"><span data-stu-id="b4bfa-152">weight</span></span>|<span data-ttu-id="b4bfa-153">Int32</span><span class="sxs-lookup"><span data-stu-id="b4bfa-153">Int32</span></span>| <span data-ttu-id="b4bfa-154">DNS ホストで SRV レコードの*weight*プロパティを構成する場合に使用する値です。</span><span class="sxs-lookup"><span data-stu-id="b4bfa-154">Value to use when configuring the *weight* property of the SRV record at the DNS host.</span></span> |

## <a name="relationships"></a><span data-ttu-id="b4bfa-155">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="b4bfa-155">Relationships</span></span>
<span data-ttu-id="b4bfa-156">なし</span><span class="sxs-lookup"><span data-stu-id="b4bfa-156">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="b4bfa-157">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="b4bfa-157">JSON representation</span></span>
<span data-ttu-id="b4bfa-158">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="b4bfa-158">Here is a JSON representation of the resource.</span></span>

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
