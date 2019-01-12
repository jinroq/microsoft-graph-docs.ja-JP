---
title: windowsAutopilotDeploymentProfile リソースの種類
description: Windows 自動操縦装置の配置のプロファイル
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 60d72a63cfd4e062c312aeda89a37937b7e03041
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27949396"
---
# <a name="windowsautopilotdeploymentprofile-resource-type"></a>windowsAutopilotDeploymentProfile リソースの種類

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

> **注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。

Windows 自動操縦装置の配置のプロファイル
## <a name="methods"></a>メソッド
|メソッド|戻り値の型|説明|
|:---|:---|:---|
|[WindowsAutopilotDeploymentProfile を取得します。](../api/intune-enrollment-windowsautopilotdeploymentprofile-get.md)|[windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)|[WindowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)オブジェクトのプロパティと関係を参照してください。|
|[assign action](../api/intune-enrollment-windowsautopilotdeploymentprofile-assign.md)|なし|まだ文書化されていません|

## <a name="properties"></a>プロパティ
|プロパティ|種類|説明|
|:---|:---|:---|
|ID|String|プロファイル キー|
|displayName|String|プロファイルの名前|
|説明|String|プロファイルの説明|
|language|String|デバイスで構成されている言語|
|createdDateTime|DateTimeOffset|プロファイルの作成時|
|lastModifiedDateTime|DateTimeOffset|プロファイルの最終更新時刻|
|outOfBoxExperienceSettings|[outOfBoxExperienceSettings](../resources/intune-enrollment-outofboxexperiencesettings.md)|ボックスの設定が発生します。|
|enrollmentStatusScreenSettings|[windowsEnrollmentStatusScreenSettings](../resources/intune-enrollment-windowsenrollmentstatusscreensettings.md)|登録ステータス画面の設定|
|extractHardwareHash|Boolean|プロファイルの HardwareHash の抽出|
|deviceNameTemplate|String|自動操縦装置のデバイスの名前を指定するために使用するテンプレートです。 これは、ユーザー設定のテキスト、デバイスのシリアル番号またはランダムに生成された番号のいずれかが含まれていることもできます。 テンプレートによって生成されたテキストの長さの合計は、15 個以内の文字を使用できます。|

## <a name="relationships"></a>リレーションシップ
|リレーションシップ|型|説明|
|:---|:---|:---|
|assignedDevices|[windowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md)コレクション|プロファイルに割り当てられているデバイスの一覧です。|
|assignments|[windowsAutopilotDeploymentProfileAssignment](../resources/intune-enrollment-windowsautopilotdeploymentprofileassignment.md)コレクション|一連のプロファイルの割り当てをグループ化します。|

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
  "deviceNameTemplate": "String"
}
```





