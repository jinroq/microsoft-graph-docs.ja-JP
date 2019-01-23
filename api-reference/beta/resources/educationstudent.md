---
title: educationStudent リソースの種類
description: ユーザーの primaryRole が `student` の場合に存在する educationUser に追加される、その他の情報。
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 19ce3e28ccedc5f6165c8c333afb2ccd10343f14
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29406907"
---
# <a name="educationstudent-resource-type"></a><span data-ttu-id="5b074-103">educationStudent リソースの種類</span><span class="sxs-lookup"><span data-stu-id="5b074-103">educationStudent resource type</span></span>

> <span data-ttu-id="5b074-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="5b074-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="5b074-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="5b074-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="5b074-106">ユーザーの primaryRole が `student` の場合に存在する [educationUser](educationuser.md) に追加される、その他の情報。</span><span class="sxs-lookup"><span data-stu-id="5b074-106">Additional information added to an [educationUser](educationuser.md) that is present when the primaryRole of a user is `student`.</span></span>

## <a name="properties"></a><span data-ttu-id="5b074-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="5b074-107">Properties</span></span>
| <span data-ttu-id="5b074-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="5b074-108">Property</span></span>     | <span data-ttu-id="5b074-109">型</span><span class="sxs-lookup"><span data-stu-id="5b074-109">Type</span></span>   |<span data-ttu-id="5b074-110">説明</span><span class="sxs-lookup"><span data-stu-id="5b074-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="5b074-111">birthDate</span><span class="sxs-lookup"><span data-stu-id="5b074-111">birthDate</span></span>|<span data-ttu-id="5b074-112">Date</span><span class="sxs-lookup"><span data-stu-id="5b074-112">Date</span></span>| <span data-ttu-id="5b074-113">学生の生年月日。</span><span class="sxs-lookup"><span data-stu-id="5b074-113">Birth date of the student.</span></span>|
|<span data-ttu-id="5b074-114">externalId</span><span class="sxs-lookup"><span data-stu-id="5b074-114">externalId</span></span>|<span data-ttu-id="5b074-115">String</span><span class="sxs-lookup"><span data-stu-id="5b074-115">String</span></span>| <span data-ttu-id="5b074-116">ソース システムの学生の ID。</span><span class="sxs-lookup"><span data-stu-id="5b074-116">ID of the student in the source system.</span></span>|
|<span data-ttu-id="5b074-117">gender</span><span class="sxs-lookup"><span data-stu-id="5b074-117">gender</span></span>|<span data-ttu-id="5b074-118">educationGender</span><span class="sxs-lookup"><span data-stu-id="5b074-118">educationGender</span></span>| <span data-ttu-id="5b074-119">使用可能な値: `female`、`male`、`other`、`unkownFutureValue`。</span><span class="sxs-lookup"><span data-stu-id="5b074-119">Possible values are: `female`, `male`, `other`, `unkownFutureValue`.</span></span>|
|<span data-ttu-id="5b074-120">grade</span><span class="sxs-lookup"><span data-stu-id="5b074-120">grade</span></span>|<span data-ttu-id="5b074-121">String</span><span class="sxs-lookup"><span data-stu-id="5b074-121">String</span></span>|<span data-ttu-id="5b074-122">学生の現在の学年。</span><span class="sxs-lookup"><span data-stu-id="5b074-122">Current grade level of the student.</span></span>|
|<span data-ttu-id="5b074-123">graduationYear</span><span class="sxs-lookup"><span data-stu-id="5b074-123">graduationYear</span></span>|<span data-ttu-id="5b074-124">String</span><span class="sxs-lookup"><span data-stu-id="5b074-124">String</span></span>| <span data-ttu-id="5b074-125">学生が学校から卒業する年。</span><span class="sxs-lookup"><span data-stu-id="5b074-125">Year the student is graduating from the school.</span></span>|
|<span data-ttu-id="5b074-126">studentNumber</span><span class="sxs-lookup"><span data-stu-id="5b074-126">studentNumber</span></span>|<span data-ttu-id="5b074-127">String</span><span class="sxs-lookup"><span data-stu-id="5b074-127">String</span></span>| <span data-ttu-id="5b074-128">学生番号。</span><span class="sxs-lookup"><span data-stu-id="5b074-128">Student Number.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="5b074-129">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="5b074-129">JSON representation</span></span>

<span data-ttu-id="5b074-130">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="5b074-130">The following is a JSON representation of the resource.</span></span>

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
