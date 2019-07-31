---
title: filterClause リソースの種類
description: 候補オブジェクトが満たす必要がある1つのアサーションを表し、(オブジェクト`true`がアサートを満たす) または`false` (オブジェクトはアサーションを満たしていない) のどちらかに評価されます。
localization_priority: Normal
doc_type: resourcePageType
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 83b9c68bd86f716b47a3ba3774022ff3ba520770
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36007936"
---
# <a name="filterclause-resource-type"></a><span data-ttu-id="2674e-103">filterClause リソースの種類</span><span class="sxs-lookup"><span data-stu-id="2674e-103">filterClause resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2674e-104">候補オブジェクトが満たす必要がある1つのアサーションを表し、(オブジェクト`true`がアサートを満たす) または`false` (オブジェクトはアサーションを満たしていない) のどちらかに評価されます。</span><span class="sxs-lookup"><span data-stu-id="2674e-104">Represents a single assertion that a candidate object must satisfy, and is evaluated to either `true` (object satisfies the assertion) or `false` (object does not satisfy the assertion).</span></span>

## <a name="properties"></a><span data-ttu-id="2674e-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="2674e-105">Properties</span></span>
| <span data-ttu-id="2674e-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="2674e-106">Property</span></span>     | <span data-ttu-id="2674e-107">型</span><span class="sxs-lookup"><span data-stu-id="2674e-107">Type</span></span>   |<span data-ttu-id="2674e-108">説明</span><span class="sxs-lookup"><span data-stu-id="2674e-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="2674e-109">オペレーター名</span><span class="sxs-lookup"><span data-stu-id="2674e-109">operatorName</span></span>|<span data-ttu-id="2674e-110">String</span><span class="sxs-lookup"><span data-stu-id="2674e-110">String</span></span>|<span data-ttu-id="2674e-111">ソースとターゲットのオペランドに適用される演算子の名前です。</span><span class="sxs-lookup"><span data-stu-id="2674e-111">Name of the operator to be applied to the source and target operands.</span></span> <span data-ttu-id="2674e-112">サポートされている演算子のいずれかである必要があります。</span><span class="sxs-lookup"><span data-stu-id="2674e-112">Must be one of the supported operators.</span></span> <span data-ttu-id="2674e-113">サポートされている演算子を検出できます。</span><span class="sxs-lookup"><span data-stu-id="2674e-113">Supported operators can be discovered.</span></span>|
|<span data-ttu-id="2674e-114">sourceOperandName</span><span class="sxs-lookup"><span data-stu-id="2674e-114">sourceOperandName</span></span>|<span data-ttu-id="2674e-115">String</span><span class="sxs-lookup"><span data-stu-id="2674e-115">String</span></span>|<span data-ttu-id="2674e-116">Source オペランドの名前 (テストされているオペランド)。</span><span class="sxs-lookup"><span data-stu-id="2674e-116">Name of source operand (the operand being tested).</span></span> <span data-ttu-id="2674e-117">ソースのオペランド名は、ソースオブジェクトの属性名のいずれかと一致している必要があります。</span><span class="sxs-lookup"><span data-stu-id="2674e-117">The source operand name must match one of the attribute names on the source object.</span></span>|
|<span data-ttu-id="2674e-118">targetOperand</span><span class="sxs-lookup"><span data-stu-id="2674e-118">targetOperand</span></span>|[<span data-ttu-id="2674e-119">filterOperand</span><span class="sxs-lookup"><span data-stu-id="2674e-119">filterOperand</span></span>](synchronization-filteroperand.md)|<span data-ttu-id="2674e-120">Source オペランドのテスト対象となる値を指定します。</span><span class="sxs-lookup"><span data-stu-id="2674e-120">Values that the source operand will be tested against.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="2674e-121">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="2674e-121">JSON representation</span></span>

<span data-ttu-id="2674e-122">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="2674e-122">The following is a JSON representation of the resource.</span></span>

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
