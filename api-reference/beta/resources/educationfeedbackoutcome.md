---
title: educationFeedbackOutcome リソースの種類
description: テキスト形式でフィードバックを提供する educationOutcome。
localization_priority: Normal
author: dipakboyed
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: e61538a62a1bb267b0a13b98b17e9b69a8ceed92
ms.sourcegitcommit: 129e58f83fc566f9d9f36e26b0c0b8cdf81d27d9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/03/2019
ms.locfileid: "36173252"
---
# <a name="educationfeedbackoutcome-resource-type"></a><span data-ttu-id="b15af-103">educationFeedbackOutcome リソースの種類</span><span class="sxs-lookup"><span data-stu-id="b15af-103">educationFeedbackOutcome resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b15af-104">テキスト形式の[educationOutcome](educationoutcome.md)オブジェクトに対するフィードバックを表します。</span><span class="sxs-lookup"><span data-stu-id="b15af-104">Represents feedback on an [educationOutcome](educationoutcome.md) object in the form of text.</span></span> 

## <a name="methods"></a><span data-ttu-id="b15af-105">メソッド</span><span class="sxs-lookup"><span data-stu-id="b15af-105">Methods</span></span>

| <span data-ttu-id="b15af-106">メソッド</span><span class="sxs-lookup"><span data-stu-id="b15af-106">Method</span></span>       | <span data-ttu-id="b15af-107">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="b15af-107">Return Type</span></span> | <span data-ttu-id="b15af-108">説明</span><span class="sxs-lookup"><span data-stu-id="b15af-108">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="b15af-109">EducationOutcome の更新</span><span class="sxs-lookup"><span data-stu-id="b15af-109">Update educationOutcome</span></span>](../api/educationoutcome-update.md) | [<span data-ttu-id="b15af-110">educationOutcome</span><span class="sxs-lookup"><span data-stu-id="b15af-110">educationOutcome</span></span>](educationoutcome.md) | <span data-ttu-id="b15af-111">EducationOutcome オブジェクトを更新します。</span><span class="sxs-lookup"><span data-stu-id="b15af-111">Update educationOutcome object.</span></span> |

## <a name="properties"></a><span data-ttu-id="b15af-112">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b15af-112">Properties</span></span>

| <span data-ttu-id="b15af-113">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b15af-113">Property</span></span>     | <span data-ttu-id="b15af-114">型</span><span class="sxs-lookup"><span data-stu-id="b15af-114">Type</span></span>        | <span data-ttu-id="b15af-115">説明</span><span class="sxs-lookup"><span data-stu-id="b15af-115">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="b15af-116">feedback</span><span class="sxs-lookup"><span data-stu-id="b15af-116">feedback</span></span>|[<span data-ttu-id="b15af-117">educationFeedback</span><span class="sxs-lookup"><span data-stu-id="b15af-117">educationFeedback</span></span>](educationfeedback.md)|<span data-ttu-id="b15af-118">教師が生徒に書面でフィードバックを送信します。</span><span class="sxs-lookup"><span data-stu-id="b15af-118">Teacher's written feedback to the student.</span></span>|
|<span data-ttu-id="b15af-119">publishedFeedback</span><span class="sxs-lookup"><span data-stu-id="b15af-119">publishedFeedback</span></span>|[<span data-ttu-id="b15af-120">educationFeedback</span><span class="sxs-lookup"><span data-stu-id="b15af-120">educationFeedback</span></span>](educationfeedback.md)|<span data-ttu-id="b15af-121">成績が生徒にリリースされたときに行われるフィードバックプロパティのコピー。</span><span class="sxs-lookup"><span data-stu-id="b15af-121">A copy of the feedback property that is made when the grade is released to the student.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b15af-122">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="b15af-122">Relationships</span></span>

<span data-ttu-id="b15af-123">なし</span><span class="sxs-lookup"><span data-stu-id="b15af-123">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="b15af-124">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="b15af-124">JSON representation</span></span>

<span data-ttu-id="b15af-125">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="b15af-125">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationFeedbackOutcome",
  "baseType": "",
  "keyProperty": "id"
}-->

```json
{
  "feedback": {"@odata.type": "microsoft.graph.educationFeedback"},
  "publishedFeedback": {"@odata.type": "microsoft.graph.educationFeedback"}
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "educationFeedbackOutcome resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->