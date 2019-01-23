---
title: androidManagedStoreAppConfigurationSchemaItem リソースの種類
description: Android アプリケーションのカスタム構成スキーマ内の項目を 1 つ構成します。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: a12c8f4dc0a07dbf74c92193ac73fdcfe9bfd883
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29398920"
---
# <a name="androidmanagedstoreappconfigurationschemaitem-resource-type"></a>androidManagedStoreAppConfigurationSchemaItem リソースの種類

> **重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。 実稼働アプリケーションでこれらの API を使用することは、サポートされていません。

> **注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

Android アプリケーションのカスタム構成スキーマ内の項目を 1 つ構成します。

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|schemaItemKey|String|アイテムを識別するためにアプリケーションが使用する一意のキー|
|displayName|String|人間が判読できる名前|
|説明|String|アプリケーション内でアイテムが制御する内容の説明|
|defaultBoolValue|Boolean|アプリの開発者が指定している場合、ブール型のアイテムの既定値|
|defaultIntValue|Int32|アプリの開発者が指定している場合、整数型のアイテムの既定値|
|defaultStringValue|String|アプリの開発者が指定している場合、文字列型のアイテムの既定値|
|defaultStringArrayValue|String コレクション|アプリの開発者が指定している場合、配列型のアイテムの既定値|
|dataType|[androidManagedStoreAppConfigurationSchemaItemDataType](../resources/intune-androidforwork-androidmanagedstoreappconfigurationschemaitemdatatype.md)|この項目を記述する値の型。 可能な値は、`bool`、`integer`、`string`、`choice`、`multiselect`、`bundle`、`bundleArray`、`hidden` です。|
|selections|[keyValuePair](../resources/intune-shared-keyvaluepair.md) コレクション|このアイテムに設定可能な有効な値に対しての、人間が判読できる名前と値の組のリスト (選択肢と複数選択項目のみ)|

## <a name="relationships"></a>リレーションシップ
なし

## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.androidManagedStoreAppConfigurationSchemaItem"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.androidManagedStoreAppConfigurationSchemaItem",
  "schemaItemKey": "String",
  "displayName": "String",
  "description": "String",
  "defaultBoolValue": true,
  "defaultIntValue": 1024,
  "defaultStringValue": "String",
  "defaultStringArrayValue": [
    "String"
  ],
  "dataType": "String",
  "selections": [
    {
      "@odata.type": "microsoft.graph.keyValuePair",
      "name": "String",
      "value": "String"
    }
  ]
}
```




