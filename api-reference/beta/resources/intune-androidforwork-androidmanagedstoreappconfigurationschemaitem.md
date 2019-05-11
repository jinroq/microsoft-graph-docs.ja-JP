---
title: androidManagedStoreAppConfigurationSchemaItem リソースの種類
description: Android アプリケーションのカスタム構成スキーマ内の単一構成アイテム。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 3012542315cd30a565da315a9d383757557b1008
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/11/2019
ms.locfileid: "33950544"
---
# <a name="androidmanagedstoreappconfigurationschemaitem-resource-type"></a>androidManagedStoreAppConfigurationSchemaItem リソースの種類

> **重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

Android アプリケーションのカスタム構成スキーマ内の単一構成アイテム。

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|schemaItemKey|String|アイテムを識別するためにアプリケーションが使用する一意のキー|
|displayName|String|人間が判読できる名前|
|description|String|アプリケーション内でアイテムが制御する内容の説明|
|defaultBoolValue|Boolean|アプリの開発者が指定している場合、ブール型のアイテムの既定値|
|defaultIntValue|Int32|アプリの開発者が指定している場合、整数型のアイテムの既定値|
|defaultStringValue|String|アプリの開発者が指定している場合、文字列型のアイテムの既定値|
|defaultStringArrayValue|String コレクション|アプリの開発者が指定している場合、配列型のアイテムの既定値|
|dataType|[androidManagedStoreAppConfigurationSchemaItemDataType](../resources/intune-androidforwork-androidmanagedstoreappconfigurationschemaitemdatatype.md)|このアイテムが記述する値の種類。 可能な値は、`bool`、`integer`、`string`、`choice`、`multiselect`、`bundle`、`bundleArray`、`hidden` です。|
|selections|[keyValuePair](../resources/intune-shared-keyvaluepair.md) コレクション|このアイテムに設定可能な有効な値に対しての、人間が判読できる名前と値の組のリスト (選択肢と複数選択項目のみ)|

## <a name="relationships"></a>関係
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




