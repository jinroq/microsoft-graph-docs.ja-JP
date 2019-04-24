---
title: macOSEnterpriseWiFiConfiguration リソースの種類
description: MacOS wi-fi WPA-エンタープライズ/WPA2-エンタープライズ構成プロファイル。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: f4643a8004bc5835cabdc5fdb19e2ddb2ea7fd34
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32460409"
---
# <a name="macosenterprisewificonfiguration-resource-type"></a>macOSEnterpriseWiFiConfiguration リソースの種類

> **重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

MacOS wi-fi WPA-エンタープライズ/WPA2-エンタープライズ構成プロファイル。


[macOSWiFiConfiguration](../resources/intune-deviceconfig-macoswificonfiguration.md)から継承します。

## <a name="methods"></a>メソッド
|メソッド|戻り値の型|説明|
|:---|:---|:---|
|[macosenterprisewi\\n onfigurたリストを表示する](../api/intune-deviceconfig-macosenterprisewificonfiguration-list.md)|[macOSEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-macosenterprisewificonfiguration.md)コレクション|[macOSEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-macosenterprisewificonfiguration.md)オブジェクトのプロパティとリレーションシップをリストします。|
|[macOSEnterpriseWiFiConfiguration を取得する](../api/intune-deviceconfig-macosenterprisewificonfiguration-get.md)|[macOSEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-macosenterprisewificonfiguration.md)|[macOSEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-macosenterprisewificonfiguration.md)オブジェクトのプロパティとリレーションシップを読み取ります。|
|[macOSEnterpriseWiFiConfiguration を作成する](../api/intune-deviceconfig-macosenterprisewificonfiguration-create.md)|[macOSEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-macosenterprisewificonfiguration.md)|新しい[macOSEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-macosenterprisewificonfiguration.md)オブジェクトを作成します。|
|[macOSEnterpriseWiFiConfiguration の削除](../api/intune-deviceconfig-macosenterprisewificonfiguration-delete.md)|なし|[macOSEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-macosenterprisewificonfiguration.md)を削除します。|
|[macOSEnterpriseWiFiConfiguration の更新](../api/intune-deviceconfig-macosenterprisewificonfiguration-update.md)|[macOSEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-macosenterprisewificonfiguration.md)|[macOSEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-macosenterprisewificonfiguration.md)オブジェクトのプロパティを更新します。|

## <a name="properties"></a>プロパティ
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
|networkname|String|[macOSWiFiConfiguration](../resources/intune-deviceconfig-macoswificonfiguration.md)から継承されたネットワーク名|
|ssid|String|これは、すべてのデバイスにブロードキャストされている wi-fi ネットワークの名前です。 [macOSWiFiConfiguration](../resources/intune-deviceconfig-macoswificonfiguration.md)から継承します。|
|connectautomatically に|Boolean|このネットワークが範囲内にあるときに自動的に接続します。 この値を true に設定すると、ユーザープロンプトがスキップされ、デバイスが wi-fi ネットワークに自動的に接続されます。 [macOSWiFiConfiguration](../resources/intune-deviceconfig-macoswificonfiguration.md)から継承します。|
|connectWhenNetworkNameIsHidden|Boolean|ネットワークが名前 (SSID) をブロードキャストしていない場合に接続します。 このプロファイルが true に設定されている場合、デバイスは、その SSID をすべてのデバイスにブロードキャストしないネットワークに強制的に接続します。 [macOSWiFiConfiguration](../resources/intune-deviceconfig-macoswificonfiguration.md)から継承します。|
|wiFiSecurityType|[wiFiSecurityType](../resources/intune-deviceconfig-wifisecuritytype.md)|wi-fi エンドポイントで EAP ベースのセキュリティの種類を使用するかどうかを示します。 [macOSWiFiConfiguration](../resources/intune-deviceconfig-macoswificonfiguration.md)から継承されます。 可能な値は `open`、`wpaPersonal`、`wpaEnterprise`、`wep`、`wpa2Personal`、`wpa2Enterprise` です。|
|proxySettings|[wiFiProxySetting](../resources/intune-deviceconfig-wifiproxysetting.md)|[macOSWiFiConfiguration](../resources/intune-deviceconfig-macoswificonfiguration.md)から継承されたこの wi-fi 接続のプロキシの種類。 使用可能な値は、`none`、`manual`、`automatic` です。|
|proxymanualaddress|String|手動構成が選択されている場合のプロキシサーバーの IP アドレスまたは DNS ホスト名。 [macOSWiFiConfiguration](../resources/intune-deviceconfig-macoswificonfiguration.md)から継承します。|
|proxymanualport|Int32|手動構成が選択されている場合のプロキシサーバーのポート。 [macOSWiFiConfiguration](../resources/intune-deviceconfig-macoswificonfiguration.md)から継承します。|
|proxyAutomaticConfigurationUrl|String|自動構成が選択されている場合のプロキシサーバーの自動構成スクリプトの URL。 この URL は、通常、PAC (プロキシ自動構成) ファイルの場所です。 [macOSWiFiConfiguration](../resources/intune-deviceconfig-macoswificonfiguration.md)から継承します。|
|preSharedKey|String|これは、WPA 個人用 wi-fi ネットワークの事前共有キーです。 [macOSWiFiConfiguration](../resources/intune-deviceconfig-macoswificonfiguration.md)から継承します。|
|eaptype|[eaptype](../resources/intune-deviceconfig-eaptype.md)|拡張認証プロトコル (EAP)。 wi-fi エンドポイント (ルーター) に設定されている EAP プロトコルの種類を示します。 可能な値は `eapTls`、`leap`、`eapSim`、`eapTtls`、`peap`、`eapFast` です。|
|eapfastconfiguration|[eapfastconfiguration](../resources/intune-deviceconfig-eapfastconfiguration.md)|eap-fast が選択した eap の種類の場合、eap-fast 構成オプション。 可能な値は、`noProtectedAccessCredential`、`useProtectedAccessCredential`、`useProtectedAccessCredentialAndProvision`、`useProtectedAccessCredentialAndProvisionAnonymously` です。|
|trustedserverの形式|String collection|eap の種類が eap-tls/TTLS/ファストまたは PEAP に構成されている場合の、信頼されたサーバー証明書の名前。 これは、信頼できる証明機関 (CA) によって発行された証明書で使用される一般的な名前です。 この情報を指定すると、エンドユーザーがこの wi-fi ネットワークに接続したときに表示される [動的信頼] ダイアログをバイパスできます。|
|authenticationMethod|[wiFiAuthenticationMethod](../resources/intune-deviceconfig-wifiauthenticationmethod.md)|eap の種類が PEAP または eap-tls に構成されている場合の認証方法。 可能な値は、`certificate`、`usernameAndPassword` です。|
|innerAuthenticationProtocolForEapTtls|[none apauthenticationmethod_ apttlstype](../resources/intune-deviceconfig-noneapauthenticationmethodforeapttlstype.md)|eap タイプが eap-tls で、Authenticationmethod がユーザー名とパスワードの場合、認証用の非 eap メソッド (内部 id)。 可能な値は、`unencryptedPassword`、`challengeHandshakeAuthenticationProtocol`、`microsoftChap`、`microsoftChapVersionTwo` です。|
|outerIdentityPrivacyTemporaryValue|String|eap の種類が eap-tls、eap-fast、または PEAP に構成されている場合は、id プライバシー (外部 id) を有効にします。 このプロパティは、入力したテキストでユーザー名をマスクします。 たとえば、' anonymous ' を使用すると、この wi-fi 接続で実際のユーザー名を使用して認証する各ユーザーは、' anonymous ' と表示されます。|

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
|rootcertificateforservervalidation|[macOSTrustedRootCertificate](../resources/intune-deviceconfig-macostrustedrootcertificate.md)|eap タイプが eap-tls/TTLS/ファストまたは PEAP に構成されている場合に、サーバー検証用の信頼できるルート証明書。|
|identity certificateforclientauthentication|[macoscertificateprofilebase](../resources/intune-deviceconfig-macoscertificateprofilebase.md)|eap タイプが eap-tls、eap-tls (証明書認証を使用)、または PEAP (証明書認証付き) に構成されている場合の、クライアント認証用の id 証明書。|

## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.macOSEnterpriseWiFiConfiguration"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.macOSEnterpriseWiFiConfiguration",
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
  "networkName": "String",
  "ssid": "String",
  "connectAutomatically": true,
  "connectWhenNetworkNameIsHidden": true,
  "wiFiSecurityType": "String",
  "proxySettings": "String",
  "proxyManualAddress": "String",
  "proxyManualPort": 1024,
  "proxyAutomaticConfigurationUrl": "String",
  "preSharedKey": "String",
  "eapType": "String",
  "eapFastConfiguration": "String",
  "trustedServerCertificateNames": [
    "String"
  ],
  "authenticationMethod": "String",
  "innerAuthenticationProtocolForEapTtls": "String",
  "outerIdentityPrivacyTemporaryValue": "String"
}
```





