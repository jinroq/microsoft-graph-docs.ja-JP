# <a name="domaindnsunavailablerecord-resource-type"></a><span data-ttu-id="0a15f-101">domainDnsUnavailableRecord リソースの種類</span><span class="sxs-lookup"><span data-stu-id="0a15f-101">domainDnsUnavailableRecord resource type</span></span>

<span data-ttu-id="0a15f-p101">[Domain](domain.md) エンティティのナビゲーション プロパティ **serviceConfigurationRecords** に対してクエリを実行すると、[DomainDnsCnameRecord](domaindnscnamerecord.md)、[DomainDnsMxRecord](domaindnsmxrecord.md)、[DomainDnsSrvRecord](domaindnssrvrecord.md)、[DomainDnsTxtRecord](domaindnstxtrecord.md) エンティティのいずれか 1 つ以上が返される場合があります。これらのエンティティは、ドメインを Microsoft オンライン サービスで使用する前に、そのドメインのゾーン ファイルに追加する必要のある DNS レコードを示します。このようなエンティティを生成できない場合、代わりに DomainDnsUnavailableRecord エンティティが返されます。[DomainDnsRecord](domaindnsrecord.md) エンティティから継承されます。</span><span class="sxs-lookup"><span data-stu-id="0a15f-p101">When you query for the navigation property **serviceConfigurationRecords** for a [Domain](domain.md) entity, you may get back one or more [DomainDnsCnameRecord](domaindnscnamerecord.md), [DomainDnsMxRecord](domaindnsmxrecord.md), [DomainDnsSrvRecord](domaindnssrvrecord.md), and/or [DomainDnsTxtRecord](domaindnstxtrecord.md) entities. These entities indicate what DNS records you must add to the zone file of the domain, before the domain can be used by Microsoft Online Services. When it is not possible to generate such entities, a DomainDnsUnavailableRecord Entity is returned instead. Inherited from [DomainDnsRecord](domaindnsrecord.md) entity.</span></span>

## <a name="methods"></a><span data-ttu-id="0a15f-106">メソッド</span><span class="sxs-lookup"><span data-stu-id="0a15f-106">Methods</span></span>
<span data-ttu-id="0a15f-p102">このリソースへの直接クエリはサポートされていません。ドメイン サービス レコードのクエリを実行する方法の詳細については、[ドメイン](domain.md)のトピックを参照してください。</span><span class="sxs-lookup"><span data-stu-id="0a15f-p102">Direct queries to this resource are not supported. Please see the [domain](domain.md) topic for information on how to query for domain service records.</span></span>

## <a name="properties"></a><span data-ttu-id="0a15f-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="0a15f-109">Properties</span></span>
| <span data-ttu-id="0a15f-110">プロパティ</span><span class="sxs-lookup"><span data-stu-id="0a15f-110">Property</span></span>     | <span data-ttu-id="0a15f-111">タイプ</span><span class="sxs-lookup"><span data-stu-id="0a15f-111">Type</span></span>   |<span data-ttu-id="0a15f-112">説明</span><span class="sxs-lookup"><span data-stu-id="0a15f-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0a15f-113">説明</span><span class="sxs-lookup"><span data-stu-id="0a15f-113">description</span></span>|<span data-ttu-id="0a15f-114">文字列</span><span class="sxs-lookup"><span data-stu-id="0a15f-114">String</span></span>|<span data-ttu-id="0a15f-115">**DomainDnsUnavailableRecord** エンティティが返される理由を示します。</span><span class="sxs-lookup"><span data-stu-id="0a15f-115">Provides the reason why the **DomainDnsUnavailableRecord** entity is returned.</span></span> |

## <a name="relationships"></a><span data-ttu-id="0a15f-116">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="0a15f-116">Relationships</span></span>
<span data-ttu-id="0a15f-117">なし</span><span class="sxs-lookup"><span data-stu-id="0a15f-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="0a15f-118">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="0a15f-118">JSON representation</span></span>
<span data-ttu-id="0a15f-119">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="0a15f-119">Here is a JSON representation of the resource.</span></span>

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