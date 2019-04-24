---
title: educationStudent リソースの種類
description: ユーザーの primaryRole が `student` の場合に存在する educationUser に追加される、その他の情報。
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 683a290806f9a70f97bda4aa9429a64578fbcd97
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32463559"
---
# <a name="educationstudent-resource-type"></a><span data-ttu-id="3efc7-103">educationStudent リソースの種類</span><span class="sxs-lookup"><span data-stu-id="3efc7-103">educationStudent resource type</span></span>

<span data-ttu-id="3efc7-104">ユーザーの primaryRole が `student` の場合に存在する [educationUser](educationuser.md) に追加される、その他の情報。</span><span class="sxs-lookup"><span data-stu-id="3efc7-104">Additional information added to an [educationUser](educationuser.md) that is present when the primaryRole of a user is `student`.</span></span>

## <a name="properties"></a><span data-ttu-id="3efc7-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="3efc7-105">Properties</span></span>
| <span data-ttu-id="3efc7-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="3efc7-106">Property</span></span>     | <span data-ttu-id="3efc7-107">型</span><span class="sxs-lookup"><span data-stu-id="3efc7-107">Type</span></span>   |<span data-ttu-id="3efc7-108">説明</span><span class="sxs-lookup"><span data-stu-id="3efc7-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="3efc7-109">birthDate</span><span class="sxs-lookup"><span data-stu-id="3efc7-109">birthDate</span></span>|<span data-ttu-id="3efc7-110">Date</span><span class="sxs-lookup"><span data-stu-id="3efc7-110">Date</span></span>| <span data-ttu-id="3efc7-111">学生の生年月日。</span><span class="sxs-lookup"><span data-stu-id="3efc7-111">Birth date of the student.</span></span>|
|<span data-ttu-id="3efc7-112">externalId</span><span class="sxs-lookup"><span data-stu-id="3efc7-112">externalId</span></span>|<span data-ttu-id="3efc7-113">String</span><span class="sxs-lookup"><span data-stu-id="3efc7-113">String</span></span>| <span data-ttu-id="3efc7-114">ソース システムの学生の ID。</span><span class="sxs-lookup"><span data-stu-id="3efc7-114">ID of the student in the source system.</span></span>|
|<span data-ttu-id="3efc7-115">gender</span><span class="sxs-lookup"><span data-stu-id="3efc7-115">gender</span></span>|<span data-ttu-id="3efc7-116">educationGender</span><span class="sxs-lookup"><span data-stu-id="3efc7-116">educationGender</span></span>| <span data-ttu-id="3efc7-117">使用可能な値は`female`、 `male`、 `other`、 `unknownFutureValue`、です。</span><span class="sxs-lookup"><span data-stu-id="3efc7-117">The possible values are: `female`, `male`, `other`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="3efc7-118">grade</span><span class="sxs-lookup"><span data-stu-id="3efc7-118">grade</span></span>|<span data-ttu-id="3efc7-119">String</span><span class="sxs-lookup"><span data-stu-id="3efc7-119">String</span></span>|<span data-ttu-id="3efc7-120">学生の現在の学年。</span><span class="sxs-lookup"><span data-stu-id="3efc7-120">Current grade level of the student.</span></span>|
|<span data-ttu-id="3efc7-121">graduationYear</span><span class="sxs-lookup"><span data-stu-id="3efc7-121">graduationYear</span></span>|<span data-ttu-id="3efc7-122">String</span><span class="sxs-lookup"><span data-stu-id="3efc7-122">String</span></span>| <span data-ttu-id="3efc7-123">学生が学校から卒業する年。</span><span class="sxs-lookup"><span data-stu-id="3efc7-123">Year the student is graduating from the school.</span></span>|
|<span data-ttu-id="3efc7-124">studentNumber</span><span class="sxs-lookup"><span data-stu-id="3efc7-124">studentNumber</span></span>|<span data-ttu-id="3efc7-125">String</span><span class="sxs-lookup"><span data-stu-id="3efc7-125">String</span></span>| <span data-ttu-id="3efc7-126">学生番号。</span><span class="sxs-lookup"><span data-stu-id="3efc7-126">Student Number.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="3efc7-127">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="3efc7-127">JSON representation</span></span>

<span data-ttu-id="3efc7-128">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="3efc7-128">The following is a JSON representation of the resource.</span></span>

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
