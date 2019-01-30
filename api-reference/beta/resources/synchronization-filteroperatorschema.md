---
title: filterOperatorSchema リソースの種類
description: フィルターで使用できる演算子をについて説明します。
localization_priority: Normal
ms.openlocfilehash: 04bee90f81c0098832cd4b6355be266668d0f69b
ms.sourcegitcommit: d95f6d39a0479da6e531f3734c4029dc596b9a3f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/30/2019
ms.locfileid: "29641821"
---
# <a name="filteroperatorschema-resource-type"></a><span data-ttu-id="6b31f-103">filterOperatorSchema リソースの種類</span><span class="sxs-lookup"><span data-stu-id="6b31f-103">filterOperatorSchema resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6b31f-104">[フィルター](synchronization-filter.md)で使用できる演算子をについて説明します。</span><span class="sxs-lookup"><span data-stu-id="6b31f-104">Describes an operator that can be used in a [filter](synchronization-filter.md).</span></span>

## <a name="properties"></a><span data-ttu-id="6b31f-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="6b31f-105">Properties</span></span>

| <span data-ttu-id="6b31f-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="6b31f-106">Property</span></span>                   | <span data-ttu-id="6b31f-107">型</span><span class="sxs-lookup"><span data-stu-id="6b31f-107">Type</span></span>                      | <span data-ttu-id="6b31f-108">説明</span><span class="sxs-lookup"><span data-stu-id="6b31f-108">Description</span></span>    |
|:---------------------------|:--------------------------|:---------------|
|<span data-ttu-id="6b31f-109">アリティ</span><span class="sxs-lookup"><span data-stu-id="6b31f-109">arity</span></span>                       |<span data-ttu-id="6b31f-110">String</span><span class="sxs-lookup"><span data-stu-id="6b31f-110">String</span></span>          |<span data-ttu-id="6b31f-111">演算子のアリティ。</span><span class="sxs-lookup"><span data-stu-id="6b31f-111">Arity of the operator.</span></span> <span data-ttu-id="6b31f-112">使用可能な値は、`Binary`、`Unary` です。</span><span class="sxs-lookup"><span data-stu-id="6b31f-112">Possible values are: `Binary`, `Unary`.</span></span> <span data-ttu-id="6b31f-113">既定値は `Binary` です。</span><span class="sxs-lookup"><span data-stu-id="6b31f-113">The default is `Binary`.</span></span>|
|<span data-ttu-id="6b31f-114">multivaluedComparisonType</span><span class="sxs-lookup"><span data-stu-id="6b31f-114">multivaluedComparisonType</span></span>   |<span data-ttu-id="6b31f-115">scopeOperatorMultiValuedComparisonType</span><span class="sxs-lookup"><span data-stu-id="6b31f-115">scopeOperatorMultiValuedComparisonType</span></span>          |<span data-ttu-id="6b31f-116">使用可能な値は、`All`、`Any` です。</span><span class="sxs-lookup"><span data-stu-id="6b31f-116">Possible values are: `All`, `Any`.</span></span> <span data-ttu-id="6b31f-117">複数値を持つ属性にのみ適用されます。</span><span class="sxs-lookup"><span data-stu-id="6b31f-117">Applies only to multivalued attributes.</span></span> <span data-ttu-id="6b31f-118">`All`すべての値が条件を満たす必要があることを意味します。</span><span class="sxs-lookup"><span data-stu-id="6b31f-118">`All` means that all values must satisfy the condition.</span></span> <span data-ttu-id="6b31f-119">`Any`条件を満たすために、少なくとも 1 つの値が含まれていることを意味します。</span><span class="sxs-lookup"><span data-stu-id="6b31f-119">`Any` means that at least one value has to satisfy the condition.</span></span> <span data-ttu-id="6b31f-120">既定値は `All` です。</span><span class="sxs-lookup"><span data-stu-id="6b31f-120">The default is `All`.</span></span>|
|<span data-ttu-id="6b31f-121">name</span><span class="sxs-lookup"><span data-stu-id="6b31f-121">name</span></span>                        |<span data-ttu-id="6b31f-122">String</span><span class="sxs-lookup"><span data-stu-id="6b31f-122">String</span></span>                     |<span data-ttu-id="6b31f-123">オペレーター名です。</span><span class="sxs-lookup"><span data-stu-id="6b31f-123">Operator name.</span></span> |
|<span data-ttu-id="6b31f-124">supportedAttributeTypes</span><span class="sxs-lookup"><span data-stu-id="6b31f-124">supportedAttributeTypes</span></span>     |<span data-ttu-id="6b31f-125">String コレクション</span><span class="sxs-lookup"><span data-stu-id="6b31f-125">String collection</span></span>         |<span data-ttu-id="6b31f-126">属性の型が演算子でサポートします。</span><span class="sxs-lookup"><span data-stu-id="6b31f-126">Attribute types supported by the operator.</span></span> <span data-ttu-id="6b31f-127">可能な値は、`Boolean`、`Binary`、`Reference`、`Integer`、`String` です。</span><span class="sxs-lookup"><span data-stu-id="6b31f-127">Possible values are: `Boolean`, `Binary`, `Reference`, `Integer`, `String`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="6b31f-128">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="6b31f-128">JSON representation</span></span>

<span data-ttu-id="6b31f-129">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="6b31f-129">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.filterOperatorSchema"
}-->

```json
{
  "arity": "String",
  "multivaluedComparisonType": "String",
  "name": "String",
  "supportedAttributeTypes": ["String"]
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "filterOperatorSchema resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/synchronization-filteroperatorschema.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
