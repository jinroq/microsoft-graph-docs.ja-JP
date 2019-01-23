---
title: groupPolicyPresentationValueList リソースの種類
description: エンティティでは、ポリシー定義のリスト ボックスのプレゼンテーションの名前/値ペアのコレクションを表します。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: c0a4ea5193edbf58a54da86f9478bfe9a51010d5
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29430451"
---
# <a name="grouppolicypresentationvaluelist-resource-type"></a>groupPolicyPresentationValueList リソースの種類

> **重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。 実稼働アプリケーションでこれらの API を使用することは、サポートされていません。

> **注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

エンティティでは、ポリシー定義のリスト ボックスのプレゼンテーションの名前/値ペアのコレクションを表します。


[GroupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)から継承します。

## <a name="methods"></a>メソッド
|メソッド|戻り値の型|説明|
|:---|:---|:---|
|[リスト groupPolicyPresentationValueLists](../api/intune-grouppolicy-grouppolicypresentationvaluelist-list.md)|[groupPolicyPresentationValueList](../resources/intune-grouppolicy-grouppolicypresentationvaluelist.md)コレクション|[GroupPolicyPresentationValueList](../resources/intune-grouppolicy-grouppolicypresentationvaluelist.md)オブジェクトのプロパティと関係を一覧表示します。|
|[GroupPolicyPresentationValueList を取得します。](../api/intune-grouppolicy-grouppolicypresentationvaluelist-get.md)|[groupPolicyPresentationValueList](../resources/intune-grouppolicy-grouppolicypresentationvaluelist.md)|[GroupPolicyPresentationValueList](../resources/intune-grouppolicy-grouppolicypresentationvaluelist.md)オブジェクトのプロパティと関係を参照してください。|
|[GroupPolicyPresentationValueList を作成します。](../api/intune-grouppolicy-grouppolicypresentationvaluelist-create.md)|[groupPolicyPresentationValueList](../resources/intune-grouppolicy-grouppolicypresentationvaluelist.md)|新しい[groupPolicyPresentationValueList](../resources/intune-grouppolicy-grouppolicypresentationvaluelist.md)オブジェクトを作成します。|
|[GroupPolicyPresentationValueList を削除します。](../api/intune-grouppolicy-grouppolicypresentationvaluelist-delete.md)|なし|の[groupPolicyPresentationValueList](../resources/intune-grouppolicy-grouppolicypresentationvaluelist.md)を削除します。|
|[GroupPolicyPresentationValueList を更新します。](../api/intune-grouppolicy-grouppolicypresentationvaluelist-update.md)|[groupPolicyPresentationValueList](../resources/intune-grouppolicy-grouppolicypresentationvaluelist.md)|[GroupPolicyPresentationValueList](../resources/intune-grouppolicy-grouppolicypresentationvaluelist.md)オブジェクトのプロパティを更新します。|

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|lastModifiedDateTime|DateTimeOffset|日付と時刻オブジェクトが最後に修正されました。 [GroupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)から継承されました。|
|createdDateTime|DateTimeOffset|日付と時刻オブジェクトを作成します。 [GroupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)から継承されました。|
|id|String|エンティティのキー。 [GroupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)から継承されました。|
|values|[keyValuePair](../resources/intune-shared-keyvaluepair.md) コレクション|関連付けられているプレゼンテーションのペアのリストです。|

## <a name="relationships"></a>リレーションシップ
|リレーションシップ|型|説明|
|:---|:---|:---|
|definitionValue|[groupPolicyDefinitionValue](../resources/intune-grouppolicy-grouppolicydefinitionvalue.md)|プレゼンテーションの値に関連付けられているグループ ポリシーの定義の値です。 [GroupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)から継承されました。|
|プレゼンテーション|[groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)|プレゼンテーションの値に関連付けられているグループ ポリシーのプレゼンテーションです。 [GroupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)から継承されました。|

## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.groupPolicyPresentationValueList"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.groupPolicyPresentationValueList",
  "lastModifiedDateTime": "String (timestamp)",
  "createdDateTime": "String (timestamp)",
  "id": "String (identifier)",
  "values": [
    {
      "@odata.type": "microsoft.graph.keyValuePair",
      "name": "String",
      "value": "String"
    }
  ]
}
```




