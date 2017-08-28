# <a name="alternativesecurityid-resource-type"></a><span data-ttu-id="c1728-101">alternativeSecurityId リソースの種類</span><span class="sxs-lookup"><span data-stu-id="c1728-101">alternativeSecurityId resource type</span></span>

<span data-ttu-id="c1728-p101">デバイスに関連付けられている代替のセキュリティ ID が含まれています。[デバイス](device.md) エンティティの **alternativeSecurityIds** プロパティは、**alternativeSecurityId** のコレクションです。</span><span class="sxs-lookup"><span data-stu-id="c1728-p101">Contains an alternative security ID associated with a device. The **alternativeSecurityIds** property of the [Device](device.md) entity is a collection of **alternativeSecurityId**.</span></span>

## <a name="properties"></a><span data-ttu-id="c1728-104">プロパティ</span><span class="sxs-lookup"><span data-stu-id="c1728-104">Properties</span></span>
| <span data-ttu-id="c1728-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="c1728-105">Property</span></span>     | <span data-ttu-id="c1728-106">型</span><span class="sxs-lookup"><span data-stu-id="c1728-106">Type</span></span>   |<span data-ttu-id="c1728-107">説明</span><span class="sxs-lookup"><span data-stu-id="c1728-107">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c1728-108">identityProvider</span><span class="sxs-lookup"><span data-stu-id="c1728-108">identityProvider</span></span>|<span data-ttu-id="c1728-109">String</span><span class="sxs-lookup"><span data-stu-id="c1728-109">String</span></span>|            |
|<span data-ttu-id="c1728-110">key</span><span class="sxs-lookup"><span data-stu-id="c1728-110">key</span></span>|<span data-ttu-id="c1728-111">Binary</span><span class="sxs-lookup"><span data-stu-id="c1728-111">Binary</span></span>|            |
|<span data-ttu-id="c1728-112">type</span><span class="sxs-lookup"><span data-stu-id="c1728-112">type</span></span>|<span data-ttu-id="c1728-113">Int32</span><span class="sxs-lookup"><span data-stu-id="c1728-113">Int32</span></span>|            |

## <a name="json-representation"></a><span data-ttu-id="c1728-114">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="c1728-114">JSON representation</span></span>

<span data-ttu-id="c1728-115">以下は、リソースの JSON 表記です</span><span class="sxs-lookup"><span data-stu-id="c1728-115">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.alternativeSecurityId"
}-->

```json
{
  "identityProvider": "string",
  "key": "binary",
  "type": 1024
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "alternativeSecurityId resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
