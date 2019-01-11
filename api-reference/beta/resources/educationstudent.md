---
title: educationStudent リソースの種類
description: ユーザーの primaryRole が `student` の場合に存在する educationUser に追加される、その他の情報。
author: mmast-msft
localization_priority: Normal
ms.openlocfilehash: f87bbe9b15f89660a166c0ca1d9a1aaa4bbd9eff
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27878121"
---
# <a name="educationstudent-resource-type"></a><span data-ttu-id="06bd5-103">educationStudent リソースの種類</span><span class="sxs-lookup"><span data-stu-id="06bd5-103">educationStudent resource type</span></span>

> <span data-ttu-id="06bd5-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="06bd5-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="06bd5-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="06bd5-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="06bd5-106">ユーザーの primaryRole が `student` の場合に存在する [educationUser](educationuser.md) に追加される、その他の情報。</span><span class="sxs-lookup"><span data-stu-id="06bd5-106">Additional information added to an [educationUser](educationuser.md) that is present when the primaryRole of a user is `student`.</span></span>

## <a name="properties"></a><span data-ttu-id="06bd5-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="06bd5-107">Properties</span></span>
| <span data-ttu-id="06bd5-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="06bd5-108">Property</span></span>     | <span data-ttu-id="06bd5-109">種類</span><span class="sxs-lookup"><span data-stu-id="06bd5-109">Type</span></span>   |<span data-ttu-id="06bd5-110">説明</span><span class="sxs-lookup"><span data-stu-id="06bd5-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="06bd5-111">birthDate</span><span class="sxs-lookup"><span data-stu-id="06bd5-111">birthDate</span></span>|<span data-ttu-id="06bd5-112">Date</span><span class="sxs-lookup"><span data-stu-id="06bd5-112">Date</span></span>| <span data-ttu-id="06bd5-113">学生の生年月日。</span><span class="sxs-lookup"><span data-stu-id="06bd5-113">Birth date of the student.</span></span>|
|<span data-ttu-id="06bd5-114">externalId</span><span class="sxs-lookup"><span data-stu-id="06bd5-114">externalId</span></span>|<span data-ttu-id="06bd5-115">String</span><span class="sxs-lookup"><span data-stu-id="06bd5-115">String</span></span>| <span data-ttu-id="06bd5-116">ソース システムの学生の ID。</span><span class="sxs-lookup"><span data-stu-id="06bd5-116">ID of the student in the source system.</span></span>|
|<span data-ttu-id="06bd5-117">gender</span><span class="sxs-lookup"><span data-stu-id="06bd5-117">gender</span></span>|`educationGender enumeration`| <span data-ttu-id="06bd5-118">使用可能な値: `female`、`male`、`other`、`unkownFutureValue`。</span><span class="sxs-lookup"><span data-stu-id="06bd5-118">Possible values are: `female`, `male`, `other`, `unkownFutureValue`.</span></span>|
|<span data-ttu-id="06bd5-119">grade</span><span class="sxs-lookup"><span data-stu-id="06bd5-119">grade</span></span>|<span data-ttu-id="06bd5-120">String</span><span class="sxs-lookup"><span data-stu-id="06bd5-120">String</span></span>|<span data-ttu-id="06bd5-121">学生の現在の学年。</span><span class="sxs-lookup"><span data-stu-id="06bd5-121">Current grade level of the student.</span></span>|
|<span data-ttu-id="06bd5-122">graduationYear</span><span class="sxs-lookup"><span data-stu-id="06bd5-122">graduationYear</span></span>|<span data-ttu-id="06bd5-123">String</span><span class="sxs-lookup"><span data-stu-id="06bd5-123">String</span></span>| <span data-ttu-id="06bd5-124">学生が学校から卒業する年。</span><span class="sxs-lookup"><span data-stu-id="06bd5-124">Year the student is graduating from the school.</span></span>|
|<span data-ttu-id="06bd5-125">studentNumber</span><span class="sxs-lookup"><span data-stu-id="06bd5-125">studentNumber</span></span>|<span data-ttu-id="06bd5-126">String</span><span class="sxs-lookup"><span data-stu-id="06bd5-126">String</span></span>| <span data-ttu-id="06bd5-127">学生番号。</span><span class="sxs-lookup"><span data-stu-id="06bd5-127">Student Number.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="06bd5-128">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="06bd5-128">JSON representation</span></span>

<span data-ttu-id="06bd5-129">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="06bd5-129">The following is a JSON representation of the resource.</span></span>

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
