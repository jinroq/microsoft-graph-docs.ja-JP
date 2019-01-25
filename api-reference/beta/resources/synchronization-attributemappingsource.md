---
title: attributeMappingSource リソースの種類
description: '定義の値がどのようにする必要があります抽出 (変換)、ソース オブジェクトからです。 ソース オブジェクトの特定の属性から取得した単純な値であることなど、文字列の連結/抽出/交換のいくつかのソース属性に基づいたより複雑な式であることができます。 '
localization_priority: Normal
ms.openlocfilehash: 1d15cd82c0a58ac8bdd3ac5805abc166322f27fe
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29510408"
---
# <a name="attributemappingsource-resource-type"></a><span data-ttu-id="15d7a-104">attributeMappingSource リソースの種類</span><span class="sxs-lookup"><span data-stu-id="15d7a-104">attributeMappingSource resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="15d7a-105">定義の値がどのようにする必要があります抽出 (変換)、ソース オブジェクトからです。</span><span class="sxs-lookup"><span data-stu-id="15d7a-105">Defines how a value should be extracted (or transformed) from the source object.</span></span> <span data-ttu-id="15d7a-106">ソース オブジェクトの特定の属性から取得した単純な値であることなど、文字列の連結/抽出/交換のいくつかのソース属性に基づいたより複雑な式であることができます。</span><span class="sxs-lookup"><span data-stu-id="15d7a-106">For example, it can be a simple value taken from a given attribute on the source object, or it can be a more complex expression of string concatenation/extraction/replacement based on several source attributes.</span></span> 

## <a name="properties"></a><span data-ttu-id="15d7a-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="15d7a-107">Properties</span></span>

| <span data-ttu-id="15d7a-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="15d7a-108">Property</span></span>              | <span data-ttu-id="15d7a-109">型</span><span class="sxs-lookup"><span data-stu-id="15d7a-109">Type</span></span>                      | <span data-ttu-id="15d7a-110">説明</span><span class="sxs-lookup"><span data-stu-id="15d7a-110">Description</span></span>               |
|:----------------------|:--------------------------|:--------------------------|
|<span data-ttu-id="15d7a-111">式</span><span class="sxs-lookup"><span data-stu-id="15d7a-111">expression</span></span>             |<span data-ttu-id="15d7a-112">String</span><span class="sxs-lookup"><span data-stu-id="15d7a-112">String</span></span>                     |<span data-ttu-id="15d7a-113">この**attributeMappingSource**オブジェクトの同等の式表現です。</span><span class="sxs-lookup"><span data-stu-id="15d7a-113">Equivalent expression representation of this **attributeMappingSource** object.</span></span>|
|<span data-ttu-id="15d7a-114">name</span><span class="sxs-lookup"><span data-stu-id="15d7a-114">name</span></span>                   |<span data-ttu-id="15d7a-115">String</span><span class="sxs-lookup"><span data-stu-id="15d7a-115">String</span></span>                     |<span data-ttu-id="15d7a-116">マッピングのソースの名前のパラメーター。</span><span class="sxs-lookup"><span data-stu-id="15d7a-116">Name parameter of the mapping source.</span></span> <span data-ttu-id="15d7a-117">**型**のプロパティの値によって、関数の場合、基になる属性、または使用する定数の値の名前の名前できます。</span><span class="sxs-lookup"><span data-stu-id="15d7a-117">Depending on the **type** property value, this can be the name of the function, the name of the source attribute, or a constant value to be used.</span></span> |
|<span data-ttu-id="15d7a-118">parameters</span><span class="sxs-lookup"><span data-stu-id="15d7a-118">parameters</span></span>             |<span data-ttu-id="15d7a-119">[stringKeyAttributeMappingSourceValuePair](synchronization-stringkeyattributemappingsourcevaluepair.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="15d7a-119">[stringKeyAttributeMappingSourceValuePair](synchronization-stringkeyattributemappingsourcevaluepair.md) collection</span></span> | <span data-ttu-id="15d7a-120">このオブジェクトは、関数を表している場合は、関数のパラメーターを一覧表示します。</span><span class="sxs-lookup"><span data-stu-id="15d7a-120">If this object represents a function, lists function parameters.</span></span> <span data-ttu-id="15d7a-121">パラメーターは、 **attributeMappingSource**オブジェクト自身であり、複雑な正規表現で構成されます。</span><span class="sxs-lookup"><span data-stu-id="15d7a-121">Parameters consist of **attributeMappingSource** objects themselves, allowing for complex expressions.</span></span> <span data-ttu-id="15d7a-122">**型**でない場合`Function`、このプロパティは null または空の配列になります。</span><span class="sxs-lookup"><span data-stu-id="15d7a-122">If **type** is not `Function`, this property will be null/empty array.</span></span> |
|<span data-ttu-id="15d7a-123">type</span><span class="sxs-lookup"><span data-stu-id="15d7a-123">type</span></span>                   | <span data-ttu-id="15d7a-124">String</span><span class="sxs-lookup"><span data-stu-id="15d7a-124">String</span></span>                    |<span data-ttu-id="15d7a-125">この属性のマッピングのソースの型。</span><span class="sxs-lookup"><span data-stu-id="15d7a-125">The type of this attribute mapping source.</span></span> <span data-ttu-id="15d7a-126">可能な値は、`Attribute`、`Constant`、`Function` です。</span><span class="sxs-lookup"><span data-stu-id="15d7a-126">Possible values are: `Attribute`, `Constant`, `Function`.</span></span> <span data-ttu-id="15d7a-127">既定値は `Attribute` です。</span><span class="sxs-lookup"><span data-stu-id="15d7a-127">Default is `Attribute`.</span></span>| 

## <a name="json-representation"></a><span data-ttu-id="15d7a-128">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="15d7a-128">JSON representation</span></span>

<span data-ttu-id="15d7a-129">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="15d7a-129">The following is a JSON representation of the resource.</span></span>

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

## <a name="json-examples"></a><span data-ttu-id="15d7a-130">JSON の例</span><span class="sxs-lookup"><span data-stu-id="15d7a-130">JSON Examples</span></span>

<span data-ttu-id="15d7a-131">単純な属性を属性のマッピング</span><span class="sxs-lookup"><span data-stu-id="15d7a-131">Simple attribute to attribute mapping</span></span>

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

<span data-ttu-id="15d7a-132">ソース属性の最初の 8 文字を抽出する式</span><span class="sxs-lookup"><span data-stu-id="15d7a-132">Expression extracting first 8 characters from the source attribute</span></span>

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
  "suppressions": [
    "Error: /api-reference/beta/resources/synchronization-attributemappingsource.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
