---
title: grouppolicypresentationcombobox リソースの種類
description: admx comboBox 要素と admx テキスト要素を表します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 83355dfc472945b0dd647622860d6304b01d716f
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/11/2019
ms.locfileid: "31801072"
---
# <a name="grouppolicypresentationcombobox-resource-type"></a>grouppolicypresentationcombobox リソースの種類

> **重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

admx comboBox 要素と admx テキスト要素を表します。


[groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)から継承します。

## <a name="methods"></a>メソッド
|メソッド|戻り値の型|説明|
|:---|:---|:---|
|[リスト grouppolicypresentationcomboboxes ボックス](../api/intune-grouppolicy-grouppolicypresentationcombobox-list.md)|[grouppolicypresentationcombobox](../resources/intune-grouppolicy-grouppolicypresentationcombobox.md)コレクション|[grouppolicypresentationcombobox](../resources/intune-grouppolicy-grouppolicypresentationcombobox.md)オブジェクトのプロパティとリレーションシップをリストします。|
|[grouppolicypresentationcombobox の取得](../api/intune-grouppolicy-grouppolicypresentationcombobox-get.md)|[grouppolicypresentationcombobox](../resources/intune-grouppolicy-grouppolicypresentationcombobox.md)|[grouppolicypresentationcombobox](../resources/intune-grouppolicy-grouppolicypresentationcombobox.md)オブジェクトのプロパティとリレーションシップを読み取ります。|
|[grouppolicypresentationcombobox の作成](../api/intune-grouppolicy-grouppolicypresentationcombobox-create.md)|[grouppolicypresentationcombobox](../resources/intune-grouppolicy-grouppolicypresentationcombobox.md)|新しい[grouppolicypresentationcombobox](../resources/intune-grouppolicy-grouppolicypresentationcombobox.md)オブジェクトを作成します。|
|[grouppolicypresentationcombobox の削除](../api/intune-grouppolicy-grouppolicypresentationcombobox-delete.md)|なし|[grouppolicypresentationcombobox](../resources/intune-grouppolicy-grouppolicypresentationcombobox.md)を削除します。|
|[grouppolicypresentationcombobox の更新](../api/intune-grouppolicy-grouppolicypresentationcombobox-update.md)|[grouppolicypresentationcombobox](../resources/intune-grouppolicy-grouppolicypresentationcombobox.md)|[grouppolicypresentationcombobox](../resources/intune-grouppolicy-grouppolicypresentationcombobox.md)オブジェクトのプロパティを更新します。|

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|label|文字列|任意のプレゼンテーションエンティティのローカライズされたテキストラベル。 既定値は空白です。 [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)から継承します。|
|id|String|エンティティのキー。 [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)から継承します。|
|lastModifiedDateTime|DateTimeOffset|エンティティが最後に変更された日付と時刻。 [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)から継承します。|
|defaultValue|文字列|コンボボックスに表示されるローカライズされた既定の文字列。 既定値は空白です。|
|助言|String コレクション|コンボボックスのドロップダウンリストに表示されるローカライズされた文字列。 既定値は空白です。|
|必須|Boolean|パラメーターに値を指定する必要があるかどうかを指定します。 既定値は false です。|
|maxLength|Int64|パラメーターのテキスト文字の最大数を指定する符号なし整数。 既定値は1023です。|

## <a name="relationships"></a>リレーションシップ
|リレーションシップ|型|説明|
|:---|:---|:---|
|definition|[grouppolicydefinition](../resources/intune-grouppolicy-grouppolicydefinition.md)|プレゼンテーションに関連付けられたグループポリシーの定義。 [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)から継承します。|

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





