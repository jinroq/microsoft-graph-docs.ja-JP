---
title: domainDnsMxRecord リソースの種類
description: テナント内の特定のドメインの DNS ゾーン ファイルに追加された MX レコードを表します。DomainDnsRecord エンティティから継承されます。
author: lleonard-msft
localization_priority: Normal
ms.openlocfilehash: c6ffa526b359eed6bafa7f38562d5d61c4f4562a
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27830248"
---
# <a name="domaindnsmxrecord-resource-type"></a><span data-ttu-id="0b57b-104">domainDnsMxRecord リソースの種類</span><span class="sxs-lookup"><span data-stu-id="0b57b-104">domainDnsMxRecord resource type</span></span>

> <span data-ttu-id="0b57b-105">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="0b57b-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="0b57b-106">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="0b57b-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="0b57b-p103">テナント内の特定のドメインの DNS ゾーン ファイルに追加された MX レコードを表します。[DomainDnsRecord](domaindnsrecord.md) エンティティから継承されます。</span><span class="sxs-lookup"><span data-stu-id="0b57b-p103">Represents a MX record added to the DNS zone file of a particular domain in the tenant. Inherited from [DomainDnsRecord](domaindnsrecord.md) entity.</span></span>

## <a name="methods"></a><span data-ttu-id="0b57b-109">メソッド</span><span class="sxs-lookup"><span data-stu-id="0b57b-109">Methods</span></span>
<span data-ttu-id="0b57b-p104">このリソースへの直接クエリはサポートされていません。ドメイン サービス レコードのクエリを実行する方法の詳細については、[ドメイン](domain.md)のトピックを参照してください。</span><span class="sxs-lookup"><span data-stu-id="0b57b-p104">Direct queries to this resource are not supported. Please see the [domain](domain.md) topic for information on how to query for domain service records.</span></span>

## <a name="properties"></a><span data-ttu-id="0b57b-112">プロパティ</span><span class="sxs-lookup"><span data-stu-id="0b57b-112">Properties</span></span>
| <span data-ttu-id="0b57b-113">プロパティ</span><span class="sxs-lookup"><span data-stu-id="0b57b-113">Property</span></span>     | <span data-ttu-id="0b57b-114">種類</span><span class="sxs-lookup"><span data-stu-id="0b57b-114">Type</span></span>   |<span data-ttu-id="0b57b-115">説明</span><span class="sxs-lookup"><span data-stu-id="0b57b-115">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0b57b-116">ID</span><span class="sxs-lookup"><span data-stu-id="0b57b-116">id</span></span>|<span data-ttu-id="0b57b-117">String</span><span class="sxs-lookup"><span data-stu-id="0b57b-117">String</span></span>| <span data-ttu-id="0b57b-p105">このエンティティに割り当てられた一意の識別子。null 許容ではありません。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="0b57b-p105">Unique identifier assigned to this entity. Not nullable, Read-only.</span></span>|
|<span data-ttu-id="0b57b-120">isOptional</span><span class="sxs-lookup"><span data-stu-id="0b57b-120">isOptional</span></span>|<span data-ttu-id="0b57b-121">Boolean</span><span class="sxs-lookup"><span data-stu-id="0b57b-121">Boolean</span></span>| <span data-ttu-id="0b57b-122">False の場合、MX レコードは Microsoft オンライン サービスでドメインを正しく操作するために、DNS ホストで顧客によって構成されている必要があります。</span><span class="sxs-lookup"><span data-stu-id="0b57b-122">If false, the MX record must be configured by the customer at the DNS host for Microsoft Online Services to operate correctly with the domain.</span></span> |
|<span data-ttu-id="0b57b-123">label</span><span class="sxs-lookup"><span data-stu-id="0b57b-123">label</span></span>|<span data-ttu-id="0b57b-124">String</span><span class="sxs-lookup"><span data-stu-id="0b57b-124">String</span></span>| <span data-ttu-id="0b57b-125">DNS ホストで MX レコードの *alias/host/name* プロパティを構成する場合に使用される値です。</span><span class="sxs-lookup"><span data-stu-id="0b57b-125">Value used when configuring the *alias/host/name* property of the MX record at the DNS host.</span></span> |
|<span data-ttu-id="0b57b-126">mailExchange</span><span class="sxs-lookup"><span data-stu-id="0b57b-126">mailExchange</span></span>|<span data-ttu-id="0b57b-127">String</span><span class="sxs-lookup"><span data-stu-id="0b57b-127">String</span></span>| <span data-ttu-id="0b57b-128">DNS ホストで MX レコードの *answer/destination/value* を構成する場合に使用される値です。</span><span class="sxs-lookup"><span data-stu-id="0b57b-128">Value used when configuring the *answer/destination/value* of the MX record at the DNS host.</span></span>|
|<span data-ttu-id="0b57b-129">preference</span><span class="sxs-lookup"><span data-stu-id="0b57b-129">preference</span></span>|<span data-ttu-id="0b57b-130">Int32</span><span class="sxs-lookup"><span data-stu-id="0b57b-130">Int32</span></span>| <span data-ttu-id="0b57b-131">DNS ホストで MX レコードの *Preference/Priority* プロパティを構成する場合に使用される値です。</span><span class="sxs-lookup"><span data-stu-id="0b57b-131">Value used when configuring the *Preference/Priority* property of the MX record at the DNS host.</span></span> |
|<span data-ttu-id="0b57b-132">recordType</span><span class="sxs-lookup"><span data-stu-id="0b57b-132">recordType</span></span>|<span data-ttu-id="0b57b-133">String</span><span class="sxs-lookup"><span data-stu-id="0b57b-133">String</span></span>| <span data-ttu-id="0b57b-p106">DNS レコードの種類。この値は常に *Mx* です。キー</span><span class="sxs-lookup"><span data-stu-id="0b57b-p106">Type of DNS record. The value is always *Mx*. Key</span></span> |
|<span data-ttu-id="0b57b-137">supportedService</span><span class="sxs-lookup"><span data-stu-id="0b57b-137">supportedService</span></span>|<span data-ttu-id="0b57b-138">String</span><span class="sxs-lookup"><span data-stu-id="0b57b-138">String</span></span>| <span data-ttu-id="0b57b-139">Microsoft オンライン サービスまたはこの MX レコードに依存している機能。</span><span class="sxs-lookup"><span data-stu-id="0b57b-139">Microsoft Online Service or feature that has a dependency on this MX record.</span></span></br></br><span data-ttu-id="0b57b-140">次のいずれかの値を指定できます。**null**、*Email*、*Sharepoint*、*EmailInternalRelayOnly*、*OfficeCommunicationsOnline*、*SharePointDefaultDomain*、*FullRedelegation*、*SharePointPublic*、*OrgIdAuthentication*、*Yammer*、*Intune*</span><span class="sxs-lookup"><span data-stu-id="0b57b-140">Can be one of the following values: **null**, *Email*, *Sharepoint*, *EmailInternalRelayOnly*, *OfficeCommunicationsOnline*, *SharePointDefaultDomain*, *FullRedelegation*, *SharePointPublic*, *OrgIdAuthentication*, *Yammer*, *Intune*</span></span> |
|<span data-ttu-id="0b57b-141">ttl</span><span class="sxs-lookup"><span data-stu-id="0b57b-141">ttl</span></span>|<span data-ttu-id="0b57b-142">Int32</span><span class="sxs-lookup"><span data-stu-id="0b57b-142">Int32</span></span>| <span data-ttu-id="0b57b-p107">DNS ホストで MX レコードの *Time To Live (ttl)* プロパティを設定するときに使用する値。null 許容ではありません</span><span class="sxs-lookup"><span data-stu-id="0b57b-p107">Value to use when configuring the *time-to-live (ttl)* property of the MX record at the DNS host. Not nullable</span></span> |

## <a name="relationships"></a><span data-ttu-id="0b57b-145">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="0b57b-145">Relationships</span></span>
<span data-ttu-id="0b57b-146">なし</span><span class="sxs-lookup"><span data-stu-id="0b57b-146">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="0b57b-147">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="0b57b-147">JSON representation</span></span>
<span data-ttu-id="0b57b-148">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="0b57b-148">Here is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "domainDnsMxRecord resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
