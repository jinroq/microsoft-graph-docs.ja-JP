---
title: androidmanagedstoreappconfigurationschemaitem リソースの種類
description: Android アプリケーションのカスタム構成スキーマ内の単一構成アイテム。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 964916f9f6a46cd8b276e304bfb341d6504db0d2
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/11/2019
ms.locfileid: "31785819"
---
# <a name="androidmanagedstoreappconfigurationschemaitem-resource-type"></a>androidmanagedstoreappconfigurationschemaitem リソースの種類

> **重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

Android アプリケーションのカスタム構成スキーマ内の単一構成アイテム。

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|schemaItemKey|文字列|アイテムを識別するためにアプリケーションが使用する一意のキー|
|displayName|String|人間が判読できる名前|
|説明|String|アプリケーション内でアイテムが制御する内容の説明|
|defaultBoolValue|Boolean|アプリの開発者が指定している場合、ブール型のアイテムの既定値|
|defaultIntValue|Int32|アプリの開発者が指定している場合、整数型のアイテムの既定値|
|defaultStringValue|String|アプリの開発者が指定している場合、文字列型のアイテムの既定値|
|defaultStringArrayValue|String コレクション|アプリの開発者が指定している場合、配列型のアイテムの既定値|
|dataType|[androidmanagedstoreappconfigurationschemaitemdatatype](../resources/intune-androidforwork-androidmanagedstoreappconfigurationschemaitemdatatype.md)|このアイテムが記述する値の種類。 可能な値は、`bool`、`integer`、`string`、`choice`、`multiselect`、`bundle`、`bundleArray`、`hidden` です。|
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





