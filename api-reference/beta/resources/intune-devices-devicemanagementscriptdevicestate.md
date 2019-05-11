---
title: deviceManagementScriptDeviceState リソースの種類
description: デバイス管理スクリプトのデバイスの実行状態のプロパティが含まれています。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 18e9e78898671d2c64381f7c3f4fa597ca862456
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/11/2019
ms.locfileid: "33942116"
---
# <a name="devicemanagementscriptdevicestate-resource-type"></a>deviceManagementScriptDeviceState リソースの種類

> **重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

デバイス管理スクリプトのデバイスの実行状態のプロパティが含まれています。

## <a name="methods"></a>メソッド
|メソッド|戻り値の型|説明|
|:---|:---|:---|
|[リスト deviceManagementScriptDeviceStates](../api/intune-devices-devicemanagementscriptdevicestate-list.md)|[Devicemanagementscriptdevicestate](../resources/intune-devices-devicemanagementscriptdevicestate.md)コレクション|[Devicemanagementscriptdevicestate](../resources/intune-devices-devicemanagementscriptdevicestate.md)オブジェクトのプロパティとリレーションシップをリストします。|
|[DeviceManagementScriptDeviceState の取得](../api/intune-devices-devicemanagementscriptdevicestate-get.md)|[deviceManagementScriptDeviceState](../resources/intune-devices-devicemanagementscriptdevicestate.md)|[Devicemanagementscriptdevicestate](../resources/intune-devices-devicemanagementscriptdevicestate.md)オブジェクトのプロパティとリレーションシップを読み取ります。|
|[DeviceManagementScriptDeviceState の作成](../api/intune-devices-devicemanagementscriptdevicestate-create.md)|[deviceManagementScriptDeviceState](../resources/intune-devices-devicemanagementscriptdevicestate.md)|新しい[Devicemanagementscriptdevicestate](../resources/intune-devices-devicemanagementscriptdevicestate.md)オブジェクトを作成します。|
|[DeviceManagementScriptDeviceState の削除](../api/intune-devices-devicemanagementscriptdevicestate-delete.md)|None|[Devicemanagementscriptdevicestate](../resources/intune-devices-devicemanagementscriptdevicestate.md)を削除します。|
|[DeviceManagementScriptDeviceState の更新](../api/intune-devices-devicemanagementscriptdevicestate-update.md)|[deviceManagementScriptDeviceState](../resources/intune-devices-devicemanagementscriptdevicestate.md)|[Devicemanagementscriptdevicestate](../resources/intune-devices-devicemanagementscriptdevicestate.md)オブジェクトのプロパティを更新します。|

## <a name="properties"></a>プロパティ
|プロパティ|種類|説明|
|:---|:---|:---|
|id|String|デバイス管理スクリプトのデバイス状態エンティティのキー。|
|runState|[runState](../resources/intune-shared-runstate.md)|デバイス管理スクリプトの最新の実行の状態。 可能な値は、`unknown`、`success`、`fail` です。|
|resultMessage|String|実行出力の詳細。|
|lastStateUpdateDateTime|DateTimeOffset|デバイス管理スクリプトが最後に実行された時刻。|
|errorCode|Int32|デバイス管理スクリプトの誤った実行に対応するエラーコード。|
|errorDescription|String|デバイス管理スクリプトの誤った実行に対応するエラーの説明。|

## <a name="relationships"></a>関係
|リレーションシップ|型|説明|
|:---|:---|:---|
|managedDevice|[managedDevice](../resources/intune-devices-manageddevice.md)|デバイス管理スクリプトを実行する管理対象デバイス。|

## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceManagementScriptDeviceState"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementScriptDeviceState",
  "id": "String (identifier)",
  "runState": "String",
  "resultMessage": "String",
  "lastStateUpdateDateTime": "String (timestamp)",
  "errorCode": 1024,
  "errorDescription": "String"
}
```




