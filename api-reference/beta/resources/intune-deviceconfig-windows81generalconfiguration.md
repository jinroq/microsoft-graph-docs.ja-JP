---
title: windows81GeneralConfiguration リソース タイプ
description: このトピックでは、windows81GeneralConfiguration リソースによって公開された、宣言されたメソッド、プロパティ、リレーションシップについて説明します。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 9ad1d4587dab7474675d322ceb08f3fbfe149810
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29400152"
---
# <a name="windows81generalconfiguration-resource-type"></a>windows81GeneralConfiguration リソース タイプ

> **重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。 実稼働アプリケーションでこれらの API を使用することは、サポートされていません。

> **注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

このトピックでは、windows81GeneralConfiguration リソースによって公開された、宣言されたメソッド、プロパティ、リレーションシップについて説明します。


[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します

## <a name="methods"></a>メソッド
|メソッド|戻り値の型|説明|
|:---|:---|:---|
|[List windows81GeneralConfigurations](../api/intune-deviceconfig-windows81generalconfiguration-list.md)|[windows81GeneralConfiguration](../resources/intune-deviceconfig-windows81generalconfiguration.md) コレクション|[windows81GeneralConfiguration](../resources/intune-deviceconfig-windows81generalconfiguration.md) オブジェクトのプロパティとリレーションシップをリストします。|
|[Get windows81GeneralConfiguration](../api/intune-deviceconfig-windows81generalconfiguration-get.md)|[windows81GeneralConfiguration](../resources/intune-deviceconfig-windows81generalconfiguration.md)|[windows81GeneralConfiguration](../resources/intune-deviceconfig-windows81generalconfiguration.md) オブジェクトのプロパティとリレーションシップを読み取ります。|
|[Create windows81GeneralConfiguration](../api/intune-deviceconfig-windows81generalconfiguration-create.md)|[windows81GeneralConfiguration](../resources/intune-deviceconfig-windows81generalconfiguration.md)|新しい [windows81GeneralConfiguration](../resources/intune-deviceconfig-windows81generalconfiguration.md) オブジェクトを作成します。|
|[Delete windows81GeneralConfiguration](../api/intune-deviceconfig-windows81generalconfiguration-delete.md)|なし|[windows81GeneralConfiguration](../resources/intune-deviceconfig-windows81generalconfiguration.md) を削除します。|
|[Update windows81GeneralConfiguration](../api/intune-deviceconfig-windows81generalconfiguration-update.md)|[windows81GeneralConfiguration](../resources/intune-deviceconfig-windows81generalconfiguration.md)|[windows81GeneralConfiguration](../resources/intune-deviceconfig-windows81generalconfiguration.md) オブジェクトのプロパティを更新します。|

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|id|String|エンティティのキー。 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します|
|lastModifiedDateTime|DateTimeOffset|オブジェクトが最後に変更された DateTime。 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します|
|roleScopeTagIds|String コレクション|このエンティティ インスタンスのスコープのタグのリストです。 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します|
|supportsScopeTags|Boolean|デバイスの構成を基になるスコープのタグの割り当てをサポートしているかどうかを示します。 この値が false であり、エンティティをスコープ指定されたユーザーには表示されませんがある場合、ScopeTags プロパティに割り当てることは許可されていません。 これは、Silverlight で作成されたレガシ ポリシーに対して発生し、削除して、Azure ポータル内のポリシーを再作成することで解決できます。 このプロパティは読み取りのみ可能です。 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します|
|createdDateTime|DateTimeOffset|オブジェクトが作成された DateTime。 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します|
|説明|String|デバイス構成について管理者が提供した説明。 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します|
|displayName|String|デバイス構成について管理者が指定した名前。 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します|
|version|Int32|デバイス構成のバージョン。 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します|
|accountsBlockAddingNonMicrosoftAccountEmail|Boolean|Microsoft アカウントに関連付けられていない電子メール アカウントをユーザーがデバイスに追加できないようにするかどうかを示します。|
|applyOnlyToWindows81|Boolean|このポリシーを Windows 8.1 にのみ適用するかどうかを示す値。 このプロパティは読み取り専用です。|
|browserBlockAutofill|Boolean|自動入力を禁止するかどうかを示します。|
|browserBlockAutomaticDetectionOfIntranetSites|Boolean|イントラネット サイトの自動検出をブロックするかどうかを示します。|
|browserBlockEnterpriseModeAccess|Boolean|エンタープライズ モードのアクセスを禁止するかどうかを示します。|
|browserBlockJavaScript|Boolean|ユーザーが JavaScript を使用することを禁止するかどうかを示します。|
|browserBlockPlugins|Boolean|プラグインを禁止するかどうかを示します。|
|browserBlockPopups|Boolean|ポップアップをブロックするかどうかを示します。|
|browserBlockSendingDoNotTrackHeader|Boolean|ユーザーがトラッキング拒否ヘッダーを送信することを禁止するかどうかを示します。|
|browserBlockSingleWordEntryOnIntranetSites|Boolean|イントラネット サイトでの 1 単語のエントリを禁止するかどうかを示します。|
|browserRequireSmartScreen|Boolean|スマート スクリーン フィルターの使用をユーザーに要求するかどうかを示します。|
|browserEnterpriseModeSiteListLocation|String|エンタープライズ モードのサイト リストの場所。 ローカル ファイル、ローカル ネットワーク、http の場所が該当します。|
|browserInternetSecurityLevel|[internetSiteSecurityLevel](../resources/intune-deviceconfig-internetsitesecuritylevel.md)|インターネット セキュリティ レベル。 可能な値は、`userDefined`、`medium`、`mediumHigh`、`high` です。|
|browserIntranetSecurityLevel|[siteSecurityLevel](../resources/intune-deviceconfig-sitesecuritylevel.md)|イントラネット セキュリティ レベル。 可能な値は、`userDefined`、`low`、`mediumLow`、`medium`、`mediumHigh`、`high` です。|
|browserLoggingReportLocation|String|ログ レポートの場所。|
|browserRequireHighSecurityForRestrictedSites|Boolean|制限付きサイトに対する高度なセキュリティを必要とするかどうかを示します。|
|browserRequireFirewall|Boolean|ファイアウォールが必要かどうかを示します。|
|browserRequireFraudWarning|Boolean|不正行為の警告を必要とするかどうかを示します。|
|browserTrustedSitesSecurityLevel|[siteSecurityLevel](../resources/intune-deviceconfig-sitesecuritylevel.md)|信頼済みサイトのセキュリティ レベル。 可能な値は、`userDefined`、`low`、`mediumLow`、`medium`、`mediumHigh`、`high` です。|
|cellularBlockDataRoaming|Boolean|データ ローミングをブロックするかどうかを示します。|
|diagnosticsBlockDataSubmission|Boolean|診断データの送信をブロックするかどうかを示します。|
|passwordBlockPicturePasswordAndPin|Boolean|ユーザーがピクチャ パスワードおよび暗証番号 (PIN) を使用することを禁止するかどうかを示します。|
|passwordExpirationDays|Int32|パスワードの有効期限 (日数)。|
|passwordMinimumLength|Int32|パスワードの最小文字数。|
|passwordMinutesOfInactivityBeforeScreenTimeout|Int32|画面がタイムアウトになるまでの非アクティブ時間 (分)。|
|passwordMinimumCharacterSetCount|Int32|パスワードに必要な文字セットの数。|
|passwordPreviousPasswordBlockCount|Int32|再使用を禁止する、以前のパスワードの数。 有効な値は 0 から 24 までです|
|passwordRequiredType|[requiredPasswordType](../resources/intune-deviceconfig-requiredpasswordtype.md)|必要なパスワードの種類。 可能な値は、`deviceDefault`、`alphanumeric`、`numeric` です。|
|passwordSignInFailureCountBeforeFactoryReset|Int32|出荷時の設定にリセットされるサインインの失敗回数。|
|storageRequireDeviceEncryption|Boolean|モバイル デバイスでの暗号化が必要かどうかを示します。|
|minimumAutoInstallClassification|[updateClassification](../resources/intune-deviceconfig-updateclassification.md)|最小値は、自動的にインストールするのにはクラス分けを更新します。 可能な値は、`userDefined`、`recommendedAndImportant`、`important`、`none` です。|
|updatesMinimumAutoInstallClassification|[updateClassification](../resources/intune-deviceconfig-updateclassification.md)|最小値は、自動的にインストールするのにはクラス分けを更新します。 可能な値は、`userDefined`、`recommendedAndImportant`、`important`、`none` です。|
|updatesRequireAutomaticUpdates|Boolean|自動更新が必要かどうかを示します。|
|userAccountControlSettings|[windowsUserAccountControlSettings](../resources/intune-deviceconfig-windowsuseraccountcontrolsettings.md)|ユーザー アカウント制御の設定。 可能な値は、`userDefined`、`alwaysNotify`、`notifyOnAppChanges`、`notifyOnAppChangesWithoutDimming`、`neverNotify` です。|
|workFoldersUrl|String|作業フォルダーの URL。|

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
  "@odata.type": "microsoft.graph.windows81GeneralConfiguration"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windows81GeneralConfiguration",
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
  "accountsBlockAddingNonMicrosoftAccountEmail": true,
  "applyOnlyToWindows81": true,
  "browserBlockAutofill": true,
  "browserBlockAutomaticDetectionOfIntranetSites": true,
  "browserBlockEnterpriseModeAccess": true,
  "browserBlockJavaScript": true,
  "browserBlockPlugins": true,
  "browserBlockPopups": true,
  "browserBlockSendingDoNotTrackHeader": true,
  "browserBlockSingleWordEntryOnIntranetSites": true,
  "browserRequireSmartScreen": true,
  "browserEnterpriseModeSiteListLocation": "String",
  "browserInternetSecurityLevel": "String",
  "browserIntranetSecurityLevel": "String",
  "browserLoggingReportLocation": "String",
  "browserRequireHighSecurityForRestrictedSites": true,
  "browserRequireFirewall": true,
  "browserRequireFraudWarning": true,
  "browserTrustedSitesSecurityLevel": "String",
  "cellularBlockDataRoaming": true,
  "diagnosticsBlockDataSubmission": true,
  "passwordBlockPicturePasswordAndPin": true,
  "passwordExpirationDays": 1024,
  "passwordMinimumLength": 1024,
  "passwordMinutesOfInactivityBeforeScreenTimeout": 1024,
  "passwordMinimumCharacterSetCount": 1024,
  "passwordPreviousPasswordBlockCount": 1024,
  "passwordRequiredType": "String",
  "passwordSignInFailureCountBeforeFactoryReset": 1024,
  "storageRequireDeviceEncryption": true,
  "minimumAutoInstallClassification": "String",
  "updatesMinimumAutoInstallClassification": "String",
  "updatesRequireAutomaticUpdates": true,
  "userAccountControlSettings": "String",
  "workFoldersUrl": "String"
}
```




