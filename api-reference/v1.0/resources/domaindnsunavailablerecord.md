---
title: domainDnsUnavailableRecord リソースの種類
description: ドメイン エンティティのナビゲーション プロパティの**serviceConfigurationRecords**のクエリを実行すると、1 つ以上の DomainDnsCnameRecord、DomainDnsMxRecord、DomainDnsSrvRecord、および DomainDnsTxtRecord のエンティティが表示されます。 これらのエンティティは、Microsoft Online Services で使用するドメインに、ドメインのゾーン ファイルに追加する必要がありますどのような DNS レコードを指定します。 このようなエンティティを生成できない場合は、DomainDnsUnavailableRecord のエンティティが返されます。 DomainDnsRecord エンティティから継承されます。
localization_priority: Normal
ms.openlocfilehash: 064fd294a89b48f6b7cfba58fa3d1076bf74a7ac
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27836184"
---
# <a name="domaindnsunavailablerecord-resource-type"></a><span data-ttu-id="57e3d-106">domainDnsUnavailableRecord リソースの種類</span><span class="sxs-lookup"><span data-stu-id="57e3d-106">domainDnsUnavailableRecord resource type</span></span>

<span data-ttu-id="57e3d-p102">[Domain](domain.md) エンティティのナビゲーション プロパティ **serviceConfigurationRecords** に対してクエリを実行すると、[DomainDnsCnameRecord](domaindnscnamerecord.md)、[DomainDnsMxRecord](domaindnsmxrecord.md)、[DomainDnsSrvRecord](domaindnssrvrecord.md)、[DomainDnsTxtRecord](domaindnstxtrecord.md) エンティティのいずれか 1 つ以上が返される場合があります。これらのエンティティは、ドメインを Microsoft オンライン サービスで使用する前に、そのドメインのゾーン ファイルに追加する必要のある DNS レコードを示します。このようなエンティティを生成できない場合、代わりに DomainDnsUnavailableRecord エンティティが返されます。[DomainDnsRecord](domaindnsrecord.md) エンティティから継承されます。</span><span class="sxs-lookup"><span data-stu-id="57e3d-p102">When you query for the navigation property **serviceConfigurationRecords** for a [Domain](domain.md) entity, you may get back one or more [DomainDnsCnameRecord](domaindnscnamerecord.md), [DomainDnsMxRecord](domaindnsmxrecord.md), [DomainDnsSrvRecord](domaindnssrvrecord.md), and/or [DomainDnsTxtRecord](domaindnstxtrecord.md) entities. These entities indicate what DNS records you must add to the zone file of the domain, before the domain can be used by Microsoft Online Services. When it is not possible to generate such entities, a DomainDnsUnavailableRecord Entity is returned instead. Inherited from [DomainDnsRecord](domaindnsrecord.md) entity.</span></span>

## <a name="methods"></a><span data-ttu-id="57e3d-111">メソッド</span><span class="sxs-lookup"><span data-stu-id="57e3d-111">Methods</span></span>
<span data-ttu-id="57e3d-p103">このリソースへの直接クエリはサポートされていません。ドメイン サービス レコードのクエリを実行する方法の詳細については、[ドメイン](domain.md)のトピックを参照してください。</span><span class="sxs-lookup"><span data-stu-id="57e3d-p103">Direct queries to this resource are not supported. Please see the [domain](domain.md) topic for information on how to query for domain service records.</span></span>

## <a name="properties"></a><span data-ttu-id="57e3d-114">プロパティ</span><span class="sxs-lookup"><span data-stu-id="57e3d-114">Properties</span></span>
| <span data-ttu-id="57e3d-115">プロパティ</span><span class="sxs-lookup"><span data-stu-id="57e3d-115">Property</span></span>     | <span data-ttu-id="57e3d-116">種類</span><span class="sxs-lookup"><span data-stu-id="57e3d-116">Type</span></span>   |<span data-ttu-id="57e3d-117">説明</span><span class="sxs-lookup"><span data-stu-id="57e3d-117">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="57e3d-118">説明</span><span class="sxs-lookup"><span data-stu-id="57e3d-118">description</span></span>|<span data-ttu-id="57e3d-119">String</span><span class="sxs-lookup"><span data-stu-id="57e3d-119">String</span></span>|<span data-ttu-id="57e3d-120">**DomainDnsUnavailableRecord** エンティティが返される理由を示します。</span><span class="sxs-lookup"><span data-stu-id="57e3d-120">Provides the reason why the **DomainDnsUnavailableRecord** entity is returned.</span></span> |

## <a name="relationships"></a><span data-ttu-id="57e3d-121">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="57e3d-121">Relationships</span></span>
<span data-ttu-id="57e3d-122">なし</span><span class="sxs-lookup"><span data-stu-id="57e3d-122">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="57e3d-123">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="57e3d-123">JSON representation</span></span>
<span data-ttu-id="57e3d-124">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="57e3d-124">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.domainDnsRecord",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.domainDnsUnavailableRecord"
}-->

```json
{
  "description": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "domainDnsUnavailableRecord resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
