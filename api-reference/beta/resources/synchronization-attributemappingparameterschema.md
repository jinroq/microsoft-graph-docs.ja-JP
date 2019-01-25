---
title: attributeMappingParameterSchema リソースの種類
description: AttributeMappingFunctionSchema で使用される 1 つのパラメーターについて説明します。
localization_priority: Normal
ms.openlocfilehash: bad88fc58dcc529f086a3e3870e0bb10a9d23329
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29529951"
---
# <a name="attributemappingparameterschema-resource-type"></a><span data-ttu-id="08b07-103">attributeMappingParameterSchema リソースの種類</span><span class="sxs-lookup"><span data-stu-id="08b07-103">attributeMappingParameterSchema resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="08b07-104">[AttributeMappingFunctionSchema](../resources/synchronization-attributemappingfunctionschema.md)で使用される 1 つのパラメーターについて説明します。</span><span class="sxs-lookup"><span data-stu-id="08b07-104">Describes a single parameter used in an [attributeMappingFunctionSchema](../resources/synchronization-attributemappingfunctionschema.md).</span></span>

## <a name="properties"></a><span data-ttu-id="08b07-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="08b07-105">Properties</span></span>

| <span data-ttu-id="08b07-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="08b07-106">Property</span></span>                   | <span data-ttu-id="08b07-107">型</span><span class="sxs-lookup"><span data-stu-id="08b07-107">Type</span></span>                      | <span data-ttu-id="08b07-108">説明</span><span class="sxs-lookup"><span data-stu-id="08b07-108">Description</span></span>    |
|:---------------------------|:-------------------------|:---------------|
|<span data-ttu-id="08b07-109">allowMultipleOccurrences</span><span class="sxs-lookup"><span data-stu-id="08b07-109">allowMultipleOccurrences</span></span>    |<span data-ttu-id="08b07-110">ブール値</span><span class="sxs-lookup"><span data-stu-id="08b07-110">Boolean</span></span>                   |<span data-ttu-id="08b07-111">複数回指定したパラメーターを提供することができます (などの文字列を複数の入力、`Concatenate(string,string,...)`関数)。</span><span class="sxs-lookup"><span data-stu-id="08b07-111">The given parameter can be provided multiple times (for example, multiple input strings in the `Concatenate(string,string,...)` function).</span></span> |
|<span data-ttu-id="08b07-112">name</span><span class="sxs-lookup"><span data-stu-id="08b07-112">name</span></span>                        |<span data-ttu-id="08b07-113">String</span><span class="sxs-lookup"><span data-stu-id="08b07-113">String</span></span>                    |<span data-ttu-id="08b07-114">パラメーター名</span><span class="sxs-lookup"><span data-stu-id="08b07-114">Parameter name.</span></span> |
|<span data-ttu-id="08b07-115">必須</span><span class="sxs-lookup"><span data-stu-id="08b07-115">required</span></span>                    |<span data-ttu-id="08b07-116">ブール値</span><span class="sxs-lookup"><span data-stu-id="08b07-116">Boolean</span></span>                   |<span data-ttu-id="08b07-117">`true`場合は、パラメーターが必要です。それ以外の場合`false`。</span><span class="sxs-lookup"><span data-stu-id="08b07-117">`true` if the parameter is required; otherwise `false`.</span></span> |
|<span data-ttu-id="08b07-118">type</span><span class="sxs-lookup"><span data-stu-id="08b07-118">type</span></span>                        |<span data-ttu-id="08b07-119">String</span><span class="sxs-lookup"><span data-stu-id="08b07-119">String</span></span>                    |<span data-ttu-id="08b07-120">可能な値は、`Boolean`、`Binary`、`Reference`、`Integer`、`String` です。</span><span class="sxs-lookup"><span data-stu-id="08b07-120">Possible values are: `Boolean`, `Binary`, `Reference`, `Integer`, `String`.</span></span> <span data-ttu-id="08b07-121">既定値は `String` です。</span><span class="sxs-lookup"><span data-stu-id="08b07-121">Default is `String`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="08b07-122">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="08b07-122">JSON representation</span></span>

<span data-ttu-id="08b07-123">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="08b07-123">The following is a JSON representation of the resource.</span></span>

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
  "suppressions": [
    "Error: /api-reference/beta/resources/synchronization-attributemappingparameterschema.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
