---
title: domainDnsCnameRecord リソースの種類
description: テナント内の特定のドメインの DNS ゾーン ファイルに追加された CNAME レコードを表します。DomainDnsRecord エンティティから継承されます。
author: lleonard-msft
ms.openlocfilehash: 0ce5a748d9a1b558b4ac49e104eb9498efe674aa
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27315842"
---
# <a name="domaindnscnamerecord-resource-type"></a><span data-ttu-id="de636-104">domainDnsCnameRecord リソースの種類</span><span class="sxs-lookup"><span data-stu-id="de636-104">domainDnsCnameRecord resource type</span></span>

> <span data-ttu-id="de636-105">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="de636-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="de636-106">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="de636-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="de636-p103">テナント内の特定のドメインの DNS ゾーン ファイルに追加された CNAME レコードを表します。[DomainDnsRecord](domaindnsrecord.md) エンティティから継承されます。</span><span class="sxs-lookup"><span data-stu-id="de636-p103">Represents a CNAME record added to the DNS zone file of a particular domain in the tenant. Inherited from [DomainDnsRecord](domaindnsrecord.md) entity.</span></span>


## <a name="methods"></a><span data-ttu-id="de636-109">メソッド</span><span class="sxs-lookup"><span data-stu-id="de636-109">Methods</span></span>
<span data-ttu-id="de636-p104">このリソースへの直接クエリはサポートされていません。ドメイン サービス レコードのクエリを実行する方法の詳細については、[ドメイン](domain.md)のトピックを参照してください。</span><span class="sxs-lookup"><span data-stu-id="de636-p104">Direct queries to this resource are not supported. Please see the [domain](domain.md) topic for information on how to query for domain service records.</span></span>

## <a name="properties"></a><span data-ttu-id="de636-112">プロパティ</span><span class="sxs-lookup"><span data-stu-id="de636-112">Properties</span></span>
| <span data-ttu-id="de636-113">プロパティ</span><span class="sxs-lookup"><span data-stu-id="de636-113">Property</span></span>     | <span data-ttu-id="de636-114">種類</span><span class="sxs-lookup"><span data-stu-id="de636-114">Type</span></span>   |<span data-ttu-id="de636-115">説明</span><span class="sxs-lookup"><span data-stu-id="de636-115">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="de636-116">canonicalName</span><span class="sxs-lookup"><span data-stu-id="de636-116">canonicalName</span></span>|<span data-ttu-id="de636-117">String</span><span class="sxs-lookup"><span data-stu-id="de636-117">String</span></span>| <span data-ttu-id="de636-p105">CNAME レコードの正規名。DNS ホストで CNAME レコードを構成するために使用されます。</span><span class="sxs-lookup"><span data-stu-id="de636-p105">The canonical name of the CNAME record. Used to configure the CNAME record at the DNS host.</span></span> |
|<span data-ttu-id="de636-120">id</span><span class="sxs-lookup"><span data-stu-id="de636-120">id</span></span>|<span data-ttu-id="de636-121">String</span><span class="sxs-lookup"><span data-stu-id="de636-121">String</span></span>| <span data-ttu-id="de636-p106">このエンティティに割り当てられた一意の識別子。null 許容ではありません。読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="de636-p106">Unique identifier assigned to this entity. Not nullable, Read-only</span></span>|
|<span data-ttu-id="de636-124">isOptional</span><span class="sxs-lookup"><span data-stu-id="de636-124">isOptional</span></span>|<span data-ttu-id="de636-125">ブール型</span><span class="sxs-lookup"><span data-stu-id="de636-125">Boolean</span></span>| <span data-ttu-id="de636-p107">false の場合、ドメインが指定された Microsoft Online Services が適切に機能するには、CNAME レコードが DNS ホストで顧客によって構成されている必要があります。null 許容ではありません</span><span class="sxs-lookup"><span data-stu-id="de636-p107">If false, the CNAME record must be configured by the customer at the DNS host for Microsoft Online Services to operate correctly with the domain. Not nullable</span></span> |
|<span data-ttu-id="de636-128">label</span><span class="sxs-lookup"><span data-stu-id="de636-128">label</span></span>|<span data-ttu-id="de636-129">String</span><span class="sxs-lookup"><span data-stu-id="de636-129">String</span></span>| <span data-ttu-id="de636-130">DNS ホストで CNAME レコードの*エイリアス/ホスト/名前*を構成する場合に使用される値です。</span><span class="sxs-lookup"><span data-stu-id="de636-130">Value used when configuring the *alias/host/name* of the CNAME record at the DNS host.</span></span> |
|<span data-ttu-id="de636-131">recordType</span><span class="sxs-lookup"><span data-stu-id="de636-131">recordType</span></span>|<span data-ttu-id="de636-132">String</span><span class="sxs-lookup"><span data-stu-id="de636-132">String</span></span>| <span data-ttu-id="de636-p108">DNS レコードの種類。この値は常に *CName* です。キー</span><span class="sxs-lookup"><span data-stu-id="de636-p108">Type of DNS record. The value is always *CName*. Key</span></span>|
|<span data-ttu-id="de636-136">supportedService</span><span class="sxs-lookup"><span data-stu-id="de636-136">supportedService</span></span>|<span data-ttu-id="de636-137">String</span><span class="sxs-lookup"><span data-stu-id="de636-137">String</span></span>| <span data-ttu-id="de636-138">Microsoft オンライン サービスまたはこの CNAME レコードに依存している機能。</span><span class="sxs-lookup"><span data-stu-id="de636-138">Microsoft Online Service or feature that has a dependency on this CNAME record.</span></span></br></br><span data-ttu-id="de636-139">次のいずれかの値を指定できます。**null**、*Email*、*Sharepoint*、*EmailInternalRelayOnly*、*OfficeCommunicationsOnline*、*SharePointDefaultDomain*、*FullRedelegation*、*SharePointPublic*、*OrgIdAuthentication*、*Yammer*、*Intune*</span><span class="sxs-lookup"><span data-stu-id="de636-139">Can be one of the following values: **null**, *Email*, *Sharepoint*, *EmailInternalRelayOnly*, *OfficeCommunicationsOnline*, *SharePointDefaultDomain*, *FullRedelegation*, *SharePointPublic*, *OrgIdAuthentication*, *Yammer*, *Intune*</span></span>|
|<span data-ttu-id="de636-140">ttl</span><span class="sxs-lookup"><span data-stu-id="de636-140">ttl</span></span>|<span data-ttu-id="de636-141">Int32</span><span class="sxs-lookup"><span data-stu-id="de636-141">Int32</span></span>| <span data-ttu-id="de636-p109">DNS ホストで CNAME レコードの Time To Live (TTL) のプロパティを構成するときに使用する値。null 許容ではありません</span><span class="sxs-lookup"><span data-stu-id="de636-p109">Value to use when configuring the time-to-live (ttl) property of the CNAME record at the DNS host. Not nullable</span></span> |

## <a name="relationships"></a><span data-ttu-id="de636-144">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="de636-144">Relationships</span></span>
<span data-ttu-id="de636-145">なし</span><span class="sxs-lookup"><span data-stu-id="de636-145">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="de636-146">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="de636-146">JSON representation</span></span>
<span data-ttu-id="de636-147">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="de636-147">Here is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "domainDnsCnameRecord resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->