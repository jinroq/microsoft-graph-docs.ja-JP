---
title: attributeMappingParameterSchema リソースの種類
description: attributeMappingFunctionSchema で使用される1つのパラメーターを記述します。
localization_priority: Normal
ms.openlocfilehash: 44234e7e76b5b0d0fb514366be6106c8177b56db
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33342951"
---
# <a name="attributemappingparameterschema-resource-type"></a><span data-ttu-id="ca7d3-103">attributeMappingParameterSchema リソースの種類</span><span class="sxs-lookup"><span data-stu-id="ca7d3-103">attributeMappingParameterSchema resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ca7d3-104">[attributeMappingFunctionSchema](../resources/synchronization-attributemappingfunctionschema.md)で使用される1つのパラメーターを記述します。</span><span class="sxs-lookup"><span data-stu-id="ca7d3-104">Describes a single parameter used in an [attributeMappingFunctionSchema](../resources/synchronization-attributemappingfunctionschema.md).</span></span>

## <a name="properties"></a><span data-ttu-id="ca7d3-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="ca7d3-105">Properties</span></span>

| <span data-ttu-id="ca7d3-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="ca7d3-106">Property</span></span>                   | <span data-ttu-id="ca7d3-107">型</span><span class="sxs-lookup"><span data-stu-id="ca7d3-107">Type</span></span>                      | <span data-ttu-id="ca7d3-108">説明</span><span class="sxs-lookup"><span data-stu-id="ca7d3-108">Description</span></span>    |
|:---------------------------|:-------------------------|:---------------|
|<span data-ttu-id="ca7d3-109">allow多重オカレンス</span><span class="sxs-lookup"><span data-stu-id="ca7d3-109">allowMultipleOccurrences</span></span>    |<span data-ttu-id="ca7d3-110">Boolean</span><span class="sxs-lookup"><span data-stu-id="ca7d3-110">Boolean</span></span>                   |<span data-ttu-id="ca7d3-111">指定されたパラメーターは、複数回指定できます (たとえば、 `Concatenate(string,string,...)`関数内の複数の入力文字列)。</span><span class="sxs-lookup"><span data-stu-id="ca7d3-111">The given parameter can be provided multiple times (for example, multiple input strings in the `Concatenate(string,string,...)` function).</span></span> |
|<span data-ttu-id="ca7d3-112">name</span><span class="sxs-lookup"><span data-stu-id="ca7d3-112">name</span></span>                        |<span data-ttu-id="ca7d3-113">String</span><span class="sxs-lookup"><span data-stu-id="ca7d3-113">String</span></span>                    |<span data-ttu-id="ca7d3-114">パラメーター名。</span><span class="sxs-lookup"><span data-stu-id="ca7d3-114">Parameter name.</span></span> |
|<span data-ttu-id="ca7d3-115">必須</span><span class="sxs-lookup"><span data-stu-id="ca7d3-115">required</span></span>                    |<span data-ttu-id="ca7d3-116">Boolean</span><span class="sxs-lookup"><span data-stu-id="ca7d3-116">Boolean</span></span>                   |<span data-ttu-id="ca7d3-117">`true`パラメーターが必要な場合は、それ`false`以外の場合は。</span><span class="sxs-lookup"><span data-stu-id="ca7d3-117">`true` if the parameter is required; otherwise `false`.</span></span> |
|<span data-ttu-id="ca7d3-118">type</span><span class="sxs-lookup"><span data-stu-id="ca7d3-118">type</span></span>                        |<span data-ttu-id="ca7d3-119">String</span><span class="sxs-lookup"><span data-stu-id="ca7d3-119">String</span></span>                    |<span data-ttu-id="ca7d3-120">使用可能な値は、`Boolean`、`Binary`、`Reference`、`Integer`、`String` です。</span><span class="sxs-lookup"><span data-stu-id="ca7d3-120">Possible values are: `Boolean`, `Binary`, `Reference`, `Integer`, `String`.</span></span> <span data-ttu-id="ca7d3-121">既定値は `String` です。</span><span class="sxs-lookup"><span data-stu-id="ca7d3-121">Default is `String`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="ca7d3-122">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="ca7d3-122">JSON representation</span></span>

<span data-ttu-id="ca7d3-123">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="ca7d3-123">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.attributeMappingParameterSchema"
}-->

```json
{
  "allowMultipleOccurrences": "Boolean",
  "name": "String",
  "required": "Boolean",
  "type": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "attributeMappingParameterSchema resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
