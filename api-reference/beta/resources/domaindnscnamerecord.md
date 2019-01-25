---
title: domainDnsCnameRecord リソースの種類
description: テナント内の特定のドメインの DNS ゾーン ファイルに追加された CNAME レコードを表します。DomainDnsRecord エンティティから継承されます。
author: lleonard-msft
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: f270075556843625d1ec408f06be8ed4a065c831
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29516736"
---
# <a name="domaindnscnamerecord-resource-type"></a><span data-ttu-id="0f0ab-104">domainDnsCnameRecord リソースの種類</span><span class="sxs-lookup"><span data-stu-id="0f0ab-104">domainDnsCnameRecord resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0f0ab-p102">テナント内の特定のドメインの DNS ゾーン ファイルに追加された CNAME レコードを表します。[DomainDnsRecord](domaindnsrecord.md) エンティティから継承されます。</span><span class="sxs-lookup"><span data-stu-id="0f0ab-p102">Represents a CNAME record added to the DNS zone file of a particular domain in the tenant. Inherited from [DomainDnsRecord](domaindnsrecord.md) entity.</span></span>


## <a name="methods"></a><span data-ttu-id="0f0ab-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="0f0ab-107">Methods</span></span>
<span data-ttu-id="0f0ab-p103">このリソースへの直接クエリはサポートされていません。ドメイン サービス レコードのクエリを実行する方法の詳細については、[ドメイン](domain.md)のトピックを参照してください。</span><span class="sxs-lookup"><span data-stu-id="0f0ab-p103">Direct queries to this resource are not supported. Please see the [domain](domain.md) topic for information on how to query for domain service records.</span></span>

## <a name="properties"></a><span data-ttu-id="0f0ab-110">プロパティ</span><span class="sxs-lookup"><span data-stu-id="0f0ab-110">Properties</span></span>
| <span data-ttu-id="0f0ab-111">プロパティ</span><span class="sxs-lookup"><span data-stu-id="0f0ab-111">Property</span></span>     | <span data-ttu-id="0f0ab-112">型</span><span class="sxs-lookup"><span data-stu-id="0f0ab-112">Type</span></span>   |<span data-ttu-id="0f0ab-113">説明</span><span class="sxs-lookup"><span data-stu-id="0f0ab-113">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0f0ab-114">canonicalName</span><span class="sxs-lookup"><span data-stu-id="0f0ab-114">canonicalName</span></span>|<span data-ttu-id="0f0ab-115">String</span><span class="sxs-lookup"><span data-stu-id="0f0ab-115">String</span></span>| <span data-ttu-id="0f0ab-p104">CNAME レコードの正規名。DNS ホストで CNAME レコードを構成するために使用されます。</span><span class="sxs-lookup"><span data-stu-id="0f0ab-p104">The canonical name of the CNAME record. Used to configure the CNAME record at the DNS host.</span></span> |
|<span data-ttu-id="0f0ab-118">id</span><span class="sxs-lookup"><span data-stu-id="0f0ab-118">id</span></span>|<span data-ttu-id="0f0ab-119">String</span><span class="sxs-lookup"><span data-stu-id="0f0ab-119">String</span></span>| <span data-ttu-id="0f0ab-p105">このエンティティに割り当てられた一意の識別子。null 許容ではありません。読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="0f0ab-p105">Unique identifier assigned to this entity. Not nullable, Read-only</span></span>|
|<span data-ttu-id="0f0ab-122">isOptional</span><span class="sxs-lookup"><span data-stu-id="0f0ab-122">isOptional</span></span>|<span data-ttu-id="0f0ab-123">Boolean</span><span class="sxs-lookup"><span data-stu-id="0f0ab-123">Boolean</span></span>| <span data-ttu-id="0f0ab-p106">false の場合、ドメインが指定された Microsoft Online Services が適切に機能するには、CNAME レコードが DNS ホストで顧客によって構成されている必要があります。null 許容ではありません</span><span class="sxs-lookup"><span data-stu-id="0f0ab-p106">If false, the CNAME record must be configured by the customer at the DNS host for Microsoft Online Services to operate correctly with the domain. Not nullable</span></span> |
|<span data-ttu-id="0f0ab-126">label</span><span class="sxs-lookup"><span data-stu-id="0f0ab-126">label</span></span>|<span data-ttu-id="0f0ab-127">文字列</span><span class="sxs-lookup"><span data-stu-id="0f0ab-127">String</span></span>| <span data-ttu-id="0f0ab-128">DNS ホストで CNAME レコードの*エイリアス/ホスト/名前*を構成する場合に使用される値です。</span><span class="sxs-lookup"><span data-stu-id="0f0ab-128">Value used when configuring the *alias/host/name* of the CNAME record at the DNS host.</span></span> |
|<span data-ttu-id="0f0ab-129">recordType</span><span class="sxs-lookup"><span data-stu-id="0f0ab-129">recordType</span></span>|<span data-ttu-id="0f0ab-130">String</span><span class="sxs-lookup"><span data-stu-id="0f0ab-130">String</span></span>| <span data-ttu-id="0f0ab-p107">DNS レコードの種類。この値は常に *CName* です。キー</span><span class="sxs-lookup"><span data-stu-id="0f0ab-p107">Type of DNS record. The value is always *CName*. Key</span></span>|
|<span data-ttu-id="0f0ab-134">supportedService</span><span class="sxs-lookup"><span data-stu-id="0f0ab-134">supportedService</span></span>|<span data-ttu-id="0f0ab-135">String</span><span class="sxs-lookup"><span data-stu-id="0f0ab-135">String</span></span>| <span data-ttu-id="0f0ab-136">Microsoft オンライン サービスまたはこの CNAME レコードに依存している機能。</span><span class="sxs-lookup"><span data-stu-id="0f0ab-136">Microsoft Online Service or feature that has a dependency on this CNAME record.</span></span></br></br><span data-ttu-id="0f0ab-137">次のいずれかの値を指定できます。**null**、*Email*、*Sharepoint*、*EmailInternalRelayOnly*、*OfficeCommunicationsOnline*、*SharePointDefaultDomain*、*FullRedelegation*、*SharePointPublic*、*OrgIdAuthentication*、*Yammer*、*Intune*</span><span class="sxs-lookup"><span data-stu-id="0f0ab-137">Can be one of the following values: **null**, *Email*, *Sharepoint*, *EmailInternalRelayOnly*, *OfficeCommunicationsOnline*, *SharePointDefaultDomain*, *FullRedelegation*, *SharePointPublic*, *OrgIdAuthentication*, *Yammer*, *Intune*</span></span>|
|<span data-ttu-id="0f0ab-138">ttl</span><span class="sxs-lookup"><span data-stu-id="0f0ab-138">ttl</span></span>|<span data-ttu-id="0f0ab-139">Int32</span><span class="sxs-lookup"><span data-stu-id="0f0ab-139">Int32</span></span>| <span data-ttu-id="0f0ab-p108">DNS ホストで CNAME レコードの Time To Live (TTL) のプロパティを構成するときに使用する値。null 許容ではありません</span><span class="sxs-lookup"><span data-stu-id="0f0ab-p108">Value to use when configuring the time-to-live (ttl) property of the CNAME record at the DNS host. Not nullable</span></span> |

## <a name="relationships"></a><span data-ttu-id="0f0ab-142">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="0f0ab-142">Relationships</span></span>
<span data-ttu-id="0f0ab-143">なし</span><span class="sxs-lookup"><span data-stu-id="0f0ab-143">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="0f0ab-144">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="0f0ab-144">JSON representation</span></span>
<span data-ttu-id="0f0ab-145">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="0f0ab-145">Here is a JSON representation of the resource.</span></span>

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
  "suppressions": [
    "Error: /api-reference/beta/resources/domaindnscnamerecord.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
