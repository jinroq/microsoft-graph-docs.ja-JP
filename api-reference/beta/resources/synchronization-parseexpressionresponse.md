---
title: parseExpressionResponse リソースの種類
description: '応答を表す、 [synchronizationSchema: parseExpression](../api/synchronization_synchronizationschema_parseexpression.md)アクション。'
localization_priority: Normal
ms.openlocfilehash: f8ea708468e1e580693b2bd0e6f0e7f3494996f0
ms.sourcegitcommit: d95f6d39a0479da6e531f3734c4029dc596b9a3f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/30/2019
ms.locfileid: "29641058"
---
# <a name="parseexpressionresponse-resource-type"></a><span data-ttu-id="079bc-103">parseExpressionResponse リソースの種類</span><span class="sxs-lookup"><span data-stu-id="079bc-103">parseExpressionResponse resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="079bc-104">応答を表す、 [synchronizationSchema: parseExpression](../api/synchronization_synchronizationschema_parseexpression.md)アクション。</span><span class="sxs-lookup"><span data-stu-id="079bc-104">Represents the response from the [synchronizationSchema: parseExpression](../api/synchronization_synchronizationschema_parseexpression.md) action.</span></span>

## <a name="properties"></a><span data-ttu-id="079bc-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="079bc-105">Properties</span></span>
| <span data-ttu-id="079bc-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="079bc-106">Property</span></span>     | <span data-ttu-id="079bc-107">型</span><span class="sxs-lookup"><span data-stu-id="079bc-107">Type</span></span>   |<span data-ttu-id="079bc-108">説明</span><span class="sxs-lookup"><span data-stu-id="079bc-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="079bc-109">エラー</span><span class="sxs-lookup"><span data-stu-id="079bc-109">error</span></span>|<span data-ttu-id="079bc-110">odata.error</span><span class="sxs-lookup"><span data-stu-id="079bc-110">odata.error</span></span>|<span data-ttu-id="079bc-111">エラーの詳細、式の評価でエラーが発生する場合。</span><span class="sxs-lookup"><span data-stu-id="079bc-111">Error details, if expression evaluation resulted in an error.</span></span>|
|<span data-ttu-id="079bc-112">evaluationResult</span><span class="sxs-lookup"><span data-stu-id="079bc-112">evaluationResult</span></span>|<span data-ttu-id="079bc-113">String コレクション</span><span class="sxs-lookup"><span data-stu-id="079bc-113">String collection</span></span>|<span data-ttu-id="079bc-114">式の評価によって生成された値のコレクションです。</span><span class="sxs-lookup"><span data-stu-id="079bc-114">A collection of values produced by the evaluation of the expression.</span></span>|
|<span data-ttu-id="079bc-115">evaluationSucceeded</span><span class="sxs-lookup"><span data-stu-id="079bc-115">evaluationSucceeded</span></span>|<span data-ttu-id="079bc-116">Boolean</span><span class="sxs-lookup"><span data-stu-id="079bc-116">Boolean</span></span>|<span data-ttu-id="079bc-117">`true`場合は、評価が正常に完了しました。</span><span class="sxs-lookup"><span data-stu-id="079bc-117">`true` if the evaluation was successful.</span></span>|
|<span data-ttu-id="079bc-118">parsedExpression</span><span class="sxs-lookup"><span data-stu-id="079bc-118">parsedExpression</span></span>|[<span data-ttu-id="079bc-119">attributeMappingSource</span><span class="sxs-lookup"><span data-stu-id="079bc-119">attributeMappingSource</span></span>](synchronization-attributemappingsource.md)|<span data-ttu-id="079bc-120">解析された式を表す[attributeMappingSource](synchronization-attributemappingsource.md)オブジェクト。</span><span class="sxs-lookup"><span data-stu-id="079bc-120">An [attributeMappingSource](synchronization-attributemappingsource.md) object representing the parsed expression.</span></span>|
|<span data-ttu-id="079bc-121">parsingSucceeded</span><span class="sxs-lookup"><span data-stu-id="079bc-121">parsingSucceeded</span></span>|<span data-ttu-id="079bc-122">Boolean</span><span class="sxs-lookup"><span data-stu-id="079bc-122">Boolean</span></span>|<span data-ttu-id="079bc-123">`true`場合は、式が正しく解析されました。</span><span class="sxs-lookup"><span data-stu-id="079bc-123">`true` if the expression was parsed successfully.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="079bc-124">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="079bc-124">JSON representation</span></span>

<span data-ttu-id="079bc-125">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="079bc-125">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.parseExpressionResponse"
}-->

```json
{
  "error": {"@odata.type": "microsoft.graph.publicError"},
  "evaluationResult": ["String"],
  "evaluationSucceeded": true,
  "parsedExpression": {"@odata.type": "microsoft.graph.attributeMappingSource"},
  "parsingSucceeded": true
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "parseExpressionResponse resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/synchronization-parseexpressionresponse.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
