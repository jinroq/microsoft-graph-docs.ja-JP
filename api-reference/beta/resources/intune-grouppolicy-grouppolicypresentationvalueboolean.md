---
title: groupPolicyPresentationValueBoolean リソースの種類
description: エンティティでは、ポリシー定義のチェック ボックスをオンのプレゼンテーションのブール値を表します。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 248592bdb918064ffd84c8cf925658fa11fc40d0
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29430278"
---
# <a name="grouppolicypresentationvalueboolean-resource-type"></a>groupPolicyPresentationValueBoolean リソースの種類

> **重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。 実稼働アプリケーションでこれらの API を使用することは、サポートされていません。

> **注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

エンティティでは、ポリシー定義のチェック ボックスをオンのプレゼンテーションのブール値を表します。


[GroupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)から継承します。

## <a name="methods"></a>メソッド
|メソッド|戻り値の型|説明|
|:---|:---|:---|
|[リスト groupPolicyPresentationValueBooleans](../api/intune-grouppolicy-grouppolicypresentationvalueboolean-list.md)|[groupPolicyPresentationValueBoolean](../resources/intune-grouppolicy-grouppolicypresentationvalueboolean.md)コレクション|[GroupPolicyPresentationValueBoolean](../resources/intune-grouppolicy-grouppolicypresentationvalueboolean.md)オブジェクトのプロパティと関係を一覧表示します。|
|[GroupPolicyPresentationValueBoolean を取得します。](../api/intune-grouppolicy-grouppolicypresentationvalueboolean-get.md)|[groupPolicyPresentationValueBoolean](../resources/intune-grouppolicy-grouppolicypresentationvalueboolean.md)|[GroupPolicyPresentationValueBoolean](../resources/intune-grouppolicy-grouppolicypresentationvalueboolean.md)オブジェクトのプロパティと関係を参照してください。|
|[GroupPolicyPresentationValueBoolean を作成します。](../api/intune-grouppolicy-grouppolicypresentationvalueboolean-create.md)|[groupPolicyPresentationValueBoolean](../resources/intune-grouppolicy-grouppolicypresentationvalueboolean.md)|新しい[groupPolicyPresentationValueBoolean](../resources/intune-grouppolicy-grouppolicypresentationvalueboolean.md)オブジェクトを作成します。|
|[GroupPolicyPresentationValueBoolean を削除します。](../api/intune-grouppolicy-grouppolicypresentationvalueboolean-delete.md)|なし|の[groupPolicyPresentationValueBoolean](../resources/intune-grouppolicy-grouppolicypresentationvalueboolean.md)を削除します。|
|[GroupPolicyPresentationValueBoolean を更新します。](../api/intune-grouppolicy-grouppolicypresentationvalueboolean-update.md)|[groupPolicyPresentationValueBoolean](../resources/intune-grouppolicy-grouppolicypresentationvalueboolean.md)|[GroupPolicyPresentationValueBoolean](../resources/intune-grouppolicy-grouppolicypresentationvalueboolean.md)オブジェクトのプロパティを更新します。|

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|lastModifiedDateTime|DateTimeOffset|日付と時刻オブジェクトが最後に修正されました。 [GroupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)から継承されました。|
|createdDateTime|DateTimeOffset|日付と時刻オブジェクトを作成します。 [GroupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)から継承されました。|
|id|String|エンティティのキー。 [GroupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)から継承されました。|
|value|Boolean|関連付けられているプレゼンテーション用のブール値です。|

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
  "@odata.type": "microsoft.graph.groupPolicyPresentationValueBoolean"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.groupPolicyPresentationValueBoolean",
  "lastModifiedDateTime": "String (timestamp)",
  "createdDateTime": "String (timestamp)",
  "id": "String (identifier)",
  "value": true
}
```




