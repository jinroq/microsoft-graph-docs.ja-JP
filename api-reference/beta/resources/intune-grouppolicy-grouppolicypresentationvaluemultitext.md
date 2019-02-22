---
title: groupPolicyPresentationValueMultiText リソースの種類
description: エンティティは、ポリシー定義の複数行テキストボックスプレゼンテーションの文字列値を表します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 0fef2f1564f67cc3fce4e294e2d1b356f5d414ff
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/21/2019
ms.locfileid: "30162252"
---
# <a name="grouppolicypresentationvaluemultitext-resource-type"></a>groupPolicyPresentationValueMultiText リソースの種類

> **重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

エンティティは、ポリシー定義の複数行テキストボックスプレゼンテーションの文字列値を表します。


[grouppolicypresentationvalue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)から継承します

## <a name="methods"></a>メソッド
|メソッド|戻り値の型|説明|
|:---|:---|:---|
|[リスト groupPolicyPresentationValueMultiTexts](../api/intune-grouppolicy-grouppolicypresentationvaluemultitext-list.md)|[groupPolicyPresentationValueMultiText](../resources/intune-grouppolicy-grouppolicypresentationvaluemultitext.md)コレクション|[groupPolicyPresentationValueMultiText](../resources/intune-grouppolicy-grouppolicypresentationvaluemultitext.md)オブジェクトのプロパティとリレーションシップをリストします。|
|[groupPolicyPresentationValueMultiText を取得する](../api/intune-grouppolicy-grouppolicypresentationvaluemultitext-get.md)|[groupPolicyPresentationValueMultiText](../resources/intune-grouppolicy-grouppolicypresentationvaluemultitext.md)|[groupPolicyPresentationValueMultiText](../resources/intune-grouppolicy-grouppolicypresentationvaluemultitext.md)オブジェクトのプロパティとリレーションシップを読み取ります。|
|[groupPolicyPresentationValueMultiText を作成する](../api/intune-grouppolicy-grouppolicypresentationvaluemultitext-create.md)|[groupPolicyPresentationValueMultiText](../resources/intune-grouppolicy-grouppolicypresentationvaluemultitext.md)|新しい[groupPolicyPresentationValueMultiText](../resources/intune-grouppolicy-grouppolicypresentationvaluemultitext.md)オブジェクトを作成します。|
|[groupPolicyPresentationValueMultiText の削除](../api/intune-grouppolicy-grouppolicypresentationvaluemultitext-delete.md)|なし|[groupPolicyPresentationValueMultiText](../resources/intune-grouppolicy-grouppolicypresentationvaluemultitext.md)を削除します。|
|[groupPolicyPresentationValueMultiText の更新](../api/intune-grouppolicy-grouppolicypresentationvaluemultitext-update.md)|[groupPolicyPresentationValueMultiText](../resources/intune-grouppolicy-grouppolicypresentationvaluemultitext.md)|[groupPolicyPresentationValueMultiText](../resources/intune-grouppolicy-grouppolicypresentationvaluemultitext.md)オブジェクトのプロパティを更新します。|

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|lastModifiedDateTime|DateTimeOffset|オブジェクトが最後に変更された日付と時刻。 [grouppolicypresentationvalue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)から継承します。|
|createdDateTime|DateTimeOffset|オブジェクトが作成された日付と時刻。 [grouppolicypresentationvalue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)から継承します。|
|id|String|エンティティのキー。 [grouppolicypresentationvalue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)から継承します。|
|values|String collection|関連付けられたプレゼンテーションに対して空ではない文字列のコレクション。|

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
  "@odata.type": "microsoft.graph.groupPolicyPresentationValueMultiText"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.groupPolicyPresentationValueMultiText",
  "lastModifiedDateTime": "String (timestamp)",
  "createdDateTime": "String (timestamp)",
  "id": "String (identifier)",
  "values": [
    "String"
  ]
}
```




