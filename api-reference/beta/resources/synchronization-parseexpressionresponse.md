---
title: parseexpression response リソースの種類
description: '[同期スキーマ: parseexpression](../api/synchronization_synchronizationschema_parseexpression.md)アクションからの応答を表します。'
localization_priority: Normal
ms.openlocfilehash: 14fcce13d2e78b99a8712c51768e6a94928fa07f
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33345555"
---
# <a name="parseexpressionresponse-resource-type"></a><span data-ttu-id="0b567-103">parseexpression response リソースの種類</span><span class="sxs-lookup"><span data-stu-id="0b567-103">parseExpressionResponse resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0b567-104">[parseexpression](../api/synchronization-synchronizationschema-parseexpression.md)アクションからの応答を表します。</span><span class="sxs-lookup"><span data-stu-id="0b567-104">Represents the response from the [parseExpression](../api/synchronization-synchronizationschema-parseexpression.md) action.</span></span>

## <a name="properties"></a><span data-ttu-id="0b567-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="0b567-105">Properties</span></span>
| <span data-ttu-id="0b567-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="0b567-106">Property</span></span>     | <span data-ttu-id="0b567-107">型</span><span class="sxs-lookup"><span data-stu-id="0b567-107">Type</span></span>   |<span data-ttu-id="0b567-108">説明</span><span class="sxs-lookup"><span data-stu-id="0b567-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0b567-109">エラー</span><span class="sxs-lookup"><span data-stu-id="0b567-109">error</span></span>|<span data-ttu-id="0b567-110">publicerror</span><span class="sxs-lookup"><span data-stu-id="0b567-110">publicError</span></span>|<span data-ttu-id="0b567-111">エラーの詳細。式の評価結果でエラーが発生した場合。</span><span class="sxs-lookup"><span data-stu-id="0b567-111">Error details, if expression evaluation resulted in an error.</span></span>|
|<span data-ttu-id="0b567-112">evaluationresult</span><span class="sxs-lookup"><span data-stu-id="0b567-112">evaluationResult</span></span>|<span data-ttu-id="0b567-113">String collection</span><span class="sxs-lookup"><span data-stu-id="0b567-113">String collection</span></span>|<span data-ttu-id="0b567-114">式の評価によって生成された値のコレクション。</span><span class="sxs-lookup"><span data-stu-id="0b567-114">A collection of values produced by the evaluation of the expression.</span></span>|
|<span data-ttu-id="0b567-115">evaluationsucceeded</span><span class="sxs-lookup"><span data-stu-id="0b567-115">evaluationSucceeded</span></span>|<span data-ttu-id="0b567-116">Boolean</span><span class="sxs-lookup"><span data-stu-id="0b567-116">Boolean</span></span>|<span data-ttu-id="0b567-117">`true`評価が成功した場合。</span><span class="sxs-lookup"><span data-stu-id="0b567-117">`true` if the evaluation was successful.</span></span>|
|<span data-ttu-id="0b567-118">parsedExpression</span><span class="sxs-lookup"><span data-stu-id="0b567-118">parsedExpression</span></span>|[<span data-ttu-id="0b567-119">attributeMappingSource</span><span class="sxs-lookup"><span data-stu-id="0b567-119">attributeMappingSource</span></span>](synchronization-attributemappingsource.md)|<span data-ttu-id="0b567-120">解析された式を表す[attributeMappingSource](synchronization-attributemappingsource.md)オブジェクト。</span><span class="sxs-lookup"><span data-stu-id="0b567-120">An [attributeMappingSource](synchronization-attributemappingsource.md) object representing the parsed expression.</span></span>|
|<span data-ttu-id="0b567-121">parsingsucceeded</span><span class="sxs-lookup"><span data-stu-id="0b567-121">parsingSucceeded</span></span>|<span data-ttu-id="0b567-122">Boolean</span><span class="sxs-lookup"><span data-stu-id="0b567-122">Boolean</span></span>|<span data-ttu-id="0b567-123">`true`式が正常に解析された場合。</span><span class="sxs-lookup"><span data-stu-id="0b567-123">`true` if the expression was parsed successfully.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="0b567-124">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="0b567-124">JSON representation</span></span>

<span data-ttu-id="0b567-125">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="0b567-125">The following is a JSON representation of the resource.</span></span>

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
