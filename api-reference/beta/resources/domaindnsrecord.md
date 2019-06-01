---
title: domainDnsRecord リソースの種類
description: テナント内のドメインごとに、ドメインを Microsoft Online Services で使用できるようにするには、ドメインの DNS ゾーンファイルに DNS レコードを追加することが必要になることがあります。 **Domaindnsrecord**エンティティは、そのような DNS レコードを提示するために使用されます。 DomainDnsCnameRecord、DomainDnsMxRecord、DomainDnsSrvRecord、および DomainDnsSrvRecord エンティティの基本エンティティ。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 2c2bc889be77e2b324450bfd03ce28b3c53f8f51
ms.sourcegitcommit: 33f1cf5b3b79bfba6a06b52d34e558a6ba327d21
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2019
ms.locfileid: "34657092"
---
# <a name="domaindnsrecord-resource-type"></a><span data-ttu-id="02473-105">domainDnsRecord リソースの種類</span><span class="sxs-lookup"><span data-stu-id="02473-105">domainDnsRecord resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="02473-106">テナント内のドメインごとに、ドメインを Microsoft Online Services で使用できるようにするには、ドメインの DNS ゾーンファイルに DNS レコードを追加することが必要になることがあります。</span><span class="sxs-lookup"><span data-stu-id="02473-106">For each domain in the tenant, you may be required to add DNS record(s) to the DNS zone file of the domain before the domain can be used by Microsoft Online Services.</span></span> <span data-ttu-id="02473-107">**Domaindnsrecord**エンティティは、そのような DNS レコードを提示するために使用されます。</span><span class="sxs-lookup"><span data-stu-id="02473-107">The **DomainDnsRecord** entity is used to present such DNS records.</span></span> <span data-ttu-id="02473-108">[DomainDnsCnameRecord](domaindnscnamerecord.md)、 [DomainDnsMxRecord](domaindnsmxrecord.md)、 [DomainDnsSrvRecord](domaindnssrvrecord.md) 、および[DomainDnsSrvRecord](domaindnssrvrecord.md)エンティティの基本エンティティ。</span><span class="sxs-lookup"><span data-stu-id="02473-108">Base entity for [DomainDnsCnameRecord](domaindnscnamerecord.md), [DomainDnsMxRecord](domaindnsmxrecord.md), [DomainDnsSrvRecord](domaindnssrvrecord.md) and [DomainDnsSrvRecord](domaindnssrvrecord.md) entities.</span></span>

## <a name="methods"></a><span data-ttu-id="02473-109">メソッド</span><span class="sxs-lookup"><span data-stu-id="02473-109">Methods</span></span>
<span data-ttu-id="02473-110">このリソースへの直接クエリはサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="02473-110">Direct queries to this resource are not supported.</span></span> <span data-ttu-id="02473-111">ドメインサービスレコードを照会する方法については、「 [domain](domain.md) 」のトピックを参照してください。</span><span class="sxs-lookup"><span data-stu-id="02473-111">Please see the [domain](domain.md) topic for information on how to query for domain service records.</span></span>

## <a name="properties"></a><span data-ttu-id="02473-112">プロパティ</span><span class="sxs-lookup"><span data-stu-id="02473-112">Properties</span></span>
| <span data-ttu-id="02473-113">プロパティ</span><span class="sxs-lookup"><span data-stu-id="02473-113">Property</span></span>     | <span data-ttu-id="02473-114">型</span><span class="sxs-lookup"><span data-stu-id="02473-114">Type</span></span>   |<span data-ttu-id="02473-115">説明</span><span class="sxs-lookup"><span data-stu-id="02473-115">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="02473-116">id</span><span class="sxs-lookup"><span data-stu-id="02473-116">id</span></span>|<span data-ttu-id="02473-117">String</span><span class="sxs-lookup"><span data-stu-id="02473-117">String</span></span>| <span data-ttu-id="02473-118">このエンティティに割り当てられている一意の識別子。</span><span class="sxs-lookup"><span data-stu-id="02473-118">Unique identifier assigned to this entity.</span></span> <span data-ttu-id="02473-119">Null 許容ではありません。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="02473-119">Not nullable, Read-only.</span></span>|
|<span data-ttu-id="02473-120">isOptional</span><span class="sxs-lookup"><span data-stu-id="02473-120">isOptional</span></span>|<span data-ttu-id="02473-121">Boolean</span><span class="sxs-lookup"><span data-stu-id="02473-121">Boolean</span></span>| <span data-ttu-id="02473-122">False の場合、このレコードは、Microsoft Online Services がドメインで正常に動作するように、DNS ホストで顧客によって構成されている必要があります。</span><span class="sxs-lookup"><span data-stu-id="02473-122">If false, this record must be configured by the customer at the DNS host for Microsoft Online Services to operate correctly with the domain.</span></span> |
|<span data-ttu-id="02473-123">label</span><span class="sxs-lookup"><span data-stu-id="02473-123">label</span></span>|<span data-ttu-id="02473-124">String</span><span class="sxs-lookup"><span data-stu-id="02473-124">String</span></span>| <span data-ttu-id="02473-125">DNS ホストで DNS レコードの名前を構成するときに使用される値です。</span><span class="sxs-lookup"><span data-stu-id="02473-125">Value used when configuring the name of the DNS record at the DNS host.</span></span> |
|<span data-ttu-id="02473-126">recordType</span><span class="sxs-lookup"><span data-stu-id="02473-126">recordType</span></span>|<span data-ttu-id="02473-127">String</span><span class="sxs-lookup"><span data-stu-id="02473-127">String</span></span>| <span data-ttu-id="02473-128">このエンティティが表す DNS レコードの種類を示します。</span><span class="sxs-lookup"><span data-stu-id="02473-128">Indicates what type of DNS record this entity represents.</span></span></br></br><span data-ttu-id="02473-129">この値には、 *CName*、 *Mx*、 *Srv*、 *Txt*のいずれかを指定できます。</span><span class="sxs-lookup"><span data-stu-id="02473-129">The value can be one of the following: *CName*, *Mx*, *Srv*, *Txt*</span></span></br></br><span data-ttu-id="02473-130">Key</span><span class="sxs-lookup"><span data-stu-id="02473-130">Key</span></span> |
|<span data-ttu-id="02473-131">supportedService</span><span class="sxs-lookup"><span data-stu-id="02473-131">supportedService</span></span>|<span data-ttu-id="02473-132">String</span><span class="sxs-lookup"><span data-stu-id="02473-132">String</span></span>| <span data-ttu-id="02473-133">この DNS レコードに依存している Microsoft Online サービスまたは機能。</span><span class="sxs-lookup"><span data-stu-id="02473-133">Microsoft Online Service or feature that has a dependency on this DNS record.</span></span></br></br><span data-ttu-id="02473-134">**Null**、 *Email*、 *Sharepoint*、 *emailinternalrelayonly*、 *OfficeCommunicationsOnline*、 *sharepointdefaultdomain*、 *fullredelegation*、sharepointpublic のいずれかの値を使用できます。 \*\*、 *Orgidauthentication*、 *Yammer*、 *Intune*</span><span class="sxs-lookup"><span data-stu-id="02473-134">Can be one of the following values: **null**, *Email*, *Sharepoint*, *EmailInternalRelayOnly*, *OfficeCommunicationsOnline*, *SharePointDefaultDomain*, *FullRedelegation*, *SharePointPublic*, *OrgIdAuthentication*, *Yammer*, *Intune*</span></span>|
|<span data-ttu-id="02473-135">ttl</span><span class="sxs-lookup"><span data-stu-id="02473-135">ttl</span></span>|<span data-ttu-id="02473-136">Int32</span><span class="sxs-lookup"><span data-stu-id="02473-136">Int32</span></span>| <span data-ttu-id="02473-137">DNS ホストで DNS レコードの time-to-live (ttl) プロパティを構成する場合に使用する値です。</span><span class="sxs-lookup"><span data-stu-id="02473-137">Value to use when configuring the time-to-live (ttl) property of the DNS record at the DNS host.</span></span> <span data-ttu-id="02473-138">Null 許容ではない</span><span class="sxs-lookup"><span data-stu-id="02473-138">Not nullable</span></span> |

## <a name="relationships"></a><span data-ttu-id="02473-139">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="02473-139">Relationships</span></span>
<span data-ttu-id="02473-140">なし</span><span class="sxs-lookup"><span data-stu-id="02473-140">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="02473-141">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="02473-141">JSON representation</span></span>
<span data-ttu-id="02473-142">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="02473-142">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.domainDnsRecord"
}-->

```json
{
  "id": "String (identifier)",
  "isOptional": true,
  "label": "String",
  "recordType": "String",
  "supportedService": "String",
  "ttl": 1024
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "domainDnsRecord resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
