---
title: educationRubricOutcome リソースの種類
description: 採点方式を提供する educationOutcome
localization_priority: Normal
author: dipakboyed
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 4640daa1bb93945463cffc9dcf54d4db23b84da1
ms.sourcegitcommit: 129e58f83fc566f9d9f36e26b0c0b8cdf81d27d9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/03/2019
ms.locfileid: "36173259"
---
# <a name="educationrubricoutcome-resource-type"></a><span data-ttu-id="58a46-103">educationRubricOutcome リソースの種類</span><span class="sxs-lookup"><span data-stu-id="58a46-103">educationRubricOutcome resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="58a46-104">採点方式を提供する[educationOutcome](educationoutcome.md) 。</span><span class="sxs-lookup"><span data-stu-id="58a46-104">An [educationOutcome](educationoutcome.md) that provides a graded rubric.</span></span>

## <a name="methods"></a><span data-ttu-id="58a46-105">メソッド</span><span class="sxs-lookup"><span data-stu-id="58a46-105">Methods</span></span>

| <span data-ttu-id="58a46-106">メソッド</span><span class="sxs-lookup"><span data-stu-id="58a46-106">Method</span></span>       | <span data-ttu-id="58a46-107">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="58a46-107">Return Type</span></span> | <span data-ttu-id="58a46-108">説明</span><span class="sxs-lookup"><span data-stu-id="58a46-108">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="58a46-109">EducationOutcome の更新</span><span class="sxs-lookup"><span data-stu-id="58a46-109">Update educationOutcome</span></span>](../api/educationoutcome-update.md) | [<span data-ttu-id="58a46-110">educationOutcome</span><span class="sxs-lookup"><span data-stu-id="58a46-110">educationOutcome</span></span>](educationoutcome.md) | <span data-ttu-id="58a46-111">EducationOutcome オブジェクトを更新します。</span><span class="sxs-lookup"><span data-stu-id="58a46-111">Update educationOutcome object.</span></span> |

## <a name="properties"></a><span data-ttu-id="58a46-112">プロパティ</span><span class="sxs-lookup"><span data-stu-id="58a46-112">Properties</span></span>

| <span data-ttu-id="58a46-113">プロパティ</span><span class="sxs-lookup"><span data-stu-id="58a46-113">Property</span></span>     | <span data-ttu-id="58a46-114">型</span><span class="sxs-lookup"><span data-stu-id="58a46-114">Type</span></span>        | <span data-ttu-id="58a46-115">説明</span><span class="sxs-lookup"><span data-stu-id="58a46-115">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="58a46-116">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="58a46-116">lastModifiedBy</span></span>|[<span data-ttu-id="58a46-117">identitySet</span><span class="sxs-lookup"><span data-stu-id="58a46-117">identitySet</span></span>](identityset.md)|<span data-ttu-id="58a46-118">リソースを最後に変更したユーザー。</span><span class="sxs-lookup"><span data-stu-id="58a46-118">The last user to modify the resource.</span></span>|
|<span data-ttu-id="58a46-119">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="58a46-119">lastModifiedDateTime</span></span>|<span data-ttu-id="58a46-120">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="58a46-120">DateTimeOffset</span></span>|<span data-ttu-id="58a46-121">リソースが最後に変更された時点の時刻。</span><span class="sxs-lookup"><span data-stu-id="58a46-121">Moment in time when the resource was last modified.</span></span>  <span data-ttu-id="58a46-122">Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表し、必ず UTC 時間です。</span><span class="sxs-lookup"><span data-stu-id="58a46-122">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="58a46-123">たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="58a46-123">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="58a46-124">publishedRubricQualityFeedback</span><span class="sxs-lookup"><span data-stu-id="58a46-124">publishedRubricQualityFeedback</span></span>|<span data-ttu-id="58a46-125">[rubricQualityFeedbackModel](rubricqualityfeedbackmodel.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="58a46-125">[rubricQualityFeedbackModel](rubricqualityfeedbackmodel.md) collection</span></span>|<span data-ttu-id="58a46-126">成績が生徒にリリースされたときに実行される rubricQualityFeedback プロパティのコピー。</span><span class="sxs-lookup"><span data-stu-id="58a46-126">A copy of the rubricQualityFeedback property that is made when the grade is released to the student.</span></span>|
|<span data-ttu-id="58a46-127">publishedRubricQualitySelectedLevels</span><span class="sxs-lookup"><span data-stu-id="58a46-127">publishedRubricQualitySelectedLevels</span></span>|<span data-ttu-id="58a46-128">[rubricQualitySelectedColumnModel](rubricqualityselectedcolumnmodel.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="58a46-128">[rubricQualitySelectedColumnModel](rubricqualityselectedcolumnmodel.md) collection</span></span>|<span data-ttu-id="58a46-129">成績が生徒にリリースされたときに実行される rubricQualitySelectedLevels プロパティのコピー。</span><span class="sxs-lookup"><span data-stu-id="58a46-129">A copy of the rubricQualitySelectedLevels property that is made when the grade is released to the student.</span></span>|
|<span data-ttu-id="58a46-130">rubricQualityFeedback</span><span class="sxs-lookup"><span data-stu-id="58a46-130">rubricQualityFeedback</span></span>|<span data-ttu-id="58a46-131">[rubricQualityFeedbackModel](rubricqualityfeedbackmodel.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="58a46-131">[rubricQualityFeedbackModel](rubricqualityfeedbackmodel.md) collection</span></span>|<span data-ttu-id="58a46-132">この期間内の各品質に関する特定のフィードバックのコレクション。</span><span class="sxs-lookup"><span data-stu-id="58a46-132">A collection of specific feedback for each quality of this rubric.</span></span>|
|<span data-ttu-id="58a46-133">rubricQualitySelectedLevels</span><span class="sxs-lookup"><span data-stu-id="58a46-133">rubricQualitySelectedLevels</span></span>|<span data-ttu-id="58a46-134">[rubricQualitySelectedColumnModel](rubricqualityselectedcolumnmodel.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="58a46-134">[rubricQualitySelectedColumnModel](rubricqualityselectedcolumnmodel.md) collection</span></span>|<span data-ttu-id="58a46-135">この割り当てを評価する一方で、各品質に教師が選択したレベル。</span><span class="sxs-lookup"><span data-stu-id="58a46-135">The level that the teacher has selected for each quality while grading this assignment.</span></span>|

## <a name="relationships"></a><span data-ttu-id="58a46-136">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="58a46-136">Relationships</span></span>

<span data-ttu-id="58a46-137">なし</span><span class="sxs-lookup"><span data-stu-id="58a46-137">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="58a46-138">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="58a46-138">JSON representation</span></span>

<span data-ttu-id="58a46-139">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="58a46-139">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationRubricOutcome",
  "baseType": "",
  "keyProperty": "id"
}-->

```json
{
  "publishedRubricQualityFeedback": [{"@odata.type": "microsoft.graph.rubricQualityFeedbackModel"}],
  "publishedRubricQualitySelectedLevels": [{"@odata.type": "microsoft.graph.rubricQualitySelectedColumnModel"}],
  "rubricQualityFeedback": [{"@odata.type": "microsoft.graph.rubricQualityFeedbackModel"}],
  "rubricQualitySelectedLevels": [{"@odata.type": "microsoft.graph.rubricQualitySelectedColumnModel"}]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "educationRubricOutcome resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->