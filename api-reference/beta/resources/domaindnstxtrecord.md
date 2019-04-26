---
title: domaindnst・ record リソースの種類
description: テナント内の特定のドメインの DNS ゾーンファイルに追加された TXT レコードを表します。 domaindnsrecord エンティティから継承されます。
author: lleonard-msft
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 14280f7ddaa172960a269a22255db4ea3e44dc61
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33334509"
---
# <a name="domaindnstxtrecord-resource-type"></a><span data-ttu-id="4f2c6-104">domaindnst・ record リソースの種類</span><span class="sxs-lookup"><span data-stu-id="4f2c6-104">domainDnsTxtRecord resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4f2c6-105">テナント内の特定のドメインの DNS ゾーンファイルに追加された TXT レコードを表します。</span><span class="sxs-lookup"><span data-stu-id="4f2c6-105">Represents a TXT record added to the DNS zone file of a particular domain in the tenant.</span></span> <span data-ttu-id="4f2c6-106">[domaindnsrecord](domaindnsrecord.md)エンティティから継承されます。</span><span class="sxs-lookup"><span data-stu-id="4f2c6-106">Inherited from [DomainDnsRecord](domaindnsrecord.md) entity.</span></span>

## <a name="methods"></a><span data-ttu-id="4f2c6-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="4f2c6-107">Methods</span></span>
<span data-ttu-id="4f2c6-108">このリソースへの直接クエリはサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="4f2c6-108">Direct queries to this resource are not supported.</span></span> <span data-ttu-id="4f2c6-109">ドメインサービスレコードを照会する方法については、「 [domain](domain.md) 」のトピックを参照してください。</span><span class="sxs-lookup"><span data-stu-id="4f2c6-109">Please see the [domain](domain.md) topic for information on how to query for domain service records.</span></span>

## <a name="properties"></a><span data-ttu-id="4f2c6-110">プロパティ</span><span class="sxs-lookup"><span data-stu-id="4f2c6-110">Properties</span></span>
| <span data-ttu-id="4f2c6-111">プロパティ</span><span class="sxs-lookup"><span data-stu-id="4f2c6-111">Property</span></span>     | <span data-ttu-id="4f2c6-112">型</span><span class="sxs-lookup"><span data-stu-id="4f2c6-112">Type</span></span>   |<span data-ttu-id="4f2c6-113">説明</span><span class="sxs-lookup"><span data-stu-id="4f2c6-113">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="4f2c6-114">id</span><span class="sxs-lookup"><span data-stu-id="4f2c6-114">id</span></span>|<span data-ttu-id="4f2c6-115">String</span><span class="sxs-lookup"><span data-stu-id="4f2c6-115">String</span></span>| <span data-ttu-id="4f2c6-116">このエンティティに割り当てられている一意の識別子。</span><span class="sxs-lookup"><span data-stu-id="4f2c6-116">Unique identifier assigned to this entity.</span></span> <span data-ttu-id="4f2c6-117">null 許容ではありません。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="4f2c6-117">Not nullable, Read-only.</span></span> |
|<span data-ttu-id="4f2c6-118">isoptional</span><span class="sxs-lookup"><span data-stu-id="4f2c6-118">isOptional</span></span>|<span data-ttu-id="4f2c6-119">Boolean</span><span class="sxs-lookup"><span data-stu-id="4f2c6-119">Boolean</span></span>| <span data-ttu-id="4f2c6-120">false の場合は、Microsoft Online Services がドメインで正しく動作するように、DNS ホストで顧客によって TXT レコードが構成されている必要があります。</span><span class="sxs-lookup"><span data-stu-id="4f2c6-120">If false, the TXT record must be configured by the customer at the DNS host for Microsoft Online Services to operate correctly with the domain.</span></span> |
|<span data-ttu-id="4f2c6-121">label</span><span class="sxs-lookup"><span data-stu-id="4f2c6-121">label</span></span>|<span data-ttu-id="4f2c6-122">String</span><span class="sxs-lookup"><span data-stu-id="4f2c6-122">String</span></span>| <span data-ttu-id="4f2c6-123">DNS ホストで TXT レコードの*name*プロパティを構成する場合に使用する値です。</span><span class="sxs-lookup"><span data-stu-id="4f2c6-123">Value to use when configuring the *name* property of the TXT record at the DNS host.</span></span>|
|<span data-ttu-id="4f2c6-124">recordType</span><span class="sxs-lookup"><span data-stu-id="4f2c6-124">recordType</span></span>|<span data-ttu-id="4f2c6-125">String</span><span class="sxs-lookup"><span data-stu-id="4f2c6-125">String</span></span>| <span data-ttu-id="4f2c6-126">DNS レコードの種類。</span><span class="sxs-lookup"><span data-stu-id="4f2c6-126">Type of DNS record.</span></span> <span data-ttu-id="4f2c6-127">値は常に*Txt*です。</span><span class="sxs-lookup"><span data-stu-id="4f2c6-127">The value is always *Txt*.</span></span> <span data-ttu-id="4f2c6-128">Key</span><span class="sxs-lookup"><span data-stu-id="4f2c6-128">Key</span></span> |
|<span data-ttu-id="4f2c6-129">supportedservice</span><span class="sxs-lookup"><span data-stu-id="4f2c6-129">supportedService</span></span>|<span data-ttu-id="4f2c6-130">String</span><span class="sxs-lookup"><span data-stu-id="4f2c6-130">String</span></span>| <span data-ttu-id="4f2c6-131">Microsoft Online サービスまたはこの TXT レコードに依存している機能。</span><span class="sxs-lookup"><span data-stu-id="4f2c6-131">Microsoft Online Service or feature that has a dependency on this TXT record.</span></span></br></br><span data-ttu-id="4f2c6-132">**null**、 *Email*、 *Sharepoint*、 *emailinternalrelayonly*、 *OfficeCommunicationsOnline*、 *sharepointdefaultdomain*、 *fullredelegation*、sharepointpublic のいずれかの値を使用できます。 \*\*、 *orgidauthentication*、 *Yammer*、 *Intune*</span><span class="sxs-lookup"><span data-stu-id="4f2c6-132">Can be one of the following values: **null**, *Email*, *Sharepoint*, *EmailInternalRelayOnly*, *OfficeCommunicationsOnline*, *SharePointDefaultDomain*, *FullRedelegation*, *SharePointPublic*, *OrgIdAuthentication*, *Yammer*, *Intune*</span></span> |
|<span data-ttu-id="4f2c6-133">text</span><span class="sxs-lookup"><span data-stu-id="4f2c6-133">text</span></span>|<span data-ttu-id="4f2c6-134">String</span><span class="sxs-lookup"><span data-stu-id="4f2c6-134">String</span></span>| <span data-ttu-id="4f2c6-135">DNS ホストで*text*プロパティを構成する場合に使用される値です。</span><span class="sxs-lookup"><span data-stu-id="4f2c6-135">Value used when configuring the *text* property at the DNS host.</span></span> |
|<span data-ttu-id="4f2c6-136">ttl</span><span class="sxs-lookup"><span data-stu-id="4f2c6-136">ttl</span></span>|<span data-ttu-id="4f2c6-137">Int32</span><span class="sxs-lookup"><span data-stu-id="4f2c6-137">Int32</span></span>| <span data-ttu-id="4f2c6-138">DNS ホストで MX レコードの*time to live (ttl)* プロパティを構成する場合に使用する値です。</span><span class="sxs-lookup"><span data-stu-id="4f2c6-138">Value to use when configuring the *time-to-live (ttl)* property of the MX record at the DNS host.</span></span> <span data-ttu-id="4f2c6-139">null 許容ではない</span><span class="sxs-lookup"><span data-stu-id="4f2c6-139">Not nullable</span></span> |

## <a name="relationships"></a><span data-ttu-id="4f2c6-140">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="4f2c6-140">Relationships</span></span>
<span data-ttu-id="4f2c6-141">なし</span><span class="sxs-lookup"><span data-stu-id="4f2c6-141">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="4f2c6-142">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="4f2c6-142">JSON representation</span></span>
<span data-ttu-id="4f2c6-143">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="4f2c6-143">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.domainDnsTxtRecord"
}-->

```json
{
  "canonicalName": "String",
  "id": "String (identifier)",
  "isOptional": true,
  "label": "String",
  "recordType": "String",
  "supportedService": "String",
  "text": "String",
  "ttl": 1024
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "domainDnsTxtRecord resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
