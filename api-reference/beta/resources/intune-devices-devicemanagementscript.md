---
title: deviceManagementScript リソースの種類
description: Intune は、10 の登録されている windows Azure Active Directory が参加しているデバイスで、Powershell スクリプトを実行する機能を顧客に提供します。 スクリプトは、1 回だけまたは定期的に実行できます。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 0f2747b966384e5e0abaf165ca463174b60ced8b
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27932309"
---
# <a name="devicemanagementscript-resource-type"></a>deviceManagementScript リソースの種類

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

> **注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。

Intune は、10 の登録されている windows Azure Active Directory が参加しているデバイスで、Powershell スクリプトを実行する機能を顧客に提供します。 スクリプトは、1 回だけまたは定期的に実行できます。
## <a name="methods"></a>メソッド
|メソッド|戻り値の型|説明|
|:---|:---|:---|
|[リスト deviceManagementScripts](../api/intune-devices-devicemanagementscript-list.md)|[deviceManagementScript](../resources/intune-devices-devicemanagementscript.md)コレクション|[DeviceManagementScript](../resources/intune-devices-devicemanagementscript.md)オブジェクトのプロパティと関係を一覧表示します。|
|[DeviceManagementScript を取得します。](../api/intune-devices-devicemanagementscript-get.md)|[deviceManagementScript](../resources/intune-devices-devicemanagementscript.md)|[DeviceManagementScript](../resources/intune-devices-devicemanagementscript.md)オブジェクトのプロパティと関係を参照してください。|
|[DeviceManagementScript を作成します。](../api/intune-devices-devicemanagementscript-create.md)|[deviceManagementScript](../resources/intune-devices-devicemanagementscript.md)|新しい[deviceManagementScript](../resources/intune-devices-devicemanagementscript.md)オブジェクトを作成します。|
|[DeviceManagementScript を削除します。](../api/intune-devices-devicemanagementscript-delete.md)|なし|の[deviceManagementScript](../resources/intune-devices-devicemanagementscript.md)を削除します。|
|[DeviceManagementScript を更新します。](../api/intune-devices-devicemanagementscript-update.md)|[deviceManagementScript](../resources/intune-devices-devicemanagementscript.md)|[DeviceManagementScript](../resources/intune-devices-devicemanagementscript.md)オブジェクトのプロパティを更新します。|
|[assign action](../api/intune-devices-devicemanagementscript-assign.md)|なし|まだ文書化されていません|

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|ID|String|デバイス管理スクリプト用の一意の識別子。|
|displayName|String|デバイスの管理スクリプトの名前です。|
|説明|String|デバイスの管理スクリプトのオプションの説明です。|
|runSchedule|[runSchedule](../resources/intune-devices-runschedule.md)|スクリプトを実行する間隔です。 定義されていないスクリプトは実行 1 回|
|scriptContent|Binary|スクリプトの内容。|
|createdDateTime|DateTimeOffset|デバイス管理スクリプトが作成された日時です。|
|lastModifiedDateTime|DateTimeOffset|日付と時刻、デバイス管理のスクリプトが最後に修正されました。|
|runAsAccount|[runAsAccountType](../resources/intune-shared-runasaccounttype.md)|デバイス管理のスクリプトで実行される実行コンテキストの種類を示します。 使用可能な値は、`system`、`user` です。|
|enforceSignatureCheck|Boolean|スクリプト署名をチェックする必要があるかどうかを指定します。|
|fileName|String|スクリプト ファイルの名前です。|

## <a name="relationships"></a>リレーションシップ
|リレーションシップ|型|説明|
|:---|:---|:---|
|groupAssignments|[deviceManagementScriptGroupAssignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md)コレクション|一連のデバイスの管理スクリプトの割り当てをグループ化します。|
|assignments|[deviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md)コレクション|一連のデバイスの管理スクリプトの割り当てをグループ化します。|
|runSummary|[deviceManagementScriptRunSummary](../resources/intune-devices-devicemanagementscriptrunsummary.md)|概要デバイス管理のスクリプトを実行します。|
|deviceRunStates|[deviceManagementScriptDeviceState](../resources/intune-devices-devicemanagementscriptdevicestate.md)コレクション|すべてのデバイスでは、このスクリプトの実行状態のリストです。|
|userRunStates|[deviceManagementScriptUserState](../resources/intune-devices-devicemanagementscriptuserstate.md)コレクション|すべてのユーザーにこのスクリプトの実行状態のリストです。|

## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceManagementScript"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementScript",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String",
  "runSchedule": {
    "@odata.type": "microsoft.graph.runSchedule"
  },
  "scriptContent": "binary",
  "createdDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)",
  "runAsAccount": "String",
  "enforceSignatureCheck": true,
  "fileName": "String"
}
```





