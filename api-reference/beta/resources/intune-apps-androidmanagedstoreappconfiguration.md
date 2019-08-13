---
title: androidManagedStoreAppConfiguration リソースの種類
description: Android エンタープライズモバイルアプリ構成のプロパティ、継承されたプロパティ、アクションが含まれています。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 29672e2c0147ecc5e516e86d7886b2523fb9ea6e
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36366918"
---
# <a name="androidmanagedstoreappconfiguration-resource-type"></a>androidManagedStoreAppConfiguration リソースの種類

> **重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

Android エンタープライズモバイルアプリ構成のプロパティ、継承されたプロパティ、アクションが含まれています。


[managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md) から継承します

## <a name="methods"></a>メソッド
|メソッド|戻り値の型|説明|
|:---|:---|:---|
|[AndroidManagedStoreAppConfigurations のリスト](../api/intune-apps-androidmanagedstoreappconfiguration-list.md)|[Androidmanagedstoreappconfiguration](../resources/intune-apps-androidmanagedstoreappconfiguration.md)コレクション|[Androidmanagedstoreappconfiguration](../resources/intune-apps-androidmanagedstoreappconfiguration.md)オブジェクトのプロパティとリレーションシップをリストします。|
|[AndroidManagedStoreAppConfiguration の取得](../api/intune-apps-androidmanagedstoreappconfiguration-get.md)|[androidManagedStoreAppConfiguration](../resources/intune-apps-androidmanagedstoreappconfiguration.md)|[Androidmanagedstoreappconfiguration](../resources/intune-apps-androidmanagedstoreappconfiguration.md)オブジェクトのプロパティとリレーションシップを読み取ります。|
|[AndroidManagedStoreAppConfiguration の作成](../api/intune-apps-androidmanagedstoreappconfiguration-create.md)|[androidManagedStoreAppConfiguration](../resources/intune-apps-androidmanagedstoreappconfiguration.md)|新しい[Androidmanagedstoreappconfiguration](../resources/intune-apps-androidmanagedstoreappconfiguration.md)オブジェクトを作成します。|
|[AndroidManagedStoreAppConfiguration の削除](../api/intune-apps-androidmanagedstoreappconfiguration-delete.md)|None|[Androidmanagedstoreappconfiguration](../resources/intune-apps-androidmanagedstoreappconfiguration.md)を削除します。|
|[AndroidManagedStoreAppConfiguration の更新](../api/intune-apps-androidmanagedstoreappconfiguration-update.md)|[androidManagedStoreAppConfiguration](../resources/intune-apps-androidmanagedstoreappconfiguration.md)|[Androidmanagedstoreappconfiguration](../resources/intune-apps-androidmanagedstoreappconfiguration.md)オブジェクトのプロパティを更新します。|

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|id|文字列|エンティティのキー。 [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md) から継承されます|
|targetedMobileApps|String コレクション|関連するアプリです。 [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md) から継承されます|
|roleScopeTagIds|文字列コレクション|このアプリ構成エンティティのスコープタグのリスト。 [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md) から継承されます|
|createdDateTime|DateTimeOffset|オブジェクトが作成された DateTime。 [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md) から継承されます|
|description|String|デバイス構成について管理者が提供した説明。 [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md) から継承されます|
|lastModifiedDateTime|DateTimeOffset|オブジェクトが最後に変更された DateTime。 [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md) から継承されます|
|displayName|String|デバイス構成について管理者が指定した名前。 [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md) から継承されます|
|version|Int32|デバイス構成のバージョン。 [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md) から継承されます|
|packageId|String|Android エンタープライズアプリ構成パッケージ id。|
|payloadJson|String|Android エンタープライズアプリ構成 JSON ペイロード。|
|permissionActions|[Androidpermissionaction](../resources/intune-apps-androidpermissionaction.md)コレクション|Android アプリのアクセス許可と、それに対応するアクセス許可アクションのリスト。|
|appSupportsOemConfig|Boolean|この AppConfig が OEMConfig ポリシーであるかどうか。|

## <a name="relationships"></a>リレーションシップ
|リレーションシップ|型|説明|
|:---|:---|:---|
|assignments|[managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md) コレクション|アプリ構成のグループ割り当てのリストです。 [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md) から継承されます|
|deviceStatuses|[managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md)コレクション|ManagedDeviceMobileAppConfigurationDeviceStatus のリスト。 [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md) から継承されます|
|userStatuses|[managedDeviceMobileAppConfigurationUserStatus](../resources/intune-apps-manageddevicemobileappconfigurationuserstatus.md) コレクション|ManagedDeviceMobileAppConfigurationUserStatus のリストです。 [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md) から継承されます|
|deviceStatusSummary|[managedDeviceMobileAppConfigurationDeviceSummary](../resources/intune-apps-manageddevicemobileappconfigurationdevicesummary.md)|アプリ構成のデバイス状態の要約です。 [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md) から継承されます|
|userStatusSummary|[managedDeviceMobileAppConfigurationUserSummary](../resources/intune-apps-manageddevicemobileappconfigurationusersummary.md)|アプリ構成のユーザー状態の要約です。 [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md) から継承済み|

## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.androidManagedStoreAppConfiguration"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.androidManagedStoreAppConfiguration",
  "id": "String (identifier)",
  "targetedMobileApps": [
    "String"
  ],
  "roleScopeTagIds": [
    "String"
  ],
  "createdDateTime": "String (timestamp)",
  "description": "String",
  "lastModifiedDateTime": "String (timestamp)",
  "displayName": "String",
  "version": 1024,
  "packageId": "String",
  "payloadJson": "String",
  "permissionActions": [
    {
      "@odata.type": "microsoft.graph.androidPermissionAction",
      "permission": "String",
      "action": "String"
    }
  ],
  "appSupportsOemConfig": true
}
```



