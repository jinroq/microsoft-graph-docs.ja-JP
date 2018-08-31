# <a name="educationstudent-resource-type"></a><span data-ttu-id="b3dbc-101">educationStudent リソースの種類</span><span class="sxs-lookup"><span data-stu-id="b3dbc-101">educationStudent resource type</span></span>

<span data-ttu-id="b3dbc-102">ユーザーの primaryRole が `student` の場合に存在する [educationUser](educationuser.md) に追加される、その他の情報。</span><span class="sxs-lookup"><span data-stu-id="b3dbc-102">Additional information added to an [educationUser](educationuser.md) that is present when the primaryRole of a user is `student`.</span></span>

## <a name="properties"></a><span data-ttu-id="b3dbc-103">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b3dbc-103">Properties</span></span>
| <span data-ttu-id="b3dbc-104">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b3dbc-104">Property</span></span>     | <span data-ttu-id="b3dbc-105">タイプ</span><span class="sxs-lookup"><span data-stu-id="b3dbc-105">Type</span></span>   |<span data-ttu-id="b3dbc-106">説明</span><span class="sxs-lookup"><span data-stu-id="b3dbc-106">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b3dbc-107">birthDate</span><span class="sxs-lookup"><span data-stu-id="b3dbc-107">birthDate</span></span>|<span data-ttu-id="b3dbc-108">日付</span><span class="sxs-lookup"><span data-stu-id="b3dbc-108">Date</span></span>| <span data-ttu-id="b3dbc-109">学生の生年月日。</span><span class="sxs-lookup"><span data-stu-id="b3dbc-109">Birth date of the student.</span></span>|
|<span data-ttu-id="b3dbc-110">externalId</span><span class="sxs-lookup"><span data-stu-id="b3dbc-110">externalId</span></span>|<span data-ttu-id="b3dbc-111">文字列</span><span class="sxs-lookup"><span data-stu-id="b3dbc-111">String</span></span>| <span data-ttu-id="b3dbc-112">ソース システムの学生の ID。</span><span class="sxs-lookup"><span data-stu-id="b3dbc-112">ID of the student in the source system.</span></span>|
|<span data-ttu-id="b3dbc-113">性別</span><span class="sxs-lookup"><span data-stu-id="b3dbc-113">gender</span></span>|<span data-ttu-id="b3dbc-114">educationGender</span><span class="sxs-lookup"><span data-stu-id="b3dbc-114">educationGender values</span></span>| <span data-ttu-id="b3dbc-115">指定できる値は、`female`、`male`、`other`、`unknownFutureValue` です。</span><span class="sxs-lookup"><span data-stu-id="b3dbc-115">The possible values are `female`, `male`, `other`, `unknownFutureValue`, , , , , , , , or .</span></span>|
|<span data-ttu-id="b3dbc-116">成績</span><span class="sxs-lookup"><span data-stu-id="b3dbc-116">grade</span></span>|<span data-ttu-id="b3dbc-117">文字列</span><span class="sxs-lookup"><span data-stu-id="b3dbc-117">String</span></span>|<span data-ttu-id="b3dbc-118">学生の現在の学年。</span><span class="sxs-lookup"><span data-stu-id="b3dbc-118">Current grade level of the student.</span></span>|
|<span data-ttu-id="b3dbc-119">graduationYear</span><span class="sxs-lookup"><span data-stu-id="b3dbc-119">graduationYear</span></span>|<span data-ttu-id="b3dbc-120">文字列</span><span class="sxs-lookup"><span data-stu-id="b3dbc-120">String</span></span>| <span data-ttu-id="b3dbc-121">学生が学校から卒業する年。</span><span class="sxs-lookup"><span data-stu-id="b3dbc-121">Year the student is graduating from the school.</span></span>|
|<span data-ttu-id="b3dbc-122">studentNumber</span><span class="sxs-lookup"><span data-stu-id="b3dbc-122">studentNumber</span></span>|<span data-ttu-id="b3dbc-123">文字列</span><span class="sxs-lookup"><span data-stu-id="b3dbc-123">String</span></span>| <span data-ttu-id="b3dbc-124">学生番号。</span><span class="sxs-lookup"><span data-stu-id="b3dbc-124">Student Number.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="b3dbc-125">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="b3dbc-125">JSON representation</span></span>

<span data-ttu-id="b3dbc-126">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="b3dbc-126">The following is a JSON representation of the resource.</span></span>

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
