---
title: windowsAutopilotDeviceIdentity リソースの種類
description: windowsAutopilotDeviceIdentity リソースは、Windows 自動操縦デバイスを表します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 4eaa6f948354164debd73793524d047b1ba204fd
ms.sourcegitcommit: 8eb88cfb48b0eb8f992570caebef577dfa2f30d3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/14/2019
ms.locfileid: "30571439"
---
# <a name="windowsautopilotdeviceidentity-resource-type"></a>windowsAutopilotDeviceIdentity リソースの種類

> **重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

windowsAutopilotDeviceIdentity リソースは、Windows 自動操縦デバイスを表します。

## <a name="methods"></a>メソッド
|メソッド|戻り値の型|説明|
|:---|:---|:---|
|[リスト windowsAutopilotDeviceIdentities](../api/intune-enrollment-windowsautopilotdeviceidentity-list.md)|[windowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md)コレクション|[windowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md)オブジェクトのプロパティとリレーションシップをリストします。|
|[windowsAutopilotDeviceIdentity を取得する](../api/intune-enrollment-windowsautopilotdeviceidentity-get.md)|[windowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md)|[windowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md)オブジェクトのプロパティとリレーションシップを読み取ります。|
|[windowsAutopilotDeviceIdentity を作成する](../api/intune-enrollment-windowsautopilotdeviceidentity-create.md)|[windowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md)|新しい[windowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md)オブジェクトを作成します。|
|[windowsAutopilotDeviceIdentity の削除](../api/intune-enrollment-windowsautopilotdeviceidentity-delete.md)|なし|[windowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md)を削除します。|
|[windowsAutopilotDeviceIdentity の更新](../api/intune-enrollment-windowsautopilotdeviceidentity-update.md)|[windowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md)|[windowsAutopilotDeviceIdentity](../resources/intune-enrollment-windowsautopilotdeviceidentity.md)オブジェクトのプロパティを更新します。|
|[assignUserToDevice アクション](../api/intune-enrollment-windowsautopilotdeviceidentity-assignusertodevice.md)|なし|ユーザーを自動操縦装置に割り当てます。|
|[unassignUserFromDevice アクション](../api/intune-enrollment-windowsautopilotdeviceidentity-unassignuserfromdevice.md)|なし|ユーザーを自動操縦デバイスから割り当てないようにします。|
|[割り当て resourceaccounttodevice アクション](../api/intune-enrollment-windowsautopilotdeviceidentity-assignresourceaccounttodevice.md)|なし|リソースアカウントを自動操縦デバイスに割り当てます。|
|[resourceaccountfromdevice アクションの未割り当て](../api/intune-enrollment-windowsautopilotdeviceidentity-unassignresourceaccountfromdevice.md)|なし|自動操縦デバイスからリソースアカウントを割り当てないようにします。|

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|id|String|オブジェクトの GUID|
|deploymentprofileの状態|[windowsAutopilotProfileAssignmentStatus](../resources/intune-enrollment-windowsautopilotprofileassignmentstatus.md)|Windows 自動操縦デバイスのプロファイル割り当て状態。 可能な値は、`unknown`、`assignedInSync`、`assignedOutOfSync`、`assignedUnkownSyncState`、`notAssigned`、`pending`、`failed` です。|
|deploymentProfileAssignmentDetailedStatus|[windowsAutopilotProfileAssignmentDetailedStatus](../resources/intune-enrollment-windowsautopilotprofileassignmentdetailedstatus.md)|プロファイルの割り当て Windows 自動操縦デバイスの詳細な状態。 可能な値は、`none`、`hardwareRequirementsNotMet` です。|
|deploymentProfileAssignedDateTime|DateTimeOffset|プロファイル Windows 自動操縦デバイスの時間を設定します。|
|orderIdentifier|String|Windows 自動操縦デバイスの注文識別子です。|
|purchaseOrderIdentifier|String|Windows 自動操縦デバイスの注文 id。|
|シリアル番号|String|Windows オートパイロット デバイスのシリアル番号。|
|productKey|String|Windows オートパイロット デバイスのプロダクト キー。|
|manufacturer|String|Windows 自動操縦デバイスの Oem メーカー。|
|model|String|Windows 自動操縦デバイスのモデル名です。|
|enrollmentState|[enrollmentState](../resources/intune-enrollment-enrollmentstate.md)|Windows 自動操縦デバイスの Intune 登録状態。 可能な値は `unknown`、`enrolled`、`pendingReset`、`failed`、`notContacted`、`blocked` です。|
|lastContactedDateTime|DateTimeOffset|Intune 前回の接続 Windows 自動操縦デバイスの日時。|
|addressableusername|String|アドレス指定可能なユーザー名。|
|userPrincipalName|String|ユーザープリンシパル名。|
|resourceName|String|リソース名。|
|skuNumber|String|SKU 番号|
|systemfamily|String|システムファミリ|
|azureActiveDirectoryDeviceId|String|AAD デバイス ID|
|manageddeviceid|String|管理対象デバイス ID|

## <a name="relationships"></a>関係
|リレーションシップ|型|説明|
|:---|:---|:---|
|deploymentprofile|[windowsAutopilotDeploymentProfile](../resources/intune-enrollment-windowsautopilotdeploymentprofile.md)|Windows 自動操縦デバイスに現在割り当てられている展開プロファイル。|
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




