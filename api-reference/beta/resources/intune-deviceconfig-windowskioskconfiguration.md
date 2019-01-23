---
title: windowsKioskConfiguration リソースの種類
description: このエンティティは、宣言されたメソッド、プロパティおよびキオスクのリソースによって公開されているリレーションシップの説明を提供します。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: f091d9700721a1be1baf5982b0fb8ce0fe3b00ec
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29403960"
---
# <a name="windowskioskconfiguration-resource-type"></a>windowsKioskConfiguration リソースの種類

> **重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。 実稼働アプリケーションでこれらの API を使用することは、サポートされていません。

> **注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

このエンティティは、宣言されたメソッド、プロパティおよびキオスクのリソースによって公開されているリレーションシップの説明を提供します。


[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します

## <a name="methods"></a>メソッド
|メソッド|戻り値の型|説明|
|:---|:---|:---|
|[リスト windowsKioskConfigurations](../api/intune-deviceconfig-windowskioskconfiguration-list.md)|[windowsKioskConfiguration](../resources/intune-deviceconfig-windowskioskconfiguration.md)コレクション|[WindowsKioskConfiguration](../resources/intune-deviceconfig-windowskioskconfiguration.md)オブジェクトのプロパティと関係を一覧表示します。|
|[WindowsKioskConfiguration を取得します。](../api/intune-deviceconfig-windowskioskconfiguration-get.md)|[windowsKioskConfiguration](../resources/intune-deviceconfig-windowskioskconfiguration.md)|[WindowsKioskConfiguration](../resources/intune-deviceconfig-windowskioskconfiguration.md)オブジェクトのプロパティと関係を参照してください。|
|[WindowsKioskConfiguration を作成します。](../api/intune-deviceconfig-windowskioskconfiguration-create.md)|[windowsKioskConfiguration](../resources/intune-deviceconfig-windowskioskconfiguration.md)|新しい[windowsKioskConfiguration](../resources/intune-deviceconfig-windowskioskconfiguration.md)オブジェクトを作成します。|
|[WindowsKioskConfiguration を削除します。](../api/intune-deviceconfig-windowskioskconfiguration-delete.md)|なし|の[windowsKioskConfiguration](../resources/intune-deviceconfig-windowskioskconfiguration.md)を削除します。|
|[WindowsKioskConfiguration を更新します。](../api/intune-deviceconfig-windowskioskconfiguration-update.md)|[windowsKioskConfiguration](../resources/intune-deviceconfig-windowskioskconfiguration.md)|[WindowsKioskConfiguration](../resources/intune-deviceconfig-windowskioskconfiguration.md)オブジェクトのプロパティを更新します。|

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
|kioskProfiles|[windowsKioskProfile](../resources/intune-deviceconfig-windowskioskprofile.md)コレクション|このポリシー設定は、構成のキオスクのキオスクのプロファイルの一覧を定義します。 このコレクションには、3 つの要素の最大を含めることができます。|
|kioskBrowserDefaultUrl|String|起動時にブラウザーが移動する必要があります既定の URL を指定します。|
|kioskBrowserEnableHomeButton|Boolean|キオスク ブラウザーの [ホーム] ボタンを有効にします。 既定では、[ホーム] ボタンは無効になります。|
|kioskBrowserEnableNavigationButtons|Boolean|キオスク ブラウザーのナビゲーションの buttons(forward/back) を有効にします。 既定では、ナビゲーション ボタンは無効になります。|
|kioskBrowserEnableEndSessionButton|Boolean|キオスク ブラウザーの最後のセッションのボタンを有効にします。 既定では、セッションの終了] ボタンは無効になります。|
|kioskBrowserRestartOnIdleTimeInMinutes|Int32|キオスク ブラウザーを最新の状態で再起動するまで、セッションがアイドル状態の分数を指定します。  有効な値は、1 ~ 1440 です。 1 から 1440 の有効な値|
|kioskBrowserBlockedURLs|String コレクション|キオスクのブラウザーの移動先のない Url を指定します。|
|kioskBrowserBlockedUrlExceptions|String コレクション|キオスクのブラウザーに移動するのには許可されている Url を指定します。|
|edgeKioskEnablePublicBrowsing|Boolean|マイクロソフトのエッジのブラウザーの閲覧のキオスク モードを公開を有効にします。 既定では false です。|
|edgeKioskResetAfterIdleTimeInMinutes|Int32|マイクロソフトのエッジのキオスクをリセットする前に、最後のユーザーの利用状況から分単位で時間を指定します。  有効な値は、0 ~ 1440 です。 既定値は 5 です。 0 は、リセットがないことを示します。 有効な値の 0 から 1440|

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
            "appUserModelId": "String",
            "appId": "String",
            "containedAppId": "String"
          }
        ],
        "showTaskBar": true,
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
  "edgeKioskEnablePublicBrowsing": true,
  "edgeKioskResetAfterIdleTimeInMinutes": 1024
}
```




