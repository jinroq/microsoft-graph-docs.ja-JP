---
title: domainDnsUnavailableRecord リソースの種類
description: Domain エンティティのナビゲーション プロパティ serviceConfigurationRecords に対してクエリを実行すると、DomainDnsCnameRecord、DomainDnsMxRecord、DomainDnsSrvRecord、DomainDnsTxtRecord エンティティのいずれか 1 つ以上が返される場合があります。これらのエンティティは、ドメインを Microsoft オンライン サービスで使用する前に、そのドメインのゾーン ファイルに追加する必要のある DNS レコードを示します。このようなエンティティを生成できない場合、代わりに DomainDnsUnavailableRecord エンティティが返されます。DomainDnsRecord エンティティから継承されます。
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: fe3c1eeae7ae3ddb634a3c120332dd8d8996f41c
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29527872"
---
# <a name="domaindnsunavailablerecord-resource-type"></a><span data-ttu-id="21ae8-106">domainDnsUnavailableRecord リソースの種類</span><span class="sxs-lookup"><span data-stu-id="21ae8-106">domainDnsUnavailableRecord resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="21ae8-p102">[Domain](domain.md) エンティティのナビゲーション プロパティ **serviceConfigurationRecords** に対してクエリを実行すると、[DomainDnsCnameRecord](domaindnscnamerecord.md)、[DomainDnsMxRecord](domaindnsmxrecord.md)、[DomainDnsSrvRecord](domaindnssrvrecord.md)、[DomainDnsTxtRecord](domaindnstxtrecord.md) エンティティのいずれか 1 つ以上が返される場合があります。これらのエンティティは、ドメインを Microsoft オンライン サービスで使用する前に、そのドメインのゾーン ファイルに追加する必要のある DNS レコードを示します。このようなエンティティを生成できない場合、代わりに DomainDnsUnavailableRecord エンティティが返されます。[DomainDnsRecord](domaindnsrecord.md) エンティティから継承されます。</span><span class="sxs-lookup"><span data-stu-id="21ae8-p102">When you query for the navigation property **serviceConfigurationRecords** for a [Domain](domain.md) entity, you may get back one or more [DomainDnsCnameRecord](domaindnscnamerecord.md), [DomainDnsMxRecord](domaindnsmxrecord.md), [DomainDnsSrvRecord](domaindnssrvrecord.md), and/or [DomainDnsTxtRecord](domaindnstxtrecord.md) entities. These entities indicate what DNS records you must add to the zone file of the domain, before the domain can be used by Microsoft Online Services. When it is not possible to generate such entities, a DomainDnsUnavailableRecord Entity is returned instead. Inherited from [DomainDnsRecord](domaindnsrecord.md) entity.</span></span>

## <a name="methods"></a><span data-ttu-id="21ae8-111">メソッド</span><span class="sxs-lookup"><span data-stu-id="21ae8-111">Methods</span></span>
<span data-ttu-id="21ae8-p103">このリソースへの直接クエリはサポートされていません。ドメイン サービス レコードのクエリを実行する方法の詳細については、[ドメイン](domain.md)のトピックを参照してください。</span><span class="sxs-lookup"><span data-stu-id="21ae8-p103">Direct queries to this resource are not supported. Please see the [domain](domain.md) topic for information on how to query for domain service records.</span></span>

## <a name="properties"></a><span data-ttu-id="21ae8-114">プロパティ</span><span class="sxs-lookup"><span data-stu-id="21ae8-114">Properties</span></span>
| <span data-ttu-id="21ae8-115">プロパティ</span><span class="sxs-lookup"><span data-stu-id="21ae8-115">Property</span></span>     | <span data-ttu-id="21ae8-116">型</span><span class="sxs-lookup"><span data-stu-id="21ae8-116">Type</span></span>   |<span data-ttu-id="21ae8-117">説明</span><span class="sxs-lookup"><span data-stu-id="21ae8-117">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="21ae8-118">説明</span><span class="sxs-lookup"><span data-stu-id="21ae8-118">description</span></span>|<span data-ttu-id="21ae8-119">String</span><span class="sxs-lookup"><span data-stu-id="21ae8-119">String</span></span>|<span data-ttu-id="21ae8-120">**DomainDnsUnavailableRecord** エンティティが返される理由を示します。</span><span class="sxs-lookup"><span data-stu-id="21ae8-120">Provides the reason why the **DomainDnsUnavailableRecord** entity is returned.</span></span> |

## <a name="relationships"></a><span data-ttu-id="21ae8-121">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="21ae8-121">Relationships</span></span>
<span data-ttu-id="21ae8-122">なし</span><span class="sxs-lookup"><span data-stu-id="21ae8-122">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="21ae8-123">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="21ae8-123">JSON representation</span></span>
<span data-ttu-id="21ae8-124">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="21ae8-124">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.domainDnsUnavailableRecord"
}-->

```json
{
  "canonicalName": "String",
  "description": "String",
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
  "description": "domainDnsUnavailableRecord resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/domaindnsunavailablerecord.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
