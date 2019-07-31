---
title: domainDnsMxRecord リソースの種類
description: テナント内の特定のドメインの DNS ゾーンファイルに追加された MX レコードを表します。 DomainDnsRecord エンティティから継承されます。
author: davidmu1
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 7472118f1a7a7fb30ac1bc4e4775f04f4a84fca4
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35973794"
---
# <a name="domaindnsmxrecord-resource-type"></a><span data-ttu-id="b3aca-104">domainDnsMxRecord リソースの種類</span><span class="sxs-lookup"><span data-stu-id="b3aca-104">domainDnsMxRecord resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b3aca-105">テナント内の特定のドメインの DNS ゾーンファイルに追加された MX レコードを表します。</span><span class="sxs-lookup"><span data-stu-id="b3aca-105">Represents a MX record added to the DNS zone file of a particular domain in the tenant.</span></span> <span data-ttu-id="b3aca-106">[Domaindnsrecord](domaindnsrecord.md)エンティティから継承されます。</span><span class="sxs-lookup"><span data-stu-id="b3aca-106">Inherited from [DomainDnsRecord](domaindnsrecord.md) entity.</span></span>

## <a name="methods"></a><span data-ttu-id="b3aca-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="b3aca-107">Methods</span></span>
<span data-ttu-id="b3aca-108">このリソースへの直接クエリはサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b3aca-108">Direct queries to this resource are not supported.</span></span> <span data-ttu-id="b3aca-109">ドメインサービスレコードを照会する方法については、「 [domain](domain.md) 」のトピックを参照してください。</span><span class="sxs-lookup"><span data-stu-id="b3aca-109">Please see the [domain](domain.md) topic for information on how to query for domain service records.</span></span>

## <a name="properties"></a><span data-ttu-id="b3aca-110">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b3aca-110">Properties</span></span>
| <span data-ttu-id="b3aca-111">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b3aca-111">Property</span></span>     | <span data-ttu-id="b3aca-112">型</span><span class="sxs-lookup"><span data-stu-id="b3aca-112">Type</span></span>   |<span data-ttu-id="b3aca-113">説明</span><span class="sxs-lookup"><span data-stu-id="b3aca-113">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b3aca-114">id</span><span class="sxs-lookup"><span data-stu-id="b3aca-114">id</span></span>|<span data-ttu-id="b3aca-115">String</span><span class="sxs-lookup"><span data-stu-id="b3aca-115">String</span></span>| <span data-ttu-id="b3aca-116">このエンティティに割り当てられている一意の識別子。</span><span class="sxs-lookup"><span data-stu-id="b3aca-116">Unique identifier assigned to this entity.</span></span> <span data-ttu-id="b3aca-117">Null 許容ではありません。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="b3aca-117">Not nullable, Read-only.</span></span>|
|<span data-ttu-id="b3aca-118">isOptional</span><span class="sxs-lookup"><span data-stu-id="b3aca-118">isOptional</span></span>|<span data-ttu-id="b3aca-119">Boolean</span><span class="sxs-lookup"><span data-stu-id="b3aca-119">Boolean</span></span>| <span data-ttu-id="b3aca-120">False の場合、MX レコードは、Microsoft Online Services がドメインで正しく動作するように、DNS ホストで顧客によって構成されている必要があります。</span><span class="sxs-lookup"><span data-stu-id="b3aca-120">If false, the MX record must be configured by the customer at the DNS host for Microsoft Online Services to operate correctly with the domain.</span></span> |
|<span data-ttu-id="b3aca-121">label</span><span class="sxs-lookup"><span data-stu-id="b3aca-121">label</span></span>|<span data-ttu-id="b3aca-122">String</span><span class="sxs-lookup"><span data-stu-id="b3aca-122">String</span></span>| <span data-ttu-id="b3aca-123">DNS ホストで MX レコードの*alias/host/name*プロパティを構成する場合に使用される値です。</span><span class="sxs-lookup"><span data-stu-id="b3aca-123">Value used when configuring the *alias/host/name* property of the MX record at the DNS host.</span></span> |
|<span data-ttu-id="b3aca-124">mailExchange</span><span class="sxs-lookup"><span data-stu-id="b3aca-124">mailExchange</span></span>|<span data-ttu-id="b3aca-125">String</span><span class="sxs-lookup"><span data-stu-id="b3aca-125">String</span></span>| <span data-ttu-id="b3aca-126">DNS ホストで MX レコードの*応答/宛先/値*を構成する場合に使用される値です。</span><span class="sxs-lookup"><span data-stu-id="b3aca-126">Value used when configuring the *answer/destination/value* of the MX record at the DNS host.</span></span>|
|<span data-ttu-id="b3aca-127">優先順位</span><span class="sxs-lookup"><span data-stu-id="b3aca-127">preference</span></span>|<span data-ttu-id="b3aca-128">Int32</span><span class="sxs-lookup"><span data-stu-id="b3aca-128">Int32</span></span>| <span data-ttu-id="b3aca-129">DNS ホストで MX レコードの*Preference/Priority*プロパティを構成する場合に使用される値です。</span><span class="sxs-lookup"><span data-stu-id="b3aca-129">Value used when configuring the *Preference/Priority* property of the MX record at the DNS host.</span></span> |
|<span data-ttu-id="b3aca-130">recordType</span><span class="sxs-lookup"><span data-stu-id="b3aca-130">recordType</span></span>|<span data-ttu-id="b3aca-131">String</span><span class="sxs-lookup"><span data-stu-id="b3aca-131">String</span></span>| <span data-ttu-id="b3aca-132">DNS レコードの種類。</span><span class="sxs-lookup"><span data-stu-id="b3aca-132">Type of DNS record.</span></span> <span data-ttu-id="b3aca-133">値は常に*Mx*です。</span><span class="sxs-lookup"><span data-stu-id="b3aca-133">The value is always *Mx*.</span></span> <span data-ttu-id="b3aca-134">Key</span><span class="sxs-lookup"><span data-stu-id="b3aca-134">Key</span></span> |
|<span data-ttu-id="b3aca-135">supportedService</span><span class="sxs-lookup"><span data-stu-id="b3aca-135">supportedService</span></span>|<span data-ttu-id="b3aca-136">String</span><span class="sxs-lookup"><span data-stu-id="b3aca-136">String</span></span>| <span data-ttu-id="b3aca-137">この MX レコードに依存している Microsoft Online サービスまたは機能。</span><span class="sxs-lookup"><span data-stu-id="b3aca-137">Microsoft Online Service or feature that has a dependency on this MX record.</span></span></br></br><span data-ttu-id="b3aca-138">**Null**、 *Email*、 *Sharepoint*、 *emailinternalrelayonly*、 *OfficeCommunicationsOnline*、 *sharepointdefaultdomain*、 *fullredelegation*、sharepointpublic のいずれかの値を使用できます。 \*\*、 *Orgidauthentication*、 *Yammer*、 *Intune*</span><span class="sxs-lookup"><span data-stu-id="b3aca-138">Can be one of the following values: **null**, *Email*, *Sharepoint*, *EmailInternalRelayOnly*, *OfficeCommunicationsOnline*, *SharePointDefaultDomain*, *FullRedelegation*, *SharePointPublic*, *OrgIdAuthentication*, *Yammer*, *Intune*</span></span> |
|<span data-ttu-id="b3aca-139">ttl</span><span class="sxs-lookup"><span data-stu-id="b3aca-139">ttl</span></span>|<span data-ttu-id="b3aca-140">Int32</span><span class="sxs-lookup"><span data-stu-id="b3aca-140">Int32</span></span>| <span data-ttu-id="b3aca-141">DNS ホストで MX レコードの*time to live (ttl)* プロパティを構成する場合に使用する値です。</span><span class="sxs-lookup"><span data-stu-id="b3aca-141">Value to use when configuring the *time-to-live (ttl)* property of the MX record at the DNS host.</span></span> <span data-ttu-id="b3aca-142">Null 許容ではない</span><span class="sxs-lookup"><span data-stu-id="b3aca-142">Not nullable</span></span> |

## <a name="relationships"></a><span data-ttu-id="b3aca-143">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="b3aca-143">Relationships</span></span>
<span data-ttu-id="b3aca-144">なし</span><span class="sxs-lookup"><span data-stu-id="b3aca-144">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="b3aca-145">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="b3aca-145">JSON representation</span></span>
<span data-ttu-id="b3aca-146">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="b3aca-146">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.domainDnsMxRecord"
}-->

```json
{
  "canonicalName": "String",
  "id": "String (identifier)",
  "isOptional": true,
  "label": "String",
  "mailExchange": "String",
  "preference": 1024,
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
  "description": "domainDnsMxRecord resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
