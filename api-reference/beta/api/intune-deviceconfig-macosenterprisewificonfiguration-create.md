---
title: MacOSEnterpriseWiFiConfiguration を作成します。
description: 新しい macOSEnterpriseWiFiConfiguration オブジェクトを作成します。
ms.openlocfilehash: 5fa8a3e0751d39d4fae329b369c56d836d31cd77
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27069962"
---
# <a name="create-macosenterprisewificonfiguration"></a>MacOSEnterpriseWiFiConfiguration を作成します。

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

> **注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。

新しい[macOSEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-macosenterprisewificonfiguration.md)オブジェクトを作成します。
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
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a>要求ヘッダー
|ヘッダー|値|
|:---|:---|
|Authorization|ベアラー &lt;トークン&gt; が必須。|
|Accept|application/json|

## <a name="request-body"></a>要求本文
要求の本文に macOSEnterpriseWiFiConfiguration オブジェクトの JSON の形式を指定します。

次の表は、macOSEnterpriseWiFiConfiguration を作成するときに必要なプロパティを示します。

|プロパティ|型|説明|
|:---|:---|:---|
|id|String|エンティティのキー。 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します|
|lastModifiedDateTime|DateTimeOffset|オブジェクトが最後に変更された DateTime。 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します|
|roleScopeTagIds|String コレクション|このエンティティ インスタンスのスコープのタグのリストです。 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します|
|supportsScopeTags|Boolean|デバイスの構成を基になるスコープのタグの割り当てをサポートしているかどうかを示します。 この値が false であり、エンティティをスコープ指定されたユーザーには表示されませんがある場合、ScopeTags プロパティに割り当てることは許可されていません。 これは、Silverlight で作成されたレガシ ポリシーに対して発生し、削除して、Azure ポータル内のポリシーを再作成することで解決できます。 このプロパティは値の取得のみ可能です。 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します|
|createdDateTime|DateTimeOffset|オブジェクトが作成された DateTime。 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します|
|説明|String|デバイス構成について管理者が提供した説明。 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します|
|displayName|String|デバイス構成について管理者が指定した名前。 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します|
|version|Int32|デバイス構成のバージョン。 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します|
|ネットワーク名リソース|String|ネットワーク名は、 [macOSWiFiConfiguration](../resources/intune-deviceconfig-macoswificonfiguration.md)から継承されました。|
|ssid|String|これは、すべてのデバイスにブロードキャストされている Wi-fi ネットワークの名前です。 [MacOSWiFiConfiguration](../resources/intune-deviceconfig-macoswificonfiguration.md)から継承されました。|
|connectAutomatically|Boolean|このネットワークが範囲内にすると自動的に接続します。 これを true に設定、ユーザー プロンプトを省略して自動的に Wi-fi ネットワークにデバイスを接続します。 [MacOSWiFiConfiguration](../resources/intune-deviceconfig-macoswificonfiguration.md)から継承されました。|
|connectWhenNetworkNameIsHidden|Boolean|ネットワーク名 (SSID) をブロードキャストしていないときに接続します。 True の場合、このプロファイルに設定されているすべてのデバイスに SSID をブロードキャストしていないネットワークに接続するデバイスを強制します。 [MacOSWiFiConfiguration](../resources/intune-deviceconfig-macoswificonfiguration.md)から継承されました。|
|wiFiSecurityType|[wiFiSecurityType](../resources/intune-deviceconfig-wifisecuritytype.md)|Wi-fi エンドポイントがベースの EAP セキュリティ タイプを使用するかどうかを示します。 [MacOSWiFiConfiguration](../resources/intune-deviceconfig-macoswificonfiguration.md)から継承されます。 使用可能な値: `open`、`wpaPersonal`、`wpaEnterprise`、`wep`、`wpa2Personal`、`wpa2Enterprise`。|
|型のオブジェクトで|[wiFiProxySetting](../resources/intune-deviceconfig-wifiproxysetting.md)|[MacOSWiFiConfiguration](../resources/intune-deviceconfig-macoswificonfiguration.md)から継承される Wi-fi 接続のプロキシの種類です。 可能な値は、`none`、`manual`、`automatic` です。|
|proxyManualAddress|String|手動の構成が選択されている時にプロキシ サーバーの IP アドレスまたは DNS ホスト名 [MacOSWiFiConfiguration](../resources/intune-deviceconfig-macoswificonfiguration.md)から継承されました。|
|proxyManualPort|Int32|手動の構成が選択されている時にプロキシ サーバーのポートです。 [MacOSWiFiConfiguration](../resources/intune-deviceconfig-macoswificonfiguration.md)から継承されました。|
|proxyAutomaticConfigurationUrl|String|自動構成を選択すると、プロキシ サーバーの自動構成スクリプトの URL です。 この URL は、通常、PAC (プロキシの自動構成) ファイルの場所です。 [MacOSWiFiConfiguration](../resources/intune-deviceconfig-macoswificonfiguration.md)から継承されました。|
|preSharedKey|String|これは、WPA パーソナル Wi-fi ネットワークの事前共有キーです。 [MacOSWiFiConfiguration](../resources/intune-deviceconfig-macoswificonfiguration.md)から継承されました。|
|eapType|[eapType](../resources/intune-deviceconfig-eaptype.md)|拡張認証プロトコル (EAP) です。 [EAP プロトコルの種類を示します、Wi-fi エンドポイント (ルーター)。 使用可能な値: `eapTls`、`leap`、`eapSim`、`eapTtls`、`peap`、`eapFast`。|
|eapFastConfiguration|[eapFastConfiguration](../resources/intune-deviceconfig-eapfastconfiguration.md)|EAP-FAST 構成オプションには、EAP-FAST の場合は、選択した EAP の種類です。 可能な値は、`noProtectedAccessCredential`、`useProtectedAccessCredential`、`useProtectedAccessCredentialAndProvision`、`useProtectedAccessCredentialAndProvisionAnonymously` です。|
|trustedServerCertificateNames|String コレクション|EAP-TLS または TTLS/高速または PEAP に EAP の種類が構成されている場合は、サーバー証明書の名前を信頼されています。 これは、信頼された証明機関 (CA) によって発行された証明書で使用される一般的な名前です。 この情報を入力する場合は、この Wi-fi ネットワークに接続するときは、エンド ・ ユーザーのデバイスに表示されている動的な信頼] ダイアログを回避できます。|
|authenticationMethod|[wiFiAuthenticationMethod](../resources/intune-deviceconfig-wifiauthenticationmethod.md)|PEAP や EAP TTLS に EAP の種類が構成されている場合の認証方法です。 使用可能な値は、`certificate`、`usernameAndPassword` です。|
|innerAuthenticationProtocolForEapTtls|[nonEapAuthenticationMethodForEapTtlsType](../resources/intune-deviceconfig-noneapauthenticationmethodforeapttlstype.md)|(内部) するときのユーザーは EAP TTLS、EAP の種類の認証と Authenticationmethod の非 EAP メソッドは、ユーザー名とパスワードです。 可能な値は、`unencryptedPassword`、`challengeHandshakeAuthenticationProtocol`、`microsoftChap`、`microsoftChapVersionTwo` です。|
|outerIdentityPrivacyTemporaryValue|String|EAP-TTLS、高速の EAP または PEAP を EAP の種類を構成すると id プライバシー (外部ユーザー) を使用できます。 このプロパティは、テキストを入力するユーザー名をマスクします。 たとえば、'匿名' を使用する場合は、実際のユーザー名を使用してこの Wi-fi 接続で認証する各ユーザーが '匿名' として表示されます。|



## <a name="response"></a>応答
かどうかは成功すると、このメソッドが返されます、`201 Created`応答コードおよび応答の本文に[macOSEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-macosenterprisewificonfiguration.md)オブジェクトです。

## <a name="example"></a>例
### <a name="request"></a>要求
以下は、要求の例です。
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 1149

{
  "@odata.type": "#microsoft.graph.macOSEnterpriseWiFiConfiguration",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "networkName": "Network Name value",
  "ssid": "Ssid value",
  "connectAutomatically": true,
  "connectWhenNetworkNameIsHidden": true,
  "wiFiSecurityType": "wpaPersonal",
  "proxySettings": "manual",
  "proxyManualAddress": "Proxy Manual Address value",
  "proxyManualPort": 15,
  "proxyAutomaticConfigurationUrl": "https://example.com/proxyAutomaticConfigurationUrl/",
  "preSharedKey": "Pre Shared Key value",
  "eapType": "leap",
  "eapFastConfiguration": "useProtectedAccessCredential",
  "trustedServerCertificateNames": [
    "Trusted Server Certificate Names value"
  ],
  "authenticationMethod": "usernameAndPassword",
  "innerAuthenticationProtocolForEapTtls": "challengeHandshakeAuthenticationProtocol",
  "outerIdentityPrivacyTemporaryValue": "Outer Identity Privacy Temporary Value value"
}
```

### <a name="response"></a>応答
以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1257

{
  "@odata.type": "#microsoft.graph.macOSEnterpriseWiFiConfiguration",
  "id": "7a6f9a2e-9a2e-7a6f-2e9a-6f7a2e9a6f7a",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "networkName": "Network Name value",
  "ssid": "Ssid value",
  "connectAutomatically": true,
  "connectWhenNetworkNameIsHidden": true,
  "wiFiSecurityType": "wpaPersonal",
  "proxySettings": "manual",
  "proxyManualAddress": "Proxy Manual Address value",
  "proxyManualPort": 15,
  "proxyAutomaticConfigurationUrl": "https://example.com/proxyAutomaticConfigurationUrl/",
  "preSharedKey": "Pre Shared Key value",
  "eapType": "leap",
  "eapFastConfiguration": "useProtectedAccessCredential",
  "trustedServerCertificateNames": [
    "Trusted Server Certificate Names value"
  ],
  "authenticationMethod": "usernameAndPassword",
  "innerAuthenticationProtocolForEapTtls": "challengeHandshakeAuthenticationProtocol",
  "outerIdentityPrivacyTemporaryValue": "Outer Identity Privacy Temporary Value value"
}
```





