# <a name="educationteacher-resource-type"></a><span data-ttu-id="2e3e2-101">educationTeacher リソースの種類</span><span class="sxs-lookup"><span data-stu-id="2e3e2-101">educationTeacher resource type</span></span>

<span data-ttu-id="2e3e2-102">ユーザーの primaryRole が `teacher` の場合に存在する [educationUser](educationuser.md) に追加される、その他の情報。</span><span class="sxs-lookup"><span data-stu-id="2e3e2-102">Additional information added to an [educationUser](educationuser.md) that is present when the primaryRole of a user is `teacher`.</span></span>


## <a name="properties"></a><span data-ttu-id="2e3e2-103">プロパティ</span><span class="sxs-lookup"><span data-stu-id="2e3e2-103">Properties</span></span>
| <span data-ttu-id="2e3e2-104">プロパティ</span><span class="sxs-lookup"><span data-stu-id="2e3e2-104">Property</span></span>     | <span data-ttu-id="2e3e2-105">型</span><span class="sxs-lookup"><span data-stu-id="2e3e2-105">Type</span></span>   |<span data-ttu-id="2e3e2-106">説明</span><span class="sxs-lookup"><span data-stu-id="2e3e2-106">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="2e3e2-107">externalId</span><span class="sxs-lookup"><span data-stu-id="2e3e2-107">externalId</span></span>|<span data-ttu-id="2e3e2-108">String</span><span class="sxs-lookup"><span data-stu-id="2e3e2-108">String</span></span>| <span data-ttu-id="2e3e2-109">ソース システムの教師の ID。</span><span class="sxs-lookup"><span data-stu-id="2e3e2-109">ID of the teacher in the source system.</span></span>|
|<span data-ttu-id="2e3e2-110">teacherNumber</span><span class="sxs-lookup"><span data-stu-id="2e3e2-110">teacherNumber</span></span>|<span data-ttu-id="2e3e2-111">String</span><span class="sxs-lookup"><span data-stu-id="2e3e2-111">String</span></span>|<span data-ttu-id="2e3e2-112">教師の番号。</span><span class="sxs-lookup"><span data-stu-id="2e3e2-112">Teacher number.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="2e3e2-113">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="2e3e2-113">JSON representation</span></span>

<span data-ttu-id="2e3e2-114">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="2e3e2-114">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationTeacher"
}-->

```json
{
  "externalId": "String",
  "teacherNumber": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "educationTeacher resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->