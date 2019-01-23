---
title: windows10VpnConfiguration リソースの種類
description: このプロファイルの構成を提供することによって必要な VPN エンドポイントへの接続に Windows 10 デバイス (デスクトップまたはモバイル) に指示できます。 指定する認証方法とセキュリティの種類必要 VPN エンドポイントで行うことができます、VPN 接続シームレスなエンド ・ ユーザーのです。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 75710eb8d969f4bfc751405ecf6eca50ced6cfe1
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29406970"
---
# <a name="windows10vpnconfiguration-resource-type"></a>windows10VpnConfiguration リソースの種類

> **重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。 実稼働アプリケーションでこれらの API を使用することは、サポートされていません。

> **注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

このプロファイルの構成を提供することによって必要な VPN エンドポイントへの接続に Windows 10 デバイス (デスクトップまたはモバイル) に指示できます。 指定する認証方法とセキュリティの種類必要 VPN エンドポイントで行うことができます、VPN 接続シームレスなエンド ・ ユーザーのです。


[WindowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)から継承します。

## <a name="methods"></a>メソッド
|メソッド|戻り値の型|説明|
|:---|:---|:---|
|[リスト windows10VpnConfigurations](../api/intune-deviceconfig-windows10vpnconfiguration-list.md)|[windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md)コレクション|[Windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md)オブジェクトのプロパティと関係を一覧表示します。|
|[Windows10VpnConfiguration を取得します。](../api/intune-deviceconfig-windows10vpnconfiguration-get.md)|[windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md)|[Windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md)オブジェクトのプロパティと関係を参照してください。|
|[Windows10VpnConfiguration を作成します。](../api/intune-deviceconfig-windows10vpnconfiguration-create.md)|[windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md)|新しい[windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md)オブジェクトを作成します。|
|[Windows10VpnConfiguration を削除します。](../api/intune-deviceconfig-windows10vpnconfiguration-delete.md)|なし|の[windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md)を削除します。|
|[Windows10VpnConfiguration を更新します。](../api/intune-deviceconfig-windows10vpnconfiguration-update.md)|[windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md)|[Windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md)オブジェクトのプロパティを更新します。|

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|id|String|エンティティのキー。 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します|
|lastModifiedDateTime|DateTimeOffset|オブジェクトが最後に変更された DateTime。 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します|
|roleScopeTagIds|String コレクション|このエンティティ インスタンスのスコープのタグのリストです。 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します|
|supportsScopeTags|Boolean|デバイスの構成を基になるスコープのタグの割り当てをサポートしているかどうかを示します。 この値が false であり、エンティティをスコープ指定されたユーザーには表示されませんがある場合、ScopeTags プロパティに割り当てることは許可されていません。 これは、Silverlight で作成されたレガシ ポリシーに対して発生し、削除して、Azure ポータル内のポリシーを再作成することで解決できます。 このプロパティは読み取りのみ可能です。 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します|
|createdDateTime|DateTimeOffset|オブジェクトが作成された DateTime。 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します|
|説明|String|デバイス構成について管理者が提供した説明。 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します|
|displayName|String|デバイス構成について管理者が指定した名前。 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します|
|version|Int32|デバイス構成のバージョン。 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します|
|connectionName|String|接続名がユーザーに表示されます。 [WindowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)から継承されました。|
|サーバー|[vpnServer](../resources/intune-deviceconfig-vpnserver.md)コレクション|ネットワーク上の VPN サーバーの一覧です。 エンド ・ ユーザーがこれらのネットワークの場所にアクセスできることを確認します。 このコレクションには、最大で 500 個の要素を含めることができます。 [WindowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)から継承されました。|
|customXml|Binary|VPN 接続を構成するユーザー設定の XML コマンドです。 (UTF8 でエンコードされたバイト配列)[WindowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)から継承されました。|
|profileTarget|[windows10VpnProfileTarget](../resources/intune-deviceconfig-windows10vpnprofiletarget.md)|プロファイル対象の型。 可能な値は、`user`、`device`、`autoPilotDevice` です。|
|接続タイプ|[windows10VpnConnectionType](../resources/intune-deviceconfig-windows10vpnconnectiontype.md)|接続の種類です。 可能な値は、`pulseSecure`、`f5EdgeClient`、`dellSonicWallMobileConnect`、`checkPointCapsuleVpn`、`automatic`、`ikEv2`、`l2tp`、`pptp`、`citrix`、`paloAltoGlobalProtect` です。|
|enableSplitTunneling|Boolean|分割トンネリングを有効にします。|
|enableAlwaysOn|Boolean|常にモードを有効にします。|
|enableDeviceTunnel|Boolean|デバイスのトンネルを有効にします。|
|enableDnsRegistration|Boolean|内部の DNS の IP アドレスの登録を有効にします。|
|dnsSuffixes|String コレクション|短い形式の名前を適切にルーティングするのには DNS 検索一覧に追加する DNS サフィックスを指定します。|
|authenticationMethod|[windows10VpnAuthenticationMethod](../resources/intune-deviceconfig-windows10vpnauthenticationmethod.md)|認証方法です。 可能な値は、`certificate`、`usernameAndPassword`、`customEapXml` です。|
|rememberUserCredentials|Boolean|ユーザーの資格情報を覚えておいてください。|
|enableConditionalAccess|Boolean|条件付きのアクセスを有効にします。|
|enableSingleSignOnWithAlternateCertificate|Boolean|シングル サインオン (SSO) 代替の証明書を有効にします。|
|singleSignOnEku|[extendedKeyUsage](../resources/intune-deviceconfig-extendedkeyusage.md)|シングル サインオンの拡張キー使用法 (EKU)。|
|singleSignOnIssuerHash|String|シングル サインオンが発行元のハッシュです。|
|eapXml|Binary|プロトコル (EAP) の XML を拡張可能な認証です。 (UTF8 でエンコードされたバイト配列)|
|proxyServer|[windows10VpnProxyServer](../resources/intune-deviceconfig-windows10vpnproxyserver.md)|プロキシ サーバーです。|
|associatedApps|[windows10AssociatedApps](../resources/intune-deviceconfig-windows10associatedapps.md)コレクション|関連付けられているアプリケーションです。 このコレクションには、最大で 10000 個の要素を含めることができます。|
|onlyAssociatedAppsCanUseConnection|Boolean|関連付けられているアプリケーションだけでは、接続 (アプリケーションごとの VPN) を使用できます。|
|windowsInformationProtectionDomain|String|この接続に関連付けるには Windows の情報の保護 (WIP) のドメインです。|
|trafficRules|[vpnTrafficRule](../resources/intune-deviceconfig-vpntrafficrule.md)コレクション|トラフィックの規則。 このコレクションには、最大で 1000 個の要素を含めることができます。|
|ルート|[vpnRoute](../resources/intune-deviceconfig-vpnroute.md)コレクション|(サード パーティのプロバイダーでは省略可能) にルーティングします。 このコレクションには、最大で 1000 個の要素を含めることができます。|
|dnsRules|[vpnDnsRule](../resources/intune-deviceconfig-vpndnsrule.md)コレクション|DNS の規則。 このコレクションには、最大で 1000 個の要素を含めることができます。|
|trustedNetworkDomains|String コレクション|信頼できるネットワーク ・ ドメイン|

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
|identityCertificate|[windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md)|認証は、証明書とクライアントの認証に証明します。|

## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.windows10VpnConfiguration"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windows10VpnConfiguration",
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
  "profileTarget": "String",
  "connectionType": "String",
  "enableSplitTunneling": true,
  "enableAlwaysOn": true,
  "enableDeviceTunnel": true,
  "enableDnsRegistration": true,
  "dnsSuffixes": [
    "String"
  ],
  "authenticationMethod": "String",
  "rememberUserCredentials": true,
  "enableConditionalAccess": true,
  "enableSingleSignOnWithAlternateCertificate": true,
  "singleSignOnEku": {
    "@odata.type": "microsoft.graph.extendedKeyUsage",
    "name": "String",
    "objectIdentifier": "String"
  },
  "singleSignOnIssuerHash": "String",
  "eapXml": "binary",
  "proxyServer": {
    "@odata.type": "microsoft.graph.windows10VpnProxyServer",
    "automaticConfigurationScriptUrl": "String",
    "address": "String",
    "port": 1024,
    "bypassProxyServerForLocalAddress": true
  },
  "associatedApps": [
    {
      "@odata.type": "microsoft.graph.windows10AssociatedApps",
      "appType": "String",
      "identifier": "String"
    }
  ],
  "onlyAssociatedAppsCanUseConnection": true,
  "windowsInformationProtectionDomain": "String",
  "trafficRules": [
    {
      "@odata.type": "microsoft.graph.vpnTrafficRule",
      "name": "String",
      "protocols": 1024,
      "localPortRanges": [
        {
          "@odata.type": "microsoft.graph.numberRange",
          "lowerNumber": 1024,
          "upperNumber": 1024
        }
      ],
      "remotePortRanges": [
        {
          "@odata.type": "microsoft.graph.numberRange",
          "lowerNumber": 1024,
          "upperNumber": 1024
        }
      ],
      "localAddressRanges": [
        {
          "@odata.type": "microsoft.graph.iPv4Range",
          "lowerAddress": "String",
          "upperAddress": "String"
        }
      ],
      "remoteAddressRanges": [
        {
          "@odata.type": "microsoft.graph.iPv4Range",
          "lowerAddress": "String",
          "upperAddress": "String"
        }
      ],
      "appId": "String",
      "appType": "String",
      "routingPolicyType": "String",
      "claims": "String"
    }
  ],
  "routes": [
    {
      "@odata.type": "microsoft.graph.vpnRoute",
      "destinationPrefix": "String",
      "prefixSize": 1024
    }
  ],
  "dnsRules": [
    {
      "@odata.type": "microsoft.graph.vpnDnsRule",
      "name": "String",
      "servers": [
        "String"
      ],
      "proxyServerUri": "String",
      "autoTrigger": true,
      "persistent": true
    }
  ],
  "trustedNetworkDomains": [
    "String"
  ]
}
```




