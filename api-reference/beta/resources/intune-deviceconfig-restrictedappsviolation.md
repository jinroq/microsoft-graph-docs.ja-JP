---
title: restrictedAppsViolation リソースの種類
description: 各ユーザーごとのデバイスの制限されたアプリケーションの構成プロファイルの違反
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: dcbd7def59d17dcd6e906e1e6bef85e3a448b880
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29424981"
---
# <a name="restrictedappsviolation-resource-type"></a>restrictedAppsViolation リソースの種類

> **重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。 実稼働アプリケーションでこれらの API を使用することは、サポートされていません。

> **注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

各ユーザーごとのデバイスの制限されたアプリケーションの構成プロファイルの違反

## <a name="methods"></a>メソッド
|メソッド|戻り値の型|説明|
|:---|:---|:---|
|[リスト restrictedAppsViolations](../api/intune-deviceconfig-restrictedappsviolation-list.md)|[restrictedAppsViolation](../resources/intune-deviceconfig-restrictedappsviolation.md)コレクション|[RestrictedAppsViolation](../resources/intune-deviceconfig-restrictedappsviolation.md)オブジェクトのプロパティと関係を一覧表示します。|
|[RestrictedAppsViolation を取得します。](../api/intune-deviceconfig-restrictedappsviolation-get.md)|[restrictedAppsViolation](../resources/intune-deviceconfig-restrictedappsviolation.md)|[RestrictedAppsViolation](../resources/intune-deviceconfig-restrictedappsviolation.md)オブジェクトのプロパティと関係を参照してください。|
|[RestrictedAppsViolation を作成します。](../api/intune-deviceconfig-restrictedappsviolation-create.md)|[restrictedAppsViolation](../resources/intune-deviceconfig-restrictedappsviolation.md)|新しい[restrictedAppsViolation](../resources/intune-deviceconfig-restrictedappsviolation.md)オブジェクトを作成します。|
|[RestrictedAppsViolation を削除します。](../api/intune-deviceconfig-restrictedappsviolation-delete.md)|なし|の[restrictedAppsViolation](../resources/intune-deviceconfig-restrictedappsviolation.md)を削除します。|
|[RestrictedAppsViolation を更新します。](../api/intune-deviceconfig-restrictedappsviolation-update.md)|[restrictedAppsViolation](../resources/intune-deviceconfig-restrictedappsviolation.md)|[RestrictedAppsViolation](../resources/intune-deviceconfig-restrictedappsviolation.md)オブジェクトのプロパティを更新します。|

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|id|String|オブジェクトの一意の識別子です。 "Accountid"、deviceId、policyId、およびユーザー Id から構成されます。|
|userId|String|ユーザーの一意の識別子の Guid にする必要があります。|
|userName|String|ユーザー名|
|managedDeviceId|String|管理対象デバイスの一意の識別子の Guid にする必要があります。|
|deviceName|String|デバイス名|
|deviceConfigurationId|String|デバイス構成プロファイルの一意の識別子の Guid にする必要があります。|
|deviceConfigurationName|String|デバイス構成のプロファイル名|
|platformType|[policyPlatformType](../resources/intune-deviceconfig-policyplatformtype.md)|プラットフォームの種類。 可能な値は、`android`、`androidForWork`、`iOS`、`macOS`、`windowsPhone81`、`windows81AndLater`、`windows10AndLater`、`androidWorkProfile`、`all` です。|
|restrictedAppsState|[restrictedAppsState](../resources/intune-deviceconfig-restrictedappsstate.md)|アプリケーションの状態を制限します。 使用可能な値は、`prohibitedApps`、`notApprovedApps` です。|
|restrictedApps|[managedDeviceReportedApp](../resources/intune-deviceconfig-manageddevicereportedapp.md)コレクション|違反した制限されたアプリケーションの一覧|

## <a name="relationships"></a>リレーションシップ
なし

## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.restrictedAppsViolation"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.restrictedAppsViolation",
  "id": "String (identifier)",
  "userId": "String",
  "userName": "String",
  "managedDeviceId": "String",
  "deviceName": "String",
  "deviceConfigurationId": "String",
  "deviceConfigurationName": "String",
  "platformType": "String",
  "restrictedAppsState": "String",
  "restrictedApps": [
    {
      "@odata.type": "microsoft.graph.managedDeviceReportedApp",
      "appId": "String"
    }
  ]
}
```




