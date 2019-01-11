---
title: parseExpressionResponse リソースの種類
description: '応答を表す、 [synchronizationSchema: parseExpression](../api/synchronization_synchronizationschema_parseexpression.md)アクション。'
localization_priority: Normal
ms.openlocfilehash: 550a46b0c27c2ca8d2d4c01baa975d8a204546f2
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27832950"
---
# <a name="parseexpressionresponse-resource-type"></a><span data-ttu-id="c4346-103">parseExpressionResponse リソースの種類</span><span class="sxs-lookup"><span data-stu-id="c4346-103">parseExpressionResponse resource type</span></span>

> <span data-ttu-id="c4346-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="c4346-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c4346-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c4346-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="c4346-106">応答を表す、 [synchronizationSchema: parseExpression](../api/synchronization_synchronizationschema_parseexpression.md)アクション。</span><span class="sxs-lookup"><span data-stu-id="c4346-106">Represents the response from the [synchronizationSchema: parseExpression](../api/synchronization_synchronizationschema_parseexpression.md) action.</span></span>

## <a name="properties"></a><span data-ttu-id="c4346-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="c4346-107">Properties</span></span>
| <span data-ttu-id="c4346-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="c4346-108">Property</span></span>     | <span data-ttu-id="c4346-109">種類</span><span class="sxs-lookup"><span data-stu-id="c4346-109">Type</span></span>   |<span data-ttu-id="c4346-110">説明</span><span class="sxs-lookup"><span data-stu-id="c4346-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c4346-111">エラー</span><span class="sxs-lookup"><span data-stu-id="c4346-111">error</span></span>|<span data-ttu-id="c4346-112">odata.error</span><span class="sxs-lookup"><span data-stu-id="c4346-112">odata.error</span></span>|<span data-ttu-id="c4346-113">エラーの詳細、式の評価でエラーが発生する場合。</span><span class="sxs-lookup"><span data-stu-id="c4346-113">Error details, if expression evaluation resulted in an error.</span></span>|
|<span data-ttu-id="c4346-114">evaluationResult</span><span class="sxs-lookup"><span data-stu-id="c4346-114">evaluationResult</span></span>|<span data-ttu-id="c4346-115">String コレクション</span><span class="sxs-lookup"><span data-stu-id="c4346-115">String collection</span></span>|<span data-ttu-id="c4346-116">式の評価によって生成された値のコレクションです。</span><span class="sxs-lookup"><span data-stu-id="c4346-116">A collection of values produced by the evaluation of the expression.</span></span>|
|<span data-ttu-id="c4346-117">evaluationSucceeded</span><span class="sxs-lookup"><span data-stu-id="c4346-117">evaluationSucceeded</span></span>|<span data-ttu-id="c4346-118">ブール型</span><span class="sxs-lookup"><span data-stu-id="c4346-118">Boolean</span></span>|<span data-ttu-id="c4346-119">`true`場合は、評価が正常に完了しました。</span><span class="sxs-lookup"><span data-stu-id="c4346-119">`true` if the evaluation was successful.</span></span>|
|<span data-ttu-id="c4346-120">parsedExpression</span><span class="sxs-lookup"><span data-stu-id="c4346-120">parsedExpression</span></span>|[<span data-ttu-id="c4346-121">attributeMappingSource</span><span class="sxs-lookup"><span data-stu-id="c4346-121">attributeMappingSource</span></span>](synchronization-attributemappingsource.md)|<span data-ttu-id="c4346-122">解析された式を表す[attributeMappingSource](synchronization-attributemappingsource.md)オブジェクト。</span><span class="sxs-lookup"><span data-stu-id="c4346-122">An [attributeMappingSource](synchronization-attributemappingsource.md) object representing the parsed expression.</span></span>|
|<span data-ttu-id="c4346-123">parsingSucceeded</span><span class="sxs-lookup"><span data-stu-id="c4346-123">parsingSucceeded</span></span>|<span data-ttu-id="c4346-124">ブール型</span><span class="sxs-lookup"><span data-stu-id="c4346-124">Boolean</span></span>|<span data-ttu-id="c4346-125">`true`場合は、式が正しく解析されました。</span><span class="sxs-lookup"><span data-stu-id="c4346-125">`true` if the expression was parsed successfully.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="c4346-126">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="c4346-126">JSON representation</span></span>

<span data-ttu-id="c4346-127">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="c4346-127">The following is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "parseExpressionResponse resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
