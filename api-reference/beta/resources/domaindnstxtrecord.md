---
title: domainDnsTxtRecord リソースの種類
description: テナント内の特定のドメインの DNS ゾーン ファイルに追加された TXT レコードを表します。DomainDnsRecord エンティティから継承されます。
author: lleonard-msft
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 4bdcddc0ec81d8a7fc76e2113155fdc7ee871161
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29522246"
---
# <a name="domaindnstxtrecord-resource-type"></a><span data-ttu-id="5e531-104">domainDnsTxtRecord リソースの種類</span><span class="sxs-lookup"><span data-stu-id="5e531-104">domainDnsTxtRecord resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5e531-p102">テナント内の特定のドメインの DNS ゾーン ファイルに追加された TXT レコードを表します。[DomainDnsRecord](domaindnsrecord.md) エンティティから継承されます。</span><span class="sxs-lookup"><span data-stu-id="5e531-p102">Represents a TXT record added to the DNS zone file of a particular domain in the tenant. Inherited from [DomainDnsRecord](domaindnsrecord.md) entity.</span></span>

## <a name="methods"></a><span data-ttu-id="5e531-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="5e531-107">Methods</span></span>
<span data-ttu-id="5e531-p103">このリソースへの直接クエリはサポートされていません。ドメイン サービス レコードのクエリを実行する方法の詳細については、[ドメイン](domain.md)のトピックを参照してください。</span><span class="sxs-lookup"><span data-stu-id="5e531-p103">Direct queries to this resource are not supported. Please see the [domain](domain.md) topic for information on how to query for domain service records.</span></span>

## <a name="properties"></a><span data-ttu-id="5e531-110">プロパティ</span><span class="sxs-lookup"><span data-stu-id="5e531-110">Properties</span></span>
| <span data-ttu-id="5e531-111">プロパティ</span><span class="sxs-lookup"><span data-stu-id="5e531-111">Property</span></span>     | <span data-ttu-id="5e531-112">型</span><span class="sxs-lookup"><span data-stu-id="5e531-112">Type</span></span>   |<span data-ttu-id="5e531-113">説明</span><span class="sxs-lookup"><span data-stu-id="5e531-113">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="5e531-114">id</span><span class="sxs-lookup"><span data-stu-id="5e531-114">id</span></span>|<span data-ttu-id="5e531-115">String</span><span class="sxs-lookup"><span data-stu-id="5e531-115">String</span></span>| <span data-ttu-id="5e531-p104">このエンティティに割り当てられた一意の識別子。null 許容ではありません。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="5e531-p104">Unique identifier assigned to this entity. Not nullable, Read-only.</span></span> |
|<span data-ttu-id="5e531-118">isOptional</span><span class="sxs-lookup"><span data-stu-id="5e531-118">isOptional</span></span>|<span data-ttu-id="5e531-119">ブール型</span><span class="sxs-lookup"><span data-stu-id="5e531-119">Boolean</span></span>| <span data-ttu-id="5e531-120">false の場合、ドメインが指定された Microsoft Online Services が適切に機能するには、TXT レコードが DNS ホストで顧客によって構成されている必要があります。</span><span class="sxs-lookup"><span data-stu-id="5e531-120">If false, the TXT record must be configured by the customer at the DNS host for Microsoft Online Services to operate correctly with the domain.</span></span> |
|<span data-ttu-id="5e531-121">label</span><span class="sxs-lookup"><span data-stu-id="5e531-121">label</span></span>|<span data-ttu-id="5e531-122">文字列</span><span class="sxs-lookup"><span data-stu-id="5e531-122">String</span></span>| <span data-ttu-id="5e531-123">DNS ホストで TXT レコードの *name* プロパティを構成する場合に使用する値。</span><span class="sxs-lookup"><span data-stu-id="5e531-123">Value to use when configuring the *name* property of the TXT record at the DNS host.</span></span>|
|<span data-ttu-id="5e531-124">recordType</span><span class="sxs-lookup"><span data-stu-id="5e531-124">recordType</span></span>|<span data-ttu-id="5e531-125">String</span><span class="sxs-lookup"><span data-stu-id="5e531-125">String</span></span>| <span data-ttu-id="5e531-p105">DNS レコードの種類。この値は常に *Txt* です。キー</span><span class="sxs-lookup"><span data-stu-id="5e531-p105">Type of DNS record. The value is always *Txt*. Key</span></span> |
|<span data-ttu-id="5e531-129">supportedService</span><span class="sxs-lookup"><span data-stu-id="5e531-129">supportedService</span></span>|<span data-ttu-id="5e531-130">String</span><span class="sxs-lookup"><span data-stu-id="5e531-130">String</span></span>| <span data-ttu-id="5e531-131">Microsoft オンライン サービスまたはこの TXT レコードに依存している機能。</span><span class="sxs-lookup"><span data-stu-id="5e531-131">Microsoft Online Service or feature that has a dependency on this TXT record.</span></span></br></br><span data-ttu-id="5e531-132">次のいずれかの値を指定できます。**null**、*Email*、*Sharepoint*、*EmailInternalRelayOnly*、*OfficeCommunicationsOnline*、*SharePointDefaultDomain*、*FullRedelegation*、*SharePointPublic*、*OrgIdAuthentication*、*Yammer*、*Intune*</span><span class="sxs-lookup"><span data-stu-id="5e531-132">Can be one of the following values: **null**, *Email*, *Sharepoint*, *EmailInternalRelayOnly*, *OfficeCommunicationsOnline*, *SharePointDefaultDomain*, *FullRedelegation*, *SharePointPublic*, *OrgIdAuthentication*, *Yammer*, *Intune*</span></span> |
|<span data-ttu-id="5e531-133">text</span><span class="sxs-lookup"><span data-stu-id="5e531-133">text</span></span>|<span data-ttu-id="5e531-134">String</span><span class="sxs-lookup"><span data-stu-id="5e531-134">String</span></span>| <span data-ttu-id="5e531-135">DNS ホストで *text* プロパティを設定するときに使用する値。</span><span class="sxs-lookup"><span data-stu-id="5e531-135">Value used when configuring the *text* property at the DNS host.</span></span> |
|<span data-ttu-id="5e531-136">ttl</span><span class="sxs-lookup"><span data-stu-id="5e531-136">ttl</span></span>|<span data-ttu-id="5e531-137">Int32</span><span class="sxs-lookup"><span data-stu-id="5e531-137">Int32</span></span>| <span data-ttu-id="5e531-p106">DNS ホストで MX レコードの *Time To Live (ttl)* プロパティを設定するときに使用する値。null 許容ではありません</span><span class="sxs-lookup"><span data-stu-id="5e531-p106">Value to use when configuring the *time-to-live (ttl)* property of the MX record at the DNS host. Not nullable</span></span> |

## <a name="relationships"></a><span data-ttu-id="5e531-140">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="5e531-140">Relationships</span></span>
<span data-ttu-id="5e531-141">なし</span><span class="sxs-lookup"><span data-stu-id="5e531-141">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="5e531-142">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="5e531-142">JSON representation</span></span>
<span data-ttu-id="5e531-143">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="5e531-143">Here is a JSON representation of the resource.</span></span>

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
  "suppressions": [
    "Error: /api-reference/beta/resources/domaindnstxtrecord.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
