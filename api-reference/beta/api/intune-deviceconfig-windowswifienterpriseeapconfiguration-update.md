---
title: windowsWifiEnterpriseEAPConfiguration の更新
description: windowsWifiEnterpriseEAPConfiguration オブジェクトのプロパティを更新します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: a87a8e3d4d3668c5193c44925db163df14c4bce9
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32510872"
---
# <a name="update-windowswifienterpriseeapconfiguration"></a>windowsWifiEnterpriseEAPConfiguration の更新

> **重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

[windowsWifiEnterpriseEAPConfiguration](../resources/intune-deviceconfig-windowswifienterpriseeapconfiguration.md)オブジェクトのプロパティを更新します。

## <a name="prerequisites"></a>前提条件
この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。

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
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a>要求ヘッダー
|ヘッダー|値|
|:---|:---|
|Authorization|ベアラー &lt;トークン&gt; が必要です。|
|承諾|application/json|

## <a name="request-body"></a>要求本文
要求本文で、 [windowsWifiEnterpriseEAPConfiguration](../resources/intune-deviceconfig-windowswifienterpriseeapconfiguration.md)オブジェクトの JSON 表記を指定します。

次の表に、 [windowsWifiEnterpriseEAPConfiguration](../resources/intune-deviceconfig-windowswifienterpriseeapconfiguration.md)の作成時に必要なプロパティを示します。

|プロパティ|型|説明|
|:---|:---|:---|
|id|文字列型 (String)|エンティティのキー。 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します|
|lastModifiedDateTime|DateTimeOffset|オブジェクトの最終更新の DateTime。 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します|
|roleScopeTagIds|String collection|このエンティティインスタンスの範囲タグのリスト。 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します|
|supportsScopeTags|Boolean|基になるデバイス構成がスコープタグの割り当てをサポートしているかどうかを示します。 この値が false である場合、ScopeTags プロパティへの割り当ては許可されません。エンティティは、スコープを持つユーザーには表示されません。 これは Silverlight で作成された従来のポリシーに対して実行され、Azure ポータルでポリシーを削除して再作成することによって解決できます。 このプロパティに値を設定するには、 SetExtrusionDirection メソッドを適用します。 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します|
|createdDateTime|DateTimeOffset|オブジェクトが作成された DateTime。 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します|
|説明|String|管理者が指定した、デバイス構成についての説明。 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します|
|displayName|String|管理者が指定した、デバイス構成の名前。 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します|
|version|Int32|デバイス構成のバージョン。 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します|
|preSharedKey|String|これは、WPA 個人用 wi-fi ネットワークの事前共有キーです。 [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)から継承します。|
|wifiSecurityType|[wiFiSecurityType](../resources/intune-deviceconfig-wifisecuritytype.md)|Wifi セキュリティの種類を指定します。 [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)から継承されます。 可能な値は `open`、`wpaPersonal`、`wpaEnterprise`、`wep`、`wpa2Personal`、`wpa2Enterprise` です。|
|meteredconnectionlimit|[meteredConnectionLimitType](../resources/intune-deviceconfig-meteredconnectionlimittype.md)|wifi 接続の従量制課金接続制限の種類を指定します。 [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)から継承されます。 使用可能な値は、`unrestricted`、`fixed`、`variable` です。|
|ssid|String|wifi 接続の SSID を指定します。 [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)から継承します。|
|networkname|String|ネットワーク構成名を指定します。 [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)から継承します。|
|connectautomatically に|Boolean|範囲内で wifi 接続を自動的に接続するかどうかを指定します。 [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)から継承します。|
|connecttopreferrednetwork|Boolean|この接続に既に接続されている場合に、wifi 接続がより優先度の高いネットワークに接続するかどうかを指定します。  connectautomatically 自動的に true になる必要があります。 [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)から継承します。|
|connectWhenNetworkNameIsHidden|Boolean|SSID がブロードキャストされていない場合でも、wifi 接続が自動的に接続するかどうかを指定します。 [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)から継承します。|
|proxysetting|[wiFiProxySetting](../resources/intune-deviceconfig-wifiproxysetting.md)|[windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)から継承した wi-fi 構成のプロキシ設定を指定します。 使用可能な値は、`none`、`manual`、`automatic` です。|
|proxymanualaddress|String|プロキシサーバーの IP アドレスを指定します。 [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)から継承します。|
|proxymanualport|Int32|プロキシサーバーのポートを指定します。 [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)から継承します。|
|proxyAutomaticConfigurationUrl|String|プロキシサーバー構成スクリプトの URL を指定します。 [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)から継承します。|
|forcefipscompliance|Boolean|FIPS 準拠を強制するかどうかを指定します。 [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)から継承します。|
|networkSingleSignOn|[networkSingleSignOnType](../resources/intune-deviceconfig-networksinglesignontype.md)|ネットワークのシングルサインオンの種類を指定します。 使用可能な値は、`disabled`、`prelogon`、`postlogon` です。|
|maximumAuthenticationTimeoutInSeconds|Int32|[最大認証タイムアウト (秒)] を指定します。  有効な範囲: 1-120|
|promptforadditionalauthenticationcredentials|Boolean|wifi 接続で追加の認証資格情報を求めるメッセージを表示するかどうかを指定します。|
|enablePairwiseMasterKeyCaching|Boolean|wifi 接続で、ペアワイズマスターキーのキャッシュを有効にするかどうかを指定します。|
|maximumPairwiseMasterKeyCacheTimeInMinutes|Int32|最大ペアワイズマスターキーキャッシュ時間を指定します (分単位)。  有効な範囲: 5-1440|
|maximumNumberOfPairwiseMasterKeysInCache|Int32|キャッシュ内のペアワイズマスターキーの最大数を指定します。  有効な範囲: 1-255|
|enablepreauthentication 認証|Boolean|事前認証を有効にするかどうかを指定します。|
|maximumpreauthenticationattempts|Int32|事前認証の最大試行回数を指定します。  有効な範囲: 1-16|
|eaptype|[eaptype](../resources/intune-deviceconfig-eaptype.md)|拡張認証プロトコル (EAP)。 wi-fi エンドポイント (ルーター) に設定されている EAP プロトコルの種類を示します。 可能な値は `eapTls`、`leap`、`eapSim`、`eapTtls`、`peap`、`eapFast` です。|
|trustedserverの形式|String collection|信頼されたサーバー証明書の名前を指定します。|
|authenticationMethod|[wiFiAuthenticationMethod](../resources/intune-deviceconfig-wifiauthenticationmethod.md)|認証方法を指定します。 可能な値は、`certificate`、`usernameAndPassword` です。|
|innerAuthenticationProtocolForEAPTTLS|[none apauthenticationmethod_ apttlstype](../resources/intune-deviceconfig-noneapauthenticationmethodforeapttlstype.md)|EAP TTLS の内部認証プロトコルを指定します。 可能な値は、`unencryptedPassword`、`challengeHandshakeAuthenticationProtocol`、`microsoftChap`、`microsoftChapVersionTwo` です。|
|outerIdentityPrivacyTemporaryValue|String|EAP TTLS または PEAP を使用している場合は、プライバシー保護のために、ユーザー名を置換する文字列を指定します。|



## <a name="response"></a>応答
成功した場合、このメソッド`200 OK`は応答コードと、応答本文で更新された[windowsWifiEnterpriseEAPConfiguration](../resources/intune-deviceconfig-windowswifienterpriseeapconfiguration.md)オブジェクトを返します。

## <a name="example"></a>例

### <a name="request"></a>要求
以下は、要求の例です。
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
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
HTTP/1.1 200 OK
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





