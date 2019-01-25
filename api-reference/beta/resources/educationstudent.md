---
title: educationStudent リソースの種類
description: ユーザーの primaryRole が  の場合に存在する educationUser に追加される、その他の情報。
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 554763d41c4ce48a09334394330e05fcd6dd4152
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29522036"
---
# <a name="educationstudent-resource-type"></a><span data-ttu-id="465a1-103">educationStudent リソースの種類</span><span class="sxs-lookup"><span data-stu-id="465a1-103">educationStudent resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="465a1-104">ユーザーの primaryRole が `student` の場合に存在する [educationUser](educationuser.md) に追加される、その他の情報。</span><span class="sxs-lookup"><span data-stu-id="465a1-104">Additional information added to an [educationUser](educationuser.md) that is present when the primaryRole of a user is `student`.</span></span>

## <a name="properties"></a><span data-ttu-id="465a1-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="465a1-105">Properties</span></span>
| <span data-ttu-id="465a1-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="465a1-106">Property</span></span>     | <span data-ttu-id="465a1-107">型</span><span class="sxs-lookup"><span data-stu-id="465a1-107">Type</span></span>   |<span data-ttu-id="465a1-108">説明</span><span class="sxs-lookup"><span data-stu-id="465a1-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="465a1-109">birthDate</span><span class="sxs-lookup"><span data-stu-id="465a1-109">birthDate</span></span>|<span data-ttu-id="465a1-110">Date</span><span class="sxs-lookup"><span data-stu-id="465a1-110">Date</span></span>| <span data-ttu-id="465a1-111">学生の生年月日。</span><span class="sxs-lookup"><span data-stu-id="465a1-111">Birth date of the student.</span></span>|
|<span data-ttu-id="465a1-112">externalId</span><span class="sxs-lookup"><span data-stu-id="465a1-112">externalId</span></span>|<span data-ttu-id="465a1-113">String</span><span class="sxs-lookup"><span data-stu-id="465a1-113">String</span></span>| <span data-ttu-id="465a1-114">ソース システムの学生の ID。</span><span class="sxs-lookup"><span data-stu-id="465a1-114">ID of the student in the source system.</span></span>|
|<span data-ttu-id="465a1-115">gender</span><span class="sxs-lookup"><span data-stu-id="465a1-115">gender</span></span>|<span data-ttu-id="465a1-116">educationGender</span><span class="sxs-lookup"><span data-stu-id="465a1-116">educationGender</span></span>| <span data-ttu-id="465a1-117">使用可能な値: `female`、`male`、`other`、`unkownFutureValue`。</span><span class="sxs-lookup"><span data-stu-id="465a1-117">Possible values are: `female`, `male`, `other`, `unkownFutureValue`.</span></span>|
|<span data-ttu-id="465a1-118">grade</span><span class="sxs-lookup"><span data-stu-id="465a1-118">grade</span></span>|<span data-ttu-id="465a1-119">String</span><span class="sxs-lookup"><span data-stu-id="465a1-119">String</span></span>|<span data-ttu-id="465a1-120">学生の現在の学年。</span><span class="sxs-lookup"><span data-stu-id="465a1-120">Current grade level of the student.</span></span>|
|<span data-ttu-id="465a1-121">graduationYear</span><span class="sxs-lookup"><span data-stu-id="465a1-121">graduationYear</span></span>|<span data-ttu-id="465a1-122">String</span><span class="sxs-lookup"><span data-stu-id="465a1-122">String</span></span>| <span data-ttu-id="465a1-123">学生が学校から卒業する年。</span><span class="sxs-lookup"><span data-stu-id="465a1-123">Year the student is graduating from the school.</span></span>|
|<span data-ttu-id="465a1-124">studentNumber</span><span class="sxs-lookup"><span data-stu-id="465a1-124">studentNumber</span></span>|<span data-ttu-id="465a1-125">String</span><span class="sxs-lookup"><span data-stu-id="465a1-125">String</span></span>| <span data-ttu-id="465a1-126">学生番号。</span><span class="sxs-lookup"><span data-stu-id="465a1-126">Student Number.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="465a1-127">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="465a1-127">JSON representation</span></span>

<span data-ttu-id="465a1-128">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="465a1-128">The following is a JSON representation of the resource.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "educationStudent resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/educationstudent.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
