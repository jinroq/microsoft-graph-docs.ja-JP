---
title: educationOutcome リソースの種類
description: 割り当ての量を計算した結果
localization_priority: Normal
author: dipakboyed
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: a0a49b9a383f1e787fd2698c6d2011e11b3abedb
ms.sourcegitcommit: 129e58f83fc566f9d9f36e26b0c0b8cdf81d27d9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/03/2019
ms.locfileid: "36173364"
---
# <a name="educationoutcome-resource-type"></a><span data-ttu-id="5bd62-103">educationOutcome リソースの種類</span><span class="sxs-lookup"><span data-stu-id="5bd62-103">educationOutcome resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5bd62-104">割り当ての量を計算した結果。</span><span class="sxs-lookup"><span data-stu-id="5bd62-104">The result of grading an assignment.</span></span> <span data-ttu-id="5bd62-105">これは基本クラスです。派生型は、 [educationFeedbackOutcome](educationfeedbackoutcome.md)、 [EducationPointsOutcome](educationpointsoutcome.md)、および[educationRubricOutcome](educationrubricoutcome.md)です。</span><span class="sxs-lookup"><span data-stu-id="5bd62-105">This is a base class; the derived types are [educationFeedbackOutcome](educationfeedbackoutcome.md), [educationPointsOutcome](educationpointsoutcome.md), and [educationRubricOutcome](educationrubricoutcome.md).</span></span>

## <a name="methods"></a><span data-ttu-id="5bd62-106">メソッド</span><span class="sxs-lookup"><span data-stu-id="5bd62-106">Methods</span></span>

| <span data-ttu-id="5bd62-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="5bd62-107">Method</span></span>       | <span data-ttu-id="5bd62-108">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="5bd62-108">Return Type</span></span> | <span data-ttu-id="5bd62-109">説明</span><span class="sxs-lookup"><span data-stu-id="5bd62-109">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="5bd62-110">EducationOutcome の更新</span><span class="sxs-lookup"><span data-stu-id="5bd62-110">Update educationOutcome</span></span>](../api/educationoutcome-update.md) | [<span data-ttu-id="5bd62-111">educationOutcome</span><span class="sxs-lookup"><span data-stu-id="5bd62-111">educationOutcome</span></span>](educationoutcome.md) | <span data-ttu-id="5bd62-112">EducationOutcome オブジェクトを更新します。</span><span class="sxs-lookup"><span data-stu-id="5bd62-112">Update educationOutcome object.</span></span> |

## <a name="relationships"></a><span data-ttu-id="5bd62-113">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="5bd62-113">Relationships</span></span>

<span data-ttu-id="5bd62-114">なし</span><span class="sxs-lookup"><span data-stu-id="5bd62-114">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="5bd62-115">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="5bd62-115">JSON representation</span></span>

<span data-ttu-id="5bd62-116">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="5bd62-116">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationOutcome",
  "baseType": "",
  "keyProperty": "id"
}-->

```json
{
  "id": "String (identifier)",
  "lastModifiedBy": {"@odata.type": "microsoft.graph.identitySet"},
  "lastModifiedDateTime": "String (timestamp)"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "educationOutcome resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->