# <a name="educationstudent-resource-type"></a><span data-ttu-id="83c5a-101">educationStudent リソースの種類</span><span class="sxs-lookup"><span data-stu-id="83c5a-101">educationStudent resource type</span></span>

<span data-ttu-id="83c5a-102">ユーザーの primaryRole が `student` の場合に存在する [educationUser](educationuser.md) に追加される、その他の情報。</span><span class="sxs-lookup"><span data-stu-id="83c5a-102">Additional information added to an [educationUser](educationuser.md) that is present when the primaryRole of a user is `student`.</span></span>

## <a name="properties"></a><span data-ttu-id="83c5a-103">プロパティ</span><span class="sxs-lookup"><span data-stu-id="83c5a-103">Properties</span></span>
| <span data-ttu-id="83c5a-104">プロパティ</span><span class="sxs-lookup"><span data-stu-id="83c5a-104">Property</span></span>     | <span data-ttu-id="83c5a-105">型</span><span class="sxs-lookup"><span data-stu-id="83c5a-105">Type</span></span>   |<span data-ttu-id="83c5a-106">説明</span><span class="sxs-lookup"><span data-stu-id="83c5a-106">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="83c5a-107">birthDate</span><span class="sxs-lookup"><span data-stu-id="83c5a-107">birthDate</span></span>|<span data-ttu-id="83c5a-108">Date</span><span class="sxs-lookup"><span data-stu-id="83c5a-108">Date</span></span>| <span data-ttu-id="83c5a-109">学生の生年月日。</span><span class="sxs-lookup"><span data-stu-id="83c5a-109">Birth date of the student.</span></span>|
|<span data-ttu-id="83c5a-110">externalId</span><span class="sxs-lookup"><span data-stu-id="83c5a-110">externalId</span></span>|<span data-ttu-id="83c5a-111">String</span><span class="sxs-lookup"><span data-stu-id="83c5a-111">String</span></span>| <span data-ttu-id="83c5a-112">ソース システムの学生の ID。</span><span class="sxs-lookup"><span data-stu-id="83c5a-112">ID of the student in the source system.</span></span>|
|<span data-ttu-id="83c5a-113">gender</span><span class="sxs-lookup"><span data-stu-id="83c5a-113">Gender</span></span>|`educationGender enumeration`| <span data-ttu-id="83c5a-114">使用可能な値: `female`、`male`、`other`、`unkownFutureValue`。</span><span class="sxs-lookup"><span data-stu-id="83c5a-114">Possible values are: `female`, `male`, `other`, `unkownFutureValue`.</span></span>|
|<span data-ttu-id="83c5a-115">grade</span><span class="sxs-lookup"><span data-stu-id="83c5a-115">grade</span></span>|<span data-ttu-id="83c5a-116">String</span><span class="sxs-lookup"><span data-stu-id="83c5a-116">String</span></span>|<span data-ttu-id="83c5a-117">学生の現在の学年。</span><span class="sxs-lookup"><span data-stu-id="83c5a-117">Current grade level of the student.</span></span>|
|<span data-ttu-id="83c5a-118">graduationYear</span><span class="sxs-lookup"><span data-stu-id="83c5a-118">graduationYear</span></span>|<span data-ttu-id="83c5a-119">String</span><span class="sxs-lookup"><span data-stu-id="83c5a-119">String</span></span>| <span data-ttu-id="83c5a-120">学生が学校から卒業する年。</span><span class="sxs-lookup"><span data-stu-id="83c5a-120">Year the student is graduating from the school.</span></span>|
|<span data-ttu-id="83c5a-121">studentNumber</span><span class="sxs-lookup"><span data-stu-id="83c5a-121">studentNumber</span></span>|<span data-ttu-id="83c5a-122">String</span><span class="sxs-lookup"><span data-stu-id="83c5a-122">String</span></span>| <span data-ttu-id="83c5a-123">学生番号。</span><span class="sxs-lookup"><span data-stu-id="83c5a-123">Student Number.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="83c5a-124">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="83c5a-124">JSON representation</span></span>

<span data-ttu-id="83c5a-125">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="83c5a-125">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationStudent"
}-->

```json
{
  "birthDate": "String (timestamp)",
  "externalId": "String",
  "gender": "educationGender",
  "grade": "String",
  "graduationYear": "String",
  "studentNumber": "String"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "educationStudent resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->