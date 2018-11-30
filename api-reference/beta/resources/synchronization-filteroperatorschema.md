---
title: filterOperatorSchema リソースの種類
description: フィルターで使用できる演算子をについて説明します。
ms.openlocfilehash: 1a4e21aea2b65073a00c9797065f6788a66e2334
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27067703"
---
# <a name="filteroperatorschema-resource-type"></a><span data-ttu-id="d0720-103">filterOperatorSchema リソースの種類</span><span class="sxs-lookup"><span data-stu-id="d0720-103">filterOperatorSchema resource type</span></span>

> <span data-ttu-id="d0720-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="d0720-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d0720-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d0720-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="d0720-106">[フィルター](synchronization-filter.md)で使用できる演算子をについて説明します。</span><span class="sxs-lookup"><span data-stu-id="d0720-106">Describes an operator that can be used in a [filter](synchronization-filter.md).</span></span>

## <a name="properties"></a><span data-ttu-id="d0720-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="d0720-107">Properties</span></span>

| <span data-ttu-id="d0720-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="d0720-108">Property</span></span>                   | <span data-ttu-id="d0720-109">型</span><span class="sxs-lookup"><span data-stu-id="d0720-109">Type</span></span>                      | <span data-ttu-id="d0720-110">説明</span><span class="sxs-lookup"><span data-stu-id="d0720-110">Description</span></span>    |
|:---------------------------|:--------------------------|:---------------|
|<span data-ttu-id="d0720-111">アリティ</span><span class="sxs-lookup"><span data-stu-id="d0720-111">arity</span></span>                       |<span data-ttu-id="d0720-112">String</span><span class="sxs-lookup"><span data-stu-id="d0720-112">String</span></span>          |<span data-ttu-id="d0720-113">演算子のアリティ。</span><span class="sxs-lookup"><span data-stu-id="d0720-113">Arity of the operator.</span></span> <span data-ttu-id="d0720-114">使用可能な値は、`Binary`、`Unary` です。</span><span class="sxs-lookup"><span data-stu-id="d0720-114">Possible values are: `Binary`, `Unary`.</span></span> <span data-ttu-id="d0720-115">既定値は `Binary` です。</span><span class="sxs-lookup"><span data-stu-id="d0720-115">The default is `Binary`.</span></span>|
|<span data-ttu-id="d0720-116">multivaluedComparisonType</span><span class="sxs-lookup"><span data-stu-id="d0720-116">multivaluedComparisonType</span></span>   |<span data-ttu-id="d0720-117">scopeOperatorMultiValuedComparisonType</span><span class="sxs-lookup"><span data-stu-id="d0720-117">scopeOperatorMultiValuedComparisonType</span></span>          |<span data-ttu-id="d0720-118">使用可能な値は、`All`、`Any` です。</span><span class="sxs-lookup"><span data-stu-id="d0720-118">Possible values are: `All`, `Any`.</span></span> <span data-ttu-id="d0720-119">複数値を持つ属性にのみ適用されます。</span><span class="sxs-lookup"><span data-stu-id="d0720-119">Applies only to multivalued attributes.</span></span> <span data-ttu-id="d0720-120">`All`すべての値が条件を満たす必要があることを意味します。</span><span class="sxs-lookup"><span data-stu-id="d0720-120">`All` means that all values must satisfy the condition.</span></span> <span data-ttu-id="d0720-121">`Any`条件を満たすために、少なくとも 1 つの値が含まれていることを意味します。</span><span class="sxs-lookup"><span data-stu-id="d0720-121">`Any` means that at least one value has to satisfy the condition.</span></span> <span data-ttu-id="d0720-122">既定値は `All` です。</span><span class="sxs-lookup"><span data-stu-id="d0720-122">The default is `All`.</span></span>|
|<span data-ttu-id="d0720-123">名前</span><span class="sxs-lookup"><span data-stu-id="d0720-123">name</span></span>                        |<span data-ttu-id="d0720-124">String</span><span class="sxs-lookup"><span data-stu-id="d0720-124">String</span></span>                     |<span data-ttu-id="d0720-125">オペレーター名です。</span><span class="sxs-lookup"><span data-stu-id="d0720-125">Operator name.</span></span> |
|<span data-ttu-id="d0720-126">supportedAttributeTypes</span><span class="sxs-lookup"><span data-stu-id="d0720-126">supportedAttributeTypes</span></span>     |<span data-ttu-id="d0720-127">String コレクション</span><span class="sxs-lookup"><span data-stu-id="d0720-127">String collection</span></span>         |<span data-ttu-id="d0720-128">属性の型が演算子でサポートします。</span><span class="sxs-lookup"><span data-stu-id="d0720-128">Attribute types supported by the operator.</span></span> <span data-ttu-id="d0720-129">可能な値は、`Boolean`、`Binary`、`Reference`、`Integer`、`String` です。</span><span class="sxs-lookup"><span data-stu-id="d0720-129">Possible values are: `Boolean`, `Binary`, `Reference`, `Integer`, `String`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="d0720-130">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="d0720-130">JSON representation</span></span>

<span data-ttu-id="d0720-131">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="d0720-131">The following is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "filterOperatorSchema resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->