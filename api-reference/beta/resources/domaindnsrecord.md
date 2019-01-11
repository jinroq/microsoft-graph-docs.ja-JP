---
title: domainDnsRecord リソースの種類
description: テナント内の各ドメインのドメインは、Microsoft Online Services で使用できるようにするドメインの DNS ゾーン ファイルを DNS レコードを追加する必要があります。 **DomainDnsRecord**エンティティを使用して、このような DNS レコードを表示します。 DomainDnsCnameRecord、DomainDnsMxRecord、DomainDnsSrvRecord および DomainDnsSrvRecord のエンティティの基本エンティティです。
localization_priority: Normal
ms.openlocfilehash: 194e25ca78a1937415b15f455e98ac526c4fb4be
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27811411"
---
# <a name="domaindnsrecord-resource-type"></a><span data-ttu-id="d3c2b-105">domainDnsRecord リソースの種類</span><span class="sxs-lookup"><span data-stu-id="d3c2b-105">domainDnsRecord resource type</span></span>

> <span data-ttu-id="d3c2b-106">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="d3c2b-106">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d3c2b-107">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d3c2b-107">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="d3c2b-p103">テナント内の各ドメインでは、Microsoft オンライン サービスでドメインを使用できるようにするために、DNS レコードをそのドメインの DNS ゾーン ファイルに追加しなければならない場合があります。**DomainDnsRecord** エンティティはこのような DNS レコードの表示に使用されます。[DomainDnsCnameRecord](domaindnscnamerecord.md)、[DomainDnsMxRecord](domaindnsmxrecord.md)、[DomainDnsSrvRecord](domaindnssrvrecord.md)、[DomainDnsSrvRecord](domaindnssrvrecord.md) エンティティのベース エンティティ。</span><span class="sxs-lookup"><span data-stu-id="d3c2b-p103">For each domain in the tenant, you may be required to add DNS record(s) to the DNS zone file of the domain before the domain can be used by Microsoft Online Services. The **DomainDnsRecord** entity is used to present such DNS records. Base entity for [DomainDnsCnameRecord](domaindnscnamerecord.md), [DomainDnsMxRecord](domaindnsmxrecord.md), [DomainDnsSrvRecord](domaindnssrvrecord.md) and [DomainDnsSrvRecord](domaindnssrvrecord.md) entities.</span></span>

## <a name="methods"></a><span data-ttu-id="d3c2b-111">メソッド</span><span class="sxs-lookup"><span data-stu-id="d3c2b-111">Methods</span></span>
<span data-ttu-id="d3c2b-p104">このリソースへの直接クエリはサポートされていません。ドメイン サービス レコードのクエリを実行する方法の詳細については、[ドメイン](domain.md)のトピックを参照してください。</span><span class="sxs-lookup"><span data-stu-id="d3c2b-p104">Direct queries to this resource are not supported. Please see the [domain](domain.md) topic for information on how to query for domain service records.</span></span>

## <a name="properties"></a><span data-ttu-id="d3c2b-114">プロパティ</span><span class="sxs-lookup"><span data-stu-id="d3c2b-114">Properties</span></span>
| <span data-ttu-id="d3c2b-115">プロパティ</span><span class="sxs-lookup"><span data-stu-id="d3c2b-115">Property</span></span>     | <span data-ttu-id="d3c2b-116">種類</span><span class="sxs-lookup"><span data-stu-id="d3c2b-116">Type</span></span>   |<span data-ttu-id="d3c2b-117">説明</span><span class="sxs-lookup"><span data-stu-id="d3c2b-117">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d3c2b-118">ID</span><span class="sxs-lookup"><span data-stu-id="d3c2b-118">id</span></span>|<span data-ttu-id="d3c2b-119">String</span><span class="sxs-lookup"><span data-stu-id="d3c2b-119">String</span></span>| <span data-ttu-id="d3c2b-p105">このエンティティに割り当てられた一意の識別子。null 許容ではありません。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="d3c2b-p105">Unique identifier assigned to this entity. Not nullable, Read-only.</span></span>|
|<span data-ttu-id="d3c2b-122">isOptional</span><span class="sxs-lookup"><span data-stu-id="d3c2b-122">isOptional</span></span>|<span data-ttu-id="d3c2b-123">Boolean</span><span class="sxs-lookup"><span data-stu-id="d3c2b-123">Boolean</span></span>| <span data-ttu-id="d3c2b-124">False の場合、このレコードは Microsoft オンライン サービスでドメインを正しく操作するために、DNS ホストで顧客によって構成されている必要があります。</span><span class="sxs-lookup"><span data-stu-id="d3c2b-124">If false, this record must be configured by the customer at the DNS host for Microsoft Online Services to operate correctly with the domain.</span></span> |
|<span data-ttu-id="d3c2b-125">label</span><span class="sxs-lookup"><span data-stu-id="d3c2b-125">label</span></span>|<span data-ttu-id="d3c2b-126">String</span><span class="sxs-lookup"><span data-stu-id="d3c2b-126">String</span></span>| <span data-ttu-id="d3c2b-127">DNS ホストで DNS レコードの名前を設定するときに使用する値。</span><span class="sxs-lookup"><span data-stu-id="d3c2b-127">Value used when configuring the name of the DNS record at the DNS host.</span></span> |
|<span data-ttu-id="d3c2b-128">recordType</span><span class="sxs-lookup"><span data-stu-id="d3c2b-128">recordType</span></span>|<span data-ttu-id="d3c2b-129">String</span><span class="sxs-lookup"><span data-stu-id="d3c2b-129">String</span></span>| <span data-ttu-id="d3c2b-130">このエンティティが表す DNS レコードの種類を示します。</span><span class="sxs-lookup"><span data-stu-id="d3c2b-130">Indicates what type of DNS record this entity represents.</span></span></br></br><span data-ttu-id="d3c2b-131">値は次のいずれかを指定できます。*CName*、*Mx*、*Srv*、*Txt*</span><span class="sxs-lookup"><span data-stu-id="d3c2b-131">The value can be one of the following: *CName*, *Mx*, *Srv*, *Txt*</span></span></br></br><span data-ttu-id="d3c2b-132">キー</span><span class="sxs-lookup"><span data-stu-id="d3c2b-132">Key</span></span> |
|<span data-ttu-id="d3c2b-133">supportedService</span><span class="sxs-lookup"><span data-stu-id="d3c2b-133">supportedService</span></span>|<span data-ttu-id="d3c2b-134">String</span><span class="sxs-lookup"><span data-stu-id="d3c2b-134">String</span></span>| <span data-ttu-id="d3c2b-135">Microsoft オンライン サービスまたはこの DNS レコードに依存している機能。</span><span class="sxs-lookup"><span data-stu-id="d3c2b-135">Microsoft Online Service or feature that has a dependency on this DNS record.</span></span></br></br><span data-ttu-id="d3c2b-136">次のいずれかの値を指定できます。**null**、*Email*、*Sharepoint*、*EmailInternalRelayOnly*、*OfficeCommunicationsOnline*、*SharePointDefaultDomain*、*FullRedelegation*、*SharePointPublic*、*OrgIdAuthentication*、*Yammer*、*Intune*</span><span class="sxs-lookup"><span data-stu-id="d3c2b-136">Can be one of the following values: **null**, *Email*, *Sharepoint*, *EmailInternalRelayOnly*, *OfficeCommunicationsOnline*, *SharePointDefaultDomain*, *FullRedelegation*, *SharePointPublic*, *OrgIdAuthentication*, *Yammer*, *Intune*</span></span>|
|<span data-ttu-id="d3c2b-137">ttl</span><span class="sxs-lookup"><span data-stu-id="d3c2b-137">ttl</span></span>|<span data-ttu-id="d3c2b-138">Int32</span><span class="sxs-lookup"><span data-stu-id="d3c2b-138">Int32</span></span>| <span data-ttu-id="d3c2b-p106">DNS ホストの DNS レコードの Time to Live (TTL) のプロパティを構成するときに使用する値です。null 許容ではありません</span><span class="sxs-lookup"><span data-stu-id="d3c2b-p106">Value to use when configuring the time-to-live (ttl) property of the DNS record at the DNS host. Not nullable</span></span> |

## <a name="relationships"></a><span data-ttu-id="d3c2b-141">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="d3c2b-141">Relationships</span></span>
<span data-ttu-id="d3c2b-142">なし</span><span class="sxs-lookup"><span data-stu-id="d3c2b-142">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="d3c2b-143">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="d3c2b-143">JSON representation</span></span>
<span data-ttu-id="d3c2b-144">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="d3c2b-144">Here is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "domainDnsRecord resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
