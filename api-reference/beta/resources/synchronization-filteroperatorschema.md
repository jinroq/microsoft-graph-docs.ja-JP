---
title: filter演算子スキーマリソースの種類
description: フィルターで使用できる演算子を記述します。
localization_priority: Normal
ms.openlocfilehash: 04bee90f81c0098832cd4b6355be266668d0f69b
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32581738"
---
# <a name="filteroperatorschema-resource-type"></a><span data-ttu-id="1cfc5-103">filter演算子スキーマリソースの種類</span><span class="sxs-lookup"><span data-stu-id="1cfc5-103">filterOperatorSchema resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1cfc5-104">[フィルター](synchronization-filter.md)で使用できる演算子を記述します。</span><span class="sxs-lookup"><span data-stu-id="1cfc5-104">Describes an operator that can be used in a [filter](synchronization-filter.md).</span></span>

## <a name="properties"></a><span data-ttu-id="1cfc5-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="1cfc5-105">Properties</span></span>

| <span data-ttu-id="1cfc5-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="1cfc5-106">Property</span></span>                   | <span data-ttu-id="1cfc5-107">型</span><span class="sxs-lookup"><span data-stu-id="1cfc5-107">Type</span></span>                      | <span data-ttu-id="1cfc5-108">説明</span><span class="sxs-lookup"><span data-stu-id="1cfc5-108">Description</span></span>    |
|:---------------------------|:--------------------------|:---------------|
|<span data-ttu-id="1cfc5-109">アリ</span><span class="sxs-lookup"><span data-stu-id="1cfc5-109">arity</span></span>                       |<span data-ttu-id="1cfc5-110">String</span><span class="sxs-lookup"><span data-stu-id="1cfc5-110">String</span></span>          |<span data-ttu-id="1cfc5-111">演算子のアリティ。</span><span class="sxs-lookup"><span data-stu-id="1cfc5-111">Arity of the operator.</span></span> <span data-ttu-id="1cfc5-112">可能な値は、`Binary`、`Unary` です。</span><span class="sxs-lookup"><span data-stu-id="1cfc5-112">Possible values are: `Binary`, `Unary`.</span></span> <span data-ttu-id="1cfc5-113">既定値は `Binary` です。</span><span class="sxs-lookup"><span data-stu-id="1cfc5-113">The default is `Binary`.</span></span>|
|<span data-ttu-id="1cfc5-114">multivaluedComparisonType</span><span class="sxs-lookup"><span data-stu-id="1cfc5-114">multivaluedComparisonType</span></span>   |<span data-ttu-id="1cfc5-115">scopeOperatorMultiValuedComparisonType</span><span class="sxs-lookup"><span data-stu-id="1cfc5-115">scopeOperatorMultiValuedComparisonType</span></span>          |<span data-ttu-id="1cfc5-116">可能な値は、`All`、`Any` です。</span><span class="sxs-lookup"><span data-stu-id="1cfc5-116">Possible values are: `All`, `Any`.</span></span> <span data-ttu-id="1cfc5-117">複数値属性にのみ適用されます。</span><span class="sxs-lookup"><span data-stu-id="1cfc5-117">Applies only to multivalued attributes.</span></span> <span data-ttu-id="1cfc5-118">`All`すべての値が条件を満たす必要があることを意味します。</span><span class="sxs-lookup"><span data-stu-id="1cfc5-118">`All` means that all values must satisfy the condition.</span></span> <span data-ttu-id="1cfc5-119">`Any`少なくとも1つの値が条件を満たす必要があることを意味します。</span><span class="sxs-lookup"><span data-stu-id="1cfc5-119">`Any` means that at least one value has to satisfy the condition.</span></span> <span data-ttu-id="1cfc5-120">既定値は `All` です。</span><span class="sxs-lookup"><span data-stu-id="1cfc5-120">The default is `All`.</span></span>|
|<span data-ttu-id="1cfc5-121">name</span><span class="sxs-lookup"><span data-stu-id="1cfc5-121">name</span></span>                        |<span data-ttu-id="1cfc5-122">String</span><span class="sxs-lookup"><span data-stu-id="1cfc5-122">String</span></span>                     |<span data-ttu-id="1cfc5-123">オペレーター名。</span><span class="sxs-lookup"><span data-stu-id="1cfc5-123">Operator name.</span></span> |
|<span data-ttu-id="1cfc5-124">supportedAttributeTypes</span><span class="sxs-lookup"><span data-stu-id="1cfc5-124">supportedAttributeTypes</span></span>     |<span data-ttu-id="1cfc5-125">String collection</span><span class="sxs-lookup"><span data-stu-id="1cfc5-125">String collection</span></span>         |<span data-ttu-id="1cfc5-126">演算子でサポートされている属性の種類。</span><span class="sxs-lookup"><span data-stu-id="1cfc5-126">Attribute types supported by the operator.</span></span> <span data-ttu-id="1cfc5-127">可能な値は、`Boolean`、`Binary`、`Reference`、`Integer`、`String` です。</span><span class="sxs-lookup"><span data-stu-id="1cfc5-127">Possible values are: `Boolean`, `Binary`, `Reference`, `Integer`, `String`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="1cfc5-128">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="1cfc5-128">JSON representation</span></span>

<span data-ttu-id="1cfc5-129">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="1cfc5-129">The following is a JSON representation of the resource.</span></span>

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
