---
title: windowsAutopilotDeploymentProfile リソースの種類
description: Windows 自動操縦展開プロファイル
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 69035ba93b04ac66ce9e8883c7b5f7b04dff429a
ms.sourcegitcommit: f58ff560fa02ac95e296375c143b0922fb6a425c
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/19/2019
ms.locfileid: "30572461"
---
# <a name="windowsautopilotdeploymentprofile-resource-type"></a>windowsAutopilotDeploymentProfile リソースの種類

> **重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

Windows 自動操縦展開プロファイル

## <a name="methods"></a>メソッド
|メソッド|戻り値の型|説明|
|:---|:---|:---|
|[windowsAutopilotDeploymentProfile を取得する](../api/intune-enrollment-windowsautopilotdeploymentprofile-get.md)|[windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)|[windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)オブジェクトのプロパティとリレーションシップを読み取ります。|
|[assign アクション](../api/intune-enrollment-windowsautopilotdeploymentprofile-assign.md)|なし|まだ文書化されていません|

## <a name="properties"></a>プロパティ
|プロパティ|種類|説明|
|:---|:---|:---|
|id|String|プロファイルキー|
|displayName|String|プロファイルの名前|
|description|String|プロファイルの説明|
|language|String|デバイスで構成されている言語|
|createdDateTime|DateTimeOffset|プロファイルの作成時刻|
|lastModifiedDateTime|DateTimeOffset|プロファイルの最終変更日時|
|outOfBoxExperienceSettings|[outOfBoxExperienceSettings](../resources/intune-enrollment-outofboxexperiencesettings.md)|不在時の環境設定|
|enrollmentStatusScreenSettings|[windowsEnrollmentStatusScreenSettings](../resources/intune-enrollment-windowsenrollmentstatusscreensettings.md)|登録の状態画面の設定|
|extractHardwareHash|Boolean|プロファイルのハードウェアハッシュ抽出|
|deviceNameTemplate|String|自動操縦デバイスの名前を指定するときに使用するテンプレートを指定します。 これはカスタムテキストにすることができ、デバイスのシリアル番号またはランダムに生成された番号のいずれかを含めることもできます。 テンプレートによって生成されるテキストの合計の長さは、15文字以下でなければなりません。|
|deviceType|[windowsAutopilotDeviceType](../resources/intune-enrollment-windowsautopilotdevicetype.md)|このプロファイルを適用できる自動操縦デバイスの種類。 可能な値は、`windowsPc`、`surfaceHub2` です。|
|enableホワイトグローブ|Boolean|プロファイルの自動操縦白の手袋を有効にします。|

## <a name="relationships"></a>関係
|リレーションシップ|型|説明|
|:---|:---|:---|
|assignedDevices|[windowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md)コレクション|プロファイルに割り当てられているデバイスのリスト。|
|assignments|[windowsAutopilotDeploymentProfileAssignment](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md)コレクション|プロファイルのグループの割り当てのリスト。|

## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.windowsAutopilotDeploymentProfile"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsAutopilotDeploymentProfile",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String",
  "language": "String",
  "createdDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)",
  "outOfBoxExperienceSettings": {
    "@odata.type": "microsoft.graph.outOfBoxExperienceSettings",
    "hidePrivacySettings": true,
    "hideEULA": true,
    "userType": "String",
    "deviceUsageType": "String",
    "skipKeyboardSelectionPage": true,
    "hideEscapeLink": true
  },
  "enrollmentStatusScreenSettings": {
    "@odata.type": "microsoft.graph.windowsEnrollmentStatusScreenSettings",
    "hideInstallationProgress": true,
    "allowDeviceUseBeforeProfileAndAppInstallComplete": true,
    "blockDeviceSetupRetryByUser": true,
    "allowLogCollectionOnInstallFailure": true,
    "customErrorMessage": "String",
    "installProgressTimeoutInMinutes": 1024,
    "allowDeviceUseOnInstallFailure": true
  },
  "extractHardwareHash": true,
  "deviceNameTemplate": "String",
  "deviceType": "String",
  "enableWhiteGlove": true
}
```




