---
title: domainDnsMxRecord リソースの種類
description: テナント内の特定のドメインの DNS ゾーン ファイルに追加された MX レコードを表します。DomainDnsRecord エンティティから継承されます。
author: lleonard-msft
ms.openlocfilehash: e06b3c405f4ad5e2e561e57876ef010bddb1068d
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27345837"
---
# <a name="domaindnsmxrecord-resource-type"></a><span data-ttu-id="95cc8-104">domainDnsMxRecord リソースの種類</span><span class="sxs-lookup"><span data-stu-id="95cc8-104">domainDnsMxRecord resource type</span></span>

<span data-ttu-id="95cc8-p102">テナント内の特定のドメインの DNS ゾーン ファイルに追加された MX レコードを表します。[DomainDnsRecord](domaindnsrecord.md) エンティティから継承されます。</span><span class="sxs-lookup"><span data-stu-id="95cc8-p102">Represents a MX record added to the DNS zone file of a particular domain in the tenant. Inherited from [DomainDnsRecord](domaindnsrecord.md) entity.</span></span>

## <a name="methods"></a><span data-ttu-id="95cc8-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="95cc8-107">Methods</span></span>
<span data-ttu-id="95cc8-p103">このリソースへの直接クエリはサポートされていません。ドメイン サービス レコードのクエリを実行する方法の詳細については、[ドメイン](domain.md)のトピックを参照してください。</span><span class="sxs-lookup"><span data-stu-id="95cc8-p103">Direct queries to this resource are not supported. Please see the [domain](domain.md) topic for information on how to query for domain service records.</span></span>

## <a name="properties"></a><span data-ttu-id="95cc8-110">プロパティ</span><span class="sxs-lookup"><span data-stu-id="95cc8-110">Properties</span></span>
| <span data-ttu-id="95cc8-111">プロパティ</span><span class="sxs-lookup"><span data-stu-id="95cc8-111">Property</span></span>     | <span data-ttu-id="95cc8-112">種類</span><span class="sxs-lookup"><span data-stu-id="95cc8-112">Type</span></span>   |<span data-ttu-id="95cc8-113">説明</span><span class="sxs-lookup"><span data-stu-id="95cc8-113">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="95cc8-114">ID</span><span class="sxs-lookup"><span data-stu-id="95cc8-114">id</span></span>|<span data-ttu-id="95cc8-115">String</span><span class="sxs-lookup"><span data-stu-id="95cc8-115">String</span></span>| <span data-ttu-id="95cc8-p104">このエンティティに割り当てられた一意の識別子。null 許容ではありません。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="95cc8-p104">Unique identifier assigned to this entity. Not nullable, Read-only.</span></span>|
|<span data-ttu-id="95cc8-118">isOptional</span><span class="sxs-lookup"><span data-stu-id="95cc8-118">isOptional</span></span>|<span data-ttu-id="95cc8-119">Boolean</span><span class="sxs-lookup"><span data-stu-id="95cc8-119">Boolean</span></span>| <span data-ttu-id="95cc8-120">False の場合、MX レコードは Microsoft オンライン サービスでドメインを正しく操作するために、DNS ホストで顧客によって構成されている必要があります。</span><span class="sxs-lookup"><span data-stu-id="95cc8-120">If false, the MX record must be configured by the customer at the DNS host for Microsoft Online Services to operate correctly with the domain.</span></span> |
|<span data-ttu-id="95cc8-121">label</span><span class="sxs-lookup"><span data-stu-id="95cc8-121">label</span></span>|<span data-ttu-id="95cc8-122">String</span><span class="sxs-lookup"><span data-stu-id="95cc8-122">String</span></span>| <span data-ttu-id="95cc8-123">DNS ホストで MX レコードの *alias/host/name* プロパティを構成する場合に使用される値です。</span><span class="sxs-lookup"><span data-stu-id="95cc8-123">Value used when configuring the *alias/host/name* property of the MX record at the DNS host.</span></span> |
|<span data-ttu-id="95cc8-124">mailExchange</span><span class="sxs-lookup"><span data-stu-id="95cc8-124">mailExchange</span></span>|<span data-ttu-id="95cc8-125">String</span><span class="sxs-lookup"><span data-stu-id="95cc8-125">String</span></span>| <span data-ttu-id="95cc8-126">DNS ホストで MX レコードの *answer/destination/value* を構成する場合に使用される値です。</span><span class="sxs-lookup"><span data-stu-id="95cc8-126">Value used when configuring the *answer/destination/value* of the MX record at the DNS host.</span></span>|
|<span data-ttu-id="95cc8-127">preference</span><span class="sxs-lookup"><span data-stu-id="95cc8-127">preference</span></span>|<span data-ttu-id="95cc8-128">Int32</span><span class="sxs-lookup"><span data-stu-id="95cc8-128">Int32</span></span>| <span data-ttu-id="95cc8-129">DNS ホストで MX レコードの *Preference/Priority* プロパティを構成する場合に使用される値です。</span><span class="sxs-lookup"><span data-stu-id="95cc8-129">Value used when configuring the *Preference/Priority* property of the MX record at the DNS host.</span></span> |
|<span data-ttu-id="95cc8-130">recordType</span><span class="sxs-lookup"><span data-stu-id="95cc8-130">recordType</span></span>|<span data-ttu-id="95cc8-131">String</span><span class="sxs-lookup"><span data-stu-id="95cc8-131">String</span></span>| <span data-ttu-id="95cc8-p105">DNS レコードの種類。この値は常に *Mx* です。キー</span><span class="sxs-lookup"><span data-stu-id="95cc8-p105">Type of DNS record. The value is always *Mx*. Key</span></span> |
|<span data-ttu-id="95cc8-135">supportedService</span><span class="sxs-lookup"><span data-stu-id="95cc8-135">supportedService</span></span>|<span data-ttu-id="95cc8-136">String</span><span class="sxs-lookup"><span data-stu-id="95cc8-136">String</span></span>| <span data-ttu-id="95cc8-137">Microsoft オンライン サービスまたはこの MX レコードに依存している機能。</span><span class="sxs-lookup"><span data-stu-id="95cc8-137">Microsoft Online Service or feature that has a dependency on this MX record.</span></span></br></br><span data-ttu-id="95cc8-138">次のいずれかの値を指定できます。**null**、*Email*、*Sharepoint*、*EmailInternalRelayOnly*、*OfficeCommunicationsOnline*、*SharePointDefaultDomain*、*FullRedelegation*、*SharePointPublic*、*OrgIdAuthentication*、*Yammer*、*Intune*</span><span class="sxs-lookup"><span data-stu-id="95cc8-138">Can be one of the following values: **null**, *Email*, *Sharepoint*, *EmailInternalRelayOnly*, *OfficeCommunicationsOnline*, *SharePointDefaultDomain*, *FullRedelegation*, *SharePointPublic*, *OrgIdAuthentication*, *Yammer*, *Intune*</span></span> |
|<span data-ttu-id="95cc8-139">ttl</span><span class="sxs-lookup"><span data-stu-id="95cc8-139">ttl</span></span>|<span data-ttu-id="95cc8-140">Int32</span><span class="sxs-lookup"><span data-stu-id="95cc8-140">Int32</span></span>| <span data-ttu-id="95cc8-p106">DNS ホストで MX レコードの *Time To Live (ttl)* プロパティを設定するときに使用する値。null 許容ではありません</span><span class="sxs-lookup"><span data-stu-id="95cc8-p106">Value to use when configuring the *time-to-live (ttl)* property of the MX record at the DNS host. Not nullable</span></span> |

## <a name="relationships"></a><span data-ttu-id="95cc8-143">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="95cc8-143">Relationships</span></span>
<span data-ttu-id="95cc8-144">なし</span><span class="sxs-lookup"><span data-stu-id="95cc8-144">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="95cc8-145">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="95cc8-145">JSON representation</span></span>
<span data-ttu-id="95cc8-146">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="95cc8-146">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.domainDnsRecord",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.domainDnsMxRecord"
}-->

```json
{
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
<!-- {
  "type": "#page.annotation",
  "description": "domainDnsMxRecord resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->