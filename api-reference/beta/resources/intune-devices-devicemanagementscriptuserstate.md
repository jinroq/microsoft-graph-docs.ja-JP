---
title: deviceManagementScriptUserState リソースの種類
description: デバイス管理スクリプトのユーザー実行状態のプロパティが含まれています。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: ce2d0971e953199cb8f79ca0963d3f2e53843f91
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36369998"
---
# <a name="devicemanagementscriptuserstate-resource-type"></a>deviceManagementScriptUserState リソースの種類

> **重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

デバイス管理スクリプトのユーザー実行状態のプロパティが含まれています。

## <a name="methods"></a>メソッド
|メソッド|戻り値の型|説明|
|:---|:---|:---|
|[DeviceManagementScriptUserStates のリスト](../api/intune-devices-devicemanagementscriptuserstate-list.md)|[Devicemanagementscriptuserstate](../resources/intune-devices-devicemanagementscriptuserstate.md)コレクション|[Devicemanagementscriptuserstate](../resources/intune-devices-devicemanagementscriptuserstate.md)オブジェクトのプロパティとリレーションシップをリストします。|
|[DeviceManagementScriptUserState の取得](../api/intune-devices-devicemanagementscriptuserstate-get.md)|[deviceManagementScriptUserState](../resources/intune-devices-devicemanagementscriptuserstate.md)|[Devicemanagementscriptuserstate](../resources/intune-devices-devicemanagementscriptuserstate.md)オブジェクトのプロパティとリレーションシップを読み取ります。|
|[DeviceManagementScriptUserState の作成](../api/intune-devices-devicemanagementscriptuserstate-create.md)|[deviceManagementScriptUserState](../resources/intune-devices-devicemanagementscriptuserstate.md)|新しい[Devicemanagementscriptuserstate](../resources/intune-devices-devicemanagementscriptuserstate.md)オブジェクトを作成します。|
|[DeviceManagementScriptUserState の削除](../api/intune-devices-devicemanagementscriptuserstate-delete.md)|None|[Devicemanagementscriptuserstate](../resources/intune-devices-devicemanagementscriptuserstate.md)を削除します。|
|[DeviceManagementScriptUserState の更新](../api/intune-devices-devicemanagementscriptuserstate-update.md)|[deviceManagementScriptUserState](../resources/intune-devices-devicemanagementscriptuserstate.md)|[Devicemanagementscriptuserstate](../resources/intune-devices-devicemanagementscriptuserstate.md)オブジェクトのプロパティを更新します。|

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|id|文字列|デバイス管理スクリプトのユーザー状態エンティティのキー。|
|successDeviceCount|Int32|特定のユーザーの成功デバイス数。|
|errorDeviceCount|Int32|特定のユーザーのエラーデバイス数。|
|userPrincipalName|String|特定のユーザーのユーザープリンシパル名。|

## <a name="relationships"></a>リレーションシップ
|リレーションシップ|型|説明|
|:---|:---|:---|
|deviceRunStates|[Devicemanagementscriptdevicestate](../resources/intune-devices-devicemanagementscriptdevicestate.md)コレクション|特定のユーザーのすべてのデバイスでこのスクリプトの実行状態を一覧表示します。|

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



