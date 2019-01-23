---
title: groupPolicyPresentationDecimalTextBox リソースの種類
description: ADMX decimalTextBox 要素と ADMX 10 進数の要素を表します。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 846b57e42a8f6d36049e57a589682fd652f960ae
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29431620"
---
# <a name="grouppolicypresentationdecimaltextbox-resource-type"></a>groupPolicyPresentationDecimalTextBox リソースの種類

> **重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。 実稼働アプリケーションでこれらの API を使用することは、サポートされていません。

> **注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

ADMX decimalTextBox 要素と ADMX 10 進数の要素を表します。


[GroupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)から継承します。

## <a name="methods"></a>メソッド
|メソッド|戻り値の型|説明|
|:---|:---|:---|
|[リスト groupPolicyPresentationDecimalTextBoxes](../api/intune-grouppolicy-grouppolicypresentationdecimaltextbox-list.md)|[groupPolicyPresentationDecimalTextBox](../resources/intune-grouppolicy-grouppolicypresentationdecimaltextbox.md)コレクション|[GroupPolicyPresentationDecimalTextBox](../resources/intune-grouppolicy-grouppolicypresentationdecimaltextbox.md)オブジェクトのプロパティと関係を一覧表示します。|
|[GroupPolicyPresentationDecimalTextBox を取得します。](../api/intune-grouppolicy-grouppolicypresentationdecimaltextbox-get.md)|[groupPolicyPresentationDecimalTextBox](../resources/intune-grouppolicy-grouppolicypresentationdecimaltextbox.md)|[GroupPolicyPresentationDecimalTextBox](../resources/intune-grouppolicy-grouppolicypresentationdecimaltextbox.md)オブジェクトのプロパティと関係を参照してください。|
|[GroupPolicyPresentationDecimalTextBox を作成します。](../api/intune-grouppolicy-grouppolicypresentationdecimaltextbox-create.md)|[groupPolicyPresentationDecimalTextBox](../resources/intune-grouppolicy-grouppolicypresentationdecimaltextbox.md)|新しい[groupPolicyPresentationDecimalTextBox](../resources/intune-grouppolicy-grouppolicypresentationdecimaltextbox.md)オブジェクトを作成します。|
|[GroupPolicyPresentationDecimalTextBox を削除します。](../api/intune-grouppolicy-grouppolicypresentationdecimaltextbox-delete.md)|なし|の[groupPolicyPresentationDecimalTextBox](../resources/intune-grouppolicy-grouppolicypresentationdecimaltextbox.md)を削除します。|
|[GroupPolicyPresentationDecimalTextBox を更新します。](../api/intune-grouppolicy-grouppolicypresentationdecimaltextbox-update.md)|[groupPolicyPresentationDecimalTextBox](../resources/intune-grouppolicy-grouppolicypresentationdecimaltextbox.md)|[GroupPolicyPresentationDecimalTextBox](../resources/intune-grouppolicy-grouppolicypresentationdecimaltextbox.md)オブジェクトのプロパティを更新します。|

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|label|String|プレゼンテーションの任意のエンティティのローカライズされたテキスト ラベルです。 既定値は空です。 [GroupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)から継承されました。|
|id|String|エンティティのキー。 [GroupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)から継承されました。|
|lastModifiedDateTime|DateTimeOffset|日付と時刻、エンティティが最後に修正されました。 [GroupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)から継承されました。|
|defaultValue|Int64|符号なし整数を 10 進数のテキスト ボックスの初期値を指定します。 既定値は 1 です。|
|スピン|Boolean|True の場合、スピン コントロールを作成します。それ以外の場合、数値入力用のテキスト ボックスを作成します。 既定値は、true を指定します。|
|spinStep|Int64|スピン コントロールの変更の増分値を指定する符号なし整数。 既定値は 1 です。|
|必須|Boolean|パラメーター] ボックスに値を入力するための要件です。 既定値は、false を指定します。|
|minValue|Int64|指定できる最小の値を指定する符号なし整数。 既定値は 0 です。|
|maxValue|Int64|最大許容値を指定する符号なし整数。 既定値は、9999 です。|

## <a name="relationships"></a>リレーションシップ
|リレーションシップ|型|説明|
|:---|:---|:---|
|definition|[groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md)|プレゼンテーションに関連付けられているグループ ポリシーの定義です。 [GroupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)から継承されました。|

## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.groupPolicyPresentationDecimalTextBox"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.groupPolicyPresentationDecimalTextBox",
  "label": "String",
  "id": "String (identifier)",
  "lastModifiedDateTime": "String (timestamp)",
  "defaultValue": 1024,
  "spin": true,
  "spinStep": 1024,
  "required": true,
  "minValue": 1024,
  "maxValue": 1024
}
```




