---
title: Domaindnst・ Record リソースの種類
description: テナント内の特定のドメインの DNS ゾーンファイルに追加された TXT レコードを表します。 DomainDnsRecord エンティティから継承されます。
author: davidmu1
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 4032ac4987f423efed49a61b0bebf5090ba42c09
ms.sourcegitcommit: 33f1cf5b3b79bfba6a06b52d34e558a6ba327d21
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2019
ms.locfileid: "34657162"
---
# <a name="domaindnstxtrecord-resource-type"></a><span data-ttu-id="5e46c-104">Domaindnst・ Record リソースの種類</span><span class="sxs-lookup"><span data-stu-id="5e46c-104">domainDnsTxtRecord resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5e46c-105">テナント内の特定のドメインの DNS ゾーンファイルに追加された TXT レコードを表します。</span><span class="sxs-lookup"><span data-stu-id="5e46c-105">Represents a TXT record added to the DNS zone file of a particular domain in the tenant.</span></span> <span data-ttu-id="5e46c-106">[Domaindnsrecord](domaindnsrecord.md)エンティティから継承されます。</span><span class="sxs-lookup"><span data-stu-id="5e46c-106">Inherited from [DomainDnsRecord](domaindnsrecord.md) entity.</span></span>

## <a name="methods"></a><span data-ttu-id="5e46c-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="5e46c-107">Methods</span></span>
<span data-ttu-id="5e46c-108">このリソースへの直接クエリはサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="5e46c-108">Direct queries to this resource are not supported.</span></span> <span data-ttu-id="5e46c-109">ドメインサービスレコードを照会する方法については、「 [domain](domain.md) 」のトピックを参照してください。</span><span class="sxs-lookup"><span data-stu-id="5e46c-109">Please see the [domain](domain.md) topic for information on how to query for domain service records.</span></span>

## <a name="properties"></a><span data-ttu-id="5e46c-110">プロパティ</span><span class="sxs-lookup"><span data-stu-id="5e46c-110">Properties</span></span>
| <span data-ttu-id="5e46c-111">プロパティ</span><span class="sxs-lookup"><span data-stu-id="5e46c-111">Property</span></span>     | <span data-ttu-id="5e46c-112">型</span><span class="sxs-lookup"><span data-stu-id="5e46c-112">Type</span></span>   |<span data-ttu-id="5e46c-113">説明</span><span class="sxs-lookup"><span data-stu-id="5e46c-113">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="5e46c-114">id</span><span class="sxs-lookup"><span data-stu-id="5e46c-114">id</span></span>|<span data-ttu-id="5e46c-115">String</span><span class="sxs-lookup"><span data-stu-id="5e46c-115">String</span></span>| <span data-ttu-id="5e46c-116">このエンティティに割り当てられている一意の識別子。</span><span class="sxs-lookup"><span data-stu-id="5e46c-116">Unique identifier assigned to this entity.</span></span> <span data-ttu-id="5e46c-117">Null 許容ではありません。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="5e46c-117">Not nullable, Read-only.</span></span> |
|<span data-ttu-id="5e46c-118">isOptional</span><span class="sxs-lookup"><span data-stu-id="5e46c-118">isOptional</span></span>|<span data-ttu-id="5e46c-119">Boolean</span><span class="sxs-lookup"><span data-stu-id="5e46c-119">Boolean</span></span>| <span data-ttu-id="5e46c-120">False の場合は、Microsoft Online Services がドメインで正しく動作するように、DNS ホストで顧客によって TXT レコードが構成されている必要があります。</span><span class="sxs-lookup"><span data-stu-id="5e46c-120">If false, the TXT record must be configured by the customer at the DNS host for Microsoft Online Services to operate correctly with the domain.</span></span> |
|<span data-ttu-id="5e46c-121">label</span><span class="sxs-lookup"><span data-stu-id="5e46c-121">label</span></span>|<span data-ttu-id="5e46c-122">String</span><span class="sxs-lookup"><span data-stu-id="5e46c-122">String</span></span>| <span data-ttu-id="5e46c-123">DNS ホストで TXT レコードの*name*プロパティを構成する場合に使用する値です。</span><span class="sxs-lookup"><span data-stu-id="5e46c-123">Value to use when configuring the *name* property of the TXT record at the DNS host.</span></span>|
|<span data-ttu-id="5e46c-124">recordType</span><span class="sxs-lookup"><span data-stu-id="5e46c-124">recordType</span></span>|<span data-ttu-id="5e46c-125">String</span><span class="sxs-lookup"><span data-stu-id="5e46c-125">String</span></span>| <span data-ttu-id="5e46c-126">DNS レコードの種類。</span><span class="sxs-lookup"><span data-stu-id="5e46c-126">Type of DNS record.</span></span> <span data-ttu-id="5e46c-127">値は常に*Txt*です。</span><span class="sxs-lookup"><span data-stu-id="5e46c-127">The value is always *Txt*.</span></span> <span data-ttu-id="5e46c-128">Key</span><span class="sxs-lookup"><span data-stu-id="5e46c-128">Key</span></span> |
|<span data-ttu-id="5e46c-129">supportedService</span><span class="sxs-lookup"><span data-stu-id="5e46c-129">supportedService</span></span>|<span data-ttu-id="5e46c-130">String</span><span class="sxs-lookup"><span data-stu-id="5e46c-130">String</span></span>| <span data-ttu-id="5e46c-131">Microsoft Online サービスまたはこの TXT レコードに依存している機能。</span><span class="sxs-lookup"><span data-stu-id="5e46c-131">Microsoft Online Service or feature that has a dependency on this TXT record.</span></span></br></br><span data-ttu-id="5e46c-132">**Null**、 *Email*、 *Sharepoint*、 *emailinternalrelayonly*、 *OfficeCommunicationsOnline*、 *sharepointdefaultdomain*、 *fullredelegation*、sharepointpublic のいずれかの値を使用できます。 \*\*、 *Orgidauthentication*、 *Yammer*、 *Intune*</span><span class="sxs-lookup"><span data-stu-id="5e46c-132">Can be one of the following values: **null**, *Email*, *Sharepoint*, *EmailInternalRelayOnly*, *OfficeCommunicationsOnline*, *SharePointDefaultDomain*, *FullRedelegation*, *SharePointPublic*, *OrgIdAuthentication*, *Yammer*, *Intune*</span></span> |
|<span data-ttu-id="5e46c-133">text</span><span class="sxs-lookup"><span data-stu-id="5e46c-133">text</span></span>|<span data-ttu-id="5e46c-134">String</span><span class="sxs-lookup"><span data-stu-id="5e46c-134">String</span></span>| <span data-ttu-id="5e46c-135">DNS ホストで*text*プロパティを構成する場合に使用される値です。</span><span class="sxs-lookup"><span data-stu-id="5e46c-135">Value used when configuring the *text* property at the DNS host.</span></span> |
|<span data-ttu-id="5e46c-136">ttl</span><span class="sxs-lookup"><span data-stu-id="5e46c-136">ttl</span></span>|<span data-ttu-id="5e46c-137">Int32</span><span class="sxs-lookup"><span data-stu-id="5e46c-137">Int32</span></span>| <span data-ttu-id="5e46c-138">DNS ホストで MX レコードの*time to live (ttl)* プロパティを構成する場合に使用する値です。</span><span class="sxs-lookup"><span data-stu-id="5e46c-138">Value to use when configuring the *time-to-live (ttl)* property of the MX record at the DNS host.</span></span> <span data-ttu-id="5e46c-139">Null 許容ではない</span><span class="sxs-lookup"><span data-stu-id="5e46c-139">Not nullable</span></span> |

## <a name="relationships"></a><span data-ttu-id="5e46c-140">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="5e46c-140">Relationships</span></span>
<span data-ttu-id="5e46c-141">なし</span><span class="sxs-lookup"><span data-stu-id="5e46c-141">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="5e46c-142">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="5e46c-142">JSON representation</span></span>
<span data-ttu-id="5e46c-143">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="5e46c-143">Here is a JSON representation of the resource.</span></span>

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
