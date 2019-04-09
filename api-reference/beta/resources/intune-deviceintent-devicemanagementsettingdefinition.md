---
title: devicemanagementsettingdefinition リソースの種類
description: 指定した設定の定義を表すエンティティ
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 1a37046b80ce51a698ba52f08c2693af821b7e52
ms.sourcegitcommit: 77f485ec03a8c917f59d2fbed4df1ec755f3da58
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/08/2019
ms.locfileid: "31524485"
---
# <a name="devicemanagementsettingdefinition-resource-type"></a>devicemanagementsettingdefinition リソースの種類

> **重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

指定した設定の定義を表すエンティティ

## <a name="methods"></a>メソッド
|メソッド|戻り値の型|説明|
|:---|:---|:---|
|[devicemanagementsettingdefinitions のリスト](../api/intune-deviceintent-devicemanagementsettingdefinition-list.md)|[devicemanagementsettingdefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)コレクション|[devicemanagementsettingdefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)オブジェクトのプロパティとリレーションシップをリストします。|
|[devicemanagementsettingdefinition の取得](../api/intune-deviceintent-devicemanagementsettingdefinition-get.md)|[devicemanagementsettingdefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)|[devicemanagementsettingdefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)オブジェクトのプロパティとリレーションシップを読み取ります。|
|[devicemanagementsettingdefinition の作成](../api/intune-deviceintent-devicemanagementsettingdefinition-create.md)|[devicemanagementsettingdefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)|新しい[devicemanagementsettingdefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)オブジェクトを作成します。|
|[devicemanagementsettingdefinition の削除](../api/intune-deviceintent-devicemanagementsettingdefinition-delete.md)|なし|[devicemanagementsettingdefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)を削除します。|
|[devicemanagementsettingdefinition の更新](../api/intune-deviceintent-devicemanagementsettingdefinition-update.md)|[devicemanagementsettingdefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)|[devicemanagementsettingdefinition](../resources/intune-deviceintent-devicemanagementsettingdefinition.md)オブジェクトのプロパティを更新します。|

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|id|文字列|設定定義の ID|
|valueType|[deviceManangementIntentValueType](../resources/intune-deviceintent-devicemanangementintentvaluetype.md)|値のデータ型。 可能な値は `integer`、`boolean`、`string`、`complex`、`collection`、`abstractComplex` です。|
|displayName|String|設定の表示名|
|isTopLevel|Boolean|設定が最上位レベルの場合は、コレクションまたは複雑な設定でラップする必要がなく構成できます。|
|説明|String|設定の説明|
|documentation url|文字列|ドキュメントを設定するための Url|
|keywords|String コレクション|設定に関連付けられているキーワード|
|式|[devicemanagementconstraint](../resources/intune-deviceintent-devicemanagementconstraint.md)コレクション|設定値の制約のコレクション|
|ヲ|[devicemanagementsettingdependency](../resources/intune-deviceintent-devicemanagementsettingdependency.md)コレクション|他の設定に対する依存関係のコレクション|

## <a name="relationships"></a>リレーションシップ
なし

## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceManagementSettingDefinition"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementSettingDefinition",
  "id": "String (identifier)",
  "valueType": "String",
  "displayName": "String",
  "isTopLevel": true,
  "description": "String",
  "documentationUrl": "String",
  "keywords": [
    "String"
  ],
  "constraints": [
    {
      "@odata.type": "microsoft.graph.deviceManagementSettingXmlConstraint"
    }
  ],
  "dependencies": [
    {
      "@odata.type": "microsoft.graph.deviceManagementSettingDependency",
      "definitionId": "String",
      "constraints": [
        {
          "@odata.type": "microsoft.graph.deviceManagementSettingXmlConstraint"
        }
      ]
    }
  ]
}
```







