---
title: deviceManagementScriptUserState リソースの種類
description: 状態のデバイスの管理スクリプトを実行するユーザーのプロパティが含まれています。
ms.openlocfilehash: 4e444c1eee438acba558a85e2a4ada14e44849bc
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27074260"
---
# <a name="devicemanagementscriptuserstate-resource-type"></a>deviceManagementScriptUserState リソースの種類

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

> **注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。

状態のデバイスの管理スクリプトを実行するユーザーのプロパティが含まれています。
## <a name="methods"></a>メソッド
|メソッド|戻り値の型|説明|
|:---|:---|:---|
|[リスト deviceManagementScriptUserStates](../api/intune-devices-devicemanagementscriptuserstate-list.md)|[deviceManagementScriptUserState](../resources/intune-devices-devicemanagementscriptuserstate.md)コレクション|[DeviceManagementScriptUserState](../resources/intune-devices-devicemanagementscriptuserstate.md)オブジェクトのプロパティと関係を一覧表示します。|
|[DeviceManagementScriptUserState を取得します。](../api/intune-devices-devicemanagementscriptuserstate-get.md)|[deviceManagementScriptUserState](../resources/intune-devices-devicemanagementscriptuserstate.md)|[DeviceManagementScriptUserState](../resources/intune-devices-devicemanagementscriptuserstate.md)オブジェクトのプロパティと関係を参照してください。|
|[DeviceManagementScriptUserState を作成します。](../api/intune-devices-devicemanagementscriptuserstate-create.md)|[deviceManagementScriptUserState](../resources/intune-devices-devicemanagementscriptuserstate.md)|新しい[deviceManagementScriptUserState](../resources/intune-devices-devicemanagementscriptuserstate.md)オブジェクトを作成します。|
|[DeviceManagementScriptUserState を削除します。](../api/intune-devices-devicemanagementscriptuserstate-delete.md)|なし|の[deviceManagementScriptUserState](../resources/intune-devices-devicemanagementscriptuserstate.md)を削除します。|
|[DeviceManagementScriptUserState を更新します。](../api/intune-devices-devicemanagementscriptuserstate-update.md)|[deviceManagementScriptUserState](../resources/intune-devices-devicemanagementscriptuserstate.md)|[DeviceManagementScriptUserState](../resources/intune-devices-devicemanagementscriptuserstate.md)オブジェクトのプロパティを更新します。|

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|id|String|デバイス管理スクリプト ユーザー状態のエンティティのキーです。|
|successDeviceCount|Int32|デバイスの数の特定のユーザーに成功します。|
|errorDeviceCount|Int32|特定のユーザー エラー デバイスの数。|
|userPrincipalName|String|特定のユーザーのユーザー プリンシパル名です。|

## <a name="relationships"></a>リレーションシップ
|リレーションシップ|型|説明|
|:---|:---|:---|
|deviceRunStates|[deviceManagementScriptDeviceState](../resources/intune-devices-devicemanagementscriptdevicestate.md)コレクション|特定のユーザーのすべてのデバイスでは、このスクリプトの実行状態のリストです。|

## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceManagementScriptUserState"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementScriptUserState",
  "id": "String (identifier)",
  "successDeviceCount": 1024,
  "errorDeviceCount": 1024,
  "userPrincipalName": "String"
}
```





