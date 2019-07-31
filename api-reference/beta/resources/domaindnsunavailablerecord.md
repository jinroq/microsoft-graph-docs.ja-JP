---
title: domainDnsUnavailableRecord リソースの種類
description: ドメインエンティティのナビゲーションプロパティ**serviceConfigurationRecords**に対してクエリを実行すると、1つ以上の DomainDnsCnameRecord、DomainDnsMxRecord、DomainDnsSrvRecord、または Domaindnst record エンティティが返される場合があります。 これらのエンティティは、ドメインを Microsoft Online Services で使用できるようにするために、ドメインのゾーンファイルに追加する必要がある DNS レコードを示します。 そのようなエンティティを生成できない場合は、代わりに DomainDnsUnavailableRecord エンティティが返されます。 DomainDnsRecord エンティティから継承されます。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: bf51b05614a89318fb7ba1afee9c4154ea1f6f27
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35973110"
---
# <a name="domaindnsunavailablerecord-resource-type"></a><span data-ttu-id="66ff9-106">domainDnsUnavailableRecord リソースの種類</span><span class="sxs-lookup"><span data-stu-id="66ff9-106">domainDnsUnavailableRecord resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="66ff9-107">[ドメイン](domain.md)エンティティに対してナビゲーションプロパティ**serviceConfigurationRecords**に対してクエリを実行すると、1つ以上の[DomainDnsCnameRecord](domaindnscnamerecord.md)、 [DomainDnsMxRecord](domaindnsmxrecord.md)、 [DomainDnsSrvRecord](domaindnssrvrecord.md)、または[が返されることがあります。Domaindnst・ Record](domaindnstxtrecord.md)エンティティ。</span><span class="sxs-lookup"><span data-stu-id="66ff9-107">When you query for the navigation property **serviceConfigurationRecords** for a [Domain](domain.md) entity, you may get back one or more [DomainDnsCnameRecord](domaindnscnamerecord.md), [DomainDnsMxRecord](domaindnsmxrecord.md), [DomainDnsSrvRecord](domaindnssrvrecord.md), and/or [DomainDnsTxtRecord](domaindnstxtrecord.md) entities.</span></span> <span data-ttu-id="66ff9-108">これらのエンティティは、ドメインを Microsoft Online Services で使用できるようにするために、ドメインのゾーンファイルに追加する必要がある DNS レコードを示します。</span><span class="sxs-lookup"><span data-stu-id="66ff9-108">These entities indicate what DNS records you must add to the zone file of the domain, before the domain can be used by Microsoft Online Services.</span></span> <span data-ttu-id="66ff9-109">そのようなエンティティを生成できない場合は、代わりに DomainDnsUnavailableRecord エンティティが返されます。</span><span class="sxs-lookup"><span data-stu-id="66ff9-109">When it is not possible to generate such entities, a DomainDnsUnavailableRecord Entity is returned instead.</span></span> <span data-ttu-id="66ff9-110">[Domaindnsrecord](domaindnsrecord.md)エンティティから継承されます。</span><span class="sxs-lookup"><span data-stu-id="66ff9-110">Inherited from [DomainDnsRecord](domaindnsrecord.md) entity.</span></span>

## <a name="methods"></a><span data-ttu-id="66ff9-111">メソッド</span><span class="sxs-lookup"><span data-stu-id="66ff9-111">Methods</span></span>
<span data-ttu-id="66ff9-112">このリソースへの直接クエリはサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="66ff9-112">Direct queries to this resource are not supported.</span></span> <span data-ttu-id="66ff9-113">ドメインサービスレコードを照会する方法については、「 [domain](domain.md) 」のトピックを参照してください。</span><span class="sxs-lookup"><span data-stu-id="66ff9-113">Please see the [domain](domain.md) topic for information on how to query for domain service records.</span></span>

## <a name="properties"></a><span data-ttu-id="66ff9-114">プロパティ</span><span class="sxs-lookup"><span data-stu-id="66ff9-114">Properties</span></span>
| <span data-ttu-id="66ff9-115">プロパティ</span><span class="sxs-lookup"><span data-stu-id="66ff9-115">Property</span></span>     | <span data-ttu-id="66ff9-116">型</span><span class="sxs-lookup"><span data-stu-id="66ff9-116">Type</span></span>   |<span data-ttu-id="66ff9-117">説明</span><span class="sxs-lookup"><span data-stu-id="66ff9-117">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="66ff9-118">description</span><span class="sxs-lookup"><span data-stu-id="66ff9-118">description</span></span>|<span data-ttu-id="66ff9-119">String</span><span class="sxs-lookup"><span data-stu-id="66ff9-119">String</span></span>|<span data-ttu-id="66ff9-120">**DomainDnsUnavailableRecord**エンティティが返される理由を示します。</span><span class="sxs-lookup"><span data-stu-id="66ff9-120">Provides the reason why the **DomainDnsUnavailableRecord** entity is returned.</span></span> |

## <a name="relationships"></a><span data-ttu-id="66ff9-121">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="66ff9-121">Relationships</span></span>
<span data-ttu-id="66ff9-122">なし</span><span class="sxs-lookup"><span data-stu-id="66ff9-122">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="66ff9-123">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="66ff9-123">JSON representation</span></span>
<span data-ttu-id="66ff9-124">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="66ff9-124">Here is a JSON representation of the resource.</span></span>

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
