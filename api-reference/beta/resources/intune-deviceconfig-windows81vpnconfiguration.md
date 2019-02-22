---
title: windows81VpnConfiguration リソースの種類
description: このプロファイルの構成を指定することで、Windows 8.1 以降のデバイスに、目的の VPN エンドポイントに接続するよう指示することができます。 vpn エンドポイントによって想定される認証方法とセキュリティの種類を指定することにより、エンドユーザーにとってシームレスに vpn 接続を確立できます。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: ef93e3207fbd7d9171d7d9d28d20f8b07936517a
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/21/2019
ms.locfileid: "30161601"
---
# <a name="windows81vpnconfiguration-resource-type"></a>windows81VpnConfiguration リソースの種類

> **重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

このプロファイルの構成を指定することで、Windows 8.1 以降のデバイスに、目的の VPN エンドポイントに接続するよう指示することができます。 vpn エンドポイントによって想定される認証方法とセキュリティの種類を指定することにより、エンドユーザーにとってシームレスに vpn 接続を確立できます。


[windowsvpnconfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)から継承します

## <a name="methods"></a>メソッド
|メソッド|戻り値の型|説明|
|:---|:---|:---|
|[リスト windows81VpnConfigurations](../api/intune-deviceconfig-windows81vpnconfiguration-list.md)|[windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md)コレクション|[windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md)オブジェクトのプロパティとリレーションシップをリストします。|
|[windows81VpnConfiguration を取得する](../api/intune-deviceconfig-windows81vpnconfiguration-get.md)|[windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md)|[windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md)オブジェクトのプロパティとリレーションシップを読み取ります。|
|[windows81VpnConfiguration を作成する](../api/intune-deviceconfig-windows81vpnconfiguration-create.md)|[windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md)|新しい[windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md)オブジェクトを作成します。|
|[windows81VpnConfiguration の削除](../api/intune-deviceconfig-windows81vpnconfiguration-delete.md)|なし|[windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md)を削除します。|
|[windows81VpnConfiguration の更新](../api/intune-deviceconfig-windows81vpnconfiguration-update.md)|[windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md)|[windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md)オブジェクトのプロパティを更新します。|

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|id|文字列|エンティティのキー。 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します|
|lastModifiedDateTime|DateTimeOffset|オブジェクトが最後に変更された DateTime。 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します|
|roleScopeTagIds|String collection|このエンティティインスタンスの範囲タグのリスト。 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します|
|supportsScopeTags|ブール値|基になるデバイス構成がスコープタグの割り当てをサポートしているかどうかを示します。 この値が false である場合、ScopeTags プロパティへの割り当ては許可されません。エンティティは、スコープを持つユーザーには表示されません。 これは Silverlight で作成された従来のポリシーに対して実行され、Azure ポータルでポリシーを削除して再作成することによって解決できます。 このプロパティは読み取りのみ可能です。 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します|
|createdDateTime|DateTimeOffset|オブジェクトが作成された DateTime。 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します|
|説明|String|デバイス構成について管理者が提供した説明。 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します|
|displayName|String|デバイス構成について管理者が指定した名前。 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します|
|version|Int32|デバイス構成のバージョン。 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します|
|connectionName|String|ユーザーに表示される接続名。 [windowsvpnconfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)から継承します|
|サーバー|[vpnServer](../resources/intune-deviceconfig-vpnserver.md)コレクション|ネットワーク上の VPN サーバーの一覧。 エンドユーザーがこれらのネットワークの場所にアクセスできることを確認します。 このコレクションには、最大で 500 個の要素を含めることができます。 [windowsvpnconfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)から継承します|
|customXml|Binary|VPN 接続を構成するカスタム XML コマンド。 (UTF8 でエンコードされたバイト配列)[windowsvpnconfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)から継承します|
|applyOnlyToWindows81|Boolean|このポリシーを Windows 8.1 にのみ適用するかどうかを示す値。 このプロパティは読み取り専用です。|
|connectionType|[windowsvpnconnectiontype](../resources/intune-deviceconfig-windowsvpnconnectiontype.md)|接続の種類。 使用可能な値は、`pulseSecure`、`f5EdgeClient`、`dellSonicWallMobileConnect`、`checkPointCapsuleVpn` です。|
|logingroupordomain|String|接続の種類が Dell SonicWALL Mobile connection に設定されている場合のログイングループまたはドメイン。|
|enablesplittunneling|ブール値|VPN の分割トンネリングを有効にします。|
|proxyServer|[windows81VpnProxyServer](../resources/intune-deviceconfig-windows81vpnproxyserver.md)|プロキシサーバー。|

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
  "@odata.type": "microsoft.graph.windows81VpnConfiguration"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windows81VpnConfiguration",
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
  "connectionName": "String",
  "servers": [
    {
      "@odata.type": "microsoft.graph.vpnServer",
      "description": "String",
      "address": "String",
      "isDefaultServer": true
    }
  ],
  "customXml": "binary",
  "applyOnlyToWindows81": true,
  "connectionType": "String",
  "loginGroupOrDomain": "String",
  "enableSplitTunneling": true,
  "proxyServer": {
    "@odata.type": "microsoft.graph.windows81VpnProxyServer",
    "automaticConfigurationScriptUrl": "String",
    "address": "String",
    "port": 1024,
    "automaticallyDetectProxySettings": true,
    "bypassProxyServerForLocalAddress": true
  }
}
```




