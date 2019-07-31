---
title: attributeMappingParameterSchema リソースの種類
description: AttributeMappingFunctionSchema で使用される1つのパラメーターを記述します。
localization_priority: Normal
doc_type: resourcePageType
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 14be19389d7c84c3e1a212239f2ba9e414927254
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35964843"
---
# <a name="attributemappingparameterschema-resource-type"></a><span data-ttu-id="dc2c9-103">attributeMappingParameterSchema リソースの種類</span><span class="sxs-lookup"><span data-stu-id="dc2c9-103">attributeMappingParameterSchema resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="dc2c9-104">[AttributeMappingFunctionSchema](../resources/synchronization-attributemappingfunctionschema.md)で使用される1つのパラメーターを記述します。</span><span class="sxs-lookup"><span data-stu-id="dc2c9-104">Describes a single parameter used in an [attributeMappingFunctionSchema](../resources/synchronization-attributemappingfunctionschema.md).</span></span>

## <a name="properties"></a><span data-ttu-id="dc2c9-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="dc2c9-105">Properties</span></span>

| <span data-ttu-id="dc2c9-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="dc2c9-106">Property</span></span>                   | <span data-ttu-id="dc2c9-107">型</span><span class="sxs-lookup"><span data-stu-id="dc2c9-107">Type</span></span>                      | <span data-ttu-id="dc2c9-108">説明</span><span class="sxs-lookup"><span data-stu-id="dc2c9-108">Description</span></span>    |
|:---------------------------|:-------------------------|:---------------|
|<span data-ttu-id="dc2c9-109">Allow多重オカレンス</span><span class="sxs-lookup"><span data-stu-id="dc2c9-109">allowMultipleOccurrences</span></span>    |<span data-ttu-id="dc2c9-110">Boolean</span><span class="sxs-lookup"><span data-stu-id="dc2c9-110">Boolean</span></span>                   |<span data-ttu-id="dc2c9-111">指定されたパラメーターは、複数回指定できます (たとえば、 `Concatenate(string,string,...)`関数内の複数の入力文字列)。</span><span class="sxs-lookup"><span data-stu-id="dc2c9-111">The given parameter can be provided multiple times (for example, multiple input strings in the `Concatenate(string,string,...)` function).</span></span> |
|<span data-ttu-id="dc2c9-112">name</span><span class="sxs-lookup"><span data-stu-id="dc2c9-112">name</span></span>                        |<span data-ttu-id="dc2c9-113">String</span><span class="sxs-lookup"><span data-stu-id="dc2c9-113">String</span></span>                    |<span data-ttu-id="dc2c9-114">パラメーター名。</span><span class="sxs-lookup"><span data-stu-id="dc2c9-114">Parameter name.</span></span> |
|<span data-ttu-id="dc2c9-115">必須</span><span class="sxs-lookup"><span data-stu-id="dc2c9-115">required</span></span>                    |<span data-ttu-id="dc2c9-116">Boolean</span><span class="sxs-lookup"><span data-stu-id="dc2c9-116">Boolean</span></span>                   |<span data-ttu-id="dc2c9-117">`true`パラメーターが必要な場合は、それ`false`以外の場合は。</span><span class="sxs-lookup"><span data-stu-id="dc2c9-117">`true` if the parameter is required; otherwise `false`.</span></span> |
|<span data-ttu-id="dc2c9-118">type</span><span class="sxs-lookup"><span data-stu-id="dc2c9-118">type</span></span>                        |<span data-ttu-id="dc2c9-119">String</span><span class="sxs-lookup"><span data-stu-id="dc2c9-119">String</span></span>                    |<span data-ttu-id="dc2c9-120">使用可能な値は、`Boolean`、`Binary`、`Reference`、`Integer`、`String` です。</span><span class="sxs-lookup"><span data-stu-id="dc2c9-120">Possible values are: `Boolean`, `Binary`, `Reference`, `Integer`, `String`.</span></span> <span data-ttu-id="dc2c9-121">既定値は `String` です。</span><span class="sxs-lookup"><span data-stu-id="dc2c9-121">Default is `String`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="dc2c9-122">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="dc2c9-122">JSON representation</span></span>

<span data-ttu-id="dc2c9-123">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="dc2c9-123">The following is a JSON representation of the resource.</span></span>

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
