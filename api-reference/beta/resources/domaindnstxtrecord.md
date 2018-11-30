---
title: domainDnsTxtRecord リソースの種類
description: テナント内の特定のドメインの DNS ゾーン ファイルに追加された TXT レコードを表します。DomainDnsRecord エンティティから継承されます。
ms.openlocfilehash: 2c49f42c2044d58855d293d39c0e5110091e4495
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27073504"
---
# <a name="domaindnstxtrecord-resource-type"></a><span data-ttu-id="d0dbf-104">domainDnsTxtRecord リソースの種類</span><span class="sxs-lookup"><span data-stu-id="d0dbf-104">domainDnsTxtRecord resource type</span></span>

> <span data-ttu-id="d0dbf-105">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="d0dbf-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d0dbf-106">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d0dbf-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="d0dbf-p103">テナント内の特定のドメインの DNS ゾーン ファイルに追加された TXT レコードを表します。[DomainDnsRecord](domaindnsrecord.md) エンティティから継承されます。</span><span class="sxs-lookup"><span data-stu-id="d0dbf-p103">Represents a TXT record added to the DNS zone file of a particular domain in the tenant. Inherited from [DomainDnsRecord](domaindnsrecord.md) entity.</span></span>

## <a name="methods"></a><span data-ttu-id="d0dbf-109">メソッド</span><span class="sxs-lookup"><span data-stu-id="d0dbf-109">Methods</span></span>
<span data-ttu-id="d0dbf-p104">このリソースへの直接クエリはサポートされていません。ドメイン サービス レコードのクエリを実行する方法の詳細については、[ドメイン](domain.md)のトピックを参照してください。</span><span class="sxs-lookup"><span data-stu-id="d0dbf-p104">Direct queries to this resource are not supported. Please see the [domain](domain.md) topic for information on how to query for domain service records.</span></span>

## <a name="properties"></a><span data-ttu-id="d0dbf-112">プロパティ</span><span class="sxs-lookup"><span data-stu-id="d0dbf-112">Properties</span></span>
| <span data-ttu-id="d0dbf-113">プロパティ</span><span class="sxs-lookup"><span data-stu-id="d0dbf-113">Property</span></span>     | <span data-ttu-id="d0dbf-114">型</span><span class="sxs-lookup"><span data-stu-id="d0dbf-114">Type</span></span>   |<span data-ttu-id="d0dbf-115">説明</span><span class="sxs-lookup"><span data-stu-id="d0dbf-115">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d0dbf-116">id</span><span class="sxs-lookup"><span data-stu-id="d0dbf-116">id</span></span>|<span data-ttu-id="d0dbf-117">String</span><span class="sxs-lookup"><span data-stu-id="d0dbf-117">String</span></span>| <span data-ttu-id="d0dbf-p105">このエンティティに割り当てられた一意の識別子。null 許容ではありません。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="d0dbf-p105">Unique identifier assigned to this entity. Not nullable, Read-only.</span></span> |
|<span data-ttu-id="d0dbf-120">isOptional</span><span class="sxs-lookup"><span data-stu-id="d0dbf-120">isOptional</span></span>|<span data-ttu-id="d0dbf-121">ブール型</span><span class="sxs-lookup"><span data-stu-id="d0dbf-121">Boolean</span></span>| <span data-ttu-id="d0dbf-122">false の場合、ドメインが指定された Microsoft Online Services が適切に機能するには、TXT レコードが DNS ホストで顧客によって構成されている必要があります。</span><span class="sxs-lookup"><span data-stu-id="d0dbf-122">If false, the TXT record must be configured by the customer at the DNS host for Microsoft Online Services to operate correctly with the domain.</span></span> |
|<span data-ttu-id="d0dbf-123">label</span><span class="sxs-lookup"><span data-stu-id="d0dbf-123">label</span></span>|<span data-ttu-id="d0dbf-124">String</span><span class="sxs-lookup"><span data-stu-id="d0dbf-124">String</span></span>| <span data-ttu-id="d0dbf-125">DNS ホストで TXT レコードの *name* プロパティを構成する場合に使用する値。</span><span class="sxs-lookup"><span data-stu-id="d0dbf-125">Value to use when configuring the *name* property of the TXT record at the DNS host.</span></span>|
|<span data-ttu-id="d0dbf-126">recordType</span><span class="sxs-lookup"><span data-stu-id="d0dbf-126">recordType</span></span>|<span data-ttu-id="d0dbf-127">String</span><span class="sxs-lookup"><span data-stu-id="d0dbf-127">String</span></span>| <span data-ttu-id="d0dbf-p106">DNS レコードの種類。この値は常に *Txt* です。キー</span><span class="sxs-lookup"><span data-stu-id="d0dbf-p106">Type of DNS record. The value is always *Txt*. Key</span></span> |
|<span data-ttu-id="d0dbf-131">supportedService</span><span class="sxs-lookup"><span data-stu-id="d0dbf-131">supportedService</span></span>|<span data-ttu-id="d0dbf-132">String</span><span class="sxs-lookup"><span data-stu-id="d0dbf-132">String</span></span>| <span data-ttu-id="d0dbf-133">Microsoft オンライン サービスまたはこの TXT レコードに依存している機能。</span><span class="sxs-lookup"><span data-stu-id="d0dbf-133">Microsoft Online Service or feature that has a dependency on this TXT record.</span></span></br></br><span data-ttu-id="d0dbf-134">次のいずれかの値を指定できます。**null**、*Email*、*Sharepoint*、*EmailInternalRelayOnly*、*OfficeCommunicationsOnline*、*SharePointDefaultDomain*、*FullRedelegation*、*SharePointPublic*、*OrgIdAuthentication*、*Yammer*、*Intune*</span><span class="sxs-lookup"><span data-stu-id="d0dbf-134">Can be one of the following values: **null**, *Email*, *Sharepoint*, *EmailInternalRelayOnly*, *OfficeCommunicationsOnline*, *SharePointDefaultDomain*, *FullRedelegation*, *SharePointPublic*, *OrgIdAuthentication*, *Yammer*, *Intune*</span></span> |
|<span data-ttu-id="d0dbf-135">text</span><span class="sxs-lookup"><span data-stu-id="d0dbf-135">text</span></span>|<span data-ttu-id="d0dbf-136">String</span><span class="sxs-lookup"><span data-stu-id="d0dbf-136">String</span></span>| <span data-ttu-id="d0dbf-137">DNS ホストで *text* プロパティを設定するときに使用する値。</span><span class="sxs-lookup"><span data-stu-id="d0dbf-137">Value used when configuring the *text* property at the DNS host.</span></span> |
|<span data-ttu-id="d0dbf-138">ttl</span><span class="sxs-lookup"><span data-stu-id="d0dbf-138">ttl</span></span>|<span data-ttu-id="d0dbf-139">Int32</span><span class="sxs-lookup"><span data-stu-id="d0dbf-139">Int32</span></span>| <span data-ttu-id="d0dbf-p107">DNS ホストで MX レコードの *Time To Live (ttl)* プロパティを設定するときに使用する値。null 許容ではありません</span><span class="sxs-lookup"><span data-stu-id="d0dbf-p107">Value to use when configuring the *time-to-live (ttl)* property of the MX record at the DNS host. Not nullable</span></span> |

## <a name="relationships"></a><span data-ttu-id="d0dbf-142">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="d0dbf-142">Relationships</span></span>
<span data-ttu-id="d0dbf-143">なし</span><span class="sxs-lookup"><span data-stu-id="d0dbf-143">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="d0dbf-144">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="d0dbf-144">JSON representation</span></span>
<span data-ttu-id="d0dbf-145">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="d0dbf-145">Here is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "domainDnsTxtRecord resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->