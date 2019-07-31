---
title: Filter演算子スキーマリソースの種類
description: フィルターで使用できる演算子を記述します。
localization_priority: Normal
doc_type: resourcePageType
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 2ed9ef208f888026224293ff86a36b62a3486d48
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36007894"
---
# <a name="filteroperatorschema-resource-type"></a><span data-ttu-id="741d8-103">Filter演算子スキーマリソースの種類</span><span class="sxs-lookup"><span data-stu-id="741d8-103">filterOperatorSchema resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="741d8-104">[フィルター](synchronization-filter.md)で使用できる演算子を記述します。</span><span class="sxs-lookup"><span data-stu-id="741d8-104">Describes an operator that can be used in a [filter](synchronization-filter.md).</span></span>

## <a name="properties"></a><span data-ttu-id="741d8-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="741d8-105">Properties</span></span>

| <span data-ttu-id="741d8-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="741d8-106">Property</span></span>                   | <span data-ttu-id="741d8-107">型</span><span class="sxs-lookup"><span data-stu-id="741d8-107">Type</span></span>                      | <span data-ttu-id="741d8-108">説明</span><span class="sxs-lookup"><span data-stu-id="741d8-108">Description</span></span>    |
|:---------------------------|:--------------------------|:---------------|
|<span data-ttu-id="741d8-109">アリ</span><span class="sxs-lookup"><span data-stu-id="741d8-109">arity</span></span>                       |<span data-ttu-id="741d8-110">String</span><span class="sxs-lookup"><span data-stu-id="741d8-110">String</span></span>          |<span data-ttu-id="741d8-111">演算子のアリティ。</span><span class="sxs-lookup"><span data-stu-id="741d8-111">Arity of the operator.</span></span> <span data-ttu-id="741d8-112">可能な値は、`Binary`、`Unary` です。</span><span class="sxs-lookup"><span data-stu-id="741d8-112">Possible values are: `Binary`, `Unary`.</span></span> <span data-ttu-id="741d8-113">既定値は `Binary` です。</span><span class="sxs-lookup"><span data-stu-id="741d8-113">The default is `Binary`.</span></span>|
|<span data-ttu-id="741d8-114">multivaluedComparisonType</span><span class="sxs-lookup"><span data-stu-id="741d8-114">multivaluedComparisonType</span></span>   |<span data-ttu-id="741d8-115">scopeOperatorMultiValuedComparisonType</span><span class="sxs-lookup"><span data-stu-id="741d8-115">scopeOperatorMultiValuedComparisonType</span></span>          |<span data-ttu-id="741d8-116">可能な値は、`All`、`Any` です。</span><span class="sxs-lookup"><span data-stu-id="741d8-116">Possible values are: `All`, `Any`.</span></span> <span data-ttu-id="741d8-117">複数値属性にのみ適用されます。</span><span class="sxs-lookup"><span data-stu-id="741d8-117">Applies only to multivalued attributes.</span></span> <span data-ttu-id="741d8-118">`All`すべての値が条件を満たす必要があることを意味します。</span><span class="sxs-lookup"><span data-stu-id="741d8-118">`All` means that all values must satisfy the condition.</span></span> <span data-ttu-id="741d8-119">`Any`少なくとも1つの値が条件を満たす必要があることを意味します。</span><span class="sxs-lookup"><span data-stu-id="741d8-119">`Any` means that at least one value has to satisfy the condition.</span></span> <span data-ttu-id="741d8-120">既定値は `All` です。</span><span class="sxs-lookup"><span data-stu-id="741d8-120">The default is `All`.</span></span>|
|<span data-ttu-id="741d8-121">name</span><span class="sxs-lookup"><span data-stu-id="741d8-121">name</span></span>                        |<span data-ttu-id="741d8-122">String</span><span class="sxs-lookup"><span data-stu-id="741d8-122">String</span></span>                     |<span data-ttu-id="741d8-123">オペレーター名。</span><span class="sxs-lookup"><span data-stu-id="741d8-123">Operator name.</span></span> |
|<span data-ttu-id="741d8-124">supportedAttributeTypes</span><span class="sxs-lookup"><span data-stu-id="741d8-124">supportedAttributeTypes</span></span>     |<span data-ttu-id="741d8-125">文字列コレクション</span><span class="sxs-lookup"><span data-stu-id="741d8-125">String collection</span></span>         |<span data-ttu-id="741d8-126">演算子でサポートされている属性の種類。</span><span class="sxs-lookup"><span data-stu-id="741d8-126">Attribute types supported by the operator.</span></span> <span data-ttu-id="741d8-127">可能な値は、`Boolean`、`Binary`、`Reference`、`Integer`、`String` です。</span><span class="sxs-lookup"><span data-stu-id="741d8-127">Possible values are: `Boolean`, `Binary`, `Reference`, `Integer`, `String`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="741d8-128">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="741d8-128">JSON representation</span></span>

<span data-ttu-id="741d8-129">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="741d8-129">The following is a JSON representation of the resource.</span></span>

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
  "suppressions": []
}
-->
