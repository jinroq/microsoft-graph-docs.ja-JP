---
title: domainDnsCnameRecord リソースの種類
description: テナント内の特定のドメインの DNS ゾーンファイルに追加された CNAME レコードを表します。 DomainDnsRecord エンティティから継承されます。
author: davidmu1
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 4de771a543459ffa1529cb2a6bb11e480d645e43
ms.sourcegitcommit: 33f1cf5b3b79bfba6a06b52d34e558a6ba327d21
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2019
ms.locfileid: "34657848"
---
# <a name="domaindnscnamerecord-resource-type"></a><span data-ttu-id="ef14c-104">domainDnsCnameRecord リソースの種類</span><span class="sxs-lookup"><span data-stu-id="ef14c-104">domainDnsCnameRecord resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ef14c-105">テナント内の特定のドメインの DNS ゾーンファイルに追加された CNAME レコードを表します。</span><span class="sxs-lookup"><span data-stu-id="ef14c-105">Represents a CNAME record added to the DNS zone file of a particular domain in the tenant.</span></span> <span data-ttu-id="ef14c-106">[Domaindnsrecord](domaindnsrecord.md)エンティティから継承されます。</span><span class="sxs-lookup"><span data-stu-id="ef14c-106">Inherited from [DomainDnsRecord](domaindnsrecord.md) entity.</span></span>


## <a name="methods"></a><span data-ttu-id="ef14c-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="ef14c-107">Methods</span></span>
<span data-ttu-id="ef14c-108">このリソースへの直接クエリはサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ef14c-108">Direct queries to this resource are not supported.</span></span> <span data-ttu-id="ef14c-109">ドメインサービスレコードを照会する方法については、「 [domain](domain.md) 」のトピックを参照してください。</span><span class="sxs-lookup"><span data-stu-id="ef14c-109">Please see the [domain](domain.md) topic for information on how to query for domain service records.</span></span>

## <a name="properties"></a><span data-ttu-id="ef14c-110">プロパティ</span><span class="sxs-lookup"><span data-stu-id="ef14c-110">Properties</span></span>
| <span data-ttu-id="ef14c-111">プロパティ</span><span class="sxs-lookup"><span data-stu-id="ef14c-111">Property</span></span>     | <span data-ttu-id="ef14c-112">型</span><span class="sxs-lookup"><span data-stu-id="ef14c-112">Type</span></span>   |<span data-ttu-id="ef14c-113">説明</span><span class="sxs-lookup"><span data-stu-id="ef14c-113">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ef14c-114">canonicalName</span><span class="sxs-lookup"><span data-stu-id="ef14c-114">canonicalName</span></span>|<span data-ttu-id="ef14c-115">String</span><span class="sxs-lookup"><span data-stu-id="ef14c-115">String</span></span>| <span data-ttu-id="ef14c-116">CNAME レコードの標準名。</span><span class="sxs-lookup"><span data-stu-id="ef14c-116">The canonical name of the CNAME record.</span></span> <span data-ttu-id="ef14c-117">DNS ホストで CNAME レコードを構成するために使用します。</span><span class="sxs-lookup"><span data-stu-id="ef14c-117">Used to configure the CNAME record at the DNS host.</span></span> |
|<span data-ttu-id="ef14c-118">id</span><span class="sxs-lookup"><span data-stu-id="ef14c-118">id</span></span>|<span data-ttu-id="ef14c-119">String</span><span class="sxs-lookup"><span data-stu-id="ef14c-119">String</span></span>| <span data-ttu-id="ef14c-120">このエンティティに割り当てられている一意の識別子。</span><span class="sxs-lookup"><span data-stu-id="ef14c-120">Unique identifier assigned to this entity.</span></span> <span data-ttu-id="ef14c-121">Null 非許容、読み取り専用</span><span class="sxs-lookup"><span data-stu-id="ef14c-121">Not nullable, Read-only</span></span>|
|<span data-ttu-id="ef14c-122">isOptional</span><span class="sxs-lookup"><span data-stu-id="ef14c-122">isOptional</span></span>|<span data-ttu-id="ef14c-123">Boolean</span><span class="sxs-lookup"><span data-stu-id="ef14c-123">Boolean</span></span>| <span data-ttu-id="ef14c-124">False の場合は、Microsoft Online Services がドメインで正常に動作するように、DNS ホストで顧客によって CNAME レコードが構成されている必要があります。</span><span class="sxs-lookup"><span data-stu-id="ef14c-124">If false, the CNAME record must be configured by the customer at the DNS host for Microsoft Online Services to operate correctly with the domain.</span></span> <span data-ttu-id="ef14c-125">Null 許容ではない</span><span class="sxs-lookup"><span data-stu-id="ef14c-125">Not nullable</span></span> |
|<span data-ttu-id="ef14c-126">label</span><span class="sxs-lookup"><span data-stu-id="ef14c-126">label</span></span>|<span data-ttu-id="ef14c-127">String</span><span class="sxs-lookup"><span data-stu-id="ef14c-127">String</span></span>| <span data-ttu-id="ef14c-128">DNS ホストで CNAME レコードの*エイリアス/ホスト/名前*を構成する場合に使用される値です。</span><span class="sxs-lookup"><span data-stu-id="ef14c-128">Value used when configuring the *alias/host/name* of the CNAME record at the DNS host.</span></span> |
|<span data-ttu-id="ef14c-129">recordType</span><span class="sxs-lookup"><span data-stu-id="ef14c-129">recordType</span></span>|<span data-ttu-id="ef14c-130">String</span><span class="sxs-lookup"><span data-stu-id="ef14c-130">String</span></span>| <span data-ttu-id="ef14c-131">DNS レコードの種類。</span><span class="sxs-lookup"><span data-stu-id="ef14c-131">Type of DNS record.</span></span> <span data-ttu-id="ef14c-132">値は常に*CName*です。</span><span class="sxs-lookup"><span data-stu-id="ef14c-132">The value is always *CName*.</span></span> <span data-ttu-id="ef14c-133">Key</span><span class="sxs-lookup"><span data-stu-id="ef14c-133">Key</span></span>|
|<span data-ttu-id="ef14c-134">supportedService</span><span class="sxs-lookup"><span data-stu-id="ef14c-134">supportedService</span></span>|<span data-ttu-id="ef14c-135">String</span><span class="sxs-lookup"><span data-stu-id="ef14c-135">String</span></span>| <span data-ttu-id="ef14c-136">この CNAME レコードに依存している Microsoft Online サービスまたは機能。</span><span class="sxs-lookup"><span data-stu-id="ef14c-136">Microsoft Online Service or feature that has a dependency on this CNAME record.</span></span></br></br><span data-ttu-id="ef14c-137">**Null**、 *Email*、 *Sharepoint*、 *emailinternalrelayonly*、 *OfficeCommunicationsOnline*、 *sharepointdefaultdomain*、 *fullredelegation*、sharepointpublic のいずれかの値を使用できます。 \*\*、 *Orgidauthentication*、 *Yammer*、 *Intune*</span><span class="sxs-lookup"><span data-stu-id="ef14c-137">Can be one of the following values: **null**, *Email*, *Sharepoint*, *EmailInternalRelayOnly*, *OfficeCommunicationsOnline*, *SharePointDefaultDomain*, *FullRedelegation*, *SharePointPublic*, *OrgIdAuthentication*, *Yammer*, *Intune*</span></span>|
|<span data-ttu-id="ef14c-138">ttl</span><span class="sxs-lookup"><span data-stu-id="ef14c-138">ttl</span></span>|<span data-ttu-id="ef14c-139">Int32</span><span class="sxs-lookup"><span data-stu-id="ef14c-139">Int32</span></span>| <span data-ttu-id="ef14c-140">DNS ホストで CNAME レコードの time to live (ttl) プロパティを構成する場合に使用する値です。</span><span class="sxs-lookup"><span data-stu-id="ef14c-140">Value to use when configuring the time-to-live (ttl) property of the CNAME record at the DNS host.</span></span> <span data-ttu-id="ef14c-141">Null 許容ではない</span><span class="sxs-lookup"><span data-stu-id="ef14c-141">Not nullable</span></span> |

## <a name="relationships"></a><span data-ttu-id="ef14c-142">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="ef14c-142">Relationships</span></span>
<span data-ttu-id="ef14c-143">なし</span><span class="sxs-lookup"><span data-stu-id="ef14c-143">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="ef14c-144">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="ef14c-144">JSON representation</span></span>
<span data-ttu-id="ef14c-145">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="ef14c-145">Here is a JSON representation of the resource.</span></span>

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
