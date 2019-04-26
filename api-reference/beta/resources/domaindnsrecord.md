---
title: domaindnsrecord リソースの種類
description: テナント内のドメインごとに、ドメインを Microsoft Online Services で使用できるようにするには、ドメインの dns ゾーンファイルに dns レコードを追加することが必要になることがあります。 **domaindnsrecord**エンティティは、そのような DNS レコードを提示するために使用されます。 DomainDnsCnameRecord、DomainDnsMxRecord、DomainDnsSrvRecord、および DomainDnsSrvRecord エンティティの基本エンティティ。
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: da969956616d22f5b13041b1a7bc4ebcdb510565
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33340652"
---
# <a name="domaindnsrecord-resource-type"></a><span data-ttu-id="c892f-105">domaindnsrecord リソースの種類</span><span class="sxs-lookup"><span data-stu-id="c892f-105">domainDnsRecord resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c892f-106">テナント内のドメインごとに、ドメインを Microsoft Online Services で使用できるようにするには、ドメインの dns ゾーンファイルに dns レコードを追加することが必要になることがあります。</span><span class="sxs-lookup"><span data-stu-id="c892f-106">For each domain in the tenant, you may be required to add DNS record(s) to the DNS zone file of the domain before the domain can be used by Microsoft Online Services.</span></span> <span data-ttu-id="c892f-107">**domaindnsrecord**エンティティは、そのような DNS レコードを提示するために使用されます。</span><span class="sxs-lookup"><span data-stu-id="c892f-107">The **DomainDnsRecord** entity is used to present such DNS records.</span></span> <span data-ttu-id="c892f-108">[DomainDnsCnameRecord](domaindnscnamerecord.md)、 [DomainDnsMxRecord](domaindnsmxrecord.md)、 [DomainDnsSrvRecord](domaindnssrvrecord.md) 、および[DomainDnsSrvRecord](domaindnssrvrecord.md)エンティティの基本エンティティ。</span><span class="sxs-lookup"><span data-stu-id="c892f-108">Base entity for [DomainDnsCnameRecord](domaindnscnamerecord.md), [DomainDnsMxRecord](domaindnsmxrecord.md), [DomainDnsSrvRecord](domaindnssrvrecord.md) and [DomainDnsSrvRecord](domaindnssrvrecord.md) entities.</span></span>

## <a name="methods"></a><span data-ttu-id="c892f-109">メソッド</span><span class="sxs-lookup"><span data-stu-id="c892f-109">Methods</span></span>
<span data-ttu-id="c892f-110">このリソースへの直接クエリはサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c892f-110">Direct queries to this resource are not supported.</span></span> <span data-ttu-id="c892f-111">ドメインサービスレコードを照会する方法については、「 [domain](domain.md) 」のトピックを参照してください。</span><span class="sxs-lookup"><span data-stu-id="c892f-111">Please see the [domain](domain.md) topic for information on how to query for domain service records.</span></span>

## <a name="properties"></a><span data-ttu-id="c892f-112">プロパティ</span><span class="sxs-lookup"><span data-stu-id="c892f-112">Properties</span></span>
| <span data-ttu-id="c892f-113">プロパティ</span><span class="sxs-lookup"><span data-stu-id="c892f-113">Property</span></span>     | <span data-ttu-id="c892f-114">型</span><span class="sxs-lookup"><span data-stu-id="c892f-114">Type</span></span>   |<span data-ttu-id="c892f-115">説明</span><span class="sxs-lookup"><span data-stu-id="c892f-115">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c892f-116">id</span><span class="sxs-lookup"><span data-stu-id="c892f-116">id</span></span>|<span data-ttu-id="c892f-117">String</span><span class="sxs-lookup"><span data-stu-id="c892f-117">String</span></span>| <span data-ttu-id="c892f-118">このエンティティに割り当てられている一意の識別子。</span><span class="sxs-lookup"><span data-stu-id="c892f-118">Unique identifier assigned to this entity.</span></span> <span data-ttu-id="c892f-119">null 許容ではありません。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="c892f-119">Not nullable, Read-only.</span></span>|
|<span data-ttu-id="c892f-120">isoptional</span><span class="sxs-lookup"><span data-stu-id="c892f-120">isOptional</span></span>|<span data-ttu-id="c892f-121">Boolean</span><span class="sxs-lookup"><span data-stu-id="c892f-121">Boolean</span></span>| <span data-ttu-id="c892f-122">false の場合、このレコードは、Microsoft Online Services がドメインで正常に動作するように、DNS ホストで顧客によって構成されている必要があります。</span><span class="sxs-lookup"><span data-stu-id="c892f-122">If false, this record must be configured by the customer at the DNS host for Microsoft Online Services to operate correctly with the domain.</span></span> |
|<span data-ttu-id="c892f-123">label</span><span class="sxs-lookup"><span data-stu-id="c892f-123">label</span></span>|<span data-ttu-id="c892f-124">String</span><span class="sxs-lookup"><span data-stu-id="c892f-124">String</span></span>| <span data-ttu-id="c892f-125">dns ホストで dns レコードの名前を構成するときに使用される値です。</span><span class="sxs-lookup"><span data-stu-id="c892f-125">Value used when configuring the name of the DNS record at the DNS host.</span></span> |
|<span data-ttu-id="c892f-126">recordType</span><span class="sxs-lookup"><span data-stu-id="c892f-126">recordType</span></span>|<span data-ttu-id="c892f-127">String</span><span class="sxs-lookup"><span data-stu-id="c892f-127">String</span></span>| <span data-ttu-id="c892f-128">このエンティティが表す DNS レコードの種類を示します。</span><span class="sxs-lookup"><span data-stu-id="c892f-128">Indicates what type of DNS record this entity represents.</span></span></br></br><span data-ttu-id="c892f-129">この値には、 *CName*、 *Mx*、 *Srv*、 *Txt*のいずれかを指定できます。</span><span class="sxs-lookup"><span data-stu-id="c892f-129">The value can be one of the following: *CName*, *Mx*, *Srv*, *Txt*</span></span></br></br><span data-ttu-id="c892f-130">Key</span><span class="sxs-lookup"><span data-stu-id="c892f-130">Key</span></span> |
|<span data-ttu-id="c892f-131">supportedservice</span><span class="sxs-lookup"><span data-stu-id="c892f-131">supportedService</span></span>|<span data-ttu-id="c892f-132">String</span><span class="sxs-lookup"><span data-stu-id="c892f-132">String</span></span>| <span data-ttu-id="c892f-133">この DNS レコードに依存している Microsoft Online サービスまたは機能。</span><span class="sxs-lookup"><span data-stu-id="c892f-133">Microsoft Online Service or feature that has a dependency on this DNS record.</span></span></br></br><span data-ttu-id="c892f-134">**null**、 *Email*、 *Sharepoint*、 *emailinternalrelayonly*、 *OfficeCommunicationsOnline*、 *sharepointdefaultdomain*、 *fullredelegation*、sharepointpublic のいずれかの値を使用できます。 \*\*、 *orgidauthentication*、 *Yammer*、 *Intune*</span><span class="sxs-lookup"><span data-stu-id="c892f-134">Can be one of the following values: **null**, *Email*, *Sharepoint*, *EmailInternalRelayOnly*, *OfficeCommunicationsOnline*, *SharePointDefaultDomain*, *FullRedelegation*, *SharePointPublic*, *OrgIdAuthentication*, *Yammer*, *Intune*</span></span>|
|<span data-ttu-id="c892f-135">ttl</span><span class="sxs-lookup"><span data-stu-id="c892f-135">ttl</span></span>|<span data-ttu-id="c892f-136">Int32</span><span class="sxs-lookup"><span data-stu-id="c892f-136">Int32</span></span>| <span data-ttu-id="c892f-137">dns ホストで dns レコードの time-to-live (ttl) プロパティを構成する場合に使用する値です。</span><span class="sxs-lookup"><span data-stu-id="c892f-137">Value to use when configuring the time-to-live (ttl) property of the DNS record at the DNS host.</span></span> <span data-ttu-id="c892f-138">null 許容ではない</span><span class="sxs-lookup"><span data-stu-id="c892f-138">Not nullable</span></span> |

## <a name="relationships"></a><span data-ttu-id="c892f-139">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="c892f-139">Relationships</span></span>
<span data-ttu-id="c892f-140">なし</span><span class="sxs-lookup"><span data-stu-id="c892f-140">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="c892f-141">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="c892f-141">JSON representation</span></span>
<span data-ttu-id="c892f-142">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="c892f-142">Here is a JSON representation of the resource.</span></span>

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
