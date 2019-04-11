---
title: macOSDeviceFeaturesConfiguration リソースの種類
description: MacOS デバイス機能構成のプロファイル。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: e979fbfeac1c355f23c7e58ad0e34bab7b761d76
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/11/2019
ms.locfileid: "31782983"
---
# <a name="macosdevicefeaturesconfiguration-resource-type"></a>macOSDeviceFeaturesConfiguration リソースの種類

> **重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

MacOS デバイス機能構成のプロファイル。


[appleDeviceFeaturesConfigurationBase](../resources/intune-deviceconfig-appledevicefeaturesconfigurationbase.md) から継承します

## <a name="methods"></a>メソッド
|メソッド|戻り値の型|説明|
|:---|:---|:---|
|[macOSDeviceFeaturesConfigurations のリスト](../api/intune-deviceconfig-macosdevicefeaturesconfiguration-list.md)|[macOSDeviceFeaturesConfiguration](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md) コレクション|[macOSDeviceFeaturesConfiguration](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md) オブジェクトのプロパティとリレーションシップをリストします。|
|[macOSDeviceFeaturesConfiguration の取得](../api/intune-deviceconfig-macosdevicefeaturesconfiguration-get.md)|[macOSDeviceFeaturesConfiguration](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md)|[macOSDeviceFeaturesConfiguration](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md) オブジェクトのプロパティとリレーションシップを読み取ります。|
|[macOSDeviceFeaturesConfiguration の作成](../api/intune-deviceconfig-macosdevicefeaturesconfiguration-create.md)|[macOSDeviceFeaturesConfiguration](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md)|新しい [macOSDeviceFeaturesConfiguration](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md) オブジェクトを作成します。|
|[macOSDeviceFeaturesConfiguration の削除](../api/intune-deviceconfig-macosdevicefeaturesconfiguration-delete.md)|なし|[macOSDeviceFeaturesConfiguration](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md) を削除します。|
|[macOSDeviceFeaturesConfiguration の更新](../api/intune-deviceconfig-macosdevicefeaturesconfiguration-update.md)|[macOSDeviceFeaturesConfiguration](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md)|[macOSDeviceFeaturesConfiguration](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md) オブジェクトのプロパティを更新します。|

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
|放映した print行先|[放映 printdestination](../resources/intune-deviceconfig-airprintdestination.md)コレクション|常に表示される必要がある、放映中の印刷プリンターの配列です。 このコレクションには、最大で 500 個の要素を含めることができます。 [appleDeviceFeaturesConfigurationBase](../resources/intune-deviceconfig-appledevicefeaturesconfigurationbase.md)から継承します。|
|autoLaunchItems|[macoslaunchitem](../resources/intune-deviceconfig-macoslaunchitem.md)コレクション|ユーザーがログインしたときに起動するアプリケーション、ファイル、フォルダー、およびその他のアイテムのリスト。 このコレクションには、最大で 500 個の要素を含めることができます。|
|adminshoの stinfo|Boolean|ログインウィンドウに管理ホスト情報を表示するかどうかを指定します。|
|loginwindowtext|文字列|ログインウィンドウに表示されるカスタムテキスト。|
|authorizedUsersListHidden|Boolean|ログインウィンドウで [名前とパスワード] ダイアログを表示するか、ユーザーの一覧を表示するかを指定します。|
|authorizedUsersListHideLocalUsers|Boolean|ログインウィンドウの承認済みユーザーの一覧に、ネットワークユーザーとシステムユーザーのみを表示するかどうかを指定します。|
|authorizedUsersListHideMobileAccounts|Boolean|ログインウィンドウの承認されたユーザーの一覧でモバイルユーザーを非表示にするかどうかを指定します。|
|authorizedUsersListIncludeNetworkUsers|Boolean|[ログイン] ウィンドウで、承認されたユーザーの一覧にネットワークユーザーを表示するかどうかを指定します。|
|authorizedUsersListHideAdminUsers|Boolean|ログインウィンドウの承認されたユーザーの一覧で管理者ユーザーを非表示にするかどうかを指定します。|
|authorizedUsersListShowOtherManagedUsers|Boolean|[ログイン] ウィンドウで、承認されたユーザーの一覧に他のユーザーを表示するかどうかを指定します。|
|shutdowndisabled|Boolean|ログインウィンドウで [シャットダウン] ボタンの項目を非表示にするかどうかを指定します。|
|restartDisabled|Boolean|ログインウィンドウで [再起動] ボタンの項目を非表示にするかどうかを指定します。|
|sleepDisabled|Boolean|ログインウィンドウで [スリープ] メニュー項目を非表示にするかどうかを指定します。|
|consoleaccessdisabled|Boolean|他のユーザーが ' >console> 特殊ユーザー名の使用を無視するかどうか。|
|shutDownDisabledWhileLoggedIn|Boolean|ログインウィンドウの [シャットダウン] メニュー項目が、ユーザーのログイン中に無効になるかどうか。|
|restartDisabledWhileLoggedIn|Boolean|ログインウィンドウの [再起動] メニュー項目が、ユーザーのログイン中に無効になるかどうか。|
|powerOffDisabledWhileLoggedIn|Boolean|ログインウィンドウの [電源オフ] メニュー項目が、ユーザーのログイン中に無効になるかどうかを指定します。|
|logOutDisabledWhileLoggedIn|Boolean|ログインウィンドウの [Log Out] メニュー項目が、ユーザーのログイン中に無効になるかどうかを指定します。|
|screenlockdisableimmediate|Boolean|即時画面ロック機能を無効にするかどうかを指定します。|

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
  "@odata.type": "microsoft.graph.macOSDeviceFeaturesConfiguration"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.macOSDeviceFeaturesConfiguration",
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
  "airPrintDestinations": [
    {
      "@odata.type": "microsoft.graph.airPrintDestination",
      "ipAddress": "String",
      "resourcePath": "String",
      "port": 1024,
      "forceTls": true
    }
  ],
  "autoLaunchItems": [
    {
      "@odata.type": "microsoft.graph.macOSLaunchItem",
      "path": "String",
      "hide": true
    }
  ],
  "adminShowHostInfo": true,
  "loginWindowText": "String",
  "authorizedUsersListHidden": true,
  "authorizedUsersListHideLocalUsers": true,
  "authorizedUsersListHideMobileAccounts": true,
  "authorizedUsersListIncludeNetworkUsers": true,
  "authorizedUsersListHideAdminUsers": true,
  "authorizedUsersListShowOtherManagedUsers": true,
  "shutDownDisabled": true,
  "restartDisabled": true,
  "sleepDisabled": true,
  "consoleAccessDisabled": true,
  "shutDownDisabledWhileLoggedIn": true,
  "restartDisabledWhileLoggedIn": true,
  "powerOffDisabledWhileLoggedIn": true,
  "logOutDisabledWhileLoggedIn": true,
  "screenLockDisableImmediate": true
}
```





