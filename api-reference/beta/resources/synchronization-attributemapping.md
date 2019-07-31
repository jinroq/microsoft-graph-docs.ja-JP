---
title: attributeMapping リソースの種類
description: 特定のターゲット属性の値が同期中にどのように流れるかを定義します。
localization_priority: Normal
doc_type: resourcePageType
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 09ed298022e687354f7fa9905ee25f5c38f2fdfa
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35964837"
---
# <a name="attributemapping-resource-type"></a>attributeMapping リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

特定のターゲット属性の値が同期中にどのように流れるかを定義します。

## <a name="properties"></a>プロパティ

| プロパティ                  | 型                      | 説明    |
|:--------------------------|:--------------------------|:---------------|
|defaultValue               | String                    |**Source**プロパティがに`null`評価された場合に使用される既定値です。 省略可能。|
|exportMissingReferences    |String                     |内部使用のために用意されています。|
|flowBehavior               |attributeFlowBehavior      |この属性をターゲットディレクトリにエクスポートするタイミングを定義します。 可能な値は`FlowWhenChanged` 、 `FlowAlways`とです。 既定値は `FlowWhenChanged` です。 |
|flowType                   |attributeFlowType          |この属性をターゲットディレクトリでいつ更新する必要があるかを定義します。 可能な値は`Always`次のとおりです`ObjectAddOnly` (既定値)。 (新しいオブジェクトが`MultiValueAddOnly`作成された場合のみ)、(変更によって新しい値が複数値属性に追加されている場合のみ)。 |
|matchingPriority           |Int32                      |0より大きい場合は、この属性を使用して、ソースディレクトリとターゲットディレクトリの間でオブジェクトの初期一致を実行します。 同期エンジンは、一致する優先度の値が最も小さい属性を使用して、一致するオブジェクトを検索します。 見つからない場合は、次に一致する優先度の属性が使用され、一致が見つかるまで、またはそれ以上一致する属性が残っていないことを示します。 電子メールなどの一意の値を持つことが予想される属性のみを一致属性として使用する必要があります。|
|source                     |[attributeMappingSource](synchronization-attributemappingsource.md)     | ソースオブジェクトから値を抽出 (変換) する方法を定義します。 |
|targetAttributeName        |String                     |ターゲットオブジェクトの属性の名前。 |

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
  "suppressions": []
}
-->
