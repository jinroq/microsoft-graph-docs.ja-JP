# <a name="settingtemplatevalue-resource-type"></a><span data-ttu-id="9fcc5-101">settingTemplateValue リソースの種類</span><span class="sxs-lookup"><span data-stu-id="9fcc5-101">settingTemplateValue resource type</span></span>

<span data-ttu-id="9fcc5-102">設定がインスタンス化されていない場合の、設定の既定値を含む個々のテンプレートの設定定義を表します。</span><span class="sxs-lookup"><span data-stu-id="9fcc5-102">Represents an individual template setting definition, including the default value for the setting, if the setting is not instantiated.</span></span>

### <a name="properties"></a><span data-ttu-id="9fcc5-103">プロパティ</span><span class="sxs-lookup"><span data-stu-id="9fcc5-103">Properties</span></span>

| <span data-ttu-id="9fcc5-104">プロパティ</span><span class="sxs-lookup"><span data-stu-id="9fcc5-104">Property</span></span> | <span data-ttu-id="9fcc5-105">型</span><span class="sxs-lookup"><span data-stu-id="9fcc5-105">Type</span></span> | <span data-ttu-id="9fcc5-106">説明</span><span class="sxs-lookup"><span data-stu-id="9fcc5-106">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="9fcc5-107">defaultValue</span><span class="sxs-lookup"><span data-stu-id="9fcc5-107">DefaultValue</span></span>|<span data-ttu-id="9fcc5-108">文字列</span><span class="sxs-lookup"><span data-stu-id="9fcc5-108">String</span></span>| <span data-ttu-id="9fcc5-109">設定の既定値です。</span><span class="sxs-lookup"><span data-stu-id="9fcc5-109">Default value for the setting.</span></span> |
|<span data-ttu-id="9fcc5-110">説明</span><span class="sxs-lookup"><span data-stu-id="9fcc5-110">description</span></span>|<span data-ttu-id="9fcc5-111">文字列</span><span class="sxs-lookup"><span data-stu-id="9fcc5-111">String</span></span>| <span data-ttu-id="9fcc5-112">設定の説明です。</span><span class="sxs-lookup"><span data-stu-id="9fcc5-112">Description of the component.</span></span> |
|<span data-ttu-id="9fcc5-113">名前</span><span class="sxs-lookup"><span data-stu-id="9fcc5-113">name</span></span>|<span data-ttu-id="9fcc5-114">文字列</span><span class="sxs-lookup"><span data-stu-id="9fcc5-114">String</span></span>| <span data-ttu-id="9fcc5-115">設定の名前です。</span><span class="sxs-lookup"><span data-stu-id="9fcc5-115">Name of the setting.</span></span> |
|<span data-ttu-id="9fcc5-116">種類</span><span class="sxs-lookup"><span data-stu-id="9fcc5-116">type</span></span>|<span data-ttu-id="9fcc5-117">文字列</span><span class="sxs-lookup"><span data-stu-id="9fcc5-117">String</span></span>| <span data-ttu-id="9fcc5-118">設定の種類です。</span><span class="sxs-lookup"><span data-stu-id="9fcc5-118">Key of the setting.</span></span> |

### <a name="json-representation"></a><span data-ttu-id="9fcc5-119">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="9fcc5-119">JSON representation</span></span>

<span data-ttu-id="9fcc5-120">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="9fcc5-120">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.settingTemplateValue"
}-->

```json
{
  "defaultValue": "String",
  "description": "String",
  "name": "String",
  "type": "String"
}

```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "settingTemplateValue resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->