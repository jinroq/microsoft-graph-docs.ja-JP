---
title: Parseexpression Response リソースの種類
description: '[同期スキーマ: parseExpression](../api/synchronization_synchronizationschema_parseexpression.md)アクションからの応答を表します。'
localization_priority: Normal
doc_type: resourcePageType
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: a2c2bc0291eca7c04f246c6f62424b0bab10dced
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35964782"
---
# <a name="parseexpressionresponse-resource-type"></a><span data-ttu-id="3e93c-103">Parseexpression Response リソースの種類</span><span class="sxs-lookup"><span data-stu-id="3e93c-103">parseExpressionResponse resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3e93c-104">[Parseexpression](../api/synchronization-synchronizationschema-parseexpression.md)アクションからの応答を表します。</span><span class="sxs-lookup"><span data-stu-id="3e93c-104">Represents the response from the [parseExpression](../api/synchronization-synchronizationschema-parseexpression.md) action.</span></span>

## <a name="properties"></a><span data-ttu-id="3e93c-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="3e93c-105">Properties</span></span>
| <span data-ttu-id="3e93c-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="3e93c-106">Property</span></span>     | <span data-ttu-id="3e93c-107">型</span><span class="sxs-lookup"><span data-stu-id="3e93c-107">Type</span></span>   |<span data-ttu-id="3e93c-108">説明</span><span class="sxs-lookup"><span data-stu-id="3e93c-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="3e93c-109">エラー</span><span class="sxs-lookup"><span data-stu-id="3e93c-109">error</span></span>|<span data-ttu-id="3e93c-110">publicError</span><span class="sxs-lookup"><span data-stu-id="3e93c-110">publicError</span></span>|<span data-ttu-id="3e93c-111">エラーの詳細。式の評価結果でエラーが発生した場合。</span><span class="sxs-lookup"><span data-stu-id="3e93c-111">Error details, if expression evaluation resulted in an error.</span></span>|
|<span data-ttu-id="3e93c-112">evaluationResult</span><span class="sxs-lookup"><span data-stu-id="3e93c-112">evaluationResult</span></span>|<span data-ttu-id="3e93c-113">文字列コレクション</span><span class="sxs-lookup"><span data-stu-id="3e93c-113">String collection</span></span>|<span data-ttu-id="3e93c-114">式の評価によって生成された値のコレクション。</span><span class="sxs-lookup"><span data-stu-id="3e93c-114">A collection of values produced by the evaluation of the expression.</span></span>|
|<span data-ttu-id="3e93c-115">evaluationSucceeded</span><span class="sxs-lookup"><span data-stu-id="3e93c-115">evaluationSucceeded</span></span>|<span data-ttu-id="3e93c-116">Boolean</span><span class="sxs-lookup"><span data-stu-id="3e93c-116">Boolean</span></span>|<span data-ttu-id="3e93c-117">`true`評価が成功した場合。</span><span class="sxs-lookup"><span data-stu-id="3e93c-117">`true` if the evaluation was successful.</span></span>|
|<span data-ttu-id="3e93c-118">parsedExpression</span><span class="sxs-lookup"><span data-stu-id="3e93c-118">parsedExpression</span></span>|[<span data-ttu-id="3e93c-119">attributeMappingSource</span><span class="sxs-lookup"><span data-stu-id="3e93c-119">attributeMappingSource</span></span>](synchronization-attributemappingsource.md)|<span data-ttu-id="3e93c-120">解析された式を表す[attributeMappingSource](synchronization-attributemappingsource.md)オブジェクト。</span><span class="sxs-lookup"><span data-stu-id="3e93c-120">An [attributeMappingSource](synchronization-attributemappingsource.md) object representing the parsed expression.</span></span>|
|<span data-ttu-id="3e93c-121">parsingSucceeded</span><span class="sxs-lookup"><span data-stu-id="3e93c-121">parsingSucceeded</span></span>|<span data-ttu-id="3e93c-122">Boolean</span><span class="sxs-lookup"><span data-stu-id="3e93c-122">Boolean</span></span>|<span data-ttu-id="3e93c-123">`true`式が正常に解析された場合。</span><span class="sxs-lookup"><span data-stu-id="3e93c-123">`true` if the expression was parsed successfully.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="3e93c-124">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="3e93c-124">JSON representation</span></span>

<span data-ttu-id="3e93c-125">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="3e93c-125">The following is a JSON representation of the resource.</span></span>

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
  "suppressions": []
}
-->
