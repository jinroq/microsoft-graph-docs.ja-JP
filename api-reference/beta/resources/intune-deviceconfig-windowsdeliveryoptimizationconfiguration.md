---
title: windowsDeliveryOptimizationConfiguration リソースの種類
description: Windows 配信の最適化の構成
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: a3b68b0dea6eba5e08adc7afb482655e5819edae
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36371173"
---
# <a name="windowsdeliveryoptimizationconfiguration-resource-type"></a>windowsDeliveryOptimizationConfiguration リソースの種類

> **重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

Windows 配信の最適化の構成


[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します

## <a name="methods"></a>メソッド
|メソッド|戻り値の型|説明|
|:---|:---|:---|
|[リスト windowsDeliveryOptimizationConfigurations](../api/intune-deviceconfig-windowsdeliveryoptimizationconfiguration-list.md)|[windowsDeliveryOptimizationConfiguration](../resources/intune-deviceconfig-windowsdeliveryoptimizationconfiguration.md)コレクション|[WindowsDeliveryOptimizationConfiguration](../resources/intune-deviceconfig-windowsdeliveryoptimizationconfiguration.md)オブジェクトのプロパティとリレーションシップをリストします。|
|[WindowsDeliveryOptimizationConfiguration を取得する](../api/intune-deviceconfig-windowsdeliveryoptimizationconfiguration-get.md)|[windowsDeliveryOptimizationConfiguration](../resources/intune-deviceconfig-windowsdeliveryoptimizationconfiguration.md)|[WindowsDeliveryOptimizationConfiguration](../resources/intune-deviceconfig-windowsdeliveryoptimizationconfiguration.md)オブジェクトのプロパティとリレーションシップを読み取ります。|
|[WindowsDeliveryOptimizationConfiguration を作成する](../api/intune-deviceconfig-windowsdeliveryoptimizationconfiguration-create.md)|[windowsDeliveryOptimizationConfiguration](../resources/intune-deviceconfig-windowsdeliveryoptimizationconfiguration.md)|新しい[windowsDeliveryOptimizationConfiguration](../resources/intune-deviceconfig-windowsdeliveryoptimizationconfiguration.md)オブジェクトを作成します。|
|[WindowsDeliveryOptimizationConfiguration の削除](../api/intune-deviceconfig-windowsdeliveryoptimizationconfiguration-delete.md)|None|[WindowsDeliveryOptimizationConfiguration](../resources/intune-deviceconfig-windowsdeliveryoptimizationconfiguration.md)を削除します。|
|[WindowsDeliveryOptimizationConfiguration の更新](../api/intune-deviceconfig-windowsdeliveryoptimizationconfiguration-update.md)|[windowsDeliveryOptimizationConfiguration](../resources/intune-deviceconfig-windowsdeliveryoptimizationconfiguration.md)|[WindowsDeliveryOptimizationConfiguration](../resources/intune-deviceconfig-windowsdeliveryoptimizationconfiguration.md)オブジェクトのプロパティを更新します。|

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
|deliveryOptimizationMode|[windowsDeliveryOptimizationMode](../resources/intune-deviceconfig-windowsdeliveryoptimizationmode.md)|大規模なコンテンツ配信シナリオのネットワーク帯域幅の消費を管理するために、配信の最適化で使用できるダウンロード方法を指定します。 可能な値は、`userDefined`、`httpOnly`、`httpWithPeeringNat`、`httpWithPeeringPrivateGroup`、`httpWithInternetPeering`、`simpleDownload`、`bypassMode` です。|
|restrictPeerSelectionBy|[deliveryOptimizationRestrictPeerSelectionByOptions](../resources/intune-deviceconfig-deliveryoptimizationrestrictpeerselectionbyoptions.md)|選択したオプションを使用してピアの選択を制限するように指定します。
オプション 1 (サブネットマスク) は、配信最適化モードのダウンロードモード LAN (1) とグループ (2) にのみ適用されます。 可能な値は、`notConfigured`、`subnetMask` です。|
|groupIdSource|[deliveryOptimizationGroupIdSource](../resources/intune-deviceconfig-deliveryoptimizationgroupidsource.md)|ピア選択を固有ソースに制限するように指定します。
このポリシーで設定されたオプションは、配信最適化モードグループ (2) ダウンロードモードにのみ適用されます。 グループ (2) がダウンロードモードに設定されていない場合、このポリシーは無視されます。 オプション 3-DHCP オプション ID の場合、クライアントは DHCP オプション ID 234 に対してクエリを実行し、返された GUID 値をグループ ID として使用します。|
|bandwidthMode|[deliveryOptimizationBandwidth](../resources/intune-deviceconfig-deliveryoptimizationbandwidth.md)|パーセント、absolutes、または時間を使用して、フォアグラウンドおよびバックグラウンドの帯域幅の使用を指定します。|
|backgroundDownloadFromHttpDelayInSeconds|Int64|ピアツーピアの使用が許可されているバックグラウンドダウンロードで HTTP ソースを遅延させる秒数を指定します。 有効な値は 0 ~ 4294967295|
|foregroundDownloadFromHttpDelayInSeconds|Int64|ピアツーピア (0-86400) の使用が許可されているフォアグラウンドダウンロードで HTTP ソースを遅延させる秒数を指定します。 有効な値は 0 ~ 86400
0を指定すると、クラウドサービスを使用してこの設定を管理するための配信の最適化が設定されます。 有効な値は 0 ~ 86400|
|minimumRamAllowedToPeerInGigabytes|Int32|ピアキャッシュを使用するための最小 RAM サイズを GB 単位で指定します (1-100000)。 有効な値は 1 ~ 10万|
|minimumDiskSizeAllowedToPeerInGigabytes|Int32|ピアキャッシュ (1-100000) を使用するための最小ディスクサイズを GB 単位で指定します。 有効な値は 1 ~ 10万
推奨値:64 GB から 256 GB。 有効な値は 1 ~ 10万|
|minimumFileSizeToCacheInMegabytes バイト|Int32|ピアキャッシュを使用するために有効にするコンテンツファイルの最小サイズを MB 単位で指定します (1-100000)。 有効な値は 1 ~ 10万
推奨値: 1 MB ~ 10万 MB。 有効な値は 1 ~ 10万|
|minimumBatteryPercentageAllowedToUpload|Int32|デバイスがデータをアップロードできるように、最小バッテリの割合 (0-100) を指定します。 有効な値は 0 から 100 までです
既定値は 0 です。 値 0 (ゼロ) は "制限なし" を意味し、クラウドサービスの既定値が使用されます。 有効な値は 0 から 100 までです|
|modifyCacheLocation|String|配信の最適化でキャッシュに使用するドライブを指定します。|
|maximumCacheAgeInDays|Int32|正常にダウンロードされた後に、各ファイルが配信最適化キャッシュに保持される最大時間 (0-3650) を指定します。 有効な値は 0 ~ 3650|
|maximumCacheSize|[deliveryOptimizationMaxCacheSize](../resources/intune-deviceconfig-deliveryoptimizationmaxcachesize.md)|配信最適化の最大キャッシュサイズをパーセンテージまたは GB で指定します。|
|vpnPeerCaching キャッシュ|[購入](../resources/intune-shared-enablement.md)|ドメインネットワークに VPN 経由で接続している間、デバイスがピアキャッシュへの参加を許可するかどうかを指定します。 可能な値は、`notConfigured`、`enabled`、`disabled` です。|
|cacheServerHostNames 名|文字列コレクション|キャッシュサーバーのホスト名を指定します。|
|cacheServerForegroundDownloadFallbackToHttpDelayInSeconds|Int32|フォアグラウンドダウンロードのためにキャッシュサーバーから HTTP ソースへのフォールバックを遅延させる秒数を指定します。 有効な値は0から2592000です。|
|cacheServerBackgroundDownloadFallbackToHttpDelayInSeconds|Int32|バックグラウンドをダウンロードするためにキャッシュサーバーから HTTP ソースへのフォールバックを遅延させる秒数を指定します。 有効な値は0から2592000です。|

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

## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.windowsDeliveryOptimizationConfiguration"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsDeliveryOptimizationConfiguration",
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
  "deliveryOptimizationMode": "String",
  "restrictPeerSelectionBy": "String",
  "groupIdSource": {
    "@odata.type": "microsoft.graph.deliveryOptimizationGroupIdSource"
  },
  "bandwidthMode": {
    "@odata.type": "microsoft.graph.deliveryOptimizationBandwidth"
  },
  "backgroundDownloadFromHttpDelayInSeconds": 1024,
  "foregroundDownloadFromHttpDelayInSeconds": 1024,
  "minimumRamAllowedToPeerInGigabytes": 1024,
  "minimumDiskSizeAllowedToPeerInGigabytes": 1024,
  "minimumFileSizeToCacheInMegabytes": 1024,
  "minimumBatteryPercentageAllowedToUpload": 1024,
  "modifyCacheLocation": "String",
  "maximumCacheAgeInDays": 1024,
  "maximumCacheSize": {
    "@odata.type": "microsoft.graph.deliveryOptimizationMaxCacheSize"
  },
  "vpnPeerCaching": "String",
  "cacheServerHostNames": [
    "String"
  ],
  "cacheServerForegroundDownloadFallbackToHttpDelayInSeconds": 1024,
  "cacheServerBackgroundDownloadFallbackToHttpDelayInSeconds": 1024
}
```



