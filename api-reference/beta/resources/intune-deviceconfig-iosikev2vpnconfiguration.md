---
title: iosikEv2VpnConfiguration リソースの種類
description: このプロファイルに構成を提供することで、iOS デバイスに対して、目的の IKEv2 VPN エンドポイントに接続するように指示することができます。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 69a59defd2b92300593efc4385da43db02289426
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36356992"
---
# <a name="iosikev2vpnconfiguration-resource-type"></a>iosikEv2VpnConfiguration リソースの種類

> **重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

このプロファイルに構成を提供することで、iOS デバイスに対して、目的の IKEv2 VPN エンドポイントに接続するように指示することができます。


[Iosvpnconfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md)からの継承

## <a name="methods"></a>メソッド
|メソッド|戻り値の型|説明|
|:---|:---|:---|
|[リスト iosikEv2VpnConfigurations](../api/intune-deviceconfig-iosikev2vpnconfiguration-list.md)|[iosikEv2VpnConfiguration](../resources/intune-deviceconfig-iosikev2vpnconfiguration.md)コレクション|[IosikEv2VpnConfiguration](../resources/intune-deviceconfig-iosikev2vpnconfiguration.md)オブジェクトのプロパティとリレーションシップをリストします。|
|[IosikEv2VpnConfiguration を取得する](../api/intune-deviceconfig-iosikev2vpnconfiguration-get.md)|[iosikEv2VpnConfiguration](../resources/intune-deviceconfig-iosikev2vpnconfiguration.md)|[IosikEv2VpnConfiguration](../resources/intune-deviceconfig-iosikev2vpnconfiguration.md)オブジェクトのプロパティとリレーションシップを読み取ります。|
|[IosikEv2VpnConfiguration を作成する](../api/intune-deviceconfig-iosikev2vpnconfiguration-create.md)|[iosikEv2VpnConfiguration](../resources/intune-deviceconfig-iosikev2vpnconfiguration.md)|新しい[iosikEv2VpnConfiguration](../resources/intune-deviceconfig-iosikev2vpnconfiguration.md)オブジェクトを作成します。|
|[IosikEv2VpnConfiguration の削除](../api/intune-deviceconfig-iosikev2vpnconfiguration-delete.md)|None|[IosikEv2VpnConfiguration](../resources/intune-deviceconfig-iosikev2vpnconfiguration.md)を削除します。|
|[IosikEv2VpnConfiguration の更新](../api/intune-deviceconfig-iosikev2vpnconfiguration-update.md)|[iosikEv2VpnConfiguration](../resources/intune-deviceconfig-iosikev2vpnconfiguration.md)|[IosikEv2VpnConfiguration](../resources/intune-deviceconfig-iosikev2vpnconfiguration.md)オブジェクトのプロパティを更新します。|

## <a name="properties"></a>プロパティ
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
|identityCertificate|[iosCertificateProfileBase](../resources/intune-deviceconfig-ioscertificateprofilebase.md)|認証方法が証明書の場合にクライアント認証を行うための id 証明書。 [Iosvpnconfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md)から継承します|
|derivedCredentialSettings|[deviceManagementDerivedCredentialSettings](../resources/intune-deviceconfig-devicemanagementderivedcredentialsettings.md)|認証に使用される派生した資格情報のテナントレベルの設定。 [Iosvpnconfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md)から継承します|

## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.iosikEv2VpnConfiguration"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosikEv2VpnConfiguration",
  "id": "String (identifier)",
  "lastModifiedDateTime": "String (timestamp)",
  "roleScopeTagIds": [
    "String"
  ],
  "supportsScopeTags": true,
  "deviceManagementApplicabilityRuleOsEdition": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleOsEdition",
    "osEditionTypes": [
      "String"
    ],
    "name": "String",
    "ruleType": "String"
  },
  "deviceManagementApplicabilityRuleOsVersion": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleOsVersion",
    "minOSVersion": "String",
    "maxOSVersion": "String",
    "name": "String",
    "ruleType": "String"
  },
  "deviceManagementApplicabilityRuleDeviceMode": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleDeviceMode",
    "deviceMode": "String",
    "name": "String",
    "ruleType": "String"
  },
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
  "optInToDeviceIdSharing": true,
  "providerType": "String",
  "userDomain": "String",
  "strictEnforcement": true,
  "cloudName": "String",
  "excludeList": [
    "String"
  ],
  "childSecurityAssociationParameters": {
    "@odata.type": "microsoft.graph.iosVpnSecurityAssociationParameters",
    "securityEncryptionAlgorithm": "String",
    "securityIntegrityAlgorithm": "String",
    "securityDiffieHellmanGroup": 1024,
    "lifetimeInMinutes": 1024
  },
  "clientAuthenticationType": "String",
  "deadPeerDetectionRate": "String",
  "disableMobilityAndMultihoming": true,
  "disableRedirect": true,
  "enableCertificateRevocationCheck": true,
  "enableEAP": true,
  "enablePerfectForwardSecrecy": true,
  "enableUseInternalSubnetAttributes": true,
  "localIdentifier": "String",
  "remoteIdentifier": "String",
  "securityAssociationParameters": {
    "@odata.type": "microsoft.graph.iosVpnSecurityAssociationParameters",
    "securityEncryptionAlgorithm": "String",
    "securityIntegrityAlgorithm": "String",
    "securityDiffieHellmanGroup": 1024,
    "lifetimeInMinutes": 1024
  },
  "serverCertificateCommonName": "String",
  "serverCertificateIssuerCommonName": "String",
  "serverCertificateType": "String",
  "sharedSecret": "String",
  "tlsMaximumVersion": "String",
  "tlsMinimumVersion": "String",
  "allowDefaultSecurityAssociationParameters": true,
  "allowDefaultChildSecurityAssociationParameters": true
}
```



