---
title: androidforwork vpnconfiguration リソースの種類
description: このプロファイルに構成を提供することにより、Android デバイスに対して、目的の VPN エンドポイントに接続するように指示することができます。 vpn エンドポイントによって想定される認証方法とセキュリティの種類を指定することにより、エンドユーザーにとってシームレスに vpn 接続を確立できます。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: a686021d32e427ad2fbb3b6256a42918ae37cbb4
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32556173"
---
# <a name="androidforworkvpnconfiguration-resource-type"></a>androidforwork vpnconfiguration リソースの種類

> **重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

このプロファイルに構成を提供することにより、Android デバイスに対して、目的の VPN エンドポイントに接続するように指示することができます。 vpn エンドポイントによって想定される認証方法とセキュリティの種類を指定することにより、エンドユーザーにとってシームレスに vpn 接続を確立できます。


[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します

## <a name="methods"></a>メソッド
|メソッド|戻り値の型|説明|
|:---|:---|:---|
|[androidforwork vpn構成のリスト](../api/intune-deviceconfig-androidforworkvpnconfiguration-list.md)|[androidforwork vpnconfiguration](../resources/intune-deviceconfig-androidforworkvpnconfiguration.md)コレクション|[androidforwork vpnconfiguration](../resources/intune-deviceconfig-androidforworkvpnconfiguration.md)オブジェクトのプロパティとリレーションシップをリストします。|
|[androidforwork vpnconfiguration の取得](../api/intune-deviceconfig-androidforworkvpnconfiguration-get.md)|[androidForWorkVpnConfiguration](../resources/intune-deviceconfig-androidforworkvpnconfiguration.md)|[androidforwork vpnconfiguration](../resources/intune-deviceconfig-androidforworkvpnconfiguration.md)オブジェクトのプロパティとリレーションシップを読み取ります。|
|[androidforwork vpnconfiguration の作成](../api/intune-deviceconfig-androidforworkvpnconfiguration-create.md)|[androidForWorkVpnConfiguration](../resources/intune-deviceconfig-androidforworkvpnconfiguration.md)|新しい[androidforwork vpnconfiguration](../resources/intune-deviceconfig-androidforworkvpnconfiguration.md)オブジェクトを作成します。|
|[androidforwork vpnconfiguration の削除](../api/intune-deviceconfig-androidforworkvpnconfiguration-delete.md)|なし|[androidforwork vpnconfiguration](../resources/intune-deviceconfig-androidforworkvpnconfiguration.md)を削除します。|
|[androidforwork vpnconfiguration の更新](../api/intune-deviceconfig-androidforworkvpnconfiguration-update.md)|[androidForWorkVpnConfiguration](../resources/intune-deviceconfig-androidforworkvpnconfiguration.md)|[androidforwork vpnconfiguration](../resources/intune-deviceconfig-androidforworkvpnconfiguration.md)オブジェクトのプロパティを更新します。|

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|id|文字列型 (String)|エンティティのキー。 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します|
|lastModifiedDateTime|DateTimeOffset|オブジェクトの最終更新の DateTime。 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します|
|roleScopeTagIds|String collection|このエンティティインスタンスの範囲タグのリスト。 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します|
|supportsScopeTags|ブール値|基になるデバイス構成がスコープタグの割り当てをサポートしているかどうかを示します。 この値が false である場合、ScopeTags プロパティへの割り当ては許可されません。エンティティは、スコープを持つユーザーには表示されません。 これは Silverlight で作成された従来のポリシーに対して実行され、Azure ポータルでポリシーを削除して再作成することによって解決できます。 このプロパティに値を設定するには、 SetExtrusionDirection メソッドを適用します。 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します|
|createdDateTime|DateTimeOffset|オブジェクトが作成された DateTime。 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します|
|description|String|管理者が指定した、デバイス構成についての説明。 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します|
|displayName|String|管理者が指定した、デバイス構成の名前。 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します|
|version|Int32|デバイス構成のバージョン。 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します|
|connectionName|String|ユーザーに表示される接続名。|
|connectionType|[androidForWorkVpnConnectionType](../resources/intune-deviceconfig-androidforworkvpnconnectiontype.md)|接続の種類。 可能な値は `ciscoAnyConnect`、`pulseSecure`、`f5EdgeClient`、`dellSonicWallMobileConnect`、`checkPointCapsuleVpn`、`citrix` です。|
|role|String|接続の種類がパルス Secure に設定されている場合の役割。|
|領域|String|接続の種類がパルス Secure に設定されている場合の領域。|
|サーバ|[vpnServer](../resources/intune-deviceconfig-vpnserver.md)コレクション|ネットワーク上の VPN サーバーの一覧。 エンドユーザーがこれらのネットワークの場所にアクセスできることを確認します。 このコレクションには、最大で 500 個の要素を含めることができます。|
|デジタル|String|フィンガープリントは、vpn サーバーが信頼できることを確認するために使用される文字列です。これは、接続の種類が [チェックポイントカプセル VPN] の場合にのみ適用されます。|
|customData|[keyvalue](../resources/intune-deviceconfig-keyvalue.md) コレクション|接続の種類が Citrix に設定されている場合のカスタムデータ。 このコレクションには、最大25個の要素を含めることができます。|
|customKeyValueData|[keyValuePair](../resources/intune-shared-keyvaluepair.md) コレクション|接続の種類が Citrix に設定されている場合のカスタムデータ。 このコレクションには、最大25個の要素を含めることができます。|
|authenticationMethod|[vpnauthenticationmethod](../resources/intune-deviceconfig-vpnauthenticationmethod.md)|認証方法。 可能な値: `certificate`、`usernameAndPassword`。|

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
|identityCertificate|[androidForWorkCertificateProfileBase](../resources/intune-deviceconfig-androidforworkcertificateprofilebase.md)|認証方法が証明書の場合にクライアント認証を行うための id 証明書。|

## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.androidForWorkVpnConfiguration"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.androidForWorkVpnConfiguration",
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
  "connectionName": "String",
  "connectionType": "String",
  "role": "String",
  "realm": "String",
  "servers": [
    {
      "@odata.type": "microsoft.graph.vpnServer",
      "description": "String",
      "address": "String",
      "isDefaultServer": true
    }
  ],
  "fingerprint": "String",
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
  "authenticationMethod": "String"
}
```





