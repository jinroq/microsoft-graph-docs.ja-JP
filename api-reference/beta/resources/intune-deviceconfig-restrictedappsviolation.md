---
title: restrictedAppsViolation リソースの種類
description: ユーザーごとのデバイスごとの制限付きアプリ構成プロファイルの違反
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: c8764d3d84ba0706f3769ef019def43cb080660d
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/21/2019
ms.locfileid: "30139915"
---
# <a name="restrictedappsviolation-resource-type"></a>restrictedAppsViolation リソースの種類

> **重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

ユーザーごとのデバイスごとの制限付きアプリ構成プロファイルの違反

## <a name="methods"></a>メソッド
|メソッド|戻り値の型|説明|
|:---|:---|:---|
|[リスト restrictedAppsViolations](../api/intune-deviceconfig-restrictedappsviolation-list.md)|[restrictedAppsViolation](../resources/intune-deviceconfig-restrictedappsviolation.md)コレクション|[restrictedAppsViolation](../resources/intune-deviceconfig-restrictedappsviolation.md)オブジェクトのプロパティとリレーションシップをリストします。|
|[restrictedAppsViolation を取得する](../api/intune-deviceconfig-restrictedappsviolation-get.md)|[restrictedAppsViolation](../resources/intune-deviceconfig-restrictedappsviolation.md)|[restrictedAppsViolation](../resources/intune-deviceconfig-restrictedappsviolation.md)オブジェクトのプロパティとリレーションシップを読み取ります。|
|[restrictedAppsViolation を作成する](../api/intune-deviceconfig-restrictedappsviolation-create.md)|[restrictedAppsViolation](../resources/intune-deviceconfig-restrictedappsviolation.md)|新しい[restrictedAppsViolation](../resources/intune-deviceconfig-restrictedappsviolation.md)オブジェクトを作成します。|
|[restrictedAppsViolation の削除](../api/intune-deviceconfig-restrictedappsviolation-delete.md)|なし|[restrictedAppsViolation](../resources/intune-deviceconfig-restrictedappsviolation.md)を削除します。|
|[restrictedAppsViolation の更新](../api/intune-deviceconfig-restrictedappsviolation-update.md)|[restrictedAppsViolation](../resources/intune-deviceconfig-restrictedappsviolation.md)|[restrictedAppsViolation](../resources/intune-deviceconfig-restrictedappsviolation.md)オブジェクトのプロパティを更新します。|

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|id|文字列|オブジェクトの一意識別子。 accountId、deviceId、policyid、および userId から構成されます。|
|userId|String|ユーザーの一意識別子。 Guid である必要があります|
|userName|String|ユーザー名|
|manageddeviceid|String|管理デバイスの一意識別子。 Guid である必要があります|
|deviceName|String|デバイス名|
|deviceConfigurationId|String|デバイス構成プロファイルの一意識別子。 Guid である必要があります|
|deviceConfigurationName|String|デバイス構成プロファイル名|
|platformType|[policyPlatformType](../resources/intune-deviceconfig-policyplatformtype.md)|プラットフォームの種類。 可能な値は、`android`、`androidForWork`、`iOS`、`macOS`、`windowsPhone81`、`windows81AndLater`、`windows10AndLater`、`androidWorkProfile`、`all` です。|
|restrictedAppsState|[restrictedAppsState](../resources/intune-deviceconfig-restrictedappsstate.md)|制限付きアプリの状態。 使用可能な値は、`prohibitedApps`、`notApprovedApps` です。|
|restrictedApps|[manageddevicereportedapp](../resources/intune-deviceconfig-manageddevicereportedapp.md)コレクション|違反した制限付きアプリの一覧|

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




