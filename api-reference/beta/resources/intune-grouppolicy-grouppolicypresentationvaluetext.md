---
title: groupPolicyPresentationValueText リソースの種類
description: エンティティは、ポリシー定義のドロップダウンリスト、コンボボックス、またはテキストボックスの表示の文字列値を表します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 015d136db76ae7523a06e4dba10c2c7e5bc48187
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/11/2019
ms.locfileid: "31781674"
---
# <a name="grouppolicypresentationvaluetext-resource-type"></a>groupPolicyPresentationValueText リソースの種類

> **重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

エンティティは、ポリシー定義のドロップダウンリスト、コンボボックス、またはテキストボックスの表示の文字列値を表します。


[grouppolicypresentationvalue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)から継承します

## <a name="methods"></a>メソッド
|メソッド|戻り値の型|説明|
|:---|:---|:---|
|[リスト grouppolicypresentationvaluetexts](../api/intune-grouppolicy-grouppolicypresentationvaluetext-list.md)|[groupPolicyPresentationValueText](../resources/intune-grouppolicy-grouppolicypresentationvaluetext.md)コレクション|[groupPolicyPresentationValueText](../resources/intune-grouppolicy-grouppolicypresentationvaluetext.md)オブジェクトのプロパティとリレーションシップをリストします。|
|[groupPolicyPresentationValueText を取得する](../api/intune-grouppolicy-grouppolicypresentationvaluetext-get.md)|[groupPolicyPresentationValueText](../resources/intune-grouppolicy-grouppolicypresentationvaluetext.md)|[groupPolicyPresentationValueText](../resources/intune-grouppolicy-grouppolicypresentationvaluetext.md)オブジェクトのプロパティとリレーションシップを読み取ります。|
|[groupPolicyPresentationValueText を作成する](../api/intune-grouppolicy-grouppolicypresentationvaluetext-create.md)|[groupPolicyPresentationValueText](../resources/intune-grouppolicy-grouppolicypresentationvaluetext.md)|新しい[groupPolicyPresentationValueText](../resources/intune-grouppolicy-grouppolicypresentationvaluetext.md)オブジェクトを作成します。|
|[groupPolicyPresentationValueText の削除](../api/intune-grouppolicy-grouppolicypresentationvaluetext-delete.md)|なし|[groupPolicyPresentationValueText](../resources/intune-grouppolicy-grouppolicypresentationvaluetext.md)を削除します。|
|[groupPolicyPresentationValueText の更新](../api/intune-grouppolicy-grouppolicypresentationvaluetext-update.md)|[groupPolicyPresentationValueText](../resources/intune-grouppolicy-grouppolicypresentationvaluetext.md)|[groupPolicyPresentationValueText](../resources/intune-grouppolicy-grouppolicypresentationvaluetext.md)オブジェクトのプロパティを更新します。|

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|lastModifiedDateTime|DateTimeOffset|オブジェクトが最後に変更された日付と時刻。 [grouppolicypresentationvalue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)から継承します。|
|createdDateTime|DateTimeOffset|オブジェクトが作成された日付と時刻。 [grouppolicypresentationvalue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)から継承します。|
|id|String|エンティティのキー。 [grouppolicypresentationvalue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)から継承します。|
|value|文字列型 (String)|関連付けられたプレゼンテーションの文字列型 (string) の値を指定します。|

## <a name="relationships"></a>リレーションシップ
|リレーションシップ|型|説明|
|:---|:---|:---|
|definitionvalue|[grouppolicydefinitionvalue](../resources/intune-grouppolicy-grouppolicydefinitionvalue.md)|プレゼンテーション値に関連付けられているグループポリシー定義の値。 [grouppolicypresentationvalue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)から継承します。|
|プレゼンテーション|[groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)|プレゼンテーション値に関連付けられたグループポリシーのプレゼンテーション。 [grouppolicypresentationvalue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)から継承します。|

## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.groupPolicyPresentationValueText"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.groupPolicyPresentationValueText",
  "lastModifiedDateTime": "String (timestamp)",
  "createdDateTime": "String (timestamp)",
  "id": "String (identifier)",
  "value": "String"
}
```





