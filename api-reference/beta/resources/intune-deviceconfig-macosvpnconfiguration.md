---
title: macOSVpnConfiguration リソースの種類
description: このプロファイルの構成を提供することによって必要な VPN エンドポイントに接続するのには Mac のデバイスに指示できます。 指定する認証方法とセキュリティの種類必要 VPN エンドポイントで行うことができます、VPN 接続シームレスなエンド ・ ユーザーのです。
ms.openlocfilehash: c5707d0a3f345537dfdf8d99b1366f7999ced41a
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27068809"
---
# <a name="macosvpnconfiguration-resource-type"></a>macOSVpnConfiguration リソースの種類

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

> **注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。

このプロファイルの構成を提供することによって必要な VPN エンドポイントに接続するのには Mac のデバイスに指示できます。 指定する認証方法とセキュリティの種類必要 VPN エンドポイントで行うことができます、VPN 接続シームレスなエンド ・ ユーザーのです。

[AppleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)から継承します。

## <a name="methods"></a>メソッド
|メソッド|戻り値の型|説明|
|:---|:---|:---|
|[リスト macOSVpnConfigurations](../api/intune-deviceconfig-macosvpnconfiguration-list.md)|[macOSVpnConfiguration](../resources/intune-deviceconfig-macosvpnconfiguration.md)コレクション|[MacOSVpnConfiguration](../resources/intune-deviceconfig-macosvpnconfiguration.md)オブジェクトのプロパティと関係を一覧表示します。|
|[MacOSVpnConfiguration を取得します。](../api/intune-deviceconfig-macosvpnconfiguration-get.md)|[macOSVpnConfiguration](../resources/intune-deviceconfig-macosvpnconfiguration.md)|[MacOSVpnConfiguration](../resources/intune-deviceconfig-macosvpnconfiguration.md)オブジェクトのプロパティと関係を参照してください。|
|[MacOSVpnConfiguration を作成します。](../api/intune-deviceconfig-macosvpnconfiguration-create.md)|[macOSVpnConfiguration](../resources/intune-deviceconfig-macosvpnconfiguration.md)|新しい[macOSVpnConfiguration](../resources/intune-deviceconfig-macosvpnconfiguration.md)オブジェクトを作成します。|
|[MacOSVpnConfiguration を削除します。](../api/intune-deviceconfig-macosvpnconfiguration-delete.md)|なし|の[macOSVpnConfiguration](../resources/intune-deviceconfig-macosvpnconfiguration.md)を削除します。|
|[MacOSVpnConfiguration を更新します。](../api/intune-deviceconfig-macosvpnconfiguration-update.md)|[macOSVpnConfiguration](../resources/intune-deviceconfig-macosvpnconfiguration.md)|[MacOSVpnConfiguration](../resources/intune-deviceconfig-macosvpnconfiguration.md)オブジェクトのプロパティを更新します。|

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
|connectionName|String|接続名がユーザーに表示されます。 [AppleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)から継承されました。|
|接続タイプ|[appleVpnConnectionType](../resources/intune-deviceconfig-applevpnconnectiontype.md)|接続の種類です。 [AppleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)から継承されます。 使用可能な値: `ciscoAnyConnect`、 `pulseSecure`、 `f5EdgeClient`、 `dellSonicWallMobileConnect`、 `checkPointCapsuleVpn`、 `customVpn`、 `ciscoIPSec`、 `citrix`、 `ciscoAnyConnectV2`、 `paloAltoGlobalProtect`、 `zscalerPrivateAccess`、 `f5Access2018`、 `citrixSso`、 `paloAltoGlobalProtectV2`。|
|loginGroupOrDomain|String|ログイン グループまたは Dell SonicWALL のモバイル接続する接続の種類が設定されている場合はドメインです。 [AppleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)から継承されました。|
|role|String|パルスをセキュリティで保護する接続の種類が設定されている場合の役割です。 [AppleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)から継承されました。|
|領域|String|領域のパルスをセキュリティで保護する接続の種類が設定されている場合です。 [AppleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)から継承されました。|
|サーバー|[vpnServer](../resources/intune-deviceconfig-vpnserver.md)|ネットワーク上の VPN サーバーです。 エンド ・ ユーザーがこのネットワークの場所にアクセスできることを確認します。 [AppleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)から継承されました。|
|識別子|String|カスタム VPN への接続の種類が設定されている場合に、VPN ベンダーによって提供される識別子です。 例: Cisco AnyConnect は[appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)からのフォーム com.cisco.anyconnect.applevpn.plugin 継承の識別子を使用して|
|customData|[keyValue](../resources/intune-deviceconfig-keyvalue.md)コレクション|カスタム VPN への接続の種類が設定されている場合のカスタム データ。 VPN ソリューションで使用可能なのですが、Intune でサポートされていない機能を有効にするのにには、このフィールドを使用します。 これらのキーと値のペアを追加する方法については、VPN のベンダーに問い合わせてください。 このコレクションには、最大 25 の要素を含めることができます。 [AppleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)から継承されました。|
|customKeyValueData|[keyValuePair](../resources/intune-shared-keyvaluepair.md) コレクション|カスタム VPN への接続の種類が設定されている場合のカスタム データ。 VPN ソリューションで使用可能なのですが、Intune でサポートされていない機能を有効にするのにには、このフィールドを使用します。 これらのキーと値のペアを追加する方法については、VPN のベンダーに問い合わせてください。 このコレクションには、最大 25 の要素を含めることができます。 [AppleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)から継承されました。|
|enableSplitTunneling|ブール値|VPN 経由のすべてのネットワーク トラフィックを送信します。 [AppleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)から継承されました。|
|authenticationMethod|[vpnAuthenticationMethod](../resources/intune-deviceconfig-vpnauthenticationmethod.md)|この VPN 接続の認証方法です。 [AppleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)から継承されます。 使用可能な値は、`certificate`、`usernameAndPassword` です。|
|enablePerApp|ブール値|これを true に設定する可能性がある後でエンド ・ ユーザーの iOS デバイスでは、この VPN 接続を開始するアプリケーションに関連付けられているアプリケーションごとの VPN のペイロードを作成します。 [AppleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)から継承されました。|
|safariDomains|String コレクション|Safari のドメインごとのアプリケーション設定には、この VPN を有効にするとします。 この VPN に関連付けられているアプリケーションだけでなくは、Safari のドメインは、ここでもできるようになりますこの VPN 接続をトリガーを指定します。 [AppleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)から継承されました。|
|onDemandRules|[vpnOnDemandRule](../resources/intune-deviceconfig-vpnondemandrule.md)コレクション|オン ・ デマンドでのルール。 このコレクションには、最大で 500 個の要素を含めることができます。 [AppleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)から継承されました。|
|proxyServer|[vpnProxyServer](../resources/intune-deviceconfig-vpnproxyserver.md)|プロキシ サーバーです。 [AppleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)から継承されました。|
|optInToDeviceIdSharing|ブール値|オプトインのネットワーク アクセス コントロールの検証中にサードパーティ製の vpn クライアントを使用するためにデバイスの Id を共有します。 [AppleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)から継承されました。|

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
|identityCertificate|[macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md)|認証は、証明書とクライアントの認証に証明します。|

## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.macOSVpnConfiguration"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.macOSVpnConfiguration",
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
  "connectionType": "String",
  "loginGroupOrDomain": "String",
  "role": "String",
  "realm": "String",
  "server": {
    "@odata.type": "microsoft.graph.vpnServer",
    "description": "String",
    "address": "String",
    "isDefaultServer": true
  },
  "identifier": "String",
  "customData": [
    {
      "@odata.type": "microsoft.graph.keyValue",
      "key": "String",
      "value": "String"
    }
  ],
  "customKeyValueData": [
    {
      "@odata.type": "microsoft.graph.keyValuePair",
      "name": "String",
      "value": "String"
    }
  ],
  "enableSplitTunneling": true,
  "authenticationMethod": "String",
  "enablePerApp": true,
  "safariDomains": [
    "String"
  ],
  "onDemandRules": [
    {
      "@odata.type": "microsoft.graph.vpnOnDemandRule",
      "ssids": [
        "String"
      ],
      "dnsSearchDomains": [
        "String"
      ],
      "probeUrl": "String",
      "action": "String",
      "domainAction": "String",
      "domains": [
        "String"
      ],
      "probeRequiredUrl": "String"
    }
  ],
  "proxyServer": {
    "@odata.type": "microsoft.graph.vpnProxyServer",
    "automaticConfigurationScriptUrl": "String",
    "address": "String",
    "port": 1024
  },
  "optInToDeviceIdSharing": true
}
```





