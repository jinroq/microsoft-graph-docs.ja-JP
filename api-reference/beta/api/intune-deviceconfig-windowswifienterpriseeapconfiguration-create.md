---
title: WindowsWifiEnterpriseEAPConfiguration を作成します。
description: 新しい windowsWifiEnterpriseEAPConfiguration オブジェクトを作成します。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: f3ab25f8d74546bd75d4fdc65cc5306fd4c48d25
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29413480"
---
# <a name="create-windowswifienterpriseeapconfiguration"></a>WindowsWifiEnterpriseEAPConfiguration を作成します。

> **重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。 実稼働アプリケーションでこれらの API を使用することは、サポートされていません。

> **注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

新しい[windowsWifiEnterpriseEAPConfiguration](../resources/intune-deviceconfig-windowswifienterpriseeapconfiguration.md)オブジェクトを作成します。

## <a name="prerequisites"></a>前提条件
この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/concepts/permissions-reference.md)」を参照してください。

|アクセス許可の種類|アクセス許可 (特権の大きいものから小さいものへ)|
|:---|:---|
|委任 (職場または学校のアカウント)|DeviceManagementConfiguration.ReadWrite.All|
|委任 (個人用 Microsoft アカウント)|サポートされていません。|
|アプリケーション|サポートされていません。|

## <a name="http-request"></a>HTTP 要求
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a>要求ヘッダー
|ヘッダー|値|
|:---|:---|
|Authorization|ベアラー &lt;トークン&gt; が必須。|
|Accept|application/json|

## <a name="request-body"></a>要求本文
要求の本文に windowsWifiEnterpriseEAPConfiguration オブジェクトの JSON の形式を指定します。

次の表は、windowsWifiEnterpriseEAPConfiguration を作成するときに必要なプロパティを示します。

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



## <a name="response"></a>応答
かどうかは成功すると、このメソッドが返されます、`201 Created`応答コードおよび応答の本文に[windowsWifiEnterpriseEAPConfiguration](../resources/intune-deviceconfig-windowswifienterpriseeapconfiguration.md)オブジェクトです。

## <a name="example"></a>例

### <a name="request"></a>要求
以下は、要求の例です。
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 1504

{
  "@odata.type": "#microsoft.graph.windowsWifiEnterpriseEAPConfiguration",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "preSharedKey": "Pre Shared Key value",
  "wifiSecurityType": "wpaPersonal",
  "meteredConnectionLimit": "fixed",
  "ssid": "Ssid value",
  "networkName": "Network Name value",
  "connectAutomatically": true,
  "connectToPreferredNetwork": true,
  "connectWhenNetworkNameIsHidden": true,
  "proxySetting": "manual",
  "proxyManualAddress": "Proxy Manual Address value",
  "proxyManualPort": 15,
  "proxyAutomaticConfigurationUrl": "https://example.com/proxyAutomaticConfigurationUrl/",
  "forceFIPSCompliance": true,
  "networkSingleSignOn": "prelogon",
  "maximumAuthenticationTimeoutInSeconds": 5,
  "promptForAdditionalAuthenticationCredentials": true,
  "enablePairwiseMasterKeyCaching": true,
  "maximumPairwiseMasterKeyCacheTimeInMinutes": 10,
  "maximumNumberOfPairwiseMasterKeysInCache": 8,
  "enablePreAuthentication": true,
  "maximumPreAuthenticationAttempts": 0,
  "eapType": "leap",
  "trustedServerCertificateNames": [
    "Trusted Server Certificate Names value"
  ],
  "authenticationMethod": "usernameAndPassword",
  "innerAuthenticationProtocolForEAPTTLS": "challengeHandshakeAuthenticationProtocol",
  "outerIdentityPrivacyTemporaryValue": "Outer Identity Privacy Temporary Value value"
}
```

### <a name="response"></a>応答
以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1676

{
  "@odata.type": "#microsoft.graph.windowsWifiEnterpriseEAPConfiguration",
  "id": "7e7183ac-83ac-7e71-ac83-717eac83717e",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "preSharedKey": "Pre Shared Key value",
  "wifiSecurityType": "wpaPersonal",
  "meteredConnectionLimit": "fixed",
  "ssid": "Ssid value",
  "networkName": "Network Name value",
  "connectAutomatically": true,
  "connectToPreferredNetwork": true,
  "connectWhenNetworkNameIsHidden": true,
  "proxySetting": "manual",
  "proxyManualAddress": "Proxy Manual Address value",
  "proxyManualPort": 15,
  "proxyAutomaticConfigurationUrl": "https://example.com/proxyAutomaticConfigurationUrl/",
  "forceFIPSCompliance": true,
  "networkSingleSignOn": "prelogon",
  "maximumAuthenticationTimeoutInSeconds": 5,
  "promptForAdditionalAuthenticationCredentials": true,
  "enablePairwiseMasterKeyCaching": true,
  "maximumPairwiseMasterKeyCacheTimeInMinutes": 10,
  "maximumNumberOfPairwiseMasterKeysInCache": 8,
  "enablePreAuthentication": true,
  "maximumPreAuthenticationAttempts": 0,
  "eapType": "leap",
  "trustedServerCertificateNames": [
    "Trusted Server Certificate Names value"
  ],
  "authenticationMethod": "usernameAndPassword",
  "innerAuthenticationProtocolForEAPTTLS": "challengeHandshakeAuthenticationProtocol",
  "outerIdentityPrivacyTemporaryValue": "Outer Identity Privacy Temporary Value value"
}
```




