---
title: iosMobileAppConfiguration リソースの種類
description: iOS モバイル アプリ構成に関する、プロパティ、継承済みのプロパティ、アクションが含まれています。
localization_priority: Normal
author: tfitzmac
ms.prod: intune
ms.openlocfilehash: c354a1248b782d08e751a1215edc9825de1da147
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27912597"
---
# <a name="iosmobileappconfiguration-resource-type"></a>iosMobileAppConfiguration リソースの種類

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

> **注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。

iOS モバイル アプリ構成に関する、プロパティ、継承済みのプロパティ、アクションが含まれています。

[managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md) から継承します

## <a name="methods"></a>メソッド
|メソッド|戻り値の型|説明|
|:---|:---|:---|
|[iosMobileAppConfigurations のリスト](../api/intune-apps-iosmobileappconfiguration-list.md)|[iosMobileAppConfiguration](../resources/intune-apps-iosmobileappconfiguration.md) コレクション|[iosMobileAppConfiguration](../resources/intune-apps-iosmobileappconfiguration.md) オブジェクトのプロパティとリレーションシップをリストします。|
|[iosMobileAppConfiguration の取得](../api/intune-apps-iosmobileappconfiguration-get.md) |[iosMobileAppConfiguration](../resources/intune-apps-iosmobileappconfiguration.md)|[iosMobileAppConfiguration](../resources/intune-apps-iosmobileappconfiguration.md) オブジェクトのプロパティとリレーションシップを読み取ります。|
|[iosMobileAppConfiguration の作成](../api/intune-apps-iosmobileappconfiguration-create.md)|[iosMobileAppConfiguration](../resources/intune-apps-iosmobileappconfiguration.md)|新しい [iosMobileAppConfiguration](../resources/intune-apps-iosmobileappconfiguration.md) オブジェクトを作成します。|
|[iosMobileAppConfiguration の削除](../api/intune-apps-iosmobileappconfiguration-delete.md)|なし|[iosMobileAppConfiguration](../resources/intune-apps-iosmobileappconfiguration.md) を削除します。|
|[iosMobileAppConfiguration の更新](../api/intune-apps-iosmobileappconfiguration-update.md)|[iosMobileAppConfiguration](../resources/intune-apps-iosmobileappconfiguration.md)|[iosMobileAppConfiguration](../resources/intune-apps-iosmobileappconfiguration.md) オブジェクトのプロパティを更新します。|

## <a name="properties"></a>プロパティ
|プロパティ|種類|説明|
|:---|:---|:---|
|ID|String|エンティティのキー。 [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md) から継承されます|
|targetedMobileApps|String コレクション|関連するアプリです。 [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md) から継承されます|
|roleScopeTagIds|String コレクション|このアプリケーションの構成エンティティのスコープのタグの一覧です。 [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md) から継承されます|
|createdDateTime|DateTimeOffset|オブジェクトが作成された DateTime。 [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md) から継承されます|
|説明|String|デバイス構成について管理者が提供した説明。 [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md) から継承されます|
|lastModifiedDateTime|DateTimeOffset|オブジェクトが最後に変更された DateTime。 [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md) から継承されます|
|displayName|String|デバイス構成について管理者が指定した名前。 [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md) から継承されます|
|version|Int32|デバイス構成のバージョン。 [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md) から継承されます|
|encodedSettingXml|Binary|mdm アプリ 構成 Base 64 バイナリ。|
|settings|[appConfigurationSettingItem](../resources/intune-apps-appconfigurationsettingitem.md) コレクション|アプリの構成設定アイテム。|

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
  "@odata.type": "microsoft.graph.iosMobileAppConfiguration"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosMobileAppConfiguration",
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
  "encodedSettingXml": "binary",
  "settings": [
    {
      "@odata.type": "microsoft.graph.appConfigurationSettingItem",
      "appConfigKey": "String",
      "appConfigKeyType": "String",
      "appConfigKeyValue": "String"
    }
  ]
}
```





