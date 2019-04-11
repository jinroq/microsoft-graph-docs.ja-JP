---
title: androidEnterpriseWiFiConfiguration リソースの種類
description: このプロファイルに構成を提供することで、Android デバイスに接続して目的の wi-fi エンドポイントに接続するように指示することができます。 wi-fi エンドポイントで想定される認証方法とセキュリティの種類を指定することで、エンドユーザーに対して wi-fi 接続をシームレスに行うことができます。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: f2cd44e7a0f855477dbc945ee9f3260c0d0d08da
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/11/2019
ms.locfileid: "31783193"
---
# <a name="androidenterprisewificonfiguration-resource-type"></a>androidEnterpriseWiFiConfiguration リソースの種類

> **重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

このプロファイルに構成を提供することで、Android デバイスに接続して目的の wi-fi エンドポイントに接続するように指示することができます。 wi-fi エンドポイントで想定される認証方法とセキュリティの種類を指定することで、エンドユーザーに対して wi-fi 接続をシームレスに行うことができます。


[androidWiFiConfiguration](../resources/intune-deviceconfig-androidwificonfiguration.md)から継承します。

## <a name="methods"></a>メソッド
|メソッド|戻り値の型|説明|
|:---|:---|:---|
|[androidenterprisewiidmso onfigurたリスト](../api/intune-deviceconfig-androidenterprisewificonfiguration-list.md)|[androidEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-androidenterprisewificonfiguration.md)コレクション|[androidEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-androidenterprisewificonfiguration.md)オブジェクトのプロパティとリレーションシップをリストします。|
|[androidEnterpriseWiFiConfiguration を取得する](../api/intune-deviceconfig-androidenterprisewificonfiguration-get.md)|[androidEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-androidenterprisewificonfiguration.md)|[androidEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-androidenterprisewificonfiguration.md)オブジェクトのプロパティとリレーションシップを読み取ります。|
|[androidEnterpriseWiFiConfiguration を作成する](../api/intune-deviceconfig-androidenterprisewificonfiguration-create.md)|[androidEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-androidenterprisewificonfiguration.md)|新しい[androidEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-androidenterprisewificonfiguration.md)オブジェクトを作成します。|
|[androidEnterpriseWiFiConfiguration の削除](../api/intune-deviceconfig-androidenterprisewificonfiguration-delete.md)|なし|[androidEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-androidenterprisewificonfiguration.md)を削除します。|
|[androidEnterpriseWiFiConfiguration の更新](../api/intune-deviceconfig-androidenterprisewificonfiguration-update.md)|[androidEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-androidenterprisewificonfiguration.md)|[androidEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-androidenterprisewificonfiguration.md)オブジェクトのプロパティを更新します。|

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|id|文字列型 (String)|エンティティのキー。 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します|
|lastModifiedDateTime|DateTimeOffset|オブジェクトの最終更新の DateTime。 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します|
|roleScopeTagIds|String コレクション|このエンティティインスタンスの範囲タグのリスト。 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します|
|supportsScopeTags|Boolean|基になるデバイス構成がスコープタグの割り当てをサポートしているかどうかを示します。 この値が false である場合、ScopeTags プロパティへの割り当ては許可されません。エンティティは、スコープを持つユーザーには表示されません。 これは Silverlight で作成された従来のポリシーに対して実行され、Azure ポータルでポリシーを削除して再作成することによって解決できます。 このプロパティに値を設定するには、 SetExtrusionDirection メソッドを適用します。 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します|
|createdDateTime|DateTimeOffset|オブジェクトが作成された DateTime。 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します|
|説明|String|管理者が指定した、デバイス構成についての説明。 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します|
|displayName|String|管理者が指定した、デバイス構成の名前。 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します|
|version|Int32|デバイス構成のバージョン。 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します|
|networkname|文字列|[androidWiFiConfiguration](../resources/intune-deviceconfig-androidwificonfiguration.md)から継承されたネットワーク名|
|ssid|文字列|これは、すべてのデバイスにブロードキャストされている wi-fi ネットワークの名前です。 [androidWiFiConfiguration](../resources/intune-deviceconfig-androidwificonfiguration.md)から継承します。|
|connectautomatically に|Boolean|このネットワークが範囲内にあるときに自動的に接続します。 この値を true に設定すると、ユーザープロンプトがスキップされ、デバイスが wi-fi ネットワークに自動的に接続されます。 [androidWiFiConfiguration](../resources/intune-deviceconfig-androidwificonfiguration.md)から継承します。|
|connectWhenNetworkNameIsHidden|Boolean|このプロファイルが true に設定されている場合、デバイスは、その SSID をすべてのデバイスにブロードキャストしないネットワークに強制的に接続します。 [androidWiFiConfiguration](../resources/intune-deviceconfig-androidwificonfiguration.md)から継承します。|
|wiFiSecurityType|[androidWiFiSecurityType](../resources/intune-deviceconfig-androidwifisecuritytype.md)|wi-fi エンドポイントで EAP ベースのセキュリティの種類を使用するかどうかを示します。 [androidWiFiConfiguration](../resources/intune-deviceconfig-androidwificonfiguration.md)から継承されます。 可能な値は、`open`、`wpaEnterprise` です。|
|eaptype|[androide aptype](../resources/intune-deviceconfig-androideaptype.md)|wi-fi エンドポイント (ルーター) に設定されている EAP プロトコルの種類を示します。 使用可能な値は、`eapTls`、`eapTtls`、`peap` です。|
|authenticationMethod|[wiFiAuthenticationMethod](../resources/intune-deviceconfig-wifiauthenticationmethod.md)|eap の種類が PEAP または eap-tls に構成されている場合に、クライアント (デバイス) が使用する必要がある認証方法を示します。 可能な値は、`certificate`、`usernameAndPassword` です。|
|innerAuthenticationProtocolForEapTtls|[none apauthenticationmethod_ apttlstype](../resources/intune-deviceconfig-noneapauthenticationmethodforeapttlstype.md)|eap タイプが eap-tls で、Authenticationmethod がユーザー名とパスワードの場合、認証用の非 eap メソッド (内部 id)。 可能な値は、`unencryptedPassword`、`challengeHandshakeAuthenticationProtocol`、`microsoftChap`、`microsoftChapVersionTwo` です。|
|innerAuthenticationProtocolForPeap|[nonEapAuthenticationMethodForPeap](../resources/intune-deviceconfig-noneapauthenticationmethodforpeap.md)|eap の種類が PEAP で、Authenticationmethod がユーザー名とパスワードを持っている場合の認証用の非 eap メソッド (内部 id)。 可能な値は、`none`、`microsoftChapVersionTwo` です。|
|outerIdentityPrivacyTemporaryValue|文字列|eap の種類が eap-tls または PEAP に構成されている場合は、id プライバシー (外部 id) を有効にします。 ここに示す文字列を使用して、wi-fi ネットワークに接続しようとするときに個々のユーザーのユーザー名をマスクします。|

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
|rootcertificateforservervalidation|[androidtrustedrootcertificate](../resources/intune-deviceconfig-androidtrustedrootcertificate.md)|eap タイプが eap-tls、eap-tls、または PEAP に構成されている場合に、サーバー検証用の信頼できるルート証明書。 これは、デバイスが wi-fi エンドポイントに接続しようとしたときに wi-fi エンドポイントによって提示される証明書です。 デバイス (またはユーザー) は、この証明書を受け入れて接続の試行を続行する必要があります。|
|identity certificateforclientauthentication|[androidcertificateprofilebase](../resources/intune-deviceconfig-androidcertificateprofilebase.md)|eap タイプが eap-tls、eap-tls (証明書認証を使用)、または PEAP (証明書認証付き) に構成されている場合の、クライアント認証用の id 証明書。 これは、クライアントによって wi-fi エンドポイントに提示された証明書です。 wi-fi 接続を確立するには、wi-fi エンドポイントの背後にある認証サーバーがこの証明書を受け入れる必要があります。|

## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.androidEnterpriseWiFiConfiguration"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.androidEnterpriseWiFiConfiguration",
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
  "eapType": "String",
  "authenticationMethod": "String",
  "innerAuthenticationProtocolForEapTtls": "String",
  "innerAuthenticationProtocolForPeap": "String",
  "outerIdentityPrivacyTemporaryValue": "String"
}
```





