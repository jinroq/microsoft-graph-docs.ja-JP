---
title: windowsWifiEnterpriseEAPConfiguration リソースの種類
description: このエンティティは、宣言されたメソッド、プロパティ、および Wifi CSP によって公開されているリレーションシップの説明を提供します。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 1c5e7f92c8b84512ae71144d379a38eac24eb08c
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29407096"
---
# <a name="windowswifienterpriseeapconfiguration-resource-type"></a>windowsWifiEnterpriseEAPConfiguration リソースの種類

> **重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。 実稼働アプリケーションでこれらの API を使用することは、サポートされていません。

> **注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

このエンティティは、宣言されたメソッド、プロパティ、および Wifi CSP によって公開されているリレーションシップの説明を提供します。


[WindowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)から継承します。

## <a name="methods"></a>メソッド
|メソッド|戻り値の型|説明|
|:---|:---|:---|
|[リスト windowsWifiEnterpriseEAPConfigurations](../api/intune-deviceconfig-windowswifienterpriseeapconfiguration-list.md)|[windowsWifiEnterpriseEAPConfiguration](../resources/intune-deviceconfig-windowswifienterpriseeapconfiguration.md)コレクション|[WindowsWifiEnterpriseEAPConfiguration](../resources/intune-deviceconfig-windowswifienterpriseeapconfiguration.md)オブジェクトのプロパティと関係を一覧表示します。|
|[WindowsWifiEnterpriseEAPConfiguration を取得します。](../api/intune-deviceconfig-windowswifienterpriseeapconfiguration-get.md)|[windowsWifiEnterpriseEAPConfiguration](../resources/intune-deviceconfig-windowswifienterpriseeapconfiguration.md)|[WindowsWifiEnterpriseEAPConfiguration](../resources/intune-deviceconfig-windowswifienterpriseeapconfiguration.md)オブジェクトのプロパティと関係を参照してください。|
|[WindowsWifiEnterpriseEAPConfiguration を作成します。](../api/intune-deviceconfig-windowswifienterpriseeapconfiguration-create.md)|[windowsWifiEnterpriseEAPConfiguration](../resources/intune-deviceconfig-windowswifienterpriseeapconfiguration.md)|新しい[windowsWifiEnterpriseEAPConfiguration](../resources/intune-deviceconfig-windowswifienterpriseeapconfiguration.md)オブジェクトを作成します。|
|[WindowsWifiEnterpriseEAPConfiguration を削除します。](../api/intune-deviceconfig-windowswifienterpriseeapconfiguration-delete.md)|なし|の[windowsWifiEnterpriseEAPConfiguration](../resources/intune-deviceconfig-windowswifienterpriseeapconfiguration.md)を削除します。|
|[WindowsWifiEnterpriseEAPConfiguration を更新します。](../api/intune-deviceconfig-windowswifienterpriseeapconfiguration-update.md)|[windowsWifiEnterpriseEAPConfiguration](../resources/intune-deviceconfig-windowswifienterpriseeapconfiguration.md)|[WindowsWifiEnterpriseEAPConfiguration](../resources/intune-deviceconfig-windowswifienterpriseeapconfiguration.md)オブジェクトのプロパティを更新します。|

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
|preSharedKey|String|これは、WPA パーソナル Wi-fi ネットワークの事前共有キーです。 [WindowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)から継承されました。|
|wifiSecurityType|[wiFiSecurityType](../resources/intune-deviceconfig-wifisecuritytype.md)|Wifi セキュリティの種類を指定します。 [WindowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)から継承されます。 使用可能な値: `open`、`wpaPersonal`、`wpaEnterprise`、`wep`、`wpa2Personal`、`wpa2Enterprise`。|
|meteredConnectionLimit|[meteredConnectionLimitType](../resources/intune-deviceconfig-meteredconnectionlimittype.md)|Wifi 接続のメータリングされた接続の制限の種類を指定します。 [WindowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)から継承されます。 可能な値は、`unrestricted`、`fixed`、`variable` です。|
|ssid|String|Wifi 接続の SSID を指定します。 [WindowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)から継承されました。|
|ネットワーク名リソース|String|ネットワーク構成の名前を指定します。 [WindowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)から継承されました。|
|connectAutomatically|Boolean|範囲で wifi 接続が自動的に接続する必要があるかどうかを指定します。 [WindowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)から継承されました。|
|connectToPreferredNetwork|Boolean|Wifi 接続は、この 1 つに既に接続されている場合より優先するネットワークに接続する必要があるかどうかを指定します。  True を指定する ConnectAutomatically が必要です。 [WindowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)から継承されました。|
|connectWhenNetworkNameIsHidden|Boolean|かどうか、wifi 接続自動的にでもすると、SSID をブロードキャストしていないかを指定します。 [WindowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)から継承されました。|
|proxySetting|[wiFiProxySetting](../resources/intune-deviceconfig-wifiproxysetting.md)|プロキシの[windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)から Wi-fi 設定の継承の設定を指定します。 可能な値は、`none`、`manual`、`automatic` です。|
|proxyManualAddress|String|プロキシ サーバーの IP アドレスを指定します。 [WindowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)から継承されました。|
|proxyManualPort|Int32|プロキシ サーバーのポートを指定します。 [WindowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)から継承されました。|
|proxyAutomaticConfigurationUrl|String|プロキシ サーバーの構成スクリプトの URL を指定します。 [WindowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)から継承されました。|
|forceFIPSCompliance|Boolean|FIPS 準拠を強制するかどうかを指定します。 [WindowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)から継承されました。|
|networkSingleSignOn|[networkSingleSignOnType](../resources/intune-deviceconfig-networksinglesignontype.md)|型のネットワークの 1 つの記号を指定します。 可能な値は、`disabled`、`prelogon`、`postlogon` です。|
|maximumAuthenticationTimeoutInSeconds|Int32|認証の最大タイムアウトを秒単位で指定します。  有効範囲: 1 ~ 120|
|promptForAdditionalAuthenticationCredentials|Boolean|Wifi 接続がその他の認証の資格情報を促す必要があるかどうかを指定します。|
|enablePairwiseMasterKeyCaching|Boolean|Wifi 接続する必要がありますペアワイズ マスター_キーのキーのキャッシュを有効にするかどうかを指定します。|
|maximumPairwiseMasterKeyCacheTimeInMinutes|Int32|ペアワイズ マスター_キーの最大キャッシュ時間 (分単位) を指定します。  有効範囲: 5-1440|
|maximumNumberOfPairwiseMasterKeysInCache|Int32|キャッシュでは、ペアワイズ マスター_キーの最大数を指定します。  有効範囲: 1-255|
|enablePreAuthentication|Boolean|事前認証を有効にする必要があるかどうかを指定します。|
|maximumPreAuthenticationAttempts|Int32|事前認証の最大試行回数を指定します。  有効範囲: 1 ~ 16|
|eapType|[eapType](../resources/intune-deviceconfig-eaptype.md)|拡張認証プロトコル (EAP) です。 [EAP プロトコルの種類を示します、Wi-fi エンドポイント (ルーター)。 使用可能な値: `eapTls`、`leap`、`eapSim`、`eapTtls`、`peap`、`eapFast`。|
|trustedServerCertificateNames|String コレクション|信頼されたサーバー証明書名を指定します。|
|authenticationMethod|[wiFiAuthenticationMethod](../resources/intune-deviceconfig-wifiauthenticationmethod.md)|認証方法を指定します。 使用可能な値は、`certificate`、`usernameAndPassword` です。|
|innerAuthenticationProtocolForEAPTTLS|[nonEapAuthenticationMethodForEapTtlsType](../resources/intune-deviceconfig-noneapauthenticationmethodforeapttlstype.md)|EAP TTLS の内部認証プロトコルを指定します。 可能な値は、`unencryptedPassword`、`challengeHandshakeAuthenticationProtocol`、`microsoftChap`、`microsoftChapVersionTwo` です。|
|outerIdentityPrivacyTemporaryValue|String|EAP TTLS または PEAP を使用する場合は、プライバシー保護のためのユーザー名を置換する文字列を指定します。|

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
|rootCertificatesForServerValidation|[windows81TrustedRootCertificate](../resources/intune-deviceconfig-windows81trustedrootcertificate.md)コレクション|サーバー検証のためのルート証明書を指定します。|
|identityCertificateForClientAuthentication|[windowsCertificateProfileBase](../resources/intune-deviceconfig-windowscertificateprofilebase.md)|クライアント認証用の id の証明書を指定します。|

## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.windowsWifiEnterpriseEAPConfiguration"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsWifiEnterpriseEAPConfiguration",
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
  "preSharedKey": "String",
  "wifiSecurityType": "String",
  "meteredConnectionLimit": "String",
  "ssid": "String",
  "networkName": "String",
  "connectAutomatically": true,
  "connectToPreferredNetwork": true,
  "connectWhenNetworkNameIsHidden": true,
  "proxySetting": "String",
  "proxyManualAddress": "String",
  "proxyManualPort": 1024,
  "proxyAutomaticConfigurationUrl": "String",
  "forceFIPSCompliance": true,
  "networkSingleSignOn": "String",
  "maximumAuthenticationTimeoutInSeconds": 1024,
  "promptForAdditionalAuthenticationCredentials": true,
  "enablePairwiseMasterKeyCaching": true,
  "maximumPairwiseMasterKeyCacheTimeInMinutes": 1024,
  "maximumNumberOfPairwiseMasterKeysInCache": 1024,
  "enablePreAuthentication": true,
  "maximumPreAuthenticationAttempts": 1024,
  "eapType": "String",
  "trustedServerCertificateNames": [
    "String"
  ],
  "authenticationMethod": "String",
  "innerAuthenticationProtocolForEAPTTLS": "String",
  "outerIdentityPrivacyTemporaryValue": "String"
}
```




