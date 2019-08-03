---
title: educationRubric リソースの種類
description: 割り当てに関連付けることができる適用
localization_priority: Normal
author: dipakboyed
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: b43b611465af4dabb62d9dd741eb9a8670f241b9
ms.sourcegitcommit: 129e58f83fc566f9d9f36e26b0c0b8cdf81d27d9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/03/2019
ms.locfileid: "36173238"
---
# <a name="educationrubric-resource-type"></a><span data-ttu-id="56852-103">educationRubric リソースの種類</span><span class="sxs-lookup"><span data-stu-id="56852-103">educationRubric resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="56852-104">割り当てに関連付けることができる、その他の方法。</span><span class="sxs-lookup"><span data-stu-id="56852-104">A grading rubric that can be attached to an assignment.</span></span> <span data-ttu-id="56852-105">**EducationUser** (教師) に関連付けられており、1つ以上の**educationAssignment**リソースに添付されます。</span><span class="sxs-lookup"><span data-stu-id="56852-105">A rubric is associated with an **educationUser** (teacher), and attached to one or more **educationAssignment** resources.</span></span> 

<span data-ttu-id="56852-106">詳細については、「[教育機関](https://developer.microsoft.com/graph/docs/concepts/education-rubric-overview)向けの概要」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="56852-106">See [Education rubric overview](https://developer.microsoft.com/graph/docs/concepts/education-rubric-overview) for more information.</span></span>

## <a name="methods"></a><span data-ttu-id="56852-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="56852-107">Methods</span></span>

| <span data-ttu-id="56852-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="56852-108">Method</span></span>       | <span data-ttu-id="56852-109">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="56852-109">Return Type</span></span> | <span data-ttu-id="56852-110">説明</span><span class="sxs-lookup"><span data-stu-id="56852-110">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="56852-111">EducationRubric を取得する</span><span class="sxs-lookup"><span data-stu-id="56852-111">Get educationRubric</span></span>](../api/educationrubric-get.md) | [<span data-ttu-id="56852-112">educationRubric</span><span class="sxs-lookup"><span data-stu-id="56852-112">educationRubric</span></span>](educationrubric.md) | <span data-ttu-id="56852-113">EducationRubric オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="56852-113">Read properties and relationships of educationRubric object.</span></span> |
| [<span data-ttu-id="56852-114">EducationRubric の更新</span><span class="sxs-lookup"><span data-stu-id="56852-114">Update educationRubric</span></span>](../api/educationrubric-update.md) | [<span data-ttu-id="56852-115">educationRubric</span><span class="sxs-lookup"><span data-stu-id="56852-115">educationRubric</span></span>](educationrubric.md) | <span data-ttu-id="56852-116">EducationRubric オブジェクトを更新します。</span><span class="sxs-lookup"><span data-stu-id="56852-116">Update educationRubric object.</span></span> |
| [<span data-ttu-id="56852-117">EducationRubric の削除</span><span class="sxs-lookup"><span data-stu-id="56852-117">Delete educationRubric</span></span>](../api/educationrubric-delete.md) | <span data-ttu-id="56852-118">None</span><span class="sxs-lookup"><span data-stu-id="56852-118">None</span></span> | <span data-ttu-id="56852-119">EducationRubric オブジェクトを削除します。</span><span class="sxs-lookup"><span data-stu-id="56852-119">Delete educationRubric object.</span></span> |

## <a name="properties"></a><span data-ttu-id="56852-120">プロパティ</span><span class="sxs-lookup"><span data-stu-id="56852-120">Properties</span></span>

| <span data-ttu-id="56852-121">プロパティ</span><span class="sxs-lookup"><span data-stu-id="56852-121">Property</span></span>     | <span data-ttu-id="56852-122">型</span><span class="sxs-lookup"><span data-stu-id="56852-122">Type</span></span>        | <span data-ttu-id="56852-123">説明</span><span class="sxs-lookup"><span data-stu-id="56852-123">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="56852-124">createdBy</span><span class="sxs-lookup"><span data-stu-id="56852-124">createdBy</span></span>|[<span data-ttu-id="56852-125">identitySet</span><span class="sxs-lookup"><span data-stu-id="56852-125">identitySet</span></span>](identityset.md)|<span data-ttu-id="56852-126">このリソースを作成したユーザー。</span><span class="sxs-lookup"><span data-stu-id="56852-126">The user who created this resource.</span></span>|
|<span data-ttu-id="56852-127">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="56852-127">createdDateTime</span></span>|<span data-ttu-id="56852-128">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="56852-128">DateTimeOffset</span></span>|<span data-ttu-id="56852-p102">Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表し、必ず UTC 時間です。たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="56852-p102">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="56852-131">description</span><span class="sxs-lookup"><span data-stu-id="56852-131">description</span></span>|[<span data-ttu-id="56852-132">itemBody</span><span class="sxs-lookup"><span data-stu-id="56852-132">itemBody</span></span>](itembody.md)|<span data-ttu-id="56852-133">このテンプレートの説明。</span><span class="sxs-lookup"><span data-stu-id="56852-133">The description of this rubric.</span></span>|
|<span data-ttu-id="56852-134">displayName</span><span class="sxs-lookup"><span data-stu-id="56852-134">displayName</span></span>|<span data-ttu-id="56852-135">String</span><span class="sxs-lookup"><span data-stu-id="56852-135">String</span></span>|<span data-ttu-id="56852-136">この名前を指定します。</span><span class="sxs-lookup"><span data-stu-id="56852-136">The name of this rubric.</span></span>|
|<span data-ttu-id="56852-137">変化</span><span class="sxs-lookup"><span data-stu-id="56852-137">grading</span></span>|[<span data-ttu-id="56852-138">educationAssignmentGradeType</span><span class="sxs-lookup"><span data-stu-id="56852-138">educationAssignmentGradeType</span></span>](educationassignmentgradetype.md)|<span data-ttu-id="56852-139">この EducationAssignmentPointsGradeType の値の種類。非ポイントを指定しない場合は null、ポイント単位の場合は[](educationassignmentpointsgradetype.md)になります。</span><span class="sxs-lookup"><span data-stu-id="56852-139">The grading type of this rubric -- null for a no-points rubric, or [educationAssignmentPointsGradeType](educationassignmentpointsgradetype.md) for a points rubric.</span></span>|
|<span data-ttu-id="56852-140">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="56852-140">lastModifiedBy</span></span>|[<span data-ttu-id="56852-141">identitySet</span><span class="sxs-lookup"><span data-stu-id="56852-141">identitySet</span></span>](identityset.md)|<span data-ttu-id="56852-142">リソースを最後に変更したユーザー。</span><span class="sxs-lookup"><span data-stu-id="56852-142">The last user to modify the resource.</span></span>|
|<span data-ttu-id="56852-143">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="56852-143">lastModifiedDateTime</span></span>|<span data-ttu-id="56852-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="56852-144">DateTimeOffset</span></span>|<span data-ttu-id="56852-145">リソースが最後に変更された時点の時刻。</span><span class="sxs-lookup"><span data-stu-id="56852-145">Moment in time when the resource was last modified.</span></span>  <span data-ttu-id="56852-146">Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表し、必ず UTC 時間です。</span><span class="sxs-lookup"><span data-stu-id="56852-146">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="56852-147">たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="56852-147">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="56852-148">高度</span><span class="sxs-lookup"><span data-stu-id="56852-148">levels</span></span>|<span data-ttu-id="56852-149">[プリンシパル](rubriclevel.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="56852-149">[rubricLevel](rubriclevel.md) collection</span></span>|<span data-ttu-id="56852-150">このテンプレートを構成するレベルのコレクション。</span><span class="sxs-lookup"><span data-stu-id="56852-150">The collection of levels making up this rubric.</span></span>|
|<span data-ttu-id="56852-151">満たし</span><span class="sxs-lookup"><span data-stu-id="56852-151">qualities</span></span>|<span data-ttu-id="56852-152">の[最高品質](rubricquality.md)のコレクション</span><span class="sxs-lookup"><span data-stu-id="56852-152">[rubricQuality](rubricquality.md) collection</span></span>|<span data-ttu-id="56852-153">このテンプレートを構成する品質のコレクション。</span><span class="sxs-lookup"><span data-stu-id="56852-153">The collection of qualities making up this rubric.</span></span>|

## <a name="relationships"></a><span data-ttu-id="56852-154">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="56852-154">Relationships</span></span>

<span data-ttu-id="56852-155">なし</span><span class="sxs-lookup"><span data-stu-id="56852-155">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="56852-156">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="56852-156">JSON representation</span></span>

<span data-ttu-id="56852-157">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="56852-157">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationRubric",
  "baseType": "",
  "keyProperty": "id"
}-->

```json
{
  "createdBy": {"@odata.type": "microsoft.graph.identitySet"},
  "createdDateTime": "String (timestamp)",
  "description": {"@odata.type": "microsoft.graph.itemBody"},
  "displayName": "String",
  "grading": {"@odata.type": "microsoft.graph.educationAssignmentGradeType"},
  "lastModifiedBy": {"@odata.type": "microsoft.graph.identitySet"},
  "lastModifiedDateTime": "String (timestamp)",
  "levels": [{"@odata.type": "microsoft.graph.rubricLevel"}],
  "qualities": [{"@odata.type": "microsoft.graph.rubricQuality"}]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "educationRubric resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->