---
title: groupPolicyPresentationComboBox リソースの種類
description: ADMX comboBox 要素と ADMX テキスト要素を表します。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 2225cda293bd2966dd39347dfe1ed03b2a4137c4
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29431617"
---
# <a name="grouppolicypresentationcombobox-resource-type"></a>groupPolicyPresentationComboBox リソースの種類

> **重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。 実稼働アプリケーションでこれらの API を使用することは、サポートされていません。

> **注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

ADMX comboBox 要素と ADMX テキスト要素を表します。


[GroupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)から継承します。

## <a name="methods"></a>メソッド
|メソッド|戻り値の型|説明|
|:---|:---|:---|
|[リスト groupPolicyPresentationComboBoxes](../api/intune-grouppolicy-grouppolicypresentationcombobox-list.md)|[groupPolicyPresentationComboBox](../resources/intune-grouppolicy-grouppolicypresentationcombobox.md)コレクション|[GroupPolicyPresentationComboBox](../resources/intune-grouppolicy-grouppolicypresentationcombobox.md)オブジェクトのプロパティと関係を一覧表示します。|
|[GroupPolicyPresentationComboBox を取得します。](../api/intune-grouppolicy-grouppolicypresentationcombobox-get.md)|[groupPolicyPresentationComboBox](../resources/intune-grouppolicy-grouppolicypresentationcombobox.md)|[GroupPolicyPresentationComboBox](../resources/intune-grouppolicy-grouppolicypresentationcombobox.md)オブジェクトのプロパティと関係を参照してください。|
|[GroupPolicyPresentationComboBox を作成します。](../api/intune-grouppolicy-grouppolicypresentationcombobox-create.md)|[groupPolicyPresentationComboBox](../resources/intune-grouppolicy-grouppolicypresentationcombobox.md)|新しい[groupPolicyPresentationComboBox](../resources/intune-grouppolicy-grouppolicypresentationcombobox.md)オブジェクトを作成します。|
|[GroupPolicyPresentationComboBox を削除します。](../api/intune-grouppolicy-grouppolicypresentationcombobox-delete.md)|なし|の[groupPolicyPresentationComboBox](../resources/intune-grouppolicy-grouppolicypresentationcombobox.md)を削除します。|
|[GroupPolicyPresentationComboBox を更新します。](../api/intune-grouppolicy-grouppolicypresentationcombobox-update.md)|[groupPolicyPresentationComboBox](../resources/intune-grouppolicy-grouppolicypresentationcombobox.md)|[GroupPolicyPresentationComboBox](../resources/intune-grouppolicy-grouppolicypresentationcombobox.md)オブジェクトのプロパティを更新します。|

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|label|String|プレゼンテーションの任意のエンティティのローカライズされたテキスト ラベルです。 既定値は空です。 [GroupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)から継承されました。|
|id|String|エンティティのキー。 [GroupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)から継承されました。|
|lastModifiedDateTime|DateTimeOffset|日付と時刻、エンティティが最後に修正されました。 [GroupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)から継承されました。|
|defaultValue|文字列|コンボ ボックスに表示される既定の文字列をローカライズします。 既定値は空です。|
|提案|String コレクション|ローカライズされた文字列がコンボ ボックスのドロップダウン リストに一覧表示します。 既定値は空です。|
|必須|Boolean|パラメーターの値を指定する必要があるかどうかを指定します。 既定値は、false を指定します。|
|maxLength|Int64|パラメーターのテキスト文字の最大数を指定する符号なし整数。 既定値は、1023 です。|

## <a name="relationships"></a>リレーションシップ
|リレーションシップ|型|説明|
|:---|:---|:---|
|definition|[groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md)|プレゼンテーションに関連付けられているグループ ポリシーの定義です。 [GroupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)から継承されました。|

## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.groupPolicyPresentationComboBox"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.groupPolicyPresentationComboBox",
  "label": "String",
  "id": "String (identifier)",
  "lastModifiedDateTime": "String (timestamp)",
  "defaultValue": "String",
  "suggestions": [
    "String"
  ],
  "required": true,
  "maxLength": 1024
}
```




