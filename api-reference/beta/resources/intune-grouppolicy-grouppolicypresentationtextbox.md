---
title: grouppolicypresentationtextbox リソースの種類
description: admx textBox 要素と admx テキスト要素を表します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: c90355aa9c355b586b060e0e37ddeab8467e5964
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/21/2019
ms.locfileid: "30155581"
---
# <a name="grouppolicypresentationtextbox-resource-type"></a>grouppolicypresentationtextbox リソースの種類

> **重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

admx textBox 要素と admx テキスト要素を表します。


[groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)から継承します。

## <a name="methods"></a>メソッド
|メソッド|戻り値の型|説明|
|:---|:---|:---|
|[grouppolicypresentationtextboxes テキストボックスのリスト](../api/intune-grouppolicy-grouppolicypresentationtextbox-list.md)|[grouppolicypresentationtextbox](../resources/intune-grouppolicy-grouppolicypresentationtextbox.md)コレクション|[grouppolicypresentationtextbox](../resources/intune-grouppolicy-grouppolicypresentationtextbox.md)オブジェクトのプロパティとリレーションシップをリストします。|
|[grouppolicypresentationtextbox の取得](../api/intune-grouppolicy-grouppolicypresentationtextbox-get.md)|[grouppolicypresentationtextbox](../resources/intune-grouppolicy-grouppolicypresentationtextbox.md)|[grouppolicypresentationtextbox](../resources/intune-grouppolicy-grouppolicypresentationtextbox.md)オブジェクトのプロパティとリレーションシップを読み取ります。|
|[grouppolicypresentationtextbox の作成](../api/intune-grouppolicy-grouppolicypresentationtextbox-create.md)|[grouppolicypresentationtextbox](../resources/intune-grouppolicy-grouppolicypresentationtextbox.md)|新しい[grouppolicypresentationtextbox](../resources/intune-grouppolicy-grouppolicypresentationtextbox.md)オブジェクトを作成します。|
|[grouppolicypresentationtextbox の削除](../api/intune-grouppolicy-grouppolicypresentationtextbox-delete.md)|なし|[grouppolicypresentationtextbox](../resources/intune-grouppolicy-grouppolicypresentationtextbox.md)を削除します。|
|[grouppolicypresentationtextbox の更新](../api/intune-grouppolicy-grouppolicypresentationtextbox-update.md)|[grouppolicypresentationtextbox](../resources/intune-grouppolicy-grouppolicypresentationtextbox.md)|[grouppolicypresentationtextbox](../resources/intune-grouppolicy-grouppolicypresentationtextbox.md)オブジェクトのプロパティを更新します。|

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|label|String|任意のプレゼンテーションエンティティのローカライズされたテキストラベル。 既定値は empty です。 [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)から継承します。|
|id|String|エンティティのキー。 [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)から継承します。|
|lastModifiedDateTime|DateTimeOffset|エンティティが最後に変更された日付と時刻。 [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)から継承します。|
|defaultValue|文字列|テキストボックスに表示されるローカライズされた既定の文字列。 既定値は empty です。|
|必須|ブール値|テキストボックスに値を入力する必要があります。 既定値は false です。|
|maxLength|Int64|テキストの最大文字数を指定する符号なし整数。 既定値は1023です。|

## <a name="relationships"></a>リレーションシップ
|リレーションシップ|型|説明|
|:---|:---|:---|
|definition|[grouppolicydefinition](../resources/intune-grouppolicy-grouppolicydefinition.md)|プレゼンテーションに関連付けられたグループポリシーの定義。 [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)から継承します。|

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




