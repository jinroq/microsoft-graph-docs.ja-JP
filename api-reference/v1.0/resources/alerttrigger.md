# <a name="alerttrigger-resource-type"></a><span data-ttu-id="b2ba8-101">alertTrigger リソースの種類</span><span class="sxs-lookup"><span data-stu-id="b2ba8-101">alertTrigger resource type</span></span>

<span data-ttu-id="b2ba8-102">(プロパティがアラートのエンティティに存在する)、検出をトリガーするプロパティについて説明します。</span><span class="sxs-lookup"><span data-stu-id="b2ba8-102">Contains information about the properties that triggered a detection (properties exist in the alert entity).</span></span>

## <a name="properties"></a><span data-ttu-id="b2ba8-103">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b2ba8-103">Properties</span></span>

| <span data-ttu-id="b2ba8-104">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b2ba8-104">Property</span></span>   | <span data-ttu-id="b2ba8-105">型</span><span class="sxs-lookup"><span data-stu-id="b2ba8-105">Type</span></span>|<span data-ttu-id="b2ba8-106">説明</span><span class="sxs-lookup"><span data-stu-id="b2ba8-106">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b2ba8-107">名前</span><span class="sxs-lookup"><span data-stu-id="b2ba8-107">name</span></span>|<span data-ttu-id="b2ba8-108">文字列</span><span class="sxs-lookup"><span data-stu-id="b2ba8-108">String</span></span>|<span data-ttu-id="b2ba8-109">検出のトリガーとして機能するプロパティの名前です。</span><span class="sxs-lookup"><span data-stu-id="b2ba8-109">Name of the property serving as a detection trigger.</span></span>|
|<span data-ttu-id="b2ba8-110">type</span><span class="sxs-lookup"><span data-stu-id="b2ba8-110">type</span></span>|<span data-ttu-id="b2ba8-111">文字列</span><span class="sxs-lookup"><span data-stu-id="b2ba8-111">String</span></span>|<span data-ttu-id="b2ba8-112">解釈のキーと値のペアのプロパティの型。</span><span class="sxs-lookup"><span data-stu-id="b2ba8-112">Type of the property in the key:value pair for interpretation.</span></span> <span data-ttu-id="b2ba8-113">たとえば、文字列、ブール値などです。</span><span class="sxs-lookup"><span data-stu-id="b2ba8-113">For example, String, Boolean, etc.</span></span>|
|<span data-ttu-id="b2ba8-114">value</span><span class="sxs-lookup"><span data-stu-id="b2ba8-114">value</span></span>|<span data-ttu-id="b2ba8-115">文字列</span><span class="sxs-lookup"><span data-stu-id="b2ba8-115">String</span></span>|<span data-ttu-id="b2ba8-116">検出のトリガーとして機能するプロパティの値です。</span><span class="sxs-lookup"><span data-stu-id="b2ba8-116">Value of the property serving as a detection trigger.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="b2ba8-117">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="b2ba8-117">JSON representation</span></span>

<span data-ttu-id="b2ba8-118">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="b2ba8-118">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.alertTrigger"
}-->

```json
{
  "name": "String",
  "type": "String",
  "value": "String"
}

```

## <a name="example"></a><span data-ttu-id="b2ba8-119">例</span><span class="sxs-lookup"><span data-stu-id="b2ba8-119">Example</span></span>

```json
{
  "name": "hostState.privateIpAddress",
  "type": "String",
  "value": "10.154.9.40"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "alertTrigger resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->