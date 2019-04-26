---
title: domainDnsUnavailableRecord リソースの種類
description: ドメインエンティティのナビゲーションプロパティ**serviceConfigurationRecords**に対してクエリを実行すると、1つ以上の DomainDnsCnameRecord、DomainDnsMxRecord、DomainDnsSrvRecord、または domaindnst record エンティティが返される場合があります。 これらのエンティティは、ドメインを Microsoft Online Services で使用できるようにするために、ドメインのゾーンファイルに追加する必要がある DNS レコードを示します。 そのようなエンティティを生成できない場合は、代わりに DomainDnsUnavailableRecord エンティティが返されます。 domaindnsrecord エンティティから継承されます。
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 5f033c39c9cf8dc11c2a41b0cedb0b8de5ce7736
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32562770"
---
# <a name="domaindnsunavailablerecord-resource-type"></a><span data-ttu-id="e7f8b-106">domainDnsUnavailableRecord リソースの種類</span><span class="sxs-lookup"><span data-stu-id="e7f8b-106">domainDnsUnavailableRecord resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e7f8b-107">[ドメイン](domain.md)エンティティに対してナビゲーションプロパティ**serviceConfigurationRecords**に対してクエリを実行すると、1つ以上の[DomainDnsCnameRecord](domaindnscnamerecord.md)、 [DomainDnsMxRecord](domaindnsmxrecord.md)、 [DomainDnsSrvRecord](domaindnssrvrecord.md)、または[が返されることがあります。domaindnst・ record](domaindnstxtrecord.md)エンティティ。</span><span class="sxs-lookup"><span data-stu-id="e7f8b-107">When you query for the navigation property **serviceConfigurationRecords** for a [Domain](domain.md) entity, you may get back one or more [DomainDnsCnameRecord](domaindnscnamerecord.md), [DomainDnsMxRecord](domaindnsmxrecord.md), [DomainDnsSrvRecord](domaindnssrvrecord.md), and/or [DomainDnsTxtRecord](domaindnstxtrecord.md) entities.</span></span> <span data-ttu-id="e7f8b-108">これらのエンティティは、ドメインを Microsoft Online Services で使用できるようにするために、ドメインのゾーンファイルに追加する必要がある DNS レコードを示します。</span><span class="sxs-lookup"><span data-stu-id="e7f8b-108">These entities indicate what DNS records you must add to the zone file of the domain, before the domain can be used by Microsoft Online Services.</span></span> <span data-ttu-id="e7f8b-109">そのようなエンティティを生成できない場合は、代わりに DomainDnsUnavailableRecord エンティティが返されます。</span><span class="sxs-lookup"><span data-stu-id="e7f8b-109">When it is not possible to generate such entities, a DomainDnsUnavailableRecord Entity is returned instead.</span></span> <span data-ttu-id="e7f8b-110">[domaindnsrecord](domaindnsrecord.md)エンティティから継承されます。</span><span class="sxs-lookup"><span data-stu-id="e7f8b-110">Inherited from [DomainDnsRecord](domaindnsrecord.md) entity.</span></span>

## <a name="methods"></a><span data-ttu-id="e7f8b-111">メソッド</span><span class="sxs-lookup"><span data-stu-id="e7f8b-111">Methods</span></span>
<span data-ttu-id="e7f8b-112">このリソースへの直接クエリはサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e7f8b-112">Direct queries to this resource are not supported.</span></span> <span data-ttu-id="e7f8b-113">ドメインサービスレコードを照会する方法については、「 [domain](domain.md) 」のトピックを参照してください。</span><span class="sxs-lookup"><span data-stu-id="e7f8b-113">Please see the [domain](domain.md) topic for information on how to query for domain service records.</span></span>

## <a name="properties"></a><span data-ttu-id="e7f8b-114">プロパティ</span><span class="sxs-lookup"><span data-stu-id="e7f8b-114">Properties</span></span>
| <span data-ttu-id="e7f8b-115">プロパティ</span><span class="sxs-lookup"><span data-stu-id="e7f8b-115">Property</span></span>     | <span data-ttu-id="e7f8b-116">型</span><span class="sxs-lookup"><span data-stu-id="e7f8b-116">Type</span></span>   |<span data-ttu-id="e7f8b-117">説明</span><span class="sxs-lookup"><span data-stu-id="e7f8b-117">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e7f8b-118">description</span><span class="sxs-lookup"><span data-stu-id="e7f8b-118">description</span></span>|<span data-ttu-id="e7f8b-119">String</span><span class="sxs-lookup"><span data-stu-id="e7f8b-119">String</span></span>|<span data-ttu-id="e7f8b-120">**DomainDnsUnavailableRecord**エンティティが返される理由を示します。</span><span class="sxs-lookup"><span data-stu-id="e7f8b-120">Provides the reason why the **DomainDnsUnavailableRecord** entity is returned.</span></span> |

## <a name="relationships"></a><span data-ttu-id="e7f8b-121">関係</span><span class="sxs-lookup"><span data-stu-id="e7f8b-121">Relationships</span></span>
<span data-ttu-id="e7f8b-122">なし</span><span class="sxs-lookup"><span data-stu-id="e7f8b-122">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="e7f8b-123">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="e7f8b-123">JSON representation</span></span>
<span data-ttu-id="e7f8b-124">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="e7f8b-124">Here is a JSON representation of the resource.</span></span>

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
  "suppressions": []
}
-->
