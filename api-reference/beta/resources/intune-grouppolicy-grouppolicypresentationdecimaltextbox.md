---
title: groupPolicyPresentationDecimalTextBox リソースの種類
description: admx decimalTextBox 要素と admx の decimal 要素を表します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: c5ced3450144308aae2767ecca0438dc0914c04d
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/21/2019
ms.locfileid: "30160390"
---
# <a name="grouppolicypresentationdecimaltextbox-resource-type"></a>groupPolicyPresentationDecimalTextBox リソースの種類

> **重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

admx decimalTextBox 要素と admx の decimal 要素を表します。


[groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)から継承します。

## <a name="methods"></a>メソッド
|メソッド|戻り値の型|説明|
|:---|:---|:---|
|[リスト groupPolicyPresentationDecimalTextBoxes](../api/intune-grouppolicy-grouppolicypresentationdecimaltextbox-list.md)|[groupPolicyPresentationDecimalTextBox](../resources/intune-grouppolicy-grouppolicypresentationdecimaltextbox.md)コレクション|[groupPolicyPresentationDecimalTextBox](../resources/intune-grouppolicy-grouppolicypresentationdecimaltextbox.md)オブジェクトのプロパティとリレーションシップをリストします。|
|[groupPolicyPresentationDecimalTextBox を取得する](../api/intune-grouppolicy-grouppolicypresentationdecimaltextbox-get.md)|[groupPolicyPresentationDecimalTextBox](../resources/intune-grouppolicy-grouppolicypresentationdecimaltextbox.md)|[groupPolicyPresentationDecimalTextBox](../resources/intune-grouppolicy-grouppolicypresentationdecimaltextbox.md)オブジェクトのプロパティとリレーションシップを読み取ります。|
|[groupPolicyPresentationDecimalTextBox を作成する](../api/intune-grouppolicy-grouppolicypresentationdecimaltextbox-create.md)|[groupPolicyPresentationDecimalTextBox](../resources/intune-grouppolicy-grouppolicypresentationdecimaltextbox.md)|新しい[groupPolicyPresentationDecimalTextBox](../resources/intune-grouppolicy-grouppolicypresentationdecimaltextbox.md)オブジェクトを作成します。|
|[groupPolicyPresentationDecimalTextBox の削除](../api/intune-grouppolicy-grouppolicypresentationdecimaltextbox-delete.md)|なし|[groupPolicyPresentationDecimalTextBox](../resources/intune-grouppolicy-grouppolicypresentationdecimaltextbox.md)を削除します。|
|[groupPolicyPresentationDecimalTextBox の更新](../api/intune-grouppolicy-grouppolicypresentationdecimaltextbox-update.md)|[groupPolicyPresentationDecimalTextBox](../resources/intune-grouppolicy-grouppolicypresentationdecimaltextbox.md)|[groupPolicyPresentationDecimalTextBox](../resources/intune-grouppolicy-grouppolicypresentationdecimaltextbox.md)オブジェクトのプロパティを更新します。|

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|label|String|任意のプレゼンテーションエンティティのローカライズされたテキストラベル。 既定値は empty です。 [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)から継承します。|
|id|String|エンティティのキー。 [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)から継承します。|
|lastModifiedDateTime|DateTimeOffset|エンティティが最後に変更された日付と時刻。 [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)から継承します。|
|defaultValue|Int64|小数点のテキストボックスの初期値を指定する符号なし整数。 既定値は 1 です。|
|スピン|ブール値|true の場合はスピンコントロールを作成します。それ以外の場合は、数値を入力するためのテキストボックスを作成します。 既定値は true です。|
|spinstep|Int64|スピンコントロールの変更のインクリメントを指定する符号なし整数。 既定値は 1 です。|
|必須|ブール値|[パラメーター] ボックスに値を入力する必要があります。 既定値は false です。|
|minValue|Int64|最小許容値を指定する符号なし整数。 既定値は 0 です。|
|maxValue|Int64|最大許容値を指定する符号なし整数。 既定値は9999です。|

## <a name="relationships"></a>リレーションシップ
|リレーションシップ|型|説明|
|:---|:---|:---|
|definition|[grouppolicydefinition](../resources/intune-grouppolicy-grouppolicydefinition.md)|プレゼンテーションに関連付けられたグループポリシーの定義。 [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)から継承します。|

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




