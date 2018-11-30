---
title: deviceManagementScriptDeviceState リソースの種類
description: 状態のデバイスの管理スクリプトを実行するデバイスのプロパティが含まれています。
ms.openlocfilehash: 11c9e574e880df371f45181dd02fdb2292d0cb15
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27074259"
---
# <a name="devicemanagementscriptdevicestate-resource-type"></a>deviceManagementScriptDeviceState リソースの種類

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

> **注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。

状態のデバイスの管理スクリプトを実行するデバイスのプロパティが含まれています。
## <a name="methods"></a>メソッド
|メソッド|戻り値の型|説明|
|:---|:---|:---|
|[リスト deviceManagementScriptDeviceStates](../api/intune-devices-devicemanagementscriptdevicestate-list.md)|[deviceManagementScriptDeviceState](../resources/intune-devices-devicemanagementscriptdevicestate.md)コレクション|[DeviceManagementScriptDeviceState](../resources/intune-devices-devicemanagementscriptdevicestate.md)オブジェクトのプロパティと関係を一覧表示します。|
|[DeviceManagementScriptDeviceState を取得します。](../api/intune-devices-devicemanagementscriptdevicestate-get.md)|[deviceManagementScriptDeviceState](../resources/intune-devices-devicemanagementscriptdevicestate.md)|[DeviceManagementScriptDeviceState](../resources/intune-devices-devicemanagementscriptdevicestate.md)オブジェクトのプロパティと関係を参照してください。|
|[DeviceManagementScriptDeviceState を作成します。](../api/intune-devices-devicemanagementscriptdevicestate-create.md)|[deviceManagementScriptDeviceState](../resources/intune-devices-devicemanagementscriptdevicestate.md)|新しい[deviceManagementScriptDeviceState](../resources/intune-devices-devicemanagementscriptdevicestate.md)オブジェクトを作成します。|
|[DeviceManagementScriptDeviceState を削除します。](../api/intune-devices-devicemanagementscriptdevicestate-delete.md)|なし|の[deviceManagementScriptDeviceState](../resources/intune-devices-devicemanagementscriptdevicestate.md)を削除します。|
|[DeviceManagementScriptDeviceState を更新します。](../api/intune-devices-devicemanagementscriptdevicestate-update.md)|[deviceManagementScriptDeviceState](../resources/intune-devices-devicemanagementscriptdevicestate.md)|[DeviceManagementScriptDeviceState](../resources/intune-devices-devicemanagementscriptdevicestate.md)オブジェクトのプロパティを更新します。|

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|id|String|デバイス管理スクリプト デバイス状態のエンティティのキーです。|
|runState|[runState](../resources/intune-shared-runstate.md)|デバイス管理スクリプトの実行を最新の状態です。 可能な値は、`unknown`、`success`、`fail` です。|
|resultMessage|String|実行結果の詳細です。|
|lastStateUpdateDateTime|DateTimeOffset|最新の時間、デバイスの管理スクリプトを実行します。|
|errorCode|Int32|デバイス管理スクリプトの実行がエラーに対応するエラー ・ コードです。|
|errorDescription|String|デバイス管理スクリプトの実行がエラーに対応するエラーの説明です。|

## <a name="relationships"></a>リレーションシップ
|リレーションシップ|型|説明|
|:---|:---|:---|
|managedDevice|[managedDevice](../resources/intune-devices-manageddevice.md)|デバイスの管理スクリプトを実行する管理対象のデバイスです。|

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





