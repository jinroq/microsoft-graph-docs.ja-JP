---
title: windows81VpnConfiguration リソースの種類
description: このプロファイルの構成を提供することによって必要な VPN エンドポイントに接続する Windows 8.1 の (およびそれ以降) のデバイスに指示できます。 指定する認証方法とセキュリティの種類必要 VPN エンドポイントで行うことができます、VPN 接続シームレスなエンド ・ ユーザーのです。
ms.openlocfilehash: aad145c59883fe535e86694d2ba60a7100faf93b
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27073417"
---
# <a name="windows81vpnconfiguration-resource-type"></a>windows81VpnConfiguration リソースの種類

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

> **注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。

このプロファイルの構成を提供することによって必要な VPN エンドポイントに接続する Windows 8.1 の (およびそれ以降) のデバイスに指示できます。 指定する認証方法とセキュリティの種類必要 VPN エンドポイントで行うことができます、VPN 接続シームレスなエンド ・ ユーザーのです。

[WindowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)から継承します。

## <a name="methods"></a>メソッド
|メソッド|戻り値の型|説明|
|:---|:---|:---|
|[リスト windows81VpnConfigurations](../api/intune-deviceconfig-windows81vpnconfiguration-list.md)|[windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md)コレクション|[Windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md)オブジェクトのプロパティと関係を一覧表示します。|
|[Windows81VpnConfiguration を取得します。](../api/intune-deviceconfig-windows81vpnconfiguration-get.md)|[windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md)|[Windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md)オブジェクトのプロパティと関係を参照してください。|
|[Windows81VpnConfiguration を作成します。](../api/intune-deviceconfig-windows81vpnconfiguration-create.md)|[windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md)|新しい[windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md)オブジェクトを作成します。|
|[Windows81VpnConfiguration を削除します。](../api/intune-deviceconfig-windows81vpnconfiguration-delete.md)|なし|の[windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md)を削除します。|
|[Windows81VpnConfiguration を更新します。](../api/intune-deviceconfig-windows81vpnconfiguration-update.md)|[windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md)|[Windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md)オブジェクトのプロパティを更新します。|

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|id|String|エンティティのキー。 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します|
|lastModifiedDateTime|DateTimeOffset|オブジェクトが最後に変更された DateTime。 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します|
|roleScopeTagIds|String コレクション|このエンティティ インスタンスのスコープのタグのリストです。 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します|
|supportsScopeTags|ブール値|デバイスの構成を基になるスコープのタグの割り当てをサポートしているかどうかを示します。 この値が false であり、エンティティをスコープ指定されたユーザーには表示されませんがある場合、ScopeTags プロパティに割り当てることは許可されていません。 これは、Silverlight で作成されたレガシ ポリシーに対して発生し、削除して、Azure ポータル内のポリシーを再作成することで解決できます。 このプロパティは値の取得のみ可能です。 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します|
|createdDateTime|DateTimeOffset|オブジェクトが作成された DateTime。 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します|
|説明|String|デバイス構成について管理者が提供した説明。 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します|
|displayName|String|デバイス構成について管理者が指定した名前。 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します|
|version|Int32|デバイス構成のバージョン。 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します|
|connectionName|String|接続名がユーザーに表示されます。 [WindowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)から継承されました。|
|サーバー|[vpnServer](../resources/intune-deviceconfig-vpnserver.md)コレクション|ネットワーク上の VPN サーバーの一覧です。 エンド ・ ユーザーがこれらのネットワークの場所にアクセスできることを確認します。 このコレクションには、最大で 500 個の要素を含めることができます。 [WindowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)から継承されました。|
|customXml|バイナリ|VPN 接続を構成するユーザー設定の XML コマンドです。 (UTF8 でエンコードされたバイト配列)[WindowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)から継承されました。|
|applyOnlyToWindows81|Boolean|このポリシーを Windows 8.1 にのみ適用するかどうかを示す値。 このプロパティは読み取り専用です。|
|接続タイプ|[windowsVpnConnectionType](../resources/intune-deviceconfig-windowsvpnconnectiontype.md)|接続の種類です。 可能な値は、`pulseSecure`、`f5EdgeClient`、`dellSonicWallMobileConnect`、`checkPointCapsuleVpn` です。|
|loginGroupOrDomain|String|ログイン グループまたは Dell SonicWALL のモバイル接続する接続の種類が設定されている場合はドメインです。|
|enableSplitTunneling|ブール値|分割は、VPN のトンネリングを有効にします。|
|proxyServer|[windows81VpnProxyServer](../resources/intune-deviceconfig-windows81vpnproxyserver.md)|プロキシ サーバーです。|

## <a name="relationships"></a>リレーションシップ
|リレーションシップ|型|説明|
|:---|:---|:---|
|groupAssignments|[deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md)コレクション|デバイスの構成プロファイルのグループ割り当てのリストです。 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します|
|assignments|[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) コレクション|デバイスの構成プロファイルの割り当てのリスト。 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します|
|deviceStatuses|[deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md) コレクション|デバイスごとのデバイス構成のインストール状況。 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します|
|userStatuses|[deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md) コレクション|ユーザーごとのデバイス構成のインストール状態です。 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します|
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





