---
title: 式 Inputobject リソースの種類
description: '[同期スキーマ: parseexpression](../api/synchronization_synchronizationschema_parseexpression.md)アクションが式評価を実行するときに入力テストデータとして使用するオブジェクトを表します。'
localization_priority: Normal
doc_type: resourcePageType
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 113c38e540b8c41fb3d3156b27f6f5e1f1df42f2
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36007950"
---
# <a name="expressioninputobject-resource-type"></a><span data-ttu-id="99146-103">式 Inputobject リソースの種類</span><span class="sxs-lookup"><span data-stu-id="99146-103">expressionInputObject resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="99146-104">[Parseexpression](../api/synchronization-synchronizationschema-parseexpression.md)アクションが式の評価を実行するときに入力テストデータとして使用するオブジェクトを表します。</span><span class="sxs-lookup"><span data-stu-id="99146-104">Represents an object to be used as input test data when the [parseExpression](../api/synchronization-synchronizationschema-parseexpression.md) action performs an expression evaluation.</span></span>

## <a name="properties"></a><span data-ttu-id="99146-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="99146-105">Properties</span></span>
| <span data-ttu-id="99146-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="99146-106">Property</span></span>     | <span data-ttu-id="99146-107">型</span><span class="sxs-lookup"><span data-stu-id="99146-107">Type</span></span>   |<span data-ttu-id="99146-108">説明</span><span class="sxs-lookup"><span data-stu-id="99146-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="99146-109">definition</span><span class="sxs-lookup"><span data-stu-id="99146-109">definition</span></span>|[<span data-ttu-id="99146-110">objectDefinition</span><span class="sxs-lookup"><span data-stu-id="99146-110">objectDefinition</span></span>](synchronization-objectdefinition.md)|<span data-ttu-id="99146-111">Test オブジェクトの定義。</span><span class="sxs-lookup"><span data-stu-id="99146-111">Definition of the test object.</span></span>|
|<span data-ttu-id="99146-112">properties</span><span class="sxs-lookup"><span data-stu-id="99146-112">properties</span></span>|<span data-ttu-id="99146-113">[Stringkeyobjectvaluepair](synchronization-stringkeyobjectvaluepair.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="99146-113">[stringKeyObjectValuePair](synchronization-stringkeyobjectvaluepair.md) collection</span></span>|<span data-ttu-id="99146-114">Test オブジェクトのプロパティ値を指定します。</span><span class="sxs-lookup"><span data-stu-id="99146-114">Property values of the test object.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="99146-115">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="99146-115">JSON representation</span></span>

<span data-ttu-id="99146-116">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="99146-116">The following is a JSON representation of the resource.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "expressionInputObject resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
