# <a name="settingvalue-resource-type"></a><span data-ttu-id="036e3-101">settingValue リソースの種類</span><span class="sxs-lookup"><span data-stu-id="036e3-101">settingValue resource type</span></span>

<span data-ttu-id="036e3-102">名前と値の組で表される設定。</span><span class="sxs-lookup"><span data-stu-id="036e3-102">A setting represented by a name/value pair.</span></span>

### <a name="properties"></a><span data-ttu-id="036e3-103">プロパティ</span><span class="sxs-lookup"><span data-stu-id="036e3-103">Properties</span></span>

| <span data-ttu-id="036e3-104">プロパティ</span><span class="sxs-lookup"><span data-stu-id="036e3-104">Property</span></span> | <span data-ttu-id="036e3-105">型</span><span class="sxs-lookup"><span data-stu-id="036e3-105">Type</span></span> | <span data-ttu-id="036e3-106">説明</span><span class="sxs-lookup"><span data-stu-id="036e3-106">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="036e3-107">name</span><span class="sxs-lookup"><span data-stu-id="036e3-107">name</span></span>|<span data-ttu-id="036e3-108">文字列</span><span class="sxs-lookup"><span data-stu-id="036e3-108">String</span></span>| <span data-ttu-id="036e3-109">設定の名前 ([groupSettingTemplate](groupsettingtemplate.md) によって定義されている)。</span><span class="sxs-lookup"><span data-stu-id="036e3-109">Name of the setting (as defined by the [groupSettingTemplate](groupsettingtemplate.md)).</span></span> |
|<span data-ttu-id="036e3-110">値</span><span class="sxs-lookup"><span data-stu-id="036e3-110">value</span></span>|<span data-ttu-id="036e3-111">文字列</span><span class="sxs-lookup"><span data-stu-id="036e3-111">String</span></span>| <span data-ttu-id="036e3-112">設定の値です。</span><span class="sxs-lookup"><span data-stu-id="036e3-112">Value of the setting.</span></span> |

### <a name="json-representation"></a><span data-ttu-id="036e3-113">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="036e3-113">JSON representation</span></span>

<span data-ttu-id="036e3-114">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="036e3-114">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.settingValue"
}-->

```json
{
  "name": "String",
  "value": "String"
}

```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "settingValue resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->