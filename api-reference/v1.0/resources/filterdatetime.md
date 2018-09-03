# <a name="filterdatetime-resource-type"></a><span data-ttu-id="1429f-101">FilterDatetime リソースの種類</span><span class="sxs-lookup"><span data-stu-id="1429f-101">FilterDatetime resource type</span></span>

<span data-ttu-id="1429f-102">値をフィルター処理するときに日付をフィルター処理する方法を表します。</span><span class="sxs-lookup"><span data-stu-id="1429f-102">Represents how to filter a date when filtering on values.</span></span>

## <a name="properties"></a><span data-ttu-id="1429f-103">プロパティ</span><span class="sxs-lookup"><span data-stu-id="1429f-103">Properties</span></span>
| <span data-ttu-id="1429f-104">プロパティ</span><span class="sxs-lookup"><span data-stu-id="1429f-104">Property</span></span>     | <span data-ttu-id="1429f-105">タイプ</span><span class="sxs-lookup"><span data-stu-id="1429f-105">Type</span></span>   |<span data-ttu-id="1429f-106">説明</span><span class="sxs-lookup"><span data-stu-id="1429f-106">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="1429f-107">日付</span><span class="sxs-lookup"><span data-stu-id="1429f-107">date</span></span>|<span data-ttu-id="1429f-108">文字列</span><span class="sxs-lookup"><span data-stu-id="1429f-108">string</span></span>|<span data-ttu-id="1429f-109">データをフィルターをかけるための ISO8601 形式の日付です。</span><span class="sxs-lookup"><span data-stu-id="1429f-109">The date in ISO8601 format used to filter data.</span></span>|
|<span data-ttu-id="1429f-110">特定性</span><span class="sxs-lookup"><span data-stu-id="1429f-110">specificity</span></span>|<span data-ttu-id="1429f-111">文字列</span><span class="sxs-lookup"><span data-stu-id="1429f-111">string</span></span>|<span data-ttu-id="1429f-112">データを保持するのに、日付をどの程度詳細に使用するか。</span><span class="sxs-lookup"><span data-stu-id="1429f-112">How specific the date should be used to keep data.</span></span> <span data-ttu-id="1429f-113">たとえば、日付が 2005-04-02 で "month" に設定した場合、フィルター操作では 2009 年 4 月の日付データを含むすべての行が保持されます。</span><span class="sxs-lookup"><span data-stu-id="1429f-113">How specific the date should be used to keep data. For example, if the date is 2005-04-02 and the specifity is set to "month", the filter operation will keep all rows with a date in the month of april 2009. Possible values are: , , , , , .</span></span> <span data-ttu-id="1429f-114">指定できる値は、  `Year`、`Monday`、`Day`、`Hour`、`Minute`、`Second` です。</span><span class="sxs-lookup"><span data-stu-id="1429f-114">The possible values are `Year`, `Monday`, `Day`, `Hour`, `Minute`, `Second`, , , , , , or .</span></span>|

## <a name="relationships"></a><span data-ttu-id="1429f-115">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="1429f-115">Relationships</span></span>
<span data-ttu-id="1429f-116">なし</span><span class="sxs-lookup"><span data-stu-id="1429f-116">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="1429f-117">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="1429f-117">JSON representation</span></span>

<span data-ttu-id="1429f-118">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="1429f-118">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.workbookFilterDateTime"
}-->

```json
{
  "date": "string",
  "specificity": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "FilterDatetime resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->