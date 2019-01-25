---
title: domainDnsRecord リソースの種類
description: テナント内の各ドメインでは、Microsoft オンライン サービスでドメインを使用できるようにするために、DNS レコードをそのドメインの DNS ゾーン ファイルに追加しなければならない場合があります。**DomainDnsRecord** エンティティはこのような DNS レコードの表示に使用されます。DomainDnsCnameRecord、DomainDnsMxRecord、DomainDnsSrvRecord、DomainDnsSrvRecord エンティティのベース エンティティ。
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: b7b04e65da67bc61e3f3b91ed3dae7cba70a3d27
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29519284"
---
# <a name="domaindnsrecord-resource-type"></a><span data-ttu-id="d7397-105">domainDnsRecord リソースの種類</span><span class="sxs-lookup"><span data-stu-id="d7397-105">domainDnsRecord resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d7397-p102">テナント内の各ドメインでは、Microsoft オンライン サービスでドメインを使用できるようにするために、DNS レコードをそのドメインの DNS ゾーン ファイルに追加しなければならない場合があります。**DomainDnsRecord** エンティティはこのような DNS レコードの表示に使用されます。[DomainDnsCnameRecord](domaindnscnamerecord.md)、[DomainDnsMxRecord](domaindnsmxrecord.md)、[DomainDnsSrvRecord](domaindnssrvrecord.md)、[DomainDnsSrvRecord](domaindnssrvrecord.md) エンティティのベース エンティティ。</span><span class="sxs-lookup"><span data-stu-id="d7397-p102">For each domain in the tenant, you may be required to add DNS record(s) to the DNS zone file of the domain before the domain can be used by Microsoft Online Services. The **DomainDnsRecord** entity is used to present such DNS records. Base entity for [DomainDnsCnameRecord](domaindnscnamerecord.md), [DomainDnsMxRecord](domaindnsmxrecord.md), [DomainDnsSrvRecord](domaindnssrvrecord.md) and [DomainDnsSrvRecord](domaindnssrvrecord.md) entities.</span></span>

## <a name="methods"></a><span data-ttu-id="d7397-109">メソッド</span><span class="sxs-lookup"><span data-stu-id="d7397-109">Methods</span></span>
<span data-ttu-id="d7397-p103">このリソースへの直接クエリはサポートされていません。ドメイン サービス レコードのクエリを実行する方法の詳細については、[ドメイン](domain.md)のトピックを参照してください。</span><span class="sxs-lookup"><span data-stu-id="d7397-p103">Direct queries to this resource are not supported. Please see the [domain](domain.md) topic for information on how to query for domain service records.</span></span>

## <a name="properties"></a><span data-ttu-id="d7397-112">プロパティ</span><span class="sxs-lookup"><span data-stu-id="d7397-112">Properties</span></span>
| <span data-ttu-id="d7397-113">プロパティ</span><span class="sxs-lookup"><span data-stu-id="d7397-113">Property</span></span>     | <span data-ttu-id="d7397-114">型</span><span class="sxs-lookup"><span data-stu-id="d7397-114">Type</span></span>   |<span data-ttu-id="d7397-115">説明</span><span class="sxs-lookup"><span data-stu-id="d7397-115">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d7397-116">id</span><span class="sxs-lookup"><span data-stu-id="d7397-116">id</span></span>|<span data-ttu-id="d7397-117">String</span><span class="sxs-lookup"><span data-stu-id="d7397-117">String</span></span>| <span data-ttu-id="d7397-p104">このエンティティに割り当てられた一意の識別子。null 許容ではありません。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="d7397-p104">Unique identifier assigned to this entity. Not nullable, Read-only.</span></span>|
|<span data-ttu-id="d7397-120">isOptional</span><span class="sxs-lookup"><span data-stu-id="d7397-120">isOptional</span></span>|<span data-ttu-id="d7397-121">Boolean</span><span class="sxs-lookup"><span data-stu-id="d7397-121">Boolean</span></span>| <span data-ttu-id="d7397-122">False の場合、このレコードは Microsoft オンライン サービスでドメインを正しく操作するために、DNS ホストで顧客によって構成されている必要があります。</span><span class="sxs-lookup"><span data-stu-id="d7397-122">If false, this record must be configured by the customer at the DNS host for Microsoft Online Services to operate correctly with the domain.</span></span> |
|<span data-ttu-id="d7397-123">label</span><span class="sxs-lookup"><span data-stu-id="d7397-123">label</span></span>|<span data-ttu-id="d7397-124">文字列</span><span class="sxs-lookup"><span data-stu-id="d7397-124">String</span></span>| <span data-ttu-id="d7397-125">DNS ホストで DNS レコードの名前を設定するときに使用する値。</span><span class="sxs-lookup"><span data-stu-id="d7397-125">Value used when configuring the name of the DNS record at the DNS host.</span></span> |
|<span data-ttu-id="d7397-126">recordType</span><span class="sxs-lookup"><span data-stu-id="d7397-126">recordType</span></span>|<span data-ttu-id="d7397-127">String</span><span class="sxs-lookup"><span data-stu-id="d7397-127">String</span></span>| <span data-ttu-id="d7397-128">このエンティティが表す DNS レコードの種類を示します。</span><span class="sxs-lookup"><span data-stu-id="d7397-128">Indicates what type of DNS record this entity represents.</span></span></br></br><span data-ttu-id="d7397-129">値は次のいずれかを指定できます。*CName*、*Mx*、*Srv*、*Txt*</span><span class="sxs-lookup"><span data-stu-id="d7397-129">The value can be one of the following: *CName*, *Mx*, *Srv*, *Txt*</span></span></br></br><span data-ttu-id="d7397-130">キー</span><span class="sxs-lookup"><span data-stu-id="d7397-130">Key</span></span> |
|<span data-ttu-id="d7397-131">supportedService</span><span class="sxs-lookup"><span data-stu-id="d7397-131">supportedService</span></span>|<span data-ttu-id="d7397-132">String</span><span class="sxs-lookup"><span data-stu-id="d7397-132">String</span></span>| <span data-ttu-id="d7397-133">Microsoft オンライン サービスまたはこの DNS レコードに依存している機能。</span><span class="sxs-lookup"><span data-stu-id="d7397-133">Microsoft Online Service or feature that has a dependency on this DNS record.</span></span></br></br><span data-ttu-id="d7397-134">次のいずれかの値を指定できます。**null**、*Email*、*Sharepoint*、*EmailInternalRelayOnly*、*OfficeCommunicationsOnline*、*SharePointDefaultDomain*、*FullRedelegation*、*SharePointPublic*、*OrgIdAuthentication*、*Yammer*、*Intune*</span><span class="sxs-lookup"><span data-stu-id="d7397-134">Can be one of the following values: **null**, *Email*, *Sharepoint*, *EmailInternalRelayOnly*, *OfficeCommunicationsOnline*, *SharePointDefaultDomain*, *FullRedelegation*, *SharePointPublic*, *OrgIdAuthentication*, *Yammer*, *Intune*</span></span>|
|<span data-ttu-id="d7397-135">ttl</span><span class="sxs-lookup"><span data-stu-id="d7397-135">ttl</span></span>|<span data-ttu-id="d7397-136">Int32</span><span class="sxs-lookup"><span data-stu-id="d7397-136">Int32</span></span>| <span data-ttu-id="d7397-p105">DNS ホストの DNS レコードの Time to Live (TTL) のプロパティを構成するときに使用する値です。null 許容ではありません</span><span class="sxs-lookup"><span data-stu-id="d7397-p105">Value to use when configuring the time-to-live (ttl) property of the DNS record at the DNS host. Not nullable</span></span> |

## <a name="relationships"></a><span data-ttu-id="d7397-139">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="d7397-139">Relationships</span></span>
<span data-ttu-id="d7397-140">なし</span><span class="sxs-lookup"><span data-stu-id="d7397-140">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="d7397-141">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="d7397-141">JSON representation</span></span>
<span data-ttu-id="d7397-142">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="d7397-142">Here is a JSON representation of the resource.</span></span>

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
  "suppressions": [
    "Error: /api-reference/beta/resources/domaindnsrecord.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
