# <a name="extension-resource-type"></a><span data-ttu-id="5d92d-101">拡張子リソースの種類</span><span class="sxs-lookup"><span data-stu-id="5d92d-101">extension resource type</span></span>

<span data-ttu-id="5d92d-102">OData v4 のオープン型 [openTypeExtension](openTypeExtension.md) をサポートする抽象型。</span><span class="sxs-lookup"><span data-stu-id="5d92d-102">An abstract type to support the OData v4 open type [openTypeExtension](openTypeExtension.md).</span></span>

## <a name="json-representation"></a><span data-ttu-id="5d92d-103">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="5d92d-103">JSON representation</span></span>

<span data-ttu-id="5d92d-104">以下は、リソースの JSON 表記です</span><span class="sxs-lookup"><span data-stu-id="5d92d-104">Here is a JSON representation of the resource</span></span>

<!-- {
  "abstract": "true",
  "baseType": "microsoft.graph.entity",
  "blockType": "resource",
  "openType": true,
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.extension"
}-->

```json
{
  "id": "string (identifier)"
}

```
## <a name="properties"></a><span data-ttu-id="5d92d-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="5d92d-105">Properties</span></span>
| <span data-ttu-id="5d92d-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="5d92d-106">Property</span></span>     | <span data-ttu-id="5d92d-107">タイプ</span><span class="sxs-lookup"><span data-stu-id="5d92d-107">Type</span></span>   |<span data-ttu-id="5d92d-108">説明</span><span class="sxs-lookup"><span data-stu-id="5d92d-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="5d92d-109">ID</span><span class="sxs-lookup"><span data-stu-id="5d92d-109">id</span></span>|<span data-ttu-id="5d92d-110">文字列</span><span class="sxs-lookup"><span data-stu-id="5d92d-110">String</span></span>| <span data-ttu-id="5d92d-111">読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="5d92d-111">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="5d92d-112">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="5d92d-112">Relationships</span></span>
<span data-ttu-id="5d92d-113">なし</span><span class="sxs-lookup"><span data-stu-id="5d92d-113">None</span></span>


## <a name="methods"></a><span data-ttu-id="5d92d-114">メソッド</span><span class="sxs-lookup"><span data-stu-id="5d92d-114">Methods</span></span>

<span data-ttu-id="5d92d-115">実際にサポートされるメソッドについては、派生型「[openTypeExtension](openTypeExtension.md)」のメソッドを参照してください。</span><span class="sxs-lookup"><span data-stu-id="5d92d-115">See the methods of the derived type [openTypeExtension](openTypeExtension.md) for actually supported methods.</span></span>


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "extension resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->