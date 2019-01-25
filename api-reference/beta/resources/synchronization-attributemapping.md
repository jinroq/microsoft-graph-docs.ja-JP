---
title: attributeMapping リソースの種類
description: 特定のターゲット属性の値が同期中にフローは方法を定義します。
localization_priority: Normal
ms.openlocfilehash: 16235cce73a17b462f6f44aedf0c8759277983c1
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29509323"
---
# <a name="attributemapping-resource-type"></a>attributeMapping リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

特定のターゲット属性の値が同期中にフローは方法を定義します。

## <a name="properties"></a>プロパティ

| プロパティ                  | 型                      | 説明    |
|:--------------------------|:--------------------------|:---------------|
|defaultValue               | 文字列                    |既定値に、 **source**プロパティが評価された場合に使用する`null`。 省略可能。|
|exportMissingReferences    |String                     |内部使用のみ。|
|flowBehavior               |attributeFlowBehavior      |この属性をターゲット ディレクトリにエクスポートするときを定義します。 使用可能な値:`FlowWhenChanged`と`FlowAlways`。 既定値は `FlowWhenChanged` です。 |
|flowType                   |attributeFlowType          |ターゲット ディレクトリにこの属性を更新するときを定義します。 使用可能な値: `Always` (既定値)、 `ObjectAddOnly` (だけ新しいオブジェクトが作成された日時) `MultiValueAddOnly` (のみと変更は、値を追加する新しい複数値を持つ属性に)。 |
|matchingPriority           |Int32                      |0 よりも大きい場合、は、ソースとターゲットのディレクトリ間でオブジェクトの最初の一致を実行するこの属性が使用されます。 同期エンジンは、優先度と一致する最初の最小値を持つ属性を使用して一致するオブジェクトを検索しようとしています。 かどうか、次に一致する優先順位を持つ属性を使用してために、一致が見つかったか、これ以上の一致する属性が残っているまでです。 一致する属性としては、e メールのような一意の値があると予想される属性だけを使用してください。|
|source                     |[attributeMappingSource](synchronization-attributemappingsource.md)     | 定義の値がどのようにする必要があります抽出 (変換)、ソース オブジェクトからです。 |
|targetAttributeName        |String                     |対象のオブジェクトの属性の名前です。 |

## <a name="json-representation"></a>JSON 表記

リソースの JSON 表記を次に示します。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.attributeMapping"
}-->

```json
{
  "defaultValue": "String",
  "exportMissingReferences": true,
  "flowBehavior": "String",
  "flowType": "String",
  "matchingPriority": 1024,
  "source": {"@odata.type": "microsoft.graph.attributeMappingSource"},
  "targetAttributeName": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "attributeMapping resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/synchronization-attributemapping.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
