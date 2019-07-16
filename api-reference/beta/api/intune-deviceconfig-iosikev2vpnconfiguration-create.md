---
title: IosikEv2VpnConfiguration を作成する
description: 新しい iosikEv2VpnConfiguration オブジェクトを作成します。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 7635a187a399e74498b91d72b7f8cae6a0678a61
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35715390"
---
# <a name="create-iosikev2vpnconfiguration"></a>IosikEv2VpnConfiguration を作成する

> **重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

新しい[iosikEv2VpnConfiguration](../resources/intune-deviceconfig-iosikev2vpnconfiguration.md)オブジェクトを作成します。

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
|Authorization|ベアラー &lt;トークン&gt; が必要です。|
|承諾|application/json|

## <a name="request-body"></a>要求本文
要求本文で、iosikEv2VpnConfiguration オブジェクトの JSON 表記を指定します。

次の表に、iosikEv2VpnConfiguration の作成時に必要なプロパティを示します。

|プロパティ|型|説明|
|:---|:---|:---|
|id|文字列|エンティティのキー。 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します|
|lastModifiedDateTime|DateTimeOffset|オブジェクトの最終更新の DateTime。 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します|
|roleScopeTagIds|文字列コレクション|このエンティティインスタンスの範囲タグのリスト。 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します|
|supportsScopeTags|Boolean|基になるデバイス構成がスコープタグの割り当てをサポートしているかどうかを示します。 この値が false である場合、ScopeTags プロパティへの割り当ては許可されません。エンティティは、スコープを持つユーザーには表示されません。 これは Silverlight で作成された従来のポリシーに対して実行され、Azure ポータルでポリシーを削除して再作成することによって解決できます。 このプロパティに値を設定するには、 SetExtrusionDirection メソッドを適用します。 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します|
|deviceManagementApplicabilityRuleOsEdition|[deviceManagementApplicabilityRuleOsEdition](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|このポリシーの OS エディションの適用。 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します|
|deviceManagementApplicabilityRuleOsVersion|[deviceManagementApplicabilityRuleOsVersion](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|このポリシーの OS バージョン適用ルール。 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します|
|Devicemanagementの信頼性ルール Devicemode|[Devicemanagementの信頼性ルール Devicemode](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|このポリシーのデバイスモード適用ルール。 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します|
|createdDateTime|DateTimeOffset|オブジェクトが作成された DateTime。 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します|
|description|String|管理者が指定した、デバイス構成についての説明。 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します|
|displayName|String|管理者が指定した、デバイス構成の名前。 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します|
|version|Int32|デバイス構成のバージョン。 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します|
|connectionName|String|ユーザーに表示される接続名。 [りんご Evpnconfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)からの継承|
|connectionType|[appleVpnConnectionType](../resources/intune-deviceconfig-applevpnconnectiontype.md)|接続の種類。 [[りんご Evpnconfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)から継承します。 可能な値は`ciscoAnyConnect`、 `pulseSecure`、 `f5EdgeClient` `dellSonicWallMobileConnect` `checkPointCapsuleVpn` `customVpn` `ciscoIPSec` `citrix` `ciscoAnyConnectV2` `ikEv2`、、 `paloAltoGlobalProtect`、、、、、、、、、、、、です。 `zscalerPrivateAccess` `f5Access2018` `citrixSso` `paloAltoGlobalProtectV2`|
|loginGroupOrDomain|String|接続の種類が Dell SonicWALL Mobile Connection に設定されている場合のログイングループまたはドメイン。 [りんご Evpnconfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)からの継承|
|role|String|接続の種類がパルス Secure に設定されている場合の役割。 [りんご Evpnconfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)からの継承|
|領域|String|接続の種類がパルス Secure に設定されている場合の領域。 [りんご Evpnconfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)からの継承|
|server|[vpnServer](../resources/intune-deviceconfig-vpnserver.md)|ネットワーク上の VPN サーバー。 エンドユーザーがこのネットワークの場所にアクセスできることを確認します。 [りんご Evpnconfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)からの継承|
|識別子|String|接続の種類がカスタム VPN に設定されている場合に、VPN ベンダーによって提供される識別子。 例: Cisco AnyConnect は、[りんご Evpnconfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)から継承したフォームの識別子を使用しています。|
|customData|[keyvalue](../resources/intune-deviceconfig-keyvalue.md) コレクション|カスタムデータ接続の種類がカスタム VPN に設定されている場合。 このフィールドを使用して、Intune によってサポートされていないが、VPN ソリューションで利用可能な機能を有効にします。 これらのキーと値のペアを追加する方法については、VPN ベンダーに問い合わせてください。 このコレクションには、最大25個の要素を含めることができます。 [りんご Evpnconfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)からの継承|
|customKeyValueData|[keyValuePair](../resources/intune-shared-keyvaluepair.md) コレクション|カスタムデータ接続の種類がカスタム VPN に設定されている場合。 このフィールドを使用して、Intune によってサポートされていないが、VPN ソリューションで利用可能な機能を有効にします。 これらのキーと値のペアを追加する方法については、VPN ベンダーに問い合わせてください。 このコレクションには、最大25個の要素を含めることができます。 [りんご Evpnconfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)からの継承|
|enableSplitTunneling|Boolean|すべてのネットワークトラフィックを VPN 経由で送信します。 [りんご Evpnconfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)からの継承|
|authenticationMethod|[vpnAuthenticationMethod](../resources/intune-deviceconfig-vpnauthenticationmethod.md)|この VPN 接続の認証方法。 [[りんご Evpnconfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)から継承します。 使用可能な値は、`certificate`、`usernameAndPassword`、`sharedSecret`、`derivedCredential` です。|
|enablePerApp|Boolean|この値を true に設定すると、エンドユーザーの iOS デバイス上でこの VPN 接続をトリガーできるアプリに後で関連付けることができるアプリごとの VPN ペイロードが作成されます。 [りんご Evpnconfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)からの継承|
|Saf Aridomains|文字列コレクション|この VPN がアプリごとの設定が有効になっている場合の Safari ドメイン この VPN に関連付けられているアプリに加えて、ここで指定した Safari ドメインもこの VPN 接続をトリガーすることができます。 [りんご Evpnconfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)からの継承|
|onDemandRules|[vpnOnDemandRule](../resources/intune-deviceconfig-vpnondemandrule.md)コレクション|オンデマンドルール。 このコレクションには、最大で 500 個の要素を含めることができます。 [りんご Evpnconfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)からの継承|
|proxyServer|[vpnProxyServer](../resources/intune-deviceconfig-vpnproxyserver.md)|プロキシサーバー。 [りんご Evpnconfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)からの継承|
|optInToDeviceIdSharing|Boolean|ネットワークアクセス制御の検証時に使用するために、デバイスの Id をサードパーティの vpn クライアントに共有するオプトイン。 [りんご Evpnconfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)からの継承|
|providerType|[vpnProviderType](../resources/intune-deviceconfig-vpnprovidertype.md)|アプリごとの VPN のプロバイダーの種類。 [Iosvpnconfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md)から継承されます。 可能な値は、`notConfigured`、`appProxy`、`packetTunnel` です。|
|Userdomain に|String|Zscaler のみ。 Zscaler アプリでログインフィールドに事前設定するには、静的ドメインを入力します。 この指定を省略すると、代わりにユーザーの Azure Active Directory ドメインが使用されます。 [Iosvpnconfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md)から継承します|
|Cloudname|Boolean|Zscaler のみ。 ユーザーが Zscaler アプリにサインインするまでネットワークトラフィックをブロックします。 "True" はトラフィックがブロックされることを意味します。 [Iosvpnconfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md)から継承します|
|cloudName|String|Zscaler のみ。 ユーザーが割り当てられている Zscaler cloud。 [Iosvpnconfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md)から継承します|
|excludeList|文字列コレクション|Zscaler のみ。 Zscaler クラウド経由で送信されないネットワークアドレスのリスト。 [Iosvpnconfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md)から継承します|
|childSecurityAssociationParameters|[iosVpnSecurityAssociationParameters](../resources/intune-deviceconfig-iosvpnsecurityassociationparameters.md)|子のセキュリティアソシエーションのパラメーター|
|clientAuthenticationType|[vpnClientAuthenticationType](../resources/intune-deviceconfig-vpnclientauthenticationtype.md)|VPN クライアントが使用するクライアント認証の種類。 可能な値は、`userAuthentication`、`deviceAuthentication` です。|
|deadPeerDetectionRate|[vpnDeadPeerDetectionRate](../resources/intune-deviceconfig-vpndeadpeerdetectionrate.md)|ピア接続がまだアクティブであるかどうかを確認する頻度を決定します。 . 使用可能な値は、`medium`、`none`、`low`、`high` です。|
|disableMobilityAndMultihoming|Boolean|MOBIKE を無効にする|
|disableRedirect|Boolean|リダイレクトを無効にする|
|enableCertificateRevocationCheck|Boolean|ベストエフォート型の失効チェックを有効にします。サーバー応答のタイムアウトによって失敗しない|
|enableEAP|Boolean|EAP のみの認証を有効にします|
|enablePerfectForwardSecrecy|Boolean|完全な転送機密性 (PFS) を有効にします。|
|Enableuseinternalサブネット属性|Boolean|内部サブネット属性の使用を有効にします。|
|localIdentifier|[vpnLocalIdentifier](../resources/intune-deviceconfig-vpnlocalidentifier.md)|VPN 経由で接続しようとしているクライアントを識別する方法。 . 可能な値は、`deviceFQDN`、`empty`、`clientCertificateSubjectName` です。|
|remoteIdentifier|String|IKEv2 サーバーのアドレス。 FQDN、UserFQDN、ネットワークアドレス、または ASN1DN である必要があります。|
|securityAssociationParameters|[iosVpnSecurityAssociationParameters](../resources/intune-deviceconfig-iosvpnsecurityassociationparameters.md)|セキュリティアソシエーションパラメーター|
|Server指定 Ecommonname|String|サーバー認証で使用される IKEv2 サーバー証明書の共通名|
|serverCertificateIssuerCommonName|String|認証で使用される IKEv2 サーバー証明書発行者の共通名|
|serverCertificateType|[vpnServerCertificateType](../resources/intune-deviceconfig-vpnservercertificatetype.md)|Vpn サーバーが認証のために VPN クライアントに提示する証明書の種類。 使用可能な値は、`rsa`、`ecdsa256`、`ecdsa384`、`ecdsa521` です。|
|sharedSecret|String|共有シークレット認証が選択されている場合に使用|
|tlsMaximumVersion|String|Eap-tls 認証で使用される最大 TLS バージョン|
|tlsMinimumVersion|String|Eap-tls 認証で使用する最低限の TLS バージョン|
|allowDefaultSecurityAssociationParameters|Boolean|明示的に指定されていない限り、すべてのパラメーターをデバイスの既定値に設定することによって、セキュリティアソシエーションパラメーターを使用できるようにします。|
|allowDefaultChildSecurityAssociationParameters|Boolean|明示的に指定されていない限り、すべてのパラメーターをデバイスの既定値に設定することによって、子のセキュリティアソシエーションのパラメーターを使用できるようにします。|



## <a name="response"></a>応答
成功した場合、このメソッド`201 Created`は応答コードと、応答本文で[iosikEv2VpnConfiguration](../resources/intune-deviceconfig-iosikev2vpnconfiguration.md)オブジェクトを返します。

## <a name="example"></a>例

### <a name="request"></a>要求
以下は、要求の例です。
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 4232

{
  "@odata.type": "#microsoft.graph.iosikEv2VpnConfiguration",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "deviceManagementApplicabilityRuleOsEdition": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleOsEdition",
    "osEditionTypes": [
      "windows10EnterpriseN"
    ],
    "name": "Name value",
    "ruleType": "exclude"
  },
  "deviceManagementApplicabilityRuleOsVersion": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleOsVersion",
    "minOSVersion": "Min OSVersion value",
    "maxOSVersion": "Max OSVersion value",
    "name": "Name value",
    "ruleType": "exclude"
  },
  "deviceManagementApplicabilityRuleDeviceMode": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleDeviceMode",
    "deviceMode": "sModeConfiguration",
    "name": "Name value",
    "ruleType": "exclude"
  },
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "connectionName": "Connection Name value",
  "connectionType": "pulseSecure",
  "loginGroupOrDomain": "Login Group Or Domain value",
  "role": "Role value",
  "realm": "Realm value",
  "server": {
    "@odata.type": "microsoft.graph.vpnServer",
    "description": "Description value",
    "address": "Address value",
    "isDefaultServer": true
  },
  "identifier": "Identifier value",
  "customData": [
    {
      "@odata.type": "microsoft.graph.keyValue",
      "key": "Key value",
      "value": "Value value"
    }
  ],
  "customKeyValueData": [
    {
      "@odata.type": "microsoft.graph.keyValuePair",
      "name": "Name value",
      "value": "Value value"
    }
  ],
  "enableSplitTunneling": true,
  "authenticationMethod": "usernameAndPassword",
  "enablePerApp": true,
  "safariDomains": [
    "Safari Domains value"
  ],
  "onDemandRules": [
    {
      "@odata.type": "microsoft.graph.vpnOnDemandRule",
      "ssids": [
        "Ssids value"
      ],
      "dnsSearchDomains": [
        "Dns Search Domains value"
      ],
      "probeUrl": "https://example.com/probeUrl/",
      "action": "evaluateConnection",
      "domainAction": "neverConnect",
      "domains": [
        "Domains value"
      ],
      "probeRequiredUrl": "https://example.com/probeRequiredUrl/"
    }
  ],
  "proxyServer": {
    "@odata.type": "microsoft.graph.vpnProxyServer",
    "automaticConfigurationScriptUrl": "https://example.com/automaticConfigurationScriptUrl/",
    "address": "Address value",
    "port": 4
  },
  "optInToDeviceIdSharing": true,
  "providerType": "appProxy",
  "userDomain": "User Domain value",
  "strictEnforcement": true,
  "cloudName": "Cloud Name value",
  "excludeList": [
    "Exclude List value"
  ],
  "childSecurityAssociationParameters": {
    "@odata.type": "microsoft.graph.iosVpnSecurityAssociationParameters",
    "securityEncryptionAlgorithm": "des",
    "securityIntegrityAlgorithm": "sha1_96",
    "securityDiffieHellmanGroup": 10,
    "lifetimeInMinutes": 1
  },
  "clientAuthenticationType": "deviceAuthentication",
  "deadPeerDetectionRate": "none",
  "disableMobilityAndMultihoming": true,
  "disableRedirect": true,
  "enableCertificateRevocationCheck": true,
  "enableEAP": true,
  "enablePerfectForwardSecrecy": true,
  "enableUseInternalSubnetAttributes": true,
  "localIdentifier": "empty",
  "remoteIdentifier": "Remote Identifier value",
  "securityAssociationParameters": {
    "@odata.type": "microsoft.graph.iosVpnSecurityAssociationParameters",
    "securityEncryptionAlgorithm": "des",
    "securityIntegrityAlgorithm": "sha1_96",
    "securityDiffieHellmanGroup": 10,
    "lifetimeInMinutes": 1
  },
  "serverCertificateCommonName": "Server Certificate Common Name value",
  "serverCertificateIssuerCommonName": "Server Certificate Issuer Common Name value",
  "serverCertificateType": "ecdsa256",
  "sharedSecret": "Shared Secret value",
  "tlsMaximumVersion": "Tls Maximum Version value",
  "tlsMinimumVersion": "Tls Minimum Version value",
  "allowDefaultSecurityAssociationParameters": true,
  "allowDefaultChildSecurityAssociationParameters": true
}
```

### <a name="response"></a>応答
以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 4404

{
  "@odata.type": "#microsoft.graph.iosikEv2VpnConfiguration",
  "id": "b87b0327-0327-b87b-2703-7bb827037bb8",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "deviceManagementApplicabilityRuleOsEdition": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleOsEdition",
    "osEditionTypes": [
      "windows10EnterpriseN"
    ],
    "name": "Name value",
    "ruleType": "exclude"
  },
  "deviceManagementApplicabilityRuleOsVersion": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleOsVersion",
    "minOSVersion": "Min OSVersion value",
    "maxOSVersion": "Max OSVersion value",
    "name": "Name value",
    "ruleType": "exclude"
  },
  "deviceManagementApplicabilityRuleDeviceMode": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleDeviceMode",
    "deviceMode": "sModeConfiguration",
    "name": "Name value",
    "ruleType": "exclude"
  },
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "connectionName": "Connection Name value",
  "connectionType": "pulseSecure",
  "loginGroupOrDomain": "Login Group Or Domain value",
  "role": "Role value",
  "realm": "Realm value",
  "server": {
    "@odata.type": "microsoft.graph.vpnServer",
    "description": "Description value",
    "address": "Address value",
    "isDefaultServer": true
  },
  "identifier": "Identifier value",
  "customData": [
    {
      "@odata.type": "microsoft.graph.keyValue",
      "key": "Key value",
      "value": "Value value"
    }
  ],
  "customKeyValueData": [
    {
      "@odata.type": "microsoft.graph.keyValuePair",
      "name": "Name value",
      "value": "Value value"
    }
  ],
  "enableSplitTunneling": true,
  "authenticationMethod": "usernameAndPassword",
  "enablePerApp": true,
  "safariDomains": [
    "Safari Domains value"
  ],
  "onDemandRules": [
    {
      "@odata.type": "microsoft.graph.vpnOnDemandRule",
      "ssids": [
        "Ssids value"
      ],
      "dnsSearchDomains": [
        "Dns Search Domains value"
      ],
      "probeUrl": "https://example.com/probeUrl/",
      "action": "evaluateConnection",
      "domainAction": "neverConnect",
      "domains": [
        "Domains value"
      ],
      "probeRequiredUrl": "https://example.com/probeRequiredUrl/"
    }
  ],
  "proxyServer": {
    "@odata.type": "microsoft.graph.vpnProxyServer",
    "automaticConfigurationScriptUrl": "https://example.com/automaticConfigurationScriptUrl/",
    "address": "Address value",
    "port": 4
  },
  "optInToDeviceIdSharing": true,
  "providerType": "appProxy",
  "userDomain": "User Domain value",
  "strictEnforcement": true,
  "cloudName": "Cloud Name value",
  "excludeList": [
    "Exclude List value"
  ],
  "childSecurityAssociationParameters": {
    "@odata.type": "microsoft.graph.iosVpnSecurityAssociationParameters",
    "securityEncryptionAlgorithm": "des",
    "securityIntegrityAlgorithm": "sha1_96",
    "securityDiffieHellmanGroup": 10,
    "lifetimeInMinutes": 1
  },
  "clientAuthenticationType": "deviceAuthentication",
  "deadPeerDetectionRate": "none",
  "disableMobilityAndMultihoming": true,
  "disableRedirect": true,
  "enableCertificateRevocationCheck": true,
  "enableEAP": true,
  "enablePerfectForwardSecrecy": true,
  "enableUseInternalSubnetAttributes": true,
  "localIdentifier": "empty",
  "remoteIdentifier": "Remote Identifier value",
  "securityAssociationParameters": {
    "@odata.type": "microsoft.graph.iosVpnSecurityAssociationParameters",
    "securityEncryptionAlgorithm": "des",
    "securityIntegrityAlgorithm": "sha1_96",
    "securityDiffieHellmanGroup": 10,
    "lifetimeInMinutes": 1
  },
  "serverCertificateCommonName": "Server Certificate Common Name value",
  "serverCertificateIssuerCommonName": "Server Certificate Issuer Common Name value",
  "serverCertificateType": "ecdsa256",
  "sharedSecret": "Shared Secret value",
  "tlsMaximumVersion": "Tls Maximum Version value",
  "tlsMinimumVersion": "Tls Minimum Version value",
  "allowDefaultSecurityAssociationParameters": true,
  "allowDefaultChildSecurityAssociationParameters": true
}
```





