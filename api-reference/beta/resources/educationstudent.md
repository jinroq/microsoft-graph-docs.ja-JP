---
title: educationStudent リソースの種類
description: ユーザーの primaryRole が `student` の場合に存在する educationUser に追加される、その他の情報。
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 554763d41c4ce48a09334394330e05fcd6dd4152
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32507124"
---
# <a name="educationstudent-resource-type"></a><span data-ttu-id="2270e-103">educationStudent リソースの種類</span><span class="sxs-lookup"><span data-stu-id="2270e-103">educationStudent resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2270e-104">ユーザーの primaryRole が `student` の場合に存在する [educationUser](educationuser.md) に追加される、その他の情報。</span><span class="sxs-lookup"><span data-stu-id="2270e-104">Additional information added to an [educationUser](educationuser.md) that is present when the primaryRole of a user is `student`.</span></span>

## <a name="properties"></a><span data-ttu-id="2270e-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="2270e-105">Properties</span></span>
| <span data-ttu-id="2270e-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="2270e-106">Property</span></span>     | <span data-ttu-id="2270e-107">型</span><span class="sxs-lookup"><span data-stu-id="2270e-107">Type</span></span>   |<span data-ttu-id="2270e-108">説明</span><span class="sxs-lookup"><span data-stu-id="2270e-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="2270e-109">birthDate</span><span class="sxs-lookup"><span data-stu-id="2270e-109">birthDate</span></span>|<span data-ttu-id="2270e-110">Date</span><span class="sxs-lookup"><span data-stu-id="2270e-110">Date</span></span>| <span data-ttu-id="2270e-111">学生の生年月日。</span><span class="sxs-lookup"><span data-stu-id="2270e-111">Birth date of the student.</span></span>|
|<span data-ttu-id="2270e-112">externalId</span><span class="sxs-lookup"><span data-stu-id="2270e-112">externalId</span></span>|<span data-ttu-id="2270e-113">String</span><span class="sxs-lookup"><span data-stu-id="2270e-113">String</span></span>| <span data-ttu-id="2270e-114">ソース システムの学生の ID。</span><span class="sxs-lookup"><span data-stu-id="2270e-114">ID of the student in the source system.</span></span>|
|<span data-ttu-id="2270e-115">gender</span><span class="sxs-lookup"><span data-stu-id="2270e-115">gender</span></span>|<span data-ttu-id="2270e-116">educationGender</span><span class="sxs-lookup"><span data-stu-id="2270e-116">educationGender</span></span>| <span data-ttu-id="2270e-117">使用可能な値: `female`、`male`、`other`、`unkownFutureValue`。</span><span class="sxs-lookup"><span data-stu-id="2270e-117">Possible values are: `female`, `male`, `other`, `unkownFutureValue`.</span></span>|
|<span data-ttu-id="2270e-118">grade</span><span class="sxs-lookup"><span data-stu-id="2270e-118">grade</span></span>|<span data-ttu-id="2270e-119">String</span><span class="sxs-lookup"><span data-stu-id="2270e-119">String</span></span>|<span data-ttu-id="2270e-120">学生の現在の学年。</span><span class="sxs-lookup"><span data-stu-id="2270e-120">Current grade level of the student.</span></span>|
|<span data-ttu-id="2270e-121">graduationYear</span><span class="sxs-lookup"><span data-stu-id="2270e-121">graduationYear</span></span>|<span data-ttu-id="2270e-122">String</span><span class="sxs-lookup"><span data-stu-id="2270e-122">String</span></span>| <span data-ttu-id="2270e-123">学生が学校から卒業する年。</span><span class="sxs-lookup"><span data-stu-id="2270e-123">Year the student is graduating from the school.</span></span>|
|<span data-ttu-id="2270e-124">studentNumber</span><span class="sxs-lookup"><span data-stu-id="2270e-124">studentNumber</span></span>|<span data-ttu-id="2270e-125">String</span><span class="sxs-lookup"><span data-stu-id="2270e-125">String</span></span>| <span data-ttu-id="2270e-126">学生番号。</span><span class="sxs-lookup"><span data-stu-id="2270e-126">Student Number.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="2270e-127">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="2270e-127">JSON representation</span></span>

<span data-ttu-id="2270e-128">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="2270e-128">The following is a JSON representation of the resource.</span></span>

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
