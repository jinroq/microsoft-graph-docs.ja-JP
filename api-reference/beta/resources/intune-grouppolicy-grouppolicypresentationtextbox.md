---
title: groupPolicyPresentationTextBox リソースの種類
description: ADMX textBox 要素と ADMX テキスト要素を表します。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: b5e5e034ce2cc0cd18aac27abf59730873e7998a
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29430380"
---
# <a name="grouppolicypresentationtextbox-resource-type"></a>groupPolicyPresentationTextBox リソースの種類

> **重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。 実稼働アプリケーションでこれらの API を使用することは、サポートされていません。

> **注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

ADMX textBox 要素と ADMX テキスト要素を表します。


[GroupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)から継承します。

## <a name="methods"></a>メソッド
|メソッド|戻り値の型|説明|
|:---|:---|:---|
|[リスト groupPolicyPresentationTextBoxes](../api/intune-grouppolicy-grouppolicypresentationtextbox-list.md)|[groupPolicyPresentationTextBox](../resources/intune-grouppolicy-grouppolicypresentationtextbox.md)コレクション|[GroupPolicyPresentationTextBox](../resources/intune-grouppolicy-grouppolicypresentationtextbox.md)オブジェクトのプロパティと関係を一覧表示します。|
|[GroupPolicyPresentationTextBox を取得します。](../api/intune-grouppolicy-grouppolicypresentationtextbox-get.md)|[groupPolicyPresentationTextBox](../resources/intune-grouppolicy-grouppolicypresentationtextbox.md)|[GroupPolicyPresentationTextBox](../resources/intune-grouppolicy-grouppolicypresentationtextbox.md)オブジェクトのプロパティと関係を参照してください。|
|[GroupPolicyPresentationTextBox を作成します。](../api/intune-grouppolicy-grouppolicypresentationtextbox-create.md)|[groupPolicyPresentationTextBox](../resources/intune-grouppolicy-grouppolicypresentationtextbox.md)|新しい[groupPolicyPresentationTextBox](../resources/intune-grouppolicy-grouppolicypresentationtextbox.md)オブジェクトを作成します。|
|[GroupPolicyPresentationTextBox を削除します。](../api/intune-grouppolicy-grouppolicypresentationtextbox-delete.md)|なし|の[groupPolicyPresentationTextBox](../resources/intune-grouppolicy-grouppolicypresentationtextbox.md)を削除します。|
|[GroupPolicyPresentationTextBox を更新します。](../api/intune-grouppolicy-grouppolicypresentationtextbox-update.md)|[groupPolicyPresentationTextBox](../resources/intune-grouppolicy-grouppolicypresentationtextbox.md)|[GroupPolicyPresentationTextBox](../resources/intune-grouppolicy-grouppolicypresentationtextbox.md)オブジェクトのプロパティを更新します。|

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|label|String|プレゼンテーションの任意のエンティティのローカライズされたテキスト ラベルです。 既定値は空です。 [GroupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)から継承されました。|
|id|String|エンティティのキー。 [GroupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)から継承されました。|
|lastModifiedDateTime|DateTimeOffset|日付と時刻、エンティティが最後に修正されました。 [GroupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)から継承されました。|
|defaultValue|文字列|テキスト ボックスに表示される既定の文字列をローカライズします。 既定値は空です。|
|必須|Boolean|テキスト ボックスに値を入力するための要件。 既定値は false です。|
|maxLength|Int64|テキスト文字の最大数を指定する符号なし整数。 1023 を既定値には。|

## <a name="relationships"></a>リレーションシップ
|リレーションシップ|型|説明|
|:---|:---|:---|
|definition|[groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md)|プレゼンテーションに関連付けられているグループ ポリシーの定義です。 [GroupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)から継承されました。|

## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.groupPolicyPresentationTextBox"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.groupPolicyPresentationTextBox",
  "label": "String",
  "id": "String (identifier)",
  "lastModifiedDateTime": "String (timestamp)",
  "defaultValue": "String",
  "required": true,
  "maxLength": 1024
}
```




