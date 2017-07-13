<span data-ttu-id="47a68-p102">このリソースへの直接クエリはサポートされていません。ドメイン サービス レコードのクエリを実行する方法の詳細については、[ドメイン](domain.md)のトピックを参照してください。</span><span class="sxs-lookup"><span data-stu-id="47a68-p102">Direct queries to this resource are not supported. Please see the [domain](domain.md) topic for information on how to query for domain service records.</span></span>
このリソースへの直接クエリはサポートされていません。ドメイン サービス レコードのクエリを実行する方法の詳細については、[ドメイン](domain.md)のトピックを参照してください。

## <span data-ttu-id="47a68-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="47a68-109">Properties</span></span>
<a id="properties" class="xliff"></a>
| <span data-ttu-id="47a68-110">プロパティ</span><span class="sxs-lookup"><span data-stu-id="47a68-110">Property</span></span>     | <span data-ttu-id="47a68-111">型</span><span class="sxs-lookup"><span data-stu-id="47a68-111">Type</span></span>   |<span data-ttu-id="47a68-112">説明</span><span class="sxs-lookup"><span data-stu-id="47a68-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="47a68-113">description</span><span class="sxs-lookup"><span data-stu-id="47a68-113">description</span></span>|<span data-ttu-id="47a68-114">String</span><span class="sxs-lookup"><span data-stu-id="47a68-114">String</span></span>|<span data-ttu-id="47a68-115">**DomainDnsUnavailableRecord** エンティティが返される理由を示します。</span><span class="sxs-lookup"><span data-stu-id="47a68-115">Provides the reason why the **DomainDnsUnavailableRecord** entity is returned.</span></span> |

## <span data-ttu-id="47a68-116">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="47a68-116">Relationships</span></span>
<a id="relationships" class="xliff"></a>
<span data-ttu-id="47a68-117">なし</span><span class="sxs-lookup"><span data-stu-id="47a68-117">None</span></span>

## <span data-ttu-id="47a68-118">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="47a68-118">JSON representation</span></span>
<a id="json-representation" class="xliff"></a>
<span data-ttu-id="47a68-119">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="47a68-119">Here is a JSON representation of the resource.</span></span>

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