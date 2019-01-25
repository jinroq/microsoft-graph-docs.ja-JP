---
title: filterClause リソースの種類
description: いずれかに候補オブジェクトが満たす必要があります、評価される 1 つのアサーションを表します`true`(オブジェクトでは、アサーションを満たしている) または`false`(オブジェクトでは、アサーションを満たしていません)。
localization_priority: Normal
ms.openlocfilehash: 62623cee5b2991acbe162561940adb1afd3574a1
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29523870"
---
# <a name="filterclause-resource-type"></a><span data-ttu-id="5b109-103">filterClause リソースの種類</span><span class="sxs-lookup"><span data-stu-id="5b109-103">filterClause resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5b109-104">いずれかに候補オブジェクトが満たす必要があります、評価される 1 つのアサーションを表します`true`(オブジェクトでは、アサーションを満たしている) または`false`(オブジェクトでは、アサーションを満たしていません)。</span><span class="sxs-lookup"><span data-stu-id="5b109-104">Represents a single assertion that a candidate object must satisfy, and is evaluated to either `true` (object satisfies the assertion) or `false` (object does not satisfy the assertion).</span></span>

## <a name="properties"></a><span data-ttu-id="5b109-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="5b109-105">Properties</span></span>
| <span data-ttu-id="5b109-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="5b109-106">Property</span></span>     | <span data-ttu-id="5b109-107">型</span><span class="sxs-lookup"><span data-stu-id="5b109-107">Type</span></span>   |<span data-ttu-id="5b109-108">説明</span><span class="sxs-lookup"><span data-stu-id="5b109-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="5b109-109">operatorName</span><span class="sxs-lookup"><span data-stu-id="5b109-109">operatorName</span></span>|<span data-ttu-id="5b109-110">String</span><span class="sxs-lookup"><span data-stu-id="5b109-110">String</span></span>|<span data-ttu-id="5b109-111">ソースとターゲットのオペランドに適用する演算子の名前です。</span><span class="sxs-lookup"><span data-stu-id="5b109-111">Name of the operator to be applied to the source and target operands.</span></span> <span data-ttu-id="5b109-112">サポートされている演算子のいずれかをする必要があります。</span><span class="sxs-lookup"><span data-stu-id="5b109-112">Must be one of the supported operators.</span></span> <span data-ttu-id="5b109-113">サポートされている演算子を検出することができます。</span><span class="sxs-lookup"><span data-stu-id="5b109-113">Supported operators can be discovered.</span></span>|
|<span data-ttu-id="5b109-114">sourceOperandName</span><span class="sxs-lookup"><span data-stu-id="5b109-114">sourceOperandName</span></span>|<span data-ttu-id="5b109-115">String</span><span class="sxs-lookup"><span data-stu-id="5b109-115">String</span></span>|<span data-ttu-id="5b109-116">ソース オペランド (テスト中のオペランド) の名前です。</span><span class="sxs-lookup"><span data-stu-id="5b109-116">Name of source operand (the operand being tested).</span></span> <span data-ttu-id="5b109-117">ソース オペランドの名前は、ソース オブジェクトの属性の名前のいずれかに一致しなければなりません。</span><span class="sxs-lookup"><span data-stu-id="5b109-117">The source operand name must match one of the attribute names on the source object.</span></span>|
|<span data-ttu-id="5b109-118">targetOperand</span><span class="sxs-lookup"><span data-stu-id="5b109-118">targetOperand</span></span>|[<span data-ttu-id="5b109-119">filterOperand</span><span class="sxs-lookup"><span data-stu-id="5b109-119">filterOperand</span></span>](synchronization-filteroperand.md)|<span data-ttu-id="5b109-120">ソース オペランドを比較する値です。</span><span class="sxs-lookup"><span data-stu-id="5b109-120">Values that the source operand will be tested against.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="5b109-121">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="5b109-121">JSON representation</span></span>

<span data-ttu-id="5b109-122">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="5b109-122">The following is a JSON representation of the resource.</span></span>

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
  "suppressions": [
    "Error: /api-reference/beta/resources/synchronization-filterclause.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
