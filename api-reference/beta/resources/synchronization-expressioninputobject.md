---
title: expressionInputObject リソースの種類
description: 'テストの入力データとして使用するオブジェクトを表すとき、 [synchronizationSchema: parseExpression](../api/synchronization_synchronizationschema_parseexpression.md)式の評価を実行するアクションです。'
localization_priority: Normal
ms.openlocfilehash: acf0fa5125d863224de6df76d46109b9888f8ddf
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27820112"
---
# <a name="expressioninputobject-resource-type"></a><span data-ttu-id="7874a-103">expressionInputObject リソースの種類</span><span class="sxs-lookup"><span data-stu-id="7874a-103">expressionInputObject resource type</span></span>

> <span data-ttu-id="7874a-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="7874a-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="7874a-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="7874a-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="7874a-106">テストの入力データとして使用するオブジェクトを表すとき、 [synchronizationSchema: parseExpression](../api/synchronization_synchronizationschema_parseexpression.md)式の評価を実行するアクションです。</span><span class="sxs-lookup"><span data-stu-id="7874a-106">Represents an object to be used as input test data when the [synchronizationSchema: parseExpression](../api/synchronization_synchronizationschema_parseexpression.md) action performs an expression evaluation.</span></span>

## <a name="properties"></a><span data-ttu-id="7874a-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="7874a-107">Properties</span></span>
| <span data-ttu-id="7874a-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="7874a-108">Property</span></span>     | <span data-ttu-id="7874a-109">種類</span><span class="sxs-lookup"><span data-stu-id="7874a-109">Type</span></span>   |<span data-ttu-id="7874a-110">説明</span><span class="sxs-lookup"><span data-stu-id="7874a-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="7874a-111">definition</span><span class="sxs-lookup"><span data-stu-id="7874a-111">definition</span></span>|[<span data-ttu-id="7874a-112">objectDefinition</span><span class="sxs-lookup"><span data-stu-id="7874a-112">objectDefinition</span></span>](synchronization-objectdefinition.md)|<span data-ttu-id="7874a-113">テスト オブジェクトの定義です。</span><span class="sxs-lookup"><span data-stu-id="7874a-113">Definition of the test object.</span></span>|
|<span data-ttu-id="7874a-114">プロパティ</span><span class="sxs-lookup"><span data-stu-id="7874a-114">properties</span></span>|<span data-ttu-id="7874a-115">[stringKeyObjectValuePair](synchronization-stringkeyobjectvaluepair.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="7874a-115">[stringKeyObjectValuePair](synchronization-stringkeyobjectvaluepair.md) collection</span></span>|<span data-ttu-id="7874a-116">テスト オブジェクトのプロパティの値です。</span><span class="sxs-lookup"><span data-stu-id="7874a-116">Property values of the test object.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="7874a-117">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="7874a-117">JSON representation</span></span>

<span data-ttu-id="7874a-118">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="7874a-118">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.expressionInputObject"
}-->

```json
{
  "definition": {"@odata.type": "microsoft.graph.objectDefinition"},
  "properties": [{"@odata.type": "microsoft.graph.stringKeyObjectValuePair"}]
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "expressionInputObject resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
