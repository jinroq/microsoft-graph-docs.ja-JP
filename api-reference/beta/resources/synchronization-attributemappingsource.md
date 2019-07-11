---
title: attributeMappingSource リソースの種類
description: 'ソースオブジェクトから値を抽出 (変換) する方法を定義します。 たとえば、ソースオブジェクトの特定の属性から取得した単純な値を指定することも、複数のソース属性に基づいて文字列の連結/抽出/置換を行うより複雑な式にすることもできます。 '
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 0c5ef197a72767fb0c764689558b9c005be856f8
ms.sourcegitcommit: 121c0fad692fb3c5c01dc051481b5249e4491b48
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/11/2019
ms.locfileid: "35621453"
---
# <a name="attributemappingsource-resource-type"></a><span data-ttu-id="586f2-104">attributeMappingSource リソースの種類</span><span class="sxs-lookup"><span data-stu-id="586f2-104">attributeMappingSource resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="586f2-105">ソースオブジェクトから値を抽出 (変換) する方法を定義します。</span><span class="sxs-lookup"><span data-stu-id="586f2-105">Defines how a value should be extracted (or transformed) from the source object.</span></span> <span data-ttu-id="586f2-106">たとえば、ソースオブジェクトの特定の属性から取得した単純な値を指定することも、複数のソース属性に基づいて文字列の連結/抽出/置換を行うより複雑な式にすることもできます。</span><span class="sxs-lookup"><span data-stu-id="586f2-106">For example, it can be a simple value taken from a given attribute on the source object, or it can be a more complex expression of string concatenation/extraction/replacement based on several source attributes.</span></span> 

## <a name="properties"></a><span data-ttu-id="586f2-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="586f2-107">Properties</span></span>

| <span data-ttu-id="586f2-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="586f2-108">Property</span></span>              | <span data-ttu-id="586f2-109">型</span><span class="sxs-lookup"><span data-stu-id="586f2-109">Type</span></span>                      | <span data-ttu-id="586f2-110">説明</span><span class="sxs-lookup"><span data-stu-id="586f2-110">Description</span></span>               |
|:----------------------|:--------------------------|:--------------------------|
|<span data-ttu-id="586f2-111">式</span><span class="sxs-lookup"><span data-stu-id="586f2-111">expression</span></span>             |<span data-ttu-id="586f2-112">String</span><span class="sxs-lookup"><span data-stu-id="586f2-112">String</span></span>                     |<span data-ttu-id="586f2-113">この**attributeMappingSource**オブジェクトの同等の式表現。</span><span class="sxs-lookup"><span data-stu-id="586f2-113">Equivalent expression representation of this **attributeMappingSource** object.</span></span>|
|<span data-ttu-id="586f2-114">name</span><span class="sxs-lookup"><span data-stu-id="586f2-114">name</span></span>                   |<span data-ttu-id="586f2-115">String</span><span class="sxs-lookup"><span data-stu-id="586f2-115">String</span></span>                     |<span data-ttu-id="586f2-116">マッピングソースの Name パラメーター。</span><span class="sxs-lookup"><span data-stu-id="586f2-116">Name parameter of the mapping source.</span></span> <span data-ttu-id="586f2-117">**Type**プロパティの値に応じて、関数の名前、source 属性の名前、または使用する定数値を指定できます。</span><span class="sxs-lookup"><span data-stu-id="586f2-117">Depending on the **type** property value, this can be the name of the function, the name of the source attribute, or a constant value to be used.</span></span> |
|<span data-ttu-id="586f2-118">parameters</span><span class="sxs-lookup"><span data-stu-id="586f2-118">parameters</span></span>             |<span data-ttu-id="586f2-119">[stringKeyAttributeMappingSourceValuePair](synchronization-stringkeyattributemappingsourcevaluepair.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="586f2-119">[stringKeyAttributeMappingSourceValuePair](synchronization-stringkeyattributemappingsourcevaluepair.md) collection</span></span> | <span data-ttu-id="586f2-120">このオブジェクトが関数を表す場合は、関数パラメータを一覧表示します。</span><span class="sxs-lookup"><span data-stu-id="586f2-120">If this object represents a function, lists function parameters.</span></span> <span data-ttu-id="586f2-121">パラメータは、 **attributeMappingSource**オブジェクト自体で構成され、複雑な式を使用できます。</span><span class="sxs-lookup"><span data-stu-id="586f2-121">Parameters consist of **attributeMappingSource** objects themselves, allowing for complex expressions.</span></span> <span data-ttu-id="586f2-122">**Type**がでは`Function`ない場合、このプロパティは null または空の配列になります。</span><span class="sxs-lookup"><span data-stu-id="586f2-122">If **type** is not `Function`, this property will be null/empty array.</span></span> |
|<span data-ttu-id="586f2-123">type</span><span class="sxs-lookup"><span data-stu-id="586f2-123">type</span></span>                   | <span data-ttu-id="586f2-124">String</span><span class="sxs-lookup"><span data-stu-id="586f2-124">String</span></span>                    |<span data-ttu-id="586f2-125">この属性マッピングソースの種類。</span><span class="sxs-lookup"><span data-stu-id="586f2-125">The type of this attribute mapping source.</span></span> <span data-ttu-id="586f2-126">可能な値は、`Attribute`、`Constant`、`Function` です。</span><span class="sxs-lookup"><span data-stu-id="586f2-126">Possible values are: `Attribute`, `Constant`, `Function`.</span></span> <span data-ttu-id="586f2-127">既定値は `Attribute` です。</span><span class="sxs-lookup"><span data-stu-id="586f2-127">Default is `Attribute`.</span></span>| 

## <a name="json-representation"></a><span data-ttu-id="586f2-128">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="586f2-128">JSON representation</span></span>

<span data-ttu-id="586f2-129">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="586f2-129">The following is a JSON representation of the resource.</span></span>

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

## <a name="json-examples"></a><span data-ttu-id="586f2-130">JSON の例</span><span class="sxs-lookup"><span data-stu-id="586f2-130">JSON Examples</span></span>

<span data-ttu-id="586f2-131">シンプルな属性から属性へのマッピング</span><span class="sxs-lookup"><span data-stu-id="586f2-131">Simple attribute to attribute mapping</span></span>

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

<span data-ttu-id="586f2-132">Source 属性から最初の8文字を抽出する式</span><span class="sxs-lookup"><span data-stu-id="586f2-132">Expression extracting first 8 characters from the source attribute</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "attributeMappingSource resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
