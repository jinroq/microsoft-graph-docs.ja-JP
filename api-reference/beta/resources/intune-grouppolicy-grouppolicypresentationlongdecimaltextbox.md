---
title: groupPolicyPresentationLongDecimalTextBox リソースの種類
description: ADMX longDecimalTextBox 要素と ADMX longDecimal 要素を表します。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: faddc0c6475a5f78a0f9362affbe32294b3b05be
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29430383"
---
# <a name="grouppolicypresentationlongdecimaltextbox-resource-type"></a>groupPolicyPresentationLongDecimalTextBox リソースの種類

> **重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。 実稼働アプリケーションでこれらの API を使用することは、サポートされていません。

> **注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

ADMX longDecimalTextBox 要素と ADMX longDecimal 要素を表します。


[GroupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)から継承します。

## <a name="methods"></a>メソッド
|メソッド|戻り値の型|説明|
|:---|:---|:---|
|[リスト groupPolicyPresentationLongDecimalTextBoxes](../api/intune-grouppolicy-grouppolicypresentationlongdecimaltextbox-list.md)|[groupPolicyPresentationLongDecimalTextBox](../resources/intune-grouppolicy-grouppolicypresentationlongdecimaltextbox.md)コレクション|[GroupPolicyPresentationLongDecimalTextBox](../resources/intune-grouppolicy-grouppolicypresentationlongdecimaltextbox.md)オブジェクトのプロパティと関係を一覧表示します。|
|[GroupPolicyPresentationLongDecimalTextBox を取得します。](../api/intune-grouppolicy-grouppolicypresentationlongdecimaltextbox-get.md)|[groupPolicyPresentationLongDecimalTextBox](../resources/intune-grouppolicy-grouppolicypresentationlongdecimaltextbox.md)|[GroupPolicyPresentationLongDecimalTextBox](../resources/intune-grouppolicy-grouppolicypresentationlongdecimaltextbox.md)オブジェクトのプロパティと関係を参照してください。|
|[GroupPolicyPresentationLongDecimalTextBox を作成します。](../api/intune-grouppolicy-grouppolicypresentationlongdecimaltextbox-create.md)|[groupPolicyPresentationLongDecimalTextBox](../resources/intune-grouppolicy-grouppolicypresentationlongdecimaltextbox.md)|新しい[groupPolicyPresentationLongDecimalTextBox](../resources/intune-grouppolicy-grouppolicypresentationlongdecimaltextbox.md)オブジェクトを作成します。|
|[GroupPolicyPresentationLongDecimalTextBox を削除します。](../api/intune-grouppolicy-grouppolicypresentationlongdecimaltextbox-delete.md)|なし|の[groupPolicyPresentationLongDecimalTextBox](../resources/intune-grouppolicy-grouppolicypresentationlongdecimaltextbox.md)を削除します。|
|[GroupPolicyPresentationLongDecimalTextBox を更新します。](../api/intune-grouppolicy-grouppolicypresentationlongdecimaltextbox-update.md)|[groupPolicyPresentationLongDecimalTextBox](../resources/intune-grouppolicy-grouppolicypresentationlongdecimaltextbox.md)|[GroupPolicyPresentationLongDecimalTextBox](../resources/intune-grouppolicy-grouppolicypresentationlongdecimaltextbox.md)オブジェクトのプロパティを更新します。|

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
|minValue|Int64|符号なし、許容される最小値を指定する long です。 既定値は 0 です。|
|maxValue|Int64|符号なしの値の許容最大値を指定する long です。 既定値は、9999 です。|

## <a name="relationships"></a>リレーションシップ
|リレーションシップ|型|説明|
|:---|:---|:---|
|definition|[groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md)|プレゼンテーションに関連付けられているグループ ポリシーの定義です。 [GroupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)から継承されました。|

## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.groupPolicyPresentationLongDecimalTextBox"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.groupPolicyPresentationLongDecimalTextBox",
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




