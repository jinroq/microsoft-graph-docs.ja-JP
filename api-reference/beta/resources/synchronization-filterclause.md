---
title: filterClause リソースの種類
description: いずれかに候補オブジェクトが満たす必要があります、評価される 1 つのアサーションを表します`true`(オブジェクトでは、アサーションを満たしている) または`false`(オブジェクトでは、アサーションを満たしていません)。
ms.openlocfilehash: 0861324849f224c4e750f0c7b926464280b9a377
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27067699"
---
# <a name="filterclause-resource-type"></a><span data-ttu-id="05bc6-103">filterClause リソースの種類</span><span class="sxs-lookup"><span data-stu-id="05bc6-103">filterClause resource type</span></span>

> <span data-ttu-id="05bc6-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="05bc6-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="05bc6-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="05bc6-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="05bc6-106">いずれかに候補オブジェクトが満たす必要があります、評価される 1 つのアサーションを表します`true`(オブジェクトでは、アサーションを満たしている) または`false`(オブジェクトでは、アサーションを満たしていません)。</span><span class="sxs-lookup"><span data-stu-id="05bc6-106">Represents a single assertion that a candidate object must satisfy, and is evaluated to either `true` (object satisfies the assertion) or `false` (object does not satisfy the assertion).</span></span>

## <a name="properties"></a><span data-ttu-id="05bc6-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="05bc6-107">Properties</span></span>
| <span data-ttu-id="05bc6-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="05bc6-108">Property</span></span>     | <span data-ttu-id="05bc6-109">型</span><span class="sxs-lookup"><span data-stu-id="05bc6-109">Type</span></span>   |<span data-ttu-id="05bc6-110">説明</span><span class="sxs-lookup"><span data-stu-id="05bc6-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="05bc6-111">operatorName</span><span class="sxs-lookup"><span data-stu-id="05bc6-111">operatorName</span></span>|<span data-ttu-id="05bc6-112">String</span><span class="sxs-lookup"><span data-stu-id="05bc6-112">String</span></span>|<span data-ttu-id="05bc6-113">ソースとターゲットのオペランドに適用する演算子の名前です。</span><span class="sxs-lookup"><span data-stu-id="05bc6-113">Name of the operator to be applied to the source and target operands.</span></span> <span data-ttu-id="05bc6-114">サポートされている演算子のいずれかをする必要があります。</span><span class="sxs-lookup"><span data-stu-id="05bc6-114">Must be one of the supported operators.</span></span> <span data-ttu-id="05bc6-115">サポートされている演算子を検出することができます。</span><span class="sxs-lookup"><span data-stu-id="05bc6-115">Supported operators can be discovered.</span></span>|
|<span data-ttu-id="05bc6-116">sourceOperandName</span><span class="sxs-lookup"><span data-stu-id="05bc6-116">sourceOperandName</span></span>|<span data-ttu-id="05bc6-117">String</span><span class="sxs-lookup"><span data-stu-id="05bc6-117">String</span></span>|<span data-ttu-id="05bc6-118">ソース オペランド (テスト中のオペランド) の名前です。</span><span class="sxs-lookup"><span data-stu-id="05bc6-118">Name of source operand (the operand being tested).</span></span> <span data-ttu-id="05bc6-119">ソース オペランドの名前は、ソース オブジェクトの属性の名前のいずれかに一致しなければなりません。</span><span class="sxs-lookup"><span data-stu-id="05bc6-119">The source operand name must match one of the attribute names on the source object.</span></span>|
|<span data-ttu-id="05bc6-120">targetOperand</span><span class="sxs-lookup"><span data-stu-id="05bc6-120">targetOperand</span></span>|[<span data-ttu-id="05bc6-121">filterOperand</span><span class="sxs-lookup"><span data-stu-id="05bc6-121">filterOperand</span></span>](synchronization-filteroperand.md)|<span data-ttu-id="05bc6-122">ソース オペランドを比較する値です。</span><span class="sxs-lookup"><span data-stu-id="05bc6-122">Values that the source operand will be tested against.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="05bc6-123">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="05bc6-123">JSON representation</span></span>

<span data-ttu-id="05bc6-124">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="05bc6-124">The following is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "filterClause resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->