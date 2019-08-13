---
title: macOSVpnConfiguration リソースの種類
description: このプロファイルに構成を提供することにより、Mac デバイスに対して、目的の VPN エンドポイントに接続するように指示することができます。 VPN エンドポイントによって想定される認証方法とセキュリティの種類を指定することにより、エンドユーザーにとってシームレスに VPN 接続を確立できます。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: ad72a40e50eb6659cb5983e7038d440756ca44d7
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36316165"
---
# <a name="macosvpnconfiguration-resource-type"></a>macOSVpnConfiguration リソースの種類

> **重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

このプロファイルに構成を提供することにより、Mac デバイスに対して、目的の VPN エンドポイントに接続するように指示することができます。 VPN エンドポイントによって想定される認証方法とセキュリティの種類を指定することにより、エンドユーザーにとってシームレスに VPN 接続を確立できます。


[りんご Evpnconfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)からの継承

## <a name="methods"></a>メソッド
|メソッド|戻り値の型|説明|
|:---|:---|:---|
|[MacOSVpnConfigurations を一覧表示する](../api/intune-deviceconfig-macosvpnconfiguration-list.md)|[Macosvpnconfiguration](../resources/intune-deviceconfig-macosvpnconfiguration.md)コレクション|[Macosvpnconfiguration](../resources/intune-deviceconfig-macosvpnconfiguration.md)オブジェクトのプロパティとリレーションシップをリストします。|
|[MacOSVpnConfiguration の取得](../api/intune-deviceconfig-macosvpnconfiguration-get.md)|[macOSVpnConfiguration](../resources/intune-deviceconfig-macosvpnconfiguration.md)|[Macosvpnconfiguration](../resources/intune-deviceconfig-macosvpnconfiguration.md)オブジェクトのプロパティとリレーションシップを読み取ります。|
|[MacOSVpnConfiguration の作成](../api/intune-deviceconfig-macosvpnconfiguration-create.md)|[macOSVpnConfiguration](../resources/intune-deviceconfig-macosvpnconfiguration.md)|新しい[Macosvpnconfiguration](../resources/intune-deviceconfig-macosvpnconfiguration.md)オブジェクトを作成します。|
|[MacOSVpnConfiguration の削除](../api/intune-deviceconfig-macosvpnconfiguration-delete.md)|None|[Macosvpnconfiguration](../resources/intune-deviceconfig-macosvpnconfiguration.md)を削除します。|
|[MacOSVpnConfiguration の更新](../api/intune-deviceconfig-macosvpnconfiguration-update.md)|[macOSVpnConfiguration](../resources/intune-deviceconfig-macosvpnconfiguration.md)|[Macosvpnconfiguration](../resources/intune-deviceconfig-macosvpnconfiguration.md)オブジェクトのプロパティを更新します。|

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
|identityCertificate|[macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md)|認証方法が証明書の場合にクライアント認証を行うための id 証明書。|

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
  "optInToDeviceIdSharing": true
}
```



