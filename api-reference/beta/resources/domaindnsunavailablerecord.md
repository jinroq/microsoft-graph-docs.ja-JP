---
title: domainDnsUnavailableRecord リソースの種類
description: ドメイン エンティティのナビゲーション プロパティの**serviceConfigurationRecords**のクエリを実行すると、1 つ以上の DomainDnsCnameRecord、DomainDnsMxRecord、DomainDnsSrvRecord、および DomainDnsTxtRecord のエンティティが表示されます。 これらのエンティティは、Microsoft Online Services で使用するドメインに、ドメインのゾーン ファイルに追加する必要がありますどのような DNS レコードを指定します。 このようなエンティティを生成できない場合は、DomainDnsUnavailableRecord のエンティティが返されます。 DomainDnsRecord エンティティから継承されます。
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 99da0448d75375b84bb37c05102c1f702c222a25
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27982793"
---
# <a name="domaindnsunavailablerecord-resource-type"></a><span data-ttu-id="23dd6-106">domainDnsUnavailableRecord リソースの種類</span><span class="sxs-lookup"><span data-stu-id="23dd6-106">domainDnsUnavailableRecord resource type</span></span>

> <span data-ttu-id="23dd6-107">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="23dd6-107">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="23dd6-108">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="23dd6-108">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="23dd6-p103">[Domain](domain.md) エンティティのナビゲーション プロパティ **serviceConfigurationRecords** に対してクエリを実行すると、[DomainDnsCnameRecord](domaindnscnamerecord.md)、[DomainDnsMxRecord](domaindnsmxrecord.md)、[DomainDnsSrvRecord](domaindnssrvrecord.md)、[DomainDnsTxtRecord](domaindnstxtrecord.md) エンティティのいずれか 1 つ以上が返される場合があります。これらのエンティティは、ドメインを Microsoft オンライン サービスで使用する前に、そのドメインのゾーン ファイルに追加する必要のある DNS レコードを示します。このようなエンティティを生成できない場合、代わりに DomainDnsUnavailableRecord エンティティが返されます。[DomainDnsRecord](domaindnsrecord.md) エンティティから継承されます。</span><span class="sxs-lookup"><span data-stu-id="23dd6-p103">When you query for the navigation property **serviceConfigurationRecords** for a [Domain](domain.md) entity, you may get back one or more [DomainDnsCnameRecord](domaindnscnamerecord.md), [DomainDnsMxRecord](domaindnsmxrecord.md), [DomainDnsSrvRecord](domaindnssrvrecord.md), and/or [DomainDnsTxtRecord](domaindnstxtrecord.md) entities. These entities indicate what DNS records you must add to the zone file of the domain, before the domain can be used by Microsoft Online Services. When it is not possible to generate such entities, a DomainDnsUnavailableRecord Entity is returned instead. Inherited from [DomainDnsRecord](domaindnsrecord.md) entity.</span></span>

## <a name="methods"></a><span data-ttu-id="23dd6-113">メソッド</span><span class="sxs-lookup"><span data-stu-id="23dd6-113">Methods</span></span>
<span data-ttu-id="23dd6-p104">このリソースへの直接クエリはサポートされていません。ドメイン サービス レコードのクエリを実行する方法の詳細については、[ドメイン](domain.md)のトピックを参照してください。</span><span class="sxs-lookup"><span data-stu-id="23dd6-p104">Direct queries to this resource are not supported. Please see the [domain](domain.md) topic for information on how to query for domain service records.</span></span>

## <a name="properties"></a><span data-ttu-id="23dd6-116">プロパティ</span><span class="sxs-lookup"><span data-stu-id="23dd6-116">Properties</span></span>
| <span data-ttu-id="23dd6-117">プロパティ</span><span class="sxs-lookup"><span data-stu-id="23dd6-117">Property</span></span>     | <span data-ttu-id="23dd6-118">種類</span><span class="sxs-lookup"><span data-stu-id="23dd6-118">Type</span></span>   |<span data-ttu-id="23dd6-119">説明</span><span class="sxs-lookup"><span data-stu-id="23dd6-119">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="23dd6-120">説明</span><span class="sxs-lookup"><span data-stu-id="23dd6-120">description</span></span>|<span data-ttu-id="23dd6-121">String</span><span class="sxs-lookup"><span data-stu-id="23dd6-121">String</span></span>|<span data-ttu-id="23dd6-122">**DomainDnsUnavailableRecord** エンティティが返される理由を示します。</span><span class="sxs-lookup"><span data-stu-id="23dd6-122">Provides the reason why the **DomainDnsUnavailableRecord** entity is returned.</span></span> |

## <a name="relationships"></a><span data-ttu-id="23dd6-123">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="23dd6-123">Relationships</span></span>
<span data-ttu-id="23dd6-124">なし</span><span class="sxs-lookup"><span data-stu-id="23dd6-124">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="23dd6-125">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="23dd6-125">JSON representation</span></span>
<span data-ttu-id="23dd6-126">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="23dd6-126">Here is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "domainDnsUnavailableRecord resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
