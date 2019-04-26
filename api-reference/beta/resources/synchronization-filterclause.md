---
title: filterclause リソースの種類
description: 候補オブジェクトが満たす必要がある1つのアサーションを表し、(オブジェクト`true`がアサートを満たす) または`false` (オブジェクトはアサーションを満たしていない) のどちらかに評価されます。
localization_priority: Normal
ms.openlocfilehash: 657651af512fff0b1daf08985e0f14983ca253f3
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33342976"
---
# <a name="filterclause-resource-type"></a><span data-ttu-id="e7fa0-103">filterclause リソースの種類</span><span class="sxs-lookup"><span data-stu-id="e7fa0-103">filterClause resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e7fa0-104">候補オブジェクトが満たす必要がある1つのアサーションを表し、(オブジェクト`true`がアサートを満たす) または`false` (オブジェクトはアサーションを満たしていない) のどちらかに評価されます。</span><span class="sxs-lookup"><span data-stu-id="e7fa0-104">Represents a single assertion that a candidate object must satisfy, and is evaluated to either `true` (object satisfies the assertion) or `false` (object does not satisfy the assertion).</span></span>

## <a name="properties"></a><span data-ttu-id="e7fa0-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="e7fa0-105">Properties</span></span>
| <span data-ttu-id="e7fa0-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="e7fa0-106">Property</span></span>     | <span data-ttu-id="e7fa0-107">型</span><span class="sxs-lookup"><span data-stu-id="e7fa0-107">Type</span></span>   |<span data-ttu-id="e7fa0-108">説明</span><span class="sxs-lookup"><span data-stu-id="e7fa0-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e7fa0-109">オペレーター名</span><span class="sxs-lookup"><span data-stu-id="e7fa0-109">operatorName</span></span>|<span data-ttu-id="e7fa0-110">String</span><span class="sxs-lookup"><span data-stu-id="e7fa0-110">String</span></span>|<span data-ttu-id="e7fa0-111">ソースとターゲットのオペランドに適用される演算子の名前です。</span><span class="sxs-lookup"><span data-stu-id="e7fa0-111">Name of the operator to be applied to the source and target operands.</span></span> <span data-ttu-id="e7fa0-112">サポートされている演算子のいずれかである必要があります。</span><span class="sxs-lookup"><span data-stu-id="e7fa0-112">Must be one of the supported operators.</span></span> <span data-ttu-id="e7fa0-113">サポートされている演算子を検出できます。</span><span class="sxs-lookup"><span data-stu-id="e7fa0-113">Supported operators can be discovered.</span></span>|
|<span data-ttu-id="e7fa0-114">sourceoperandname</span><span class="sxs-lookup"><span data-stu-id="e7fa0-114">sourceOperandName</span></span>|<span data-ttu-id="e7fa0-115">String</span><span class="sxs-lookup"><span data-stu-id="e7fa0-115">String</span></span>|<span data-ttu-id="e7fa0-116">source オペランドの名前 (テストされているオペランド)。</span><span class="sxs-lookup"><span data-stu-id="e7fa0-116">Name of source operand (the operand being tested).</span></span> <span data-ttu-id="e7fa0-117">ソースのオペランド名は、ソースオブジェクトの属性名のいずれかと一致している必要があります。</span><span class="sxs-lookup"><span data-stu-id="e7fa0-117">The source operand name must match one of the attribute names on the source object.</span></span>|
|<span data-ttu-id="e7fa0-118">targetoperand</span><span class="sxs-lookup"><span data-stu-id="e7fa0-118">targetOperand</span></span>|[<span data-ttu-id="e7fa0-119">filteroperand</span><span class="sxs-lookup"><span data-stu-id="e7fa0-119">filterOperand</span></span>](synchronization-filteroperand.md)|<span data-ttu-id="e7fa0-120">source オペランドのテスト対象となる値を指定します。</span><span class="sxs-lookup"><span data-stu-id="e7fa0-120">Values that the source operand will be tested against.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="e7fa0-121">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="e7fa0-121">JSON representation</span></span>

<span data-ttu-id="e7fa0-122">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="e7fa0-122">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.filterClause"
}-->

```json
{
  "operatorName": "String",
  "sourceOperandName": "String",
  "targetOperand": {"@odata.type": "microsoft.graph.filterOperand"}
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "filterClause resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
