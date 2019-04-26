---
title: domainDnsCnameRecord リソースの種類
description: テナント内の特定のドメインの DNS ゾーンファイルに追加された CNAME レコードを表します。 domaindnsrecord エンティティから継承されます。
author: lleonard-msft
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: fb730cafd1689ab95563fa1e4dd6ea23962af903
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33340698"
---
# <a name="domaindnscnamerecord-resource-type"></a><span data-ttu-id="319a1-104">domainDnsCnameRecord リソースの種類</span><span class="sxs-lookup"><span data-stu-id="319a1-104">domainDnsCnameRecord resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="319a1-105">テナント内の特定のドメインの DNS ゾーンファイルに追加された CNAME レコードを表します。</span><span class="sxs-lookup"><span data-stu-id="319a1-105">Represents a CNAME record added to the DNS zone file of a particular domain in the tenant.</span></span> <span data-ttu-id="319a1-106">[domaindnsrecord](domaindnsrecord.md)エンティティから継承されます。</span><span class="sxs-lookup"><span data-stu-id="319a1-106">Inherited from [DomainDnsRecord](domaindnsrecord.md) entity.</span></span>


## <a name="methods"></a><span data-ttu-id="319a1-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="319a1-107">Methods</span></span>
<span data-ttu-id="319a1-108">このリソースへの直接クエリはサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="319a1-108">Direct queries to this resource are not supported.</span></span> <span data-ttu-id="319a1-109">ドメインサービスレコードを照会する方法については、「 [domain](domain.md) 」のトピックを参照してください。</span><span class="sxs-lookup"><span data-stu-id="319a1-109">Please see the [domain](domain.md) topic for information on how to query for domain service records.</span></span>

## <a name="properties"></a><span data-ttu-id="319a1-110">プロパティ</span><span class="sxs-lookup"><span data-stu-id="319a1-110">Properties</span></span>
| <span data-ttu-id="319a1-111">プロパティ</span><span class="sxs-lookup"><span data-stu-id="319a1-111">Property</span></span>     | <span data-ttu-id="319a1-112">型</span><span class="sxs-lookup"><span data-stu-id="319a1-112">Type</span></span>   |<span data-ttu-id="319a1-113">説明</span><span class="sxs-lookup"><span data-stu-id="319a1-113">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="319a1-114">canonicalName</span><span class="sxs-lookup"><span data-stu-id="319a1-114">canonicalName</span></span>|<span data-ttu-id="319a1-115">String</span><span class="sxs-lookup"><span data-stu-id="319a1-115">String</span></span>| <span data-ttu-id="319a1-116">CNAME レコードの標準名。</span><span class="sxs-lookup"><span data-stu-id="319a1-116">The canonical name of the CNAME record.</span></span> <span data-ttu-id="319a1-117">DNS ホストで CNAME レコードを構成するために使用します。</span><span class="sxs-lookup"><span data-stu-id="319a1-117">Used to configure the CNAME record at the DNS host.</span></span> |
|<span data-ttu-id="319a1-118">id</span><span class="sxs-lookup"><span data-stu-id="319a1-118">id</span></span>|<span data-ttu-id="319a1-119">String</span><span class="sxs-lookup"><span data-stu-id="319a1-119">String</span></span>| <span data-ttu-id="319a1-120">このエンティティに割り当てられている一意の識別子。</span><span class="sxs-lookup"><span data-stu-id="319a1-120">Unique identifier assigned to this entity.</span></span> <span data-ttu-id="319a1-121">null 非許容、読み取り専用</span><span class="sxs-lookup"><span data-stu-id="319a1-121">Not nullable, Read-only</span></span>|
|<span data-ttu-id="319a1-122">isoptional</span><span class="sxs-lookup"><span data-stu-id="319a1-122">isOptional</span></span>|<span data-ttu-id="319a1-123">Boolean</span><span class="sxs-lookup"><span data-stu-id="319a1-123">Boolean</span></span>| <span data-ttu-id="319a1-124">false の場合は、Microsoft Online Services がドメインで正常に動作するように、DNS ホストで顧客によって CNAME レコードが構成されている必要があります。</span><span class="sxs-lookup"><span data-stu-id="319a1-124">If false, the CNAME record must be configured by the customer at the DNS host for Microsoft Online Services to operate correctly with the domain.</span></span> <span data-ttu-id="319a1-125">null 許容ではない</span><span class="sxs-lookup"><span data-stu-id="319a1-125">Not nullable</span></span> |
|<span data-ttu-id="319a1-126">label</span><span class="sxs-lookup"><span data-stu-id="319a1-126">label</span></span>|<span data-ttu-id="319a1-127">String</span><span class="sxs-lookup"><span data-stu-id="319a1-127">String</span></span>| <span data-ttu-id="319a1-128">DNS ホストで CNAME レコードの*エイリアス/ホスト/名前*を構成する場合に使用される値です。</span><span class="sxs-lookup"><span data-stu-id="319a1-128">Value used when configuring the *alias/host/name* of the CNAME record at the DNS host.</span></span> |
|<span data-ttu-id="319a1-129">recordType</span><span class="sxs-lookup"><span data-stu-id="319a1-129">recordType</span></span>|<span data-ttu-id="319a1-130">String</span><span class="sxs-lookup"><span data-stu-id="319a1-130">String</span></span>| <span data-ttu-id="319a1-131">DNS レコードの種類。</span><span class="sxs-lookup"><span data-stu-id="319a1-131">Type of DNS record.</span></span> <span data-ttu-id="319a1-132">値は常に*CName*です。</span><span class="sxs-lookup"><span data-stu-id="319a1-132">The value is always *CName*.</span></span> <span data-ttu-id="319a1-133">Key</span><span class="sxs-lookup"><span data-stu-id="319a1-133">Key</span></span>|
|<span data-ttu-id="319a1-134">supportedservice</span><span class="sxs-lookup"><span data-stu-id="319a1-134">supportedService</span></span>|<span data-ttu-id="319a1-135">String</span><span class="sxs-lookup"><span data-stu-id="319a1-135">String</span></span>| <span data-ttu-id="319a1-136">この CNAME レコードに依存している Microsoft Online サービスまたは機能。</span><span class="sxs-lookup"><span data-stu-id="319a1-136">Microsoft Online Service or feature that has a dependency on this CNAME record.</span></span></br></br><span data-ttu-id="319a1-137">**null**、 *Email*、 *Sharepoint*、 *emailinternalrelayonly*、 *OfficeCommunicationsOnline*、 *sharepointdefaultdomain*、 *fullredelegation*、sharepointpublic のいずれかの値を使用できます。 \*\*、 *orgidauthentication*、 *Yammer*、 *Intune*</span><span class="sxs-lookup"><span data-stu-id="319a1-137">Can be one of the following values: **null**, *Email*, *Sharepoint*, *EmailInternalRelayOnly*, *OfficeCommunicationsOnline*, *SharePointDefaultDomain*, *FullRedelegation*, *SharePointPublic*, *OrgIdAuthentication*, *Yammer*, *Intune*</span></span>|
|<span data-ttu-id="319a1-138">ttl</span><span class="sxs-lookup"><span data-stu-id="319a1-138">ttl</span></span>|<span data-ttu-id="319a1-139">Int32</span><span class="sxs-lookup"><span data-stu-id="319a1-139">Int32</span></span>| <span data-ttu-id="319a1-140">DNS ホストで CNAME レコードの time to live (ttl) プロパティを構成する場合に使用する値です。</span><span class="sxs-lookup"><span data-stu-id="319a1-140">Value to use when configuring the time-to-live (ttl) property of the CNAME record at the DNS host.</span></span> <span data-ttu-id="319a1-141">null 許容ではない</span><span class="sxs-lookup"><span data-stu-id="319a1-141">Not nullable</span></span> |

## <a name="relationships"></a><span data-ttu-id="319a1-142">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="319a1-142">Relationships</span></span>
<span data-ttu-id="319a1-143">なし</span><span class="sxs-lookup"><span data-stu-id="319a1-143">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="319a1-144">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="319a1-144">JSON representation</span></span>
<span data-ttu-id="319a1-145">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="319a1-145">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.domainDnsCnameRecord"
}-->

```json
{
  "canonicalName": "String",
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
  "description": "domainDnsCnameRecord resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
