---
title: macOSEnterpriseWiFiConfiguration リソースの種類
description: MacOS Wi-fi WPA-エンタープライズまたは WPA2-エンタープライズ構成のプロファイルです。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 132701b0d3bb666d8b58bed59a0f0e28b7d062c1
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27890763"
---
# <a name="macosenterprisewificonfiguration-resource-type"></a>macOSEnterpriseWiFiConfiguration リソースの種類

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

> **注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。

MacOS Wi-fi WPA-エンタープライズまたは WPA2-エンタープライズ構成のプロファイルです。

[MacOSWiFiConfiguration](../resources/intune-deviceconfig-macoswificonfiguration.md)から継承します。

## <a name="methods"></a>メソッド
|メソッド|戻り値の型|説明|
|:---|:---|:---|
|[リスト macOSEnterpriseWiFiConfigurations](../api/intune-deviceconfig-macosenterprisewificonfiguration-list.md)|[macOSEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-macosenterprisewificonfiguration.md)コレクション|[MacOSEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-macosenterprisewificonfiguration.md)オブジェクトのプロパティと関係を一覧表示します。|
|[MacOSEnterpriseWiFiConfiguration を取得します。](../api/intune-deviceconfig-macosenterprisewificonfiguration-get.md)|[macOSEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-macosenterprisewificonfiguration.md)|[MacOSEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-macosenterprisewificonfiguration.md)オブジェクトのプロパティと関係を参照してください。|
|[MacOSEnterpriseWiFiConfiguration を作成します。](../api/intune-deviceconfig-macosenterprisewificonfiguration-create.md)|[macOSEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-macosenterprisewificonfiguration.md)|新しい[macOSEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-macosenterprisewificonfiguration.md)オブジェクトを作成します。|
|[MacOSEnterpriseWiFiConfiguration を削除します。](../api/intune-deviceconfig-macosenterprisewificonfiguration-delete.md)|なし|の[macOSEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-macosenterprisewificonfiguration.md)を削除します。|
|[MacOSEnterpriseWiFiConfiguration を更新します。](../api/intune-deviceconfig-macosenterprisewificonfiguration-update.md)|[macOSEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-macosenterprisewificonfiguration.md)|[MacOSEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-macosenterprisewificonfiguration.md)オブジェクトのプロパティを更新します。|

## <a name="properties"></a>プロパティ
|プロパティ|種類|説明|
|:---|:---|:---|
|ID|String|エンティティのキー。 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します|
|lastModifiedDateTime|DateTimeOffset|オブジェクトが最後に変更された DateTime。 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します|
|roleScopeTagIds|String コレクション|このエンティティ インスタンスのスコープのタグのリストです。 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します|
|supportsScopeTags|ブール型|デバイスの構成を基になるスコープのタグの割り当てをサポートしているかどうかを示します。 この値が false であり、エンティティをスコープ指定されたユーザーには表示されませんがある場合、ScopeTags プロパティに割り当てることは許可されていません。 これは、Silverlight で作成されたレガシ ポリシーに対して発生し、削除して、Azure ポータル内のポリシーを再作成することで解決できます。 このプロパティは読み取りのみ可能です。 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します|
|createdDateTime|DateTimeOffset|オブジェクトが作成された DateTime。 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します|
|説明|String|デバイス構成について管理者が提供した説明。 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します|
|displayName|String|デバイス構成について管理者が指定した名前。 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します|
|version|Int32|デバイス構成のバージョン。 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します|
|ネットワーク名リソース|String|ネットワーク名は、 [macOSWiFiConfiguration](../resources/intune-deviceconfig-macoswificonfiguration.md)から継承されました。|
|ssid|String|これは、すべてのデバイスにブロードキャストされている Wi-fi ネットワークの名前です。 [MacOSWiFiConfiguration](../resources/intune-deviceconfig-macoswificonfiguration.md)から継承されました。|
|connectAutomatically|ブール型|このネットワークが範囲内にすると自動的に接続します。 これを true に設定、ユーザー プロンプトを省略して自動的に Wi-fi ネットワークにデバイスを接続します。 [MacOSWiFiConfiguration](../resources/intune-deviceconfig-macoswificonfiguration.md)から継承されました。|
|connectWhenNetworkNameIsHidden|ブール型|ネットワーク名 (SSID) をブロードキャストしていないときに接続します。 True の場合、このプロファイルに設定されているすべてのデバイスに SSID をブロードキャストしていないネットワークに接続するデバイスを強制します。 [MacOSWiFiConfiguration](../resources/intune-deviceconfig-macoswificonfiguration.md)から継承されました。|
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
|rootCertificateForServerValidation|[macOSTrustedRootCertificate](../resources/intune-deviceconfig-macostrustedrootcertificate.md)|EAP-TLS または TTLS/高速または PEAP に EAP の種類が構成されている場合、サーバー検証のためルート証明書を信頼します。|
|identityCertificateForClientAuthentication|[macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md)|EAP-TLS、EAP-TTLS で証明書の認証の場合)、または (証明書認証) と PEAP に EAP の種類が構成されている場合、クライアント認証用の id の証明書です。|

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





