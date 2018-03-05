# <a name="educationterm-resource-type"></a><span data-ttu-id="62b82-101">educationTerm リソースの種類</span><span class="sxs-lookup"><span data-stu-id="62b82-101">educationTerm resource type</span></span>

<span data-ttu-id="62b82-102">用語。</span><span class="sxs-lookup"><span data-stu-id="62b82-102">A term.</span></span> <span data-ttu-id="62b82-103">これは学年度の指定された部分を示します。</span><span class="sxs-lookup"><span data-stu-id="62b82-103">This represents a designated portion of the academic year.</span></span> <span data-ttu-id="62b82-104">[educationClass](educationclass.md) 内で使用します。</span><span class="sxs-lookup"><span data-stu-id="62b82-104">It is used within [educationClass](educationclass.md).</span></span>

## <a name="properties"></a><span data-ttu-id="62b82-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="62b82-105">Properties</span></span>
| <span data-ttu-id="62b82-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="62b82-106">Property</span></span>     | <span data-ttu-id="62b82-107">型</span><span class="sxs-lookup"><span data-stu-id="62b82-107">Type</span></span>   |<span data-ttu-id="62b82-108">説明</span><span class="sxs-lookup"><span data-stu-id="62b82-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="62b82-109">displayName</span><span class="sxs-lookup"><span data-stu-id="62b82-109">displayName</span></span>| <span data-ttu-id="62b82-110">String</span><span class="sxs-lookup"><span data-stu-id="62b82-110">String</span></span>| <span data-ttu-id="62b82-111">用語の表示名。</span><span class="sxs-lookup"><span data-stu-id="62b82-111">The name of the term.</span></span>| 
|<span data-ttu-id="62b82-112">externalId</span><span class="sxs-lookup"><span data-stu-id="62b82-112">externalId</span></span>|<span data-ttu-id="62b82-113">String</span><span class="sxs-lookup"><span data-stu-id="62b82-113">String</span></span>| <span data-ttu-id="62b82-114">同期システム内の用語の ID。</span><span class="sxs-lookup"><span data-stu-id="62b82-114">ID of term in the syncing system.</span></span>|
|<span data-ttu-id="62b82-115">startDate</span><span class="sxs-lookup"><span data-stu-id="62b82-115">startDate</span></span>|<span data-ttu-id="62b82-116">Date</span><span class="sxs-lookup"><span data-stu-id="62b82-116">Date</span></span>|<span data-ttu-id="62b82-117">用語の開始。</span><span class="sxs-lookup"><span data-stu-id="62b82-117">Start of the term.</span></span>|
|<span data-ttu-id="62b82-118">endDate</span><span class="sxs-lookup"><span data-stu-id="62b82-118">endDate</span></span>|<span data-ttu-id="62b82-119">Date</span><span class="sxs-lookup"><span data-stu-id="62b82-119">Date</span></span>|<span data-ttu-id="62b82-120">用語の終了。</span><span class="sxs-lookup"><span data-stu-id="62b82-120">End Date of the term of the Section</span></span>|

## <a name="json-representation"></a><span data-ttu-id="62b82-121">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="62b82-121">JSON representation</span></span>

<span data-ttu-id="62b82-122">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="62b82-122">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationTerm"
}-->

```json
{
  "displayName": "String",
  "externalId": "String",
  "startDate": "Date",
  "endDate": "Date"
}
```

<!-- uuid: 4e9d671f-3068-4e09-aba2-b39e81a0e452
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "educationTerm resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->