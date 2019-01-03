---
title: attributeMappingSource リソースの種類
description: '定義の値がどのようにする必要があります抽出 (変換)、ソース オブジェクトからです。 ソース オブジェクトの特定の属性から取得した単純な値であることなど、文字列の連結/抽出/交換のいくつかのソース属性に基づいたより複雑な式であることができます。 '
ms.openlocfilehash: aeb39c829d7be081fe9ee08aa5845e6ced1194dc
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27069825"
---
# <a name="attributemappingsource-resource-type"></a><span data-ttu-id="c55d1-104">attributeMappingSource リソースの種類</span><span class="sxs-lookup"><span data-stu-id="c55d1-104">attributeMappingSource resource type</span></span>

> <span data-ttu-id="c55d1-105">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="c55d1-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c55d1-106">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c55d1-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="c55d1-107">定義の値がどのようにする必要があります抽出 (変換)、ソース オブジェクトからです。</span><span class="sxs-lookup"><span data-stu-id="c55d1-107">Defines how a value should be extracted (or transformed) from the source object.</span></span> <span data-ttu-id="c55d1-108">ソース オブジェクトの特定の属性から取得した単純な値であることなど、文字列の連結/抽出/交換のいくつかのソース属性に基づいたより複雑な式であることができます。</span><span class="sxs-lookup"><span data-stu-id="c55d1-108">For example, it can be a simple value taken from a given attribute on the source object, or it can be a more complex expression of string concatenation/extraction/replacement based on several source attributes.</span></span> 

## <a name="properties"></a><span data-ttu-id="c55d1-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="c55d1-109">Properties</span></span>

| <span data-ttu-id="c55d1-110">プロパティ</span><span class="sxs-lookup"><span data-stu-id="c55d1-110">Property</span></span>              | <span data-ttu-id="c55d1-111">型</span><span class="sxs-lookup"><span data-stu-id="c55d1-111">Type</span></span>                      | <span data-ttu-id="c55d1-112">説明</span><span class="sxs-lookup"><span data-stu-id="c55d1-112">Description</span></span>               |
|:----------------------|:--------------------------|:--------------------------|
|<span data-ttu-id="c55d1-113">式</span><span class="sxs-lookup"><span data-stu-id="c55d1-113">expression</span></span>             |<span data-ttu-id="c55d1-114">String</span><span class="sxs-lookup"><span data-stu-id="c55d1-114">String</span></span>                     |<span data-ttu-id="c55d1-115">この**attributeMappingSource**オブジェクトの同等の式表現です。</span><span class="sxs-lookup"><span data-stu-id="c55d1-115">Equivalent expression representation of this **attributeMappingSource** object.</span></span>|
|<span data-ttu-id="c55d1-116">名前</span><span class="sxs-lookup"><span data-stu-id="c55d1-116">name</span></span>                   |<span data-ttu-id="c55d1-117">String</span><span class="sxs-lookup"><span data-stu-id="c55d1-117">String</span></span>                     |<span data-ttu-id="c55d1-118">マッピングのソースの名前のパラメーター。</span><span class="sxs-lookup"><span data-stu-id="c55d1-118">Name parameter of the mapping source.</span></span> <span data-ttu-id="c55d1-119">**型**のプロパティの値によって、関数の場合、基になる属性、または使用する定数の値の名前の名前できます。</span><span class="sxs-lookup"><span data-stu-id="c55d1-119">Depending on the **type** property value, this can be the name of the function, the name of the source attribute, or a constant value to be used.</span></span> |
|<span data-ttu-id="c55d1-120">parameters</span><span class="sxs-lookup"><span data-stu-id="c55d1-120">parameters</span></span>             |<span data-ttu-id="c55d1-121">[stringKeyAttributeMappingSourceValuePair](synchronization-stringkeyattributemappingsourcevaluepair.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="c55d1-121">[stringKeyAttributeMappingSourceValuePair](synchronization-stringkeyattributemappingsourcevaluepair.md) collection</span></span> | <span data-ttu-id="c55d1-122">このオブジェクトは、関数を表している場合は、関数のパラメーターを一覧表示します。</span><span class="sxs-lookup"><span data-stu-id="c55d1-122">If this object represents a function, lists function parameters.</span></span> <span data-ttu-id="c55d1-123">パラメーターは、 **attributeMappingSource**オブジェクト自身であり、複雑な正規表現で構成されます。</span><span class="sxs-lookup"><span data-stu-id="c55d1-123">Parameters consist of **attributeMappingSource** objects themselves, allowing for complex expressions.</span></span> <span data-ttu-id="c55d1-124">**型**でない場合`Function`、このプロパティは null または空の配列になります。</span><span class="sxs-lookup"><span data-stu-id="c55d1-124">If **type** is not `Function`, this property will be null/empty array.</span></span> |
|<span data-ttu-id="c55d1-125">type</span><span class="sxs-lookup"><span data-stu-id="c55d1-125">type</span></span>                   | <span data-ttu-id="c55d1-126">String</span><span class="sxs-lookup"><span data-stu-id="c55d1-126">String</span></span>                    |<span data-ttu-id="c55d1-127">この属性のマッピングのソースの型。</span><span class="sxs-lookup"><span data-stu-id="c55d1-127">The type of this attribute mapping source.</span></span> <span data-ttu-id="c55d1-128">可能な値は、`Attribute`、`Constant`、`Function` です。</span><span class="sxs-lookup"><span data-stu-id="c55d1-128">Possible values are: `Attribute`, `Constant`, `Function`.</span></span> <span data-ttu-id="c55d1-129">既定値は `Attribute` です。</span><span class="sxs-lookup"><span data-stu-id="c55d1-129">Default is `Attribute`.</span></span>| 

## <a name="json-representation"></a><span data-ttu-id="c55d1-130">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="c55d1-130">JSON representation</span></span>

<span data-ttu-id="c55d1-131">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="c55d1-131">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.attributeMappingSource"
}-->

```json
{
  "expression": "String",
  "name": "String",
  "parameters": [{"@odata.type": "microsoft.graph.stringKeyAttributeMappingSourceValuePair"}],
  "type": "String"
}
```

## <a name="json-examples"></a><span data-ttu-id="c55d1-132">JSON の例</span><span class="sxs-lookup"><span data-stu-id="c55d1-132">JSON Examples</span></span>

<span data-ttu-id="c55d1-133">単純な属性を属性のマッピング</span><span class="sxs-lookup"><span data-stu-id="c55d1-133">Simple attribute to attribute mapping</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.attributeMappingSource"
}-->

```json
{
    "expression": "[mail]",
    "name": "mail",
    "type": "Attribute"
}
```

<span data-ttu-id="c55d1-134">ソース属性の最初の 8 文字を抽出する式</span><span class="sxs-lookup"><span data-stu-id="c55d1-134">Expression extracting first 8 characters from the source attribute</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.attributeMappingSource"
}-->

```json
 {
    "expression": "Mid([userPrincipalName], 1, 8)",
    "name": "Mid",
    "parameters": [
        {
            "key": "source",
            "value": {
                "expression": "[userPrincipalName]",
                "name": "userPrincipalName",
                "parameters": [],
                "type": "Attribute"
            }
        },
        {
            "key": "start",
            "value": {
                "expression": "\"1\"",
                "name": "1",
                "parameters": [],
                "type": "Constant"
            }
        },
        {
            "key": "length",
            "value": {
                "expression": "\"8\"",
                "name": "8",
                "parameters": [],
                "type": "Constant"
            }
        }
    ],
    "type": "Function"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "attributeMappingSource resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->