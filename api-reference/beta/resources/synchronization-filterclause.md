---
title: filterClause リソースの種類
description: いずれかに候補オブジェクトが満たす必要があります、評価される 1 つのアサーションを表します`true`(オブジェクトでは、アサーションを満たしている) または`false`(オブジェクトでは、アサーションを満たしていません)。
localization_priority: Normal
ms.openlocfilehash: 62623cee5b2991acbe162561940adb1afd3574a1
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29523870"
---
# <a name="filterclause-resource-type"></a>filterClause リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

いずれかに候補オブジェクトが満たす必要があります、評価される 1 つのアサーションを表します`true`(オブジェクトでは、アサーションを満たしている) または`false`(オブジェクトでは、アサーションを満たしていません)。

## <a name="properties"></a>プロパティ
| プロパティ     | 型   |説明|
|:---------------|:--------|:----------|
|operatorName|String|ソースとターゲットのオペランドに適用する演算子の名前です。 サポートされている演算子のいずれかをする必要があります。 サポートされている演算子を検出することができます。|
|sourceOperandName|String|ソース オペランド (テスト中のオペランド) の名前です。 ソース オペランドの名前は、ソース オブジェクトの属性の名前のいずれかに一致しなければなりません。|
|targetOperand|[filterOperand](synchronization-filteroperand.md)|ソース オペランドを比較する値です。|

## <a name="json-representation"></a>JSON 表記

リソースの JSON 表記を次に示します。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.filterClause"
}-->

```json
{
  "operatorName": "String",
  "sourceOperandName": "String",
  "targetOperand": {"@odata.type": "microsoft.graph.filterOperand"}
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "filterClause resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/synchronization-filterclause.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
