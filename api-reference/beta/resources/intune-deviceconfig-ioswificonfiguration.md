---
title: iosWiFiConfiguration リソースの種類
description: このプロファイルの構成を提供することによって必要な Wi-fi のエンドポイントに接続するための iOS デバイスに指示できます。 指定する認証方法とセキュリティの種類必要 Wi-fi エンドポイントで行うことができます Wi-fi 接続シームレスなエンド ・ ユーザーのです。 このプロファイルは、エンタープライズ Wi-fi プロファイルよりも制限し、簡単なセキュリティの種類を提供します。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 039b50674604d2d8a108ff08ce7f865beec1f69b
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27856617"
---
# <a name="ioswificonfiguration-resource-type"></a>iosWiFiConfiguration リソースの種類

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

> **注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。

このプロファイルの構成を提供することによって必要な Wi-fi のエンドポイントに接続するための iOS デバイスに指示できます。 指定する認証方法とセキュリティの種類必要 Wi-fi エンドポイントで行うことができます Wi-fi 接続シームレスなエンド ・ ユーザーのです。 このプロファイルは、エンタープライズ Wi-fi プロファイルよりも制限し、簡単なセキュリティの種類を提供します。

[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します

## <a name="methods"></a>メソッド
|メソッド|戻り値の型|説明|
|:---|:---|:---|
|[リスト iosWiFiConfigurations](../api/intune-deviceconfig-ioswificonfiguration-list.md)|[iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md)コレクション|[IosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md)オブジェクトのプロパティと関係を一覧表示します。|
|[IosWiFiConfiguration を取得します。](../api/intune-deviceconfig-ioswificonfiguration-get.md)|[iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md)|[IosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md)オブジェクトのプロパティと関係を参照してください。|
|[IosWiFiConfiguration を作成します。](../api/intune-deviceconfig-ioswificonfiguration-create.md)|[iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md)|新しい[iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md)オブジェクトを作成します。|
|[IosWiFiConfiguration を削除します。](../api/intune-deviceconfig-ioswificonfiguration-delete.md)|なし|の[iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md)を削除します。|
|[IosWiFiConfiguration を更新します。](../api/intune-deviceconfig-ioswificonfiguration-update.md)|[iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md)|[IosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md)オブジェクトのプロパティを更新します。|

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
|ネットワーク名リソース|String|ネットワーク名|
|ssid|String|これは、すべてのデバイスにブロードキャストされている Wi-fi ネットワークの名前です。|
|connectAutomatically|ブール型|このネットワークが範囲内にすると自動的に接続します。 これを true に設定、ユーザー プロンプトを省略して自動的に Wi-fi ネットワークにデバイスを接続します。|
|connectWhenNetworkNameIsHidden|ブール型|ネットワーク名 (SSID) をブロードキャストしていないときに接続します。 True の場合、このプロファイルに設定されているすべてのデバイスに SSID をブロードキャストしていないネットワークに接続するデバイスを強制します。|
|wiFiSecurityType|[wiFiSecurityType](../resources/intune-deviceconfig-wifisecuritytype.md)|Wi-fi エンドポイントがベースの EAP セキュリティ タイプを使用するかどうかを示します。 使用可能な値: `open`、`wpaPersonal`、`wpaEnterprise`、`wep`、`wpa2Personal`、`wpa2Enterprise`。|
|型のオブジェクトで|[wiFiProxySetting](../resources/intune-deviceconfig-wifiproxysetting.md)|この Wi-fi 接続のプロキシの種類です。 可能な値は、`none`、`manual`、`automatic` です。|
|proxyManualAddress|String|手動の構成が選択されている時にプロキシ サーバーの IP アドレスまたは DNS ホスト名|
|proxyManualPort|Int32|手動の構成が選択されている時にプロキシ サーバーのポートです。|
|proxyAutomaticConfigurationUrl|String|自動構成を選択すると、プロキシ サーバーの自動構成スクリプトの URL です。 この URL は、通常、PAC (プロキシの自動構成) ファイルの場所です。|
|preSharedKey|String|これは、WPA パーソナル Wi-fi ネットワークの事前共有キーです。|

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

## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.iosWiFiConfiguration"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosWiFiConfiguration",
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
  "preSharedKey": "String"
}
```





