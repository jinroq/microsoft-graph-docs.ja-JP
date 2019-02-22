---
title: windowsUpdateForBusinessConfiguration リソースの種類
description: Windows Update for Business の構成です。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 8f1516a9b7558d6d94f3bfc26e5a55cf983354e2
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/21/2019
ms.locfileid: "30155483"
---
# <a name="windowsupdateforbusinessconfiguration-resource-type"></a>windowsUpdateForBusinessConfiguration リソースの種類

> **重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

Windows Update for Business の構成です。


[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します

## <a name="methods"></a>メソッド
|メソッド|戻り値の型|説明|
|:---|:---|:---|
|[windowsUpdateForBusinessConfigurations のリスト](../api/intune-deviceconfig-windowsupdateforbusinessconfiguration-list.md)|[windowsUpdateForBusinessConfiguration](../resources/intune-deviceconfig-windowsupdateforbusinessconfiguration.md) コレクション|[windowsUpdateForBusinessConfiguration](../resources/intune-deviceconfig-windowsupdateforbusinessconfiguration.md) オブジェクトのプロパティとリレーションシップをリストします。|
|[windowsUpdateForBusinessConfiguration の取得](../api/intune-deviceconfig-windowsupdateforbusinessconfiguration-get.md)|[windowsUpdateForBusinessConfiguration](../resources/intune-deviceconfig-windowsupdateforbusinessconfiguration.md)|[windowsUpdateForBusinessConfiguration](../resources/intune-deviceconfig-windowsupdateforbusinessconfiguration.md) オブジェクトのプロパティとリレーションシップを読み取ります。|
|[windowsUpdateForBusinessConfiguration の作成](../api/intune-deviceconfig-windowsupdateforbusinessconfiguration-create.md)|[windowsUpdateForBusinessConfiguration](../resources/intune-deviceconfig-windowsupdateforbusinessconfiguration.md)|新しい [windowsUpdateForBusinessConfiguration](../resources/intune-deviceconfig-windowsupdateforbusinessconfiguration.md) オブジェクトを作成します。|
|[windowsUpdateForBusinessConfiguration の削除](../api/intune-deviceconfig-windowsupdateforbusinessconfiguration-delete.md)|なし|[windowsUpdateForBusinessConfiguration](../resources/intune-deviceconfig-windowsupdateforbusinessconfiguration.md) を削除します。|
|[windowsUpdateForBusinessConfiguration の更新](../api/intune-deviceconfig-windowsupdateforbusinessconfiguration-update.md)|[windowsUpdateForBusinessConfiguration](../resources/intune-deviceconfig-windowsupdateforbusinessconfiguration.md)|[windowsUpdateForBusinessConfiguration](../resources/intune-deviceconfig-windowsupdateforbusinessconfiguration.md) オブジェクトのプロパティを更新します。|
|[extendFeatureUpdatesPause アクション](../api/intune-deviceconfig-windowsupdateforbusinessconfiguration-extendfeatureupdatespause.md)|なし|機能の更新プログラムが、ビジネスリングの Windows Update によって一時停止するまで停止します。|
|[extendQualityUpdatesPause アクション](../api/intune-deviceconfig-windowsupdateforbusinessconfiguration-extendqualityupdatespause.md)|なし|ビジネスリングの Windows Update に対する品質更新プログラムの一時停止を延長します。|

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|id|文字列|エンティティのキー。 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します|
|lastModifiedDateTime|DateTimeOffset|オブジェクトが最後に変更された DateTime。 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します|
|roleScopeTagIds|String collection|このエンティティインスタンスの範囲タグのリスト。 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します|
|supportsScopeTags|ブール値|基になるデバイス構成がスコープタグの割り当てをサポートしているかどうかを示します。 この値が false である場合、ScopeTags プロパティへの割り当ては許可されません。エンティティは、スコープを持つユーザーには表示されません。 これは Silverlight で作成された従来のポリシーに対して実行され、Azure ポータルでポリシーを削除して再作成することによって解決できます。 このプロパティは読み取りのみ可能です。 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します|
|createdDateTime|DateTimeOffset|オブジェクトが作成された DateTime。 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します|
|説明|String|デバイス構成について管理者が提供した説明。 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します|
|displayName|String|デバイス構成について管理者が指定した名前。 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します|
|version|Int32|デバイス構成のバージョン。 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します|
|deliveryOptimizationMode|[windowsDeliveryOptimizationMode](../resources/intune-deviceconfig-windowsdeliveryoptimizationmode.md)|配信最適化モード。 可能な値は、`userDefined`、`httpOnly`、`httpWithPeeringNat`、`httpWithPeeringPrivateGroup`、`httpWithInternetPeering`、`simpleDownload`、`bypassMode` です。|
|prereleaseFeatures|[prereleaseFeatures](../resources/intune-deviceconfig-prereleasefeatures.md)|プレリリース機能です。 可能な値は、`userDefined`、`settingsOnly`、`settingsAndExperimentations`、`notAllowed` です。|
|automaticUpdateMode|[automaticUpdateMode](../resources/intune-deviceconfig-automaticupdatemode.md)|自動更新モードです。 可能な値は、`userDefined`、`notifyDownload`、`autoInstallAtMaintenanceTime`、`autoInstallAndRebootAtMaintenanceTime`、`autoInstallAndRebootAtScheduledTime`、`autoInstallAndRebootWithoutEndUserControl`、`windowsDefault` です。|
|microsoftUpdateServiceAllowed|ブール値|Microsoft の更新サービスを許可します。|
|driversExcluded|ブール値|Windows 更新ドライバーを除外します。|
|installationSchedule|[windowsUpdateInstallScheduleType](../resources/intune-deviceconfig-windowsupdateinstallscheduletype.md)|インストールのスケジュールです|
|qualityUpdatesDeferralPeriodInDays|Int32|品質更新プログラムの実行をこの日数分延期します|
|featureUpdatesDeferralPeriodInDays|Int32|機能更新プログラムの実行をこの日数分延期します|
|qualityUpdatesPaused|Boolean|品質更新プログラムの実行を一時停止します|
|featureUpdatesPaused|Boolean|機能更新プログラムの実行を一時停止します|
|qualityUpdatesPauseExpiryDateTime|DateTimeOffset|品質更新プログラム実行一時停止の有効期限が切れる日時です|
|featureUpdatesPauseExpiryDateTime|DateTimeOffset|機能更新プログラム実行一時停止の有効期限が切れる日時です|
|businessReadyUpdatesOnly|[windowsUpdateType](../resources/intune-deviceconfig-windowsupdatetype.md)|更新プログラムを受信するブランチデバイスを決定します。 使用可能な値: `userDefined`、`all`、`businessReadyOnly`、`windowsInsiderBuildFast`、`windowsInsiderBuildSlow`、`windowsInsiderBuildRelease`。|
|skipchecksbeforerestart|ブール値|再起動前にすべてのチェックをスキップするように設定: バッテリーレベル = 40%、ユーザープレゼンス、表示が必要、プレゼンテーションモード、全画面表示モード、電話呼び出しの状態、ゲームモードなど。 |
|updateweeks|[windowsUpdateForBusinessUpdateWeeks](../resources/intune-deviceconfig-windowsupdateforbusinessupdateweeks.md)|月の週に更新プログラムのインストールをスケジュールしました。 使用可能な値: `userDefined`、`firstWeek`、`secondWeek`、`thirdWeek`、`fourthWeek`、`everyWeek`。|
|qualityUpdatesPauseStartDate|日付|品質更新の一時停止の開始日。 このプロパティは読み取りのみ可能です。|
|featureUpdatesPauseStartDate|日付|機能の更新の開始日が一時停止します。 このプロパティは読み取りのみ可能です。|
|featureUpdatesRollbackWindowInDays|Int32|ロールバックが有効になっている機能更新後の日数|
|qualityUpdatesWillBeRolledBack|ブール値|次のデバイスチェックで品質更新プログラムをロールバックするかどうかを指定します|
|featureupdateswillberolledbackqualityupdatesrollbackstartdatetime|ブール値|次回のデバイスチェックで機能の更新をロールバックするかどうかを指定します|
|追加|DateTimeOffset|品質更新プログラムのロールバック開始日時|
|featureUpdatesRollbackStartDateTime|DateTimeOffset|機能更新プログラムのロールバック開始日時|
|engagedRestartDeadlineInDays|Int32|アクティブ時間外に保留中の再起動を自動的にスケジュールして実行するまでの期限 (日数は2から30日)|
|engagedRestartSnoozeScheduleInDays|Int32|ユーザーが参加を再開できるリマインダー通知通知の有効期間が 1 ~ 3 日の場合に、再通知できる日数|
|engagedRestartTransitionScheduleInDays|Int32|アクティブ時間外に再起動が行われるようにスケジュールされた自動再起動から移行するまでの日数。0から30日の範囲で有効な範囲で、ユーザーのスケジュールを設定する必要があります。|
|autoRestartNotificationDismissal|[autoRestartNotificationDismissalMethod](../resources/intune-deviceconfig-autorestartnotificationdismissalmethod.md)|自動再起動必須通知を閉じる方法を指定します。 可能な値は `notConfigured`、`automatic`、`user` です。|
|scheduleRestartWarningInHours|Int32|自動再起動警告リマインダー通知の期間を指定します。 サポートされている値: 2、4、8、12、または 24 (時間)。|
|scheduleImminentRestartWarningInMinutes|Int32|差し迫った自動再起動警告通知の期間を指定します。 サポートされている値:15、30または 60 (分)。|
|userPauseAccess|[購入](../resources/intune-shared-enablement.md)|エンドユーザーのアクセスを有効にして、ソフトウェアの更新を一時停止するかどうかを指定します。 可能な値は、`notConfigured`、`enabled`、`disabled` です。|

## <a name="relationships"></a>関係
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
  "@odata.type": "microsoft.graph.windowsUpdateForBusinessConfiguration"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsUpdateForBusinessConfiguration",
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
  "deliveryOptimizationMode": "String",
  "prereleaseFeatures": "String",
  "automaticUpdateMode": "String",
  "microsoftUpdateServiceAllowed": true,
  "driversExcluded": true,
  "installationSchedule": {
    "@odata.type": "microsoft.graph.windowsUpdateScheduledInstall",
    "scheduledInstallDay": "String",
    "scheduledInstallTime": "String (time of day)"
  },
  "qualityUpdatesDeferralPeriodInDays": 1024,
  "featureUpdatesDeferralPeriodInDays": 1024,
  "qualityUpdatesPaused": true,
  "featureUpdatesPaused": true,
  "qualityUpdatesPauseExpiryDateTime": "String (timestamp)",
  "featureUpdatesPauseExpiryDateTime": "String (timestamp)",
  "businessReadyUpdatesOnly": "String",
  "skipChecksBeforeRestart": true,
  "updateWeeks": "String",
  "qualityUpdatesPauseStartDate": "<Unknown Primitive Type Edm.Date>",
  "featureUpdatesPauseStartDate": "<Unknown Primitive Type Edm.Date>",
  "featureUpdatesRollbackWindowInDays": 1024,
  "qualityUpdatesWillBeRolledBack": true,
  "featureUpdatesWillBeRolledBack": true,
  "qualityUpdatesRollbackStartDateTime": "String (timestamp)",
  "featureUpdatesRollbackStartDateTime": "String (timestamp)",
  "engagedRestartDeadlineInDays": 1024,
  "engagedRestartSnoozeScheduleInDays": 1024,
  "engagedRestartTransitionScheduleInDays": 1024,
  "autoRestartNotificationDismissal": "String",
  "scheduleRestartWarningInHours": 1024,
  "scheduleImminentRestartWarningInMinutes": 1024,
  "userPauseAccess": "String"
}
```




