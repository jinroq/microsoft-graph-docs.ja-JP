---
title: androidManagedStoreAppConfiguration リソースの種類
description: プロパティ、継承されたプロパティおよび Android エンタープライズ モバイル アプリケーションの構成のアクションが含まれています。
ms.openlocfilehash: e9e92065d46d311f3e6891f9dc13fa0ab60ff2b3
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27068146"
---
# <a name="androidmanagedstoreappconfiguration-resource-type"></a>androidManagedStoreAppConfiguration リソースの種類

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

> **注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。

プロパティ、継承されたプロパティおよび Android エンタープライズ モバイル アプリケーションの構成のアクションが含まれています。

[managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md) から継承します

## <a name="methods"></a>メソッド
|メソッド|戻り値の型|説明|
|:---|:---|:---|
|[リスト androidManagedStoreAppConfigurations](../api/intune-apps-androidmanagedstoreappconfiguration-list.md)|[androidManagedStoreAppConfiguration](../resources/intune-apps-androidmanagedstoreappconfiguration.md)コレクション|[AndroidManagedStoreAppConfiguration](../resources/intune-apps-androidmanagedstoreappconfiguration.md)オブジェクトのプロパティと関係を一覧表示します。|
|[AndroidManagedStoreAppConfiguration を取得します。](../api/intune-apps-androidmanagedstoreappconfiguration-get.md)|[androidManagedStoreAppConfiguration](../resources/intune-apps-androidmanagedstoreappconfiguration.md)|[AndroidManagedStoreAppConfiguration](../resources/intune-apps-androidmanagedstoreappconfiguration.md)オブジェクトのプロパティと関係を参照してください。|
|[AndroidManagedStoreAppConfiguration を作成します。](../api/intune-apps-androidmanagedstoreappconfiguration-create.md)|[androidManagedStoreAppConfiguration](../resources/intune-apps-androidmanagedstoreappconfiguration.md)|新しい[androidManagedStoreAppConfiguration](../resources/intune-apps-androidmanagedstoreappconfiguration.md)オブジェクトを作成します。|
|[AndroidManagedStoreAppConfiguration を削除します。](../api/intune-apps-androidmanagedstoreappconfiguration-delete.md)|なし|の[androidManagedStoreAppConfiguration](../resources/intune-apps-androidmanagedstoreappconfiguration.md)を削除します。|
|[AndroidManagedStoreAppConfiguration を更新します。](../api/intune-apps-androidmanagedstoreappconfiguration-update.md)|[androidManagedStoreAppConfiguration](../resources/intune-apps-androidmanagedstoreappconfiguration.md)|[AndroidManagedStoreAppConfiguration](../resources/intune-apps-androidmanagedstoreappconfiguration.md)オブジェクトのプロパティを更新します。|

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|id|String|エンティティのキー。 [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md) から継承されます|
|targetedMobileApps|String コレクション|関連するアプリです。 [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md) から継承されます|
|roleScopeTagIds|String コレクション|このアプリケーションの構成エンティティのスコープのタグの一覧です。 [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md) から継承されます|
|createdDateTime|DateTimeOffset|オブジェクトが作成された DateTime。 [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md) から継承されます|
|説明|String|デバイス構成について管理者が提供した説明。 [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md) から継承されます|
|lastModifiedDateTime|DateTimeOffset|オブジェクトが最後に変更された DateTime。 [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md) から継承されます|
|displayName|String|デバイス構成について管理者が指定した名前。 [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md) から継承されます|
|version|Int32|デバイス構成のバージョン。 [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md) から継承されます|
|packageId|String|Android エンタープライズ アプリケーションの構成パッケージの id。|
|payloadJson|String|Android エンタープライズ アプリケーション構成 JSON ペイロード。|
|permissionActions|[androidPermissionAction](../resources/intune-apps-androidpermissionaction.md)コレクション|Android アプリケーションのアクセス許可とアクセス許可の対応するアクションの一覧です。|

## <a name="relationships"></a>リレーションシップ
|リレーションシップ|型|説明|
|:---|:---|:---|
|assignments|[managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md) コレクション|アプリ構成のグループ割り当てのリストです。 [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md) から継承済み|
|deviceStatuses|[managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md)コレクション|ManagedDeviceMobileAppConfigurationDeviceStatus のリストです。 [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md) から継承済み|
|userStatuses|[managedDeviceMobileAppConfigurationUserStatus](../resources/intune-apps-manageddevicemobileappconfigurationuserstatus.md) コレクション|ManagedDeviceMobileAppConfigurationUserStatus のリストです。 [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md) から継承済み|
|deviceStatusSummary|[managedDeviceMobileAppConfigurationDeviceSummary](../resources/intune-apps-manageddevicemobileappconfigurationdevicesummary.md)|アプリ構成のデバイス状態の要約です。 [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md) から継承済み|
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
  ]
}
```





