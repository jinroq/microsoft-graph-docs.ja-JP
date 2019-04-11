---
title: windowskioskconfiguration リソースの種類
description: このエンティティは、kiosk リソースが公開する宣言されたメソッド、プロパティ、リレーションシップについて説明します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 92cea089ea86e1ad56607442ac983d83c0c78e68
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/11/2019
ms.locfileid: "31784580"
---
# <a name="windowskioskconfiguration-resource-type"></a>windowskioskconfiguration リソースの種類

> **重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

このエンティティは、kiosk リソースが公開する宣言されたメソッド、プロパティ、リレーションシップについて説明します。


[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します

## <a name="methods"></a>メソッド
|メソッド|戻り値の型|説明|
|:---|:---|:---|
|[windowskioskconfigurations を一覧表示する](../api/intune-deviceconfig-windowskioskconfiguration-list.md)|[windowskioskconfiguration](../resources/intune-deviceconfig-windowskioskconfiguration.md)コレクション|[windowskioskconfiguration](../resources/intune-deviceconfig-windowskioskconfiguration.md)オブジェクトのプロパティとリレーションシップをリストします。|
|[windowskioskconfiguration の取得](../api/intune-deviceconfig-windowskioskconfiguration-get.md)|[windowsKioskConfiguration](../resources/intune-deviceconfig-windowskioskconfiguration.md)|[windowskioskconfiguration](../resources/intune-deviceconfig-windowskioskconfiguration.md)オブジェクトのプロパティとリレーションシップを読み取ります。|
|[windowskioskconfiguration の作成](../api/intune-deviceconfig-windowskioskconfiguration-create.md)|[windowsKioskConfiguration](../resources/intune-deviceconfig-windowskioskconfiguration.md)|新しい[windowskioskconfiguration](../resources/intune-deviceconfig-windowskioskconfiguration.md)オブジェクトを作成します。|
|[windowskioskconfiguration の削除](../api/intune-deviceconfig-windowskioskconfiguration-delete.md)|なし|[windowskioskconfiguration](../resources/intune-deviceconfig-windowskioskconfiguration.md)を削除します。|
|[windowskioskconfiguration の更新](../api/intune-deviceconfig-windowskioskconfiguration-update.md)|[windowsKioskConfiguration](../resources/intune-deviceconfig-windowskioskconfiguration.md)|[windowskioskconfiguration](../resources/intune-deviceconfig-windowskioskconfiguration.md)オブジェクトのプロパティを更新します。|

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
|kioskProfiles|[windowskioskprofile](../resources/intune-deviceconfig-windowskioskprofile.md)コレクション|このポリシー設定を使用すると、キオスクの構成のキオスクプロファイルの一覧を定義できます。 このコレクションには、最大3つの要素を含めることができます。|
|kioskBrowserDefaultUrl|文字列|ブラウザーが起動時に移動する既定の URL を指定します。|
|kioskBrowserEnableHomeButton|Boolean|キオスクブラウザーの [ホーム] ボタンを有効にします。 既定では、[ホーム] ボタンは無効になっています。|
|kioskBrowserEnableNavigationButtons|Boolean|キオスクブラウザーのナビゲーションボタン (前方/後方) を有効にします。 既定では、ナビゲーションボタンは無効になっています。|
|kioskBrowserEnableEndSessionButton|Boolean|キオスクブラウザーの [セッションの終了] ボタンを有効にします。 既定では、[セッションの終了] ボタンは無効になっています。|
|kioskBrowserRestartOnIdleTimeInMinutes|Int32|キオスクブラウザーが新しい状態で再起動するまで、セッションがアイドル状態になっている時間 (分) を指定します。  有効な値は1-1440 です。 有効な値は 1 ~ 1440|
|kioskBrowserBlockedURLs|String コレクション|キオスクブラウザーが移動しない url を指定する|
|kioskBrowserBlockedUrlExceptions|String コレクション|キオスクブラウザーでの移動が許可されている url を指定する|
|edgeKioskEnablePublicBrowsing|Boolean|Microsoft Edge ブラウザーのパブリックブラウズキオスクモードを有効にします。 既定値は false です。|

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
  "@odata.type": "microsoft.graph.windowsKioskConfiguration"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsKioskConfiguration",
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
  "kioskProfiles": [
    {
      "@odata.type": "microsoft.graph.windowsKioskProfile",
      "profileId": "String",
      "profileName": "String",
      "appConfiguration": {
        "@odata.type": "microsoft.graph.windowsKioskMultipleApps",
        "apps": [
          {
            "@odata.type": "microsoft.graph.windowsKioskUWPApp",
            "startLayoutTileSize": "String",
            "name": "String",
            "appType": "String",
            "autoLaunch": true,
            "appUserModelId": "String",
            "appId": "String",
            "containedAppId": "String"
          }
        ],
        "showTaskBar": true,
        "allowAccessToDownloadsFolder": true,
        "disallowDesktopApps": true,
        "startMenuLayoutXml": "binary"
      },
      "userAccountsConfiguration": [
        {
          "@odata.type": "microsoft.graph.windowsKioskVisitor"
        }
      ]
    }
  ],
  "kioskBrowserDefaultUrl": "String",
  "kioskBrowserEnableHomeButton": true,
  "kioskBrowserEnableNavigationButtons": true,
  "kioskBrowserEnableEndSessionButton": true,
  "kioskBrowserRestartOnIdleTimeInMinutes": 1024,
  "kioskBrowserBlockedURLs": [
    "String"
  ],
  "kioskBrowserBlockedUrlExceptions": [
    "String"
  ],
  "edgeKioskEnablePublicBrowsing": true
}
```





