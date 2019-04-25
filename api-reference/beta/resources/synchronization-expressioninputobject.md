---
title: 式 inputobject リソースの種類
description: '[同期スキーマ: parseexpression](../api/synchronization_synchronizationschema_parseexpression.md)アクションが式評価を実行するときに入力テストデータとして使用するオブジェクトを表します。'
localization_priority: Normal
ms.openlocfilehash: 3e631102505408b955404c4badb33b98f314236f
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32582103"
---
# <a name="expressioninputobject-resource-type"></a><span data-ttu-id="be987-103">式 inputobject リソースの種類</span><span class="sxs-lookup"><span data-stu-id="be987-103">expressionInputObject resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="be987-104">[同期スキーマ: parseexpression](../api/synchronization_synchronizationschema_parseexpression.md)アクションが式評価を実行するときに入力テストデータとして使用するオブジェクトを表します。</span><span class="sxs-lookup"><span data-stu-id="be987-104">Represents an object to be used as input test data when the [synchronizationSchema: parseExpression](../api/synchronization_synchronizationschema_parseexpression.md) action performs an expression evaluation.</span></span>

## <a name="properties"></a><span data-ttu-id="be987-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="be987-105">Properties</span></span>
| <span data-ttu-id="be987-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="be987-106">Property</span></span>     | <span data-ttu-id="be987-107">型</span><span class="sxs-lookup"><span data-stu-id="be987-107">Type</span></span>   |<span data-ttu-id="be987-108">説明</span><span class="sxs-lookup"><span data-stu-id="be987-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="be987-109">definition</span><span class="sxs-lookup"><span data-stu-id="be987-109">definition</span></span>|[<span data-ttu-id="be987-110">objectdefinition</span><span class="sxs-lookup"><span data-stu-id="be987-110">objectDefinition</span></span>](synchronization-objectdefinition.md)|<span data-ttu-id="be987-111">test オブジェクトの定義。</span><span class="sxs-lookup"><span data-stu-id="be987-111">Definition of the test object.</span></span>|
|<span data-ttu-id="be987-112">プロパティ</span><span class="sxs-lookup"><span data-stu-id="be987-112">properties</span></span>|<span data-ttu-id="be987-113">[stringkeyobjectvaluepair](synchronization-stringkeyobjectvaluepair.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="be987-113">[stringKeyObjectValuePair](synchronization-stringkeyobjectvaluepair.md) collection</span></span>|<span data-ttu-id="be987-114">test オブジェクトのプロパティ値を指定します。</span><span class="sxs-lookup"><span data-stu-id="be987-114">Property values of the test object.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="be987-115">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="be987-115">JSON representation</span></span>

<span data-ttu-id="be987-116">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="be987-116">The following is a JSON representation of the resource.</span></span>

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
  "suppressions": [
    "Error: /api-reference/beta/resources/synchronization-expressioninputobject.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
