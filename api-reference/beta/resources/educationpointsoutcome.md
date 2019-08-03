---
title: educationPointsOutcome リソースの種類
description: 数値の成績を示す educationOutcome
localization_priority: Normal
author: dipakboyed
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 12e288e49fffd3cf385111878483408b5c6610c1
ms.sourcegitcommit: 129e58f83fc566f9d9f36e26b0c0b8cdf81d27d9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/03/2019
ms.locfileid: "36173245"
---
# <a name="educationpointsoutcome-resource-type"></a><span data-ttu-id="b21b2-103">educationPointsOutcome リソースの種類</span><span class="sxs-lookup"><span data-stu-id="b21b2-103">educationPointsOutcome resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b21b2-104">数値の評価を与える[educationOutcome](educationoutcome.md) 。</span><span class="sxs-lookup"><span data-stu-id="b21b2-104">An [educationOutcome](educationoutcome.md) that gives a numerical grade.</span></span>

## <a name="methods"></a><span data-ttu-id="b21b2-105">メソッド</span><span class="sxs-lookup"><span data-stu-id="b21b2-105">Methods</span></span>

| <span data-ttu-id="b21b2-106">メソッド</span><span class="sxs-lookup"><span data-stu-id="b21b2-106">Method</span></span>       | <span data-ttu-id="b21b2-107">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="b21b2-107">Return Type</span></span> | <span data-ttu-id="b21b2-108">説明</span><span class="sxs-lookup"><span data-stu-id="b21b2-108">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="b21b2-109">EducationOutcome の更新</span><span class="sxs-lookup"><span data-stu-id="b21b2-109">Update educationOutcome</span></span>](../api/educationoutcome-update.md) | [<span data-ttu-id="b21b2-110">educationOutcome</span><span class="sxs-lookup"><span data-stu-id="b21b2-110">educationOutcome</span></span>](educationoutcome.md) | <span data-ttu-id="b21b2-111">EducationOutcome オブジェクトを更新します。</span><span class="sxs-lookup"><span data-stu-id="b21b2-111">Update educationOutcome object.</span></span> |

## <a name="properties"></a><span data-ttu-id="b21b2-112">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b21b2-112">Properties</span></span>

| <span data-ttu-id="b21b2-113">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b21b2-113">Property</span></span>     | <span data-ttu-id="b21b2-114">型</span><span class="sxs-lookup"><span data-stu-id="b21b2-114">Type</span></span>        | <span data-ttu-id="b21b2-115">説明</span><span class="sxs-lookup"><span data-stu-id="b21b2-115">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="b21b2-116">points</span><span class="sxs-lookup"><span data-stu-id="b21b2-116">points</span></span>|[<span data-ttu-id="b21b2-117">educationAssignmentPointsGrade</span><span class="sxs-lookup"><span data-stu-id="b21b2-117">educationAssignmentPointsGrade</span></span>](educationassignmentpointsgrade.md)|<span data-ttu-id="b21b2-118">教師がこの課題に生徒を与えた成績の等級。</span><span class="sxs-lookup"><span data-stu-id="b21b2-118">The numeric grade the teacher has given the student for this assignment.</span></span>|
|<span data-ttu-id="b21b2-119">publishedPoints</span><span class="sxs-lookup"><span data-stu-id="b21b2-119">publishedPoints</span></span>|[<span data-ttu-id="b21b2-120">educationAssignmentPointsGrade</span><span class="sxs-lookup"><span data-stu-id="b21b2-120">educationAssignmentPointsGrade</span></span>](educationassignmentpointsgrade.md)|<span data-ttu-id="b21b2-121">成績が生徒にリリースされたときに実行される points プロパティのコピー。</span><span class="sxs-lookup"><span data-stu-id="b21b2-121">A copy of the points property that is made when the grade is released to the student.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b21b2-122">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="b21b2-122">Relationships</span></span>

<span data-ttu-id="b21b2-123">なし</span><span class="sxs-lookup"><span data-stu-id="b21b2-123">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="b21b2-124">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="b21b2-124">JSON representation</span></span>

<span data-ttu-id="b21b2-125">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="b21b2-125">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationPointsOutcome",
  "baseType": "",
  "keyProperty": "id"
}-->

```json
{
  "points": {"@odata.type": "microsoft.graph.educationAssignmentPointsGrade"},
  "publishedPoints": {"@odata.type": "microsoft.graph.educationAssignmentPointsGrade"}
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "educationPointsOutcome resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->