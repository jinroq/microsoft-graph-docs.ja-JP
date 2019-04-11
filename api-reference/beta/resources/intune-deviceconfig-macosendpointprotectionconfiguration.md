---
title: macosendpointprotectionconfiguration リソースの種類
description: MacOS endpoint protection 構成プロファイル。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 38781db3f01b264b67c604e90025faf82c0fa65a
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/11/2019
ms.locfileid: "31791538"
---
# <a name="macosendpointprotectionconfiguration-resource-type"></a>macosendpointprotectionconfiguration リソースの種類

> **重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

MacOS endpoint protection 構成プロファイル。


[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します

## <a name="methods"></a>メソッド
|メソッド|戻り値の型|説明|
|:---|:---|:---|
|[macosendpointprotectionconfigurations を一覧表示する](../api/intune-deviceconfig-macosendpointprotectionconfiguration-list.md)|[macosendpointprotectionconfiguration](../resources/intune-deviceconfig-macosendpointprotectionconfiguration.md)コレクション|[macosendpointprotectionconfiguration](../resources/intune-deviceconfig-macosendpointprotectionconfiguration.md)オブジェクトのプロパティとリレーションシップをリストします。|
|[macosendpointprotectionconfiguration の取得](../api/intune-deviceconfig-macosendpointprotectionconfiguration-get.md)|[macOSEndpointProtectionConfiguration](../resources/intune-deviceconfig-macosendpointprotectionconfiguration.md)|[macosendpointprotectionconfiguration](../resources/intune-deviceconfig-macosendpointprotectionconfiguration.md)オブジェクトのプロパティとリレーションシップを読み取ります。|
|[macosendpointprotectionconfiguration の作成](../api/intune-deviceconfig-macosendpointprotectionconfiguration-create.md)|[macOSEndpointProtectionConfiguration](../resources/intune-deviceconfig-macosendpointprotectionconfiguration.md)|新しい[macosendpointprotectionconfiguration](../resources/intune-deviceconfig-macosendpointprotectionconfiguration.md)オブジェクトを作成します。|
|[macosendpointprotectionconfiguration の削除](../api/intune-deviceconfig-macosendpointprotectionconfiguration-delete.md)|なし|[macosendpointprotectionconfiguration](../resources/intune-deviceconfig-macosendpointprotectionconfiguration.md)を削除します。|
|[macosendpointprotectionconfiguration の更新](../api/intune-deviceconfig-macosendpointprotectionconfiguration-update.md)|[macOSEndpointProtectionConfiguration](../resources/intune-deviceconfig-macosendpointprotectionconfiguration.md)|[macosendpointprotectionconfiguration](../resources/intune-deviceconfig-macosendpointprotectionconfiguration.md)オブジェクトのプロパティを更新します。|

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|id|文字列型 (String)|エンティティのキー。 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します|
|lastModifiedDateTime|DateTimeOffset|オブジェクトの最終更新の DateTime。 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します|
|roleScopeTagIds|String コレクション|このエンティティインスタンスの範囲タグのリスト。 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します|
|supportsScopeTags|Boolean|基になるデバイス構成がスコープタグの割り当てをサポートしているかどうかを示します。 この値が false である場合、ScopeTags プロパティへの割り当ては許可されません。エンティティは、スコープを持つユーザーには表示されません。 これは Silverlight で作成された従来のポリシーに対して実行され、Azure ポータルでポリシーを削除して再作成することによって解決できます。 このプロパティに値を設定するには、 SetExtrusionDirection メソッドを適用します。 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します|
|createdDateTime|DateTimeOffset|オブジェクトが作成された DateTime。 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します|
|説明|String|管理者が指定した、デバイス構成についての説明。 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します|
|displayName|String|管理者が指定した、デバイス構成の名前。 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します|
|version|Int32|デバイス構成のバージョン。 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します|
|gatekeeperAllowedAppSource|[macOSGatekeeperAppSources](../resources/intune-deviceconfig-macosgatekeeperappsources.md)|macOS デバイスからどのダウンロード場所のアプリを実行できるかを決定する、システムおよびプライバシー設定。 可能な値は、`notConfigured`、`macAppStore`、`macAppStoreAndIdentifiedDevelopers`、`anywhere` です。|
|gatekeeperBlockOverride|Boolean|true に設定されている場合、ゲートキーパーのユーザーオーバーライドは無効になります。|
|firewallEnabled|Boolean|ファイアウォールを有効にするかどうかを指定します。|
|firewallBlockAllIncoming|Boolean|[着信接続をすべてブロックする] オプションに対応しています。|
|firewallEnableStealthMode|Boolean|[ステルスモードを有効にする] に相当します。|
|firewallApplications|[macOSFirewallApplication](../resources/intune-deviceconfig-macosfirewallapplication.md)コレクション|ファイアウォール設定のあるアプリケーションの一覧。 この一覧にないアプリケーションのファイアウォール設定は、ユーザーによって決まります。 このコレクションには、最大で 500 個の要素を含めることができます。|

## <a name="relationships"></a>リレーションシップ
|リレーションシップ|型|説明|
|:---|:---|:---|
|groupAssignments|[deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md)コレクション|デバイスの構成プロファイルのグループ割り当てのリストです。 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します|
|assignments|[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) コレクション|デバイスの構成プロファイルの割り当てのリスト。 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します|
|deviceStatuses|[deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md) コレクション|デバイスごとのデバイス構成のインストール状況。 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します|
|userStatuses|[deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md) コレクション|ユーザーごとのデバイス構成のインストール状態。 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します|
|deviceStatusOverview|[deviceConfigurationDeviceOverview](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md)|デバイス構成のデバイス状態の概要 ([deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承)|
|userStatusOverview|[deviceConfigurationUserOverview](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md)|デバイス構成のユーザー状態の概要 ([deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承)|
|deviceSettingStateSummaries|[settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) コレクション|デバイス構成設定状態のデバイスの要約 ([deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承)|

## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.macOSEndpointProtectionConfiguration"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.macOSEndpointProtectionConfiguration",
  "id": "String (identifier)",
  "lastModifiedDateTime": "String (timestamp)",
  "roleScopeTagIds": [
    "String"
  ],
  "supportsScopeTags": true,
  "createdDateTime": "String (timestamp)",
  "description": "String",
  "displayName": "String",
  "version": 1024,
  "gatekeeperAllowedAppSource": "String",
  "gatekeeperBlockOverride": true,
  "firewallEnabled": true,
  "firewallBlockAllIncoming": true,
  "firewallEnableStealthMode": true,
  "firewallApplications": [
    {
      "@odata.type": "microsoft.graph.macOSFirewallApplication",
      "bundleId": "String",
      "allowsIncomingConnections": true
    }
  ]
}
```





