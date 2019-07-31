---
title: groupPolicyPresentationComboBox リソースの種類
description: ADMX comboBox 要素と ADMX テキスト要素を表します。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: af25adb116d08aa40a40f1cbb380decc9d69a3ac
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35998640"
---
# <a name="grouppolicypresentationcombobox-resource-type"></a>groupPolicyPresentationComboBox リソースの種類

> **重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

ADMX comboBox 要素と ADMX テキスト要素を表します。


[GroupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)から継承します。

## <a name="methods"></a>メソッド
|メソッド|戻り値の型|説明|
|:---|:---|:---|
|[リスト groupPolicyPresentationComboBoxes ボックス](../api/intune-grouppolicy-grouppolicypresentationcombobox-list.md)|[Grouppolicypresentationcombobox](../resources/intune-grouppolicy-grouppolicypresentationcombobox.md)コレクション|[Grouppolicypresentationcombobox](../resources/intune-grouppolicy-grouppolicypresentationcombobox.md)オブジェクトのプロパティとリレーションシップをリストします。|
|[GroupPolicyPresentationComboBox の取得](../api/intune-grouppolicy-grouppolicypresentationcombobox-get.md)|[groupPolicyPresentationComboBox](../resources/intune-grouppolicy-grouppolicypresentationcombobox.md)|[Grouppolicypresentationcombobox](../resources/intune-grouppolicy-grouppolicypresentationcombobox.md)オブジェクトのプロパティとリレーションシップを読み取ります。|
|[GroupPolicyPresentationComboBox の作成](../api/intune-grouppolicy-grouppolicypresentationcombobox-create.md)|[groupPolicyPresentationComboBox](../resources/intune-grouppolicy-grouppolicypresentationcombobox.md)|新しい[Grouppolicypresentationcombobox](../resources/intune-grouppolicy-grouppolicypresentationcombobox.md)オブジェクトを作成します。|
|[GroupPolicyPresentationComboBox の削除](../api/intune-grouppolicy-grouppolicypresentationcombobox-delete.md)|None|[Grouppolicypresentationcombobox](../resources/intune-grouppolicy-grouppolicypresentationcombobox.md)を削除します。|
|[GroupPolicyPresentationComboBox の更新](../api/intune-grouppolicy-grouppolicypresentationcombobox-update.md)|[groupPolicyPresentationComboBox](../resources/intune-grouppolicy-grouppolicypresentationcombobox.md)|[Grouppolicypresentationcombobox](../resources/intune-grouppolicy-grouppolicypresentationcombobox.md)オブジェクトのプロパティを更新します。|

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|label|String|任意のプレゼンテーションエンティティのローカライズされたテキストラベル。 既定値は空白です。 [GroupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)から継承します。|
|id|String|エンティティのキー。 [GroupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)から継承します。|
|lastModifiedDateTime|DateTimeOffset|エンティティが最後に変更された日付と時刻。 [GroupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)から継承します。|
|defaultValue|String|コンボボックスに表示されるローカライズされた既定の文字列。 既定値は空白です。|
|助言|文字列コレクション|コンボボックスのドロップダウンリストに表示されるローカライズされた文字列。 既定値は空白です。|
|必須|Boolean|パラメーターに値を指定する必要があるかどうかを指定します。 既定値は false です。|
|maxLength|Int64|パラメーターのテキスト文字の最大数を指定する符号なし整数。 既定値は1023です。|

## <a name="relationships"></a>リレーションシップ
|リレーションシップ|型|説明|
|:---|:---|:---|
|definition|[groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md)|プレゼンテーションに関連付けられたグループポリシーの定義。 [GroupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)から継承します。|

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





