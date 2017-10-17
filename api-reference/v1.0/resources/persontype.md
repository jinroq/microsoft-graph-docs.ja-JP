# <a name="persontype-resource-type"></a><span data-ttu-id="6b832-101">personType リソースの種類</span><span class="sxs-lookup"><span data-stu-id="6b832-101">personType resource type</span></span>

<span data-ttu-id="6b832-102">個人の種類を表します。</span><span class="sxs-lookup"><span data-stu-id="6b832-102">Represents the type of person.</span></span>


## <a name="json-representation"></a><span data-ttu-id="6b832-103">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="6b832-103">JSON representation</span></span>

<span data-ttu-id="6b832-104">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="6b832-104">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.personType"
}-->

```json
{
  "class": "string",
  "subclass": "string"
}

```
## <a name="properties"></a><span data-ttu-id="6b832-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="6b832-105">Properties</span></span>
| <span data-ttu-id="6b832-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="6b832-106">Property</span></span>     | <span data-ttu-id="6b832-107">型</span><span class="sxs-lookup"><span data-stu-id="6b832-107">Type</span></span>   |<span data-ttu-id="6b832-108">説明</span><span class="sxs-lookup"><span data-stu-id="6b832-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="6b832-109">クラス</span><span class="sxs-lookup"><span data-stu-id="6b832-109">class</span></span>|<span data-ttu-id="6b832-110">String</span><span class="sxs-lookup"><span data-stu-id="6b832-110">String</span></span>|<span data-ttu-id="6b832-111">データ ソースの種類 (Person など)。</span><span class="sxs-lookup"><span data-stu-id="6b832-111">The type of data source, such as Person.</span></span>|
|<span data-ttu-id="6b832-112">サブクラス</span><span class="sxs-lookup"><span data-stu-id="6b832-112">subclass</span></span>|<span data-ttu-id="6b832-113">String</span><span class="sxs-lookup"><span data-stu-id="6b832-113">String</span></span>|<span data-ttu-id="6b832-114">データ ソースの 2 番目の種類 (OrganizationUser など)。</span><span class="sxs-lookup"><span data-stu-id="6b832-114">The secondary type of data source, such as OrganizationUser.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "personType resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
