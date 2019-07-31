---
title: androidManagedStoreAppConfigurationSchema リソースの種類
description: Android アプリケーションのカスタム構成を説明するスキーマ。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 8923cfeaadfd82ca20bcdf72ecdf4b023026d14a
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36006172"
---
# <a name="androidmanagedstoreappconfigurationschema-resource-type"></a>androidManagedStoreAppConfigurationSchema リソースの種類

> **重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

Android アプリケーションのカスタム構成を説明するスキーマ。

## <a name="methods"></a>メソッド
|メソッド|戻り値の型|説明|
|:---|:---|:---|
|[AndroidManagedStoreAppConfigurationSchemas のリスト](../api/intune-androidforwork-androidmanagedstoreappconfigurationschema-list.md)|[Androidmanagedstoreappconfigurationschema](../resources/intune-androidforwork-androidmanagedstoreappconfigurationschema.md)コレクション|[Androidmanagedstoreappconfigurationschema](../resources/intune-androidforwork-androidmanagedstoreappconfigurationschema.md)オブジェクトのプロパティとリレーションシップをリストします。|
|[AndroidManagedStoreAppConfigurationSchema の取得](../api/intune-androidforwork-androidmanagedstoreappconfigurationschema-get.md)|[androidManagedStoreAppConfigurationSchema](../resources/intune-androidforwork-androidmanagedstoreappconfigurationschema.md)|[Androidmanagedstoreappconfigurationschema](../resources/intune-androidforwork-androidmanagedstoreappconfigurationschema.md)オブジェクトのプロパティとリレーションシップを読み取ります。|
|[AndroidManagedStoreAppConfigurationSchema の作成](../api/intune-androidforwork-androidmanagedstoreappconfigurationschema-create.md)|[androidManagedStoreAppConfigurationSchema](../resources/intune-androidforwork-androidmanagedstoreappconfigurationschema.md)|新しい[Androidmanagedstoreappconfigurationschema](../resources/intune-androidforwork-androidmanagedstoreappconfigurationschema.md)オブジェクトを作成します。|
|[AndroidManagedStoreAppConfigurationSchema の削除](../api/intune-androidforwork-androidmanagedstoreappconfigurationschema-delete.md)|None|[Androidmanagedstoreappconfigurationschema](../resources/intune-androidforwork-androidmanagedstoreappconfigurationschema.md)を削除します。|
|[AndroidManagedStoreAppConfigurationSchema の更新](../api/intune-androidforwork-androidmanagedstoreappconfigurationschema-update.md)|[androidManagedStoreAppConfigurationSchema](../resources/intune-androidforwork-androidmanagedstoreappconfigurationschema.md)|[Androidmanagedstoreappconfigurationschema](../resources/intune-androidforwork-androidmanagedstoreappconfigurationschema.md)オブジェクトのプロパティを更新します。|

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|id|String|エンティティのキー。スキーマが対応するアプリケーションの Android パッケージ名です。|
|exampleJson|Binary|このスキーマに準拠した JSON 文字列の例を含む、UTF8 でエンコードされたバイト配列。このアプリの構成の設定方法を示しています。|
|schemaItems|[Androidmanagedstoreappconfigurationschemaitem](../resources/intune-androidforwork-androidmanagedstoreappconfigurationschemaitem.md)コレクション|スキーマ内の名前付き構成オプションを表すアイテムのコレクションです。 ルートレベルの構成のみが含まれています。|
|nestedSchemaItems|[Androidmanagedstoreappconfigurationschemaitem](../resources/intune-androidforwork-androidmanagedstoreappconfigurationschemaitem.md)コレクション|スキーマ内の名前付き構成オプションを表すアイテムのコレクションです。 このファイルには、すべての構成のフラットなリストが含まれています。|

## <a name="relationships"></a>リレーションシップ
なし

## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.androidManagedStoreAppConfigurationSchema"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.androidManagedStoreAppConfigurationSchema",
  "id": "String (identifier)",
  "exampleJson": "binary",
  "schemaItems": [
    {
      "@odata.type": "microsoft.graph.androidManagedStoreAppConfigurationSchemaItem",
      "index": 1024,
      "parentIndex": 1024,
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
  ],
  "nestedSchemaItems": [
    {
      "@odata.type": "microsoft.graph.androidManagedStoreAppConfigurationSchemaItem",
      "index": 1024,
      "parentIndex": 1024,
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
  ]
}
```





