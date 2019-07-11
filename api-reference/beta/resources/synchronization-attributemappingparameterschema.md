---
title: attributeMappingParameterSchema リソースの種類
description: AttributeMappingFunctionSchema で使用される1つのパラメーターを記述します。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: d8624851d37f475df66ec51f1951ebbbe1ea97a8
ms.sourcegitcommit: 121c0fad692fb3c5c01dc051481b5249e4491b48
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/11/2019
ms.locfileid: "35620270"
---
# <a name="attributemappingparameterschema-resource-type"></a><span data-ttu-id="49ea0-103">attributeMappingParameterSchema リソースの種類</span><span class="sxs-lookup"><span data-stu-id="49ea0-103">attributeMappingParameterSchema resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="49ea0-104">[AttributeMappingFunctionSchema](../resources/synchronization-attributemappingfunctionschema.md)で使用される1つのパラメーターを記述します。</span><span class="sxs-lookup"><span data-stu-id="49ea0-104">Describes a single parameter used in an [attributeMappingFunctionSchema](../resources/synchronization-attributemappingfunctionschema.md).</span></span>

## <a name="properties"></a><span data-ttu-id="49ea0-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="49ea0-105">Properties</span></span>

| <span data-ttu-id="49ea0-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="49ea0-106">Property</span></span>                   | <span data-ttu-id="49ea0-107">型</span><span class="sxs-lookup"><span data-stu-id="49ea0-107">Type</span></span>                      | <span data-ttu-id="49ea0-108">説明</span><span class="sxs-lookup"><span data-stu-id="49ea0-108">Description</span></span>    |
|:---------------------------|:-------------------------|:---------------|
|<span data-ttu-id="49ea0-109">Allow多重オカレンス</span><span class="sxs-lookup"><span data-stu-id="49ea0-109">allowMultipleOccurrences</span></span>    |<span data-ttu-id="49ea0-110">Boolean</span><span class="sxs-lookup"><span data-stu-id="49ea0-110">Boolean</span></span>                   |<span data-ttu-id="49ea0-111">指定されたパラメーターは、複数回指定できます (たとえば、 `Concatenate(string,string,...)`関数内の複数の入力文字列)。</span><span class="sxs-lookup"><span data-stu-id="49ea0-111">The given parameter can be provided multiple times (for example, multiple input strings in the `Concatenate(string,string,...)` function).</span></span> |
|<span data-ttu-id="49ea0-112">name</span><span class="sxs-lookup"><span data-stu-id="49ea0-112">name</span></span>                        |<span data-ttu-id="49ea0-113">String</span><span class="sxs-lookup"><span data-stu-id="49ea0-113">String</span></span>                    |<span data-ttu-id="49ea0-114">パラメーター名。</span><span class="sxs-lookup"><span data-stu-id="49ea0-114">Parameter name.</span></span> |
|<span data-ttu-id="49ea0-115">必須</span><span class="sxs-lookup"><span data-stu-id="49ea0-115">required</span></span>                    |<span data-ttu-id="49ea0-116">Boolean</span><span class="sxs-lookup"><span data-stu-id="49ea0-116">Boolean</span></span>                   |<span data-ttu-id="49ea0-117">`true`パラメーターが必要な場合は、それ`false`以外の場合は。</span><span class="sxs-lookup"><span data-stu-id="49ea0-117">`true` if the parameter is required; otherwise `false`.</span></span> |
|<span data-ttu-id="49ea0-118">type</span><span class="sxs-lookup"><span data-stu-id="49ea0-118">type</span></span>                        |<span data-ttu-id="49ea0-119">String</span><span class="sxs-lookup"><span data-stu-id="49ea0-119">String</span></span>                    |<span data-ttu-id="49ea0-120">使用可能な値は、`Boolean`、`Binary`、`Reference`、`Integer`、`String` です。</span><span class="sxs-lookup"><span data-stu-id="49ea0-120">Possible values are: `Boolean`, `Binary`, `Reference`, `Integer`, `String`.</span></span> <span data-ttu-id="49ea0-121">既定値は `String` です。</span><span class="sxs-lookup"><span data-stu-id="49ea0-121">Default is `String`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="49ea0-122">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="49ea0-122">JSON representation</span></span>

<span data-ttu-id="49ea0-123">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="49ea0-123">The following is a JSON representation of the resource.</span></span>

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
