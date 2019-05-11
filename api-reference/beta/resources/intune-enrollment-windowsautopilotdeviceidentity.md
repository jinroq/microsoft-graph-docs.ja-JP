---
title: windowsAutopilotDeviceIdentity リソースの種類
description: WindowsAutopilotDeviceIdentity リソースは、Windows 自動操縦デバイスを表します。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 7ec5470519e0d68ef5fbd267130f4aa5ffdf8b8f
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/11/2019
ms.locfileid: "33941451"
---
# <a name="windowsautopilotdeviceidentity-resource-type"></a>windowsAutopilotDeviceIdentity リソースの種類

> **重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

WindowsAutopilotDeviceIdentity リソースは、Windows 自動操縦デバイスを表します。

## <a name="methods"></a>メソッド
|メソッド|戻り値の型|説明|
|:---|:---|:---|
|[リスト windowsAutopilotDeviceIdentities](../api/intune-enrollment-windowsautopilotdeviceidentity-list.md)|[windowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md)コレクション|[WindowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md)オブジェクトのプロパティとリレーションシップをリストします。|
|[WindowsAutopilotDeviceIdentity を取得する](../api/intune-enrollment-windowsautopilotdeviceidentity-get.md)|[windowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md)|[WindowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md)オブジェクトのプロパティとリレーションシップを読み取ります。|
|[WindowsAutopilotDeviceIdentity を作成する](../api/intune-enrollment-windowsautopilotdeviceidentity-create.md)|[windowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md)|新しい[windowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md)オブジェクトを作成します。|
|[WindowsAutopilotDeviceIdentity の削除](../api/intune-enrollment-windowsautopilotdeviceidentity-delete.md)|None|[WindowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md)を削除します。|
|[WindowsAutopilotDeviceIdentity の更新](../api/intune-enrollment-windowsautopilotdeviceidentity-update.md)|[windowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md)|[WindowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md)オブジェクトのプロパティを更新します。|
|[assignUserToDevice アクション](../api/intune-enrollment-windowsautopilotdeviceidentity-assignusertodevice.md)|None|ユーザーを自動操縦装置に割り当てます。|
|[unassignUserFromDevice アクション](../api/intune-enrollment-windowsautopilotdeviceidentity-unassignuserfromdevice.md)|None|ユーザーを自動操縦デバイスから割り当てないようにします。|
|[assignResourceAccountToDevice アクション](../api/intune-enrollment-windowsautopilotdeviceidentity-assignresourceaccounttodevice.md)|None|リソースアカウントを自動操縦デバイスに割り当てます。|
|[unassignResourceAccountFromDevice アクション](../api/intune-enrollment-windowsautopilotdeviceidentity-unassignresourceaccountfromdevice.md)|None|自動操縦デバイスからリソースアカウントを割り当てないようにします。|

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|id|文字列|オブジェクトの GUID|
|Deploymentprofileの状態|[windowsAutopilotProfileAssignmentStatus](../resources/intune-enrollment-windowsautopilotprofileassignmentstatus.md)|Windows 自動操縦デバイスのプロファイル割り当て状態。 可能な値は、`unknown`、`assignedInSync`、`assignedOutOfSync`、`assignedUnkownSyncState`、`notAssigned`、`pending`、`failed` です。|
|deploymentProfileAssignmentDetailedStatus|[windowsAutopilotProfileAssignmentDetailedStatus](../resources/intune-enrollment-windowsautopilotprofileassignmentdetailedstatus.md)|プロファイルの割り当て Windows 自動操縦デバイスの詳細な状態。 可能な値は、`none`、`hardwareRequirementsNotMet` です。|
|deploymentProfileAssignedDateTime|DateTimeOffset|プロファイル Windows 自動操縦デバイスの時間を設定します。|
|orderIdentifier|String|Windows 自動操縦デバイスの注文識別子-非推奨|
|groupTag|String|Windows 自動操縦デバイスのグループタグ。|
|purchaseOrderIdentifier|String|Windows 自動操縦デバイスの注文 Id。|
|シリアル番号|String|Windows オートパイロット デバイスのシリアル番号。|
|productKey|String|Windows オートパイロット デバイスのプロダクト キー。|
|manufacturer|String|Windows 自動操縦デバイスの Oem メーカー。|
|model|String|Windows 自動操縦デバイスのモデル名です。|
|enrollmentState|[enrollmentState](../resources/intune-enrollment-enrollmentstate.md)|Windows 自動操縦デバイスの Intune 登録状態。 使用可能な値: `unknown`、`enrolled`、`pendingReset`、`failed`、`notContacted`、`blocked`。|
|lastContactedDateTime|DateTimeOffset|Intune 前回の接続 Windows 自動操縦デバイスの日時。|
|addressableUserName|String|アドレス指定可能なユーザー名。|
|userPrincipalName|String|ユーザープリンシパル名。|
|resourceName|String|リソース名。|
|skuNumber|String|SKU 番号|
|systemFamily|String|システムファミリ|
|azureActiveDirectoryDeviceId|String|AAD デバイス ID|
|managedDeviceId|String|管理対象デバイス ID|

## <a name="relationships"></a>関係
|リレーションシップ|型|説明|
|:---|:---|:---|
|deploymentProfile|[windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)|Windows 自動操縦デバイスに現在割り当てられている展開プロファイル。|
|intendedDeploymentProfile|[windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)|Windows 自動操縦デバイスに割り当てられる展開プロファイル。|

## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.windowsAutopilotDeviceIdentity"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsAutopilotDeviceIdentity",
  "id": "String (identifier)",
  "deploymentProfileAssignmentStatus": "String",
  "deploymentProfileAssignmentDetailedStatus": "String",
  "deploymentProfileAssignedDateTime": "String (timestamp)",
  "orderIdentifier": "String",
  "groupTag": "String",
  "purchaseOrderIdentifier": "String",
  "serialNumber": "String",
  "productKey": "String",
  "manufacturer": "String",
  "model": "String",
  "enrollmentState": "String",
  "lastContactedDateTime": "String (timestamp)",
  "addressableUserName": "String",
  "userPrincipalName": "String",
  "resourceName": "String",
  "skuNumber": "String",
  "systemFamily": "String",
  "azureActiveDirectoryDeviceId": "String",
  "managedDeviceId": "String"
}
```




