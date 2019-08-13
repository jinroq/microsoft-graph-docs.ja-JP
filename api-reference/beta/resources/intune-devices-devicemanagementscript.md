---
title: deviceManagementScript リソースの種類
description: Intune は、登録済みの windows 10 Azure Active Directory 参加済みデバイスで Powershell スクリプトを実行する機能をお客様に提供します。 このスクリプトは、一度または定期的に実行できます。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 930431372b012977216f5ae6e4f0884fc7ad1bb4
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36370068"
---
# <a name="devicemanagementscript-resource-type"></a>deviceManagementScript リソースの種類

> **重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

Intune は、登録済みの windows 10 Azure Active Directory 参加済みデバイスで Powershell スクリプトを実行する機能をお客様に提供します。 このスクリプトは、一度または定期的に実行できます。

## <a name="methods"></a>メソッド
|メソッド|戻り値の型|説明|
|:---|:---|:---|
|[DeviceManagementScripts を一覧表示する](../api/intune-devices-devicemanagementscript-list.md)|[Devicemanagementscript](../resources/intune-devices-devicemanagementscript.md)コレクション|[Devicemanagementscript](../resources/intune-devices-devicemanagementscript.md)オブジェクトのプロパティとリレーションシップをリストします。|
|[DeviceManagementScript の取得](../api/intune-devices-devicemanagementscript-get.md)|[deviceManagementScript](../resources/intune-devices-devicemanagementscript.md)|[Devicemanagementscript](../resources/intune-devices-devicemanagementscript.md)オブジェクトのプロパティとリレーションシップを読み取ります。|
|[DeviceManagementScript の作成](../api/intune-devices-devicemanagementscript-create.md)|[deviceManagementScript](../resources/intune-devices-devicemanagementscript.md)|新しい[Devicemanagementscript](../resources/intune-devices-devicemanagementscript.md)オブジェクトを作成します。|
|[DeviceManagementScript の削除](../api/intune-devices-devicemanagementscript-delete.md)|None|[Devicemanagementscript](../resources/intune-devices-devicemanagementscript.md)を削除します。|
|[DeviceManagementScript の更新](../api/intune-devices-devicemanagementscript-update.md)|[deviceManagementScript](../resources/intune-devices-devicemanagementscript.md)|[Devicemanagementscript](../resources/intune-devices-devicemanagementscript.md)オブジェクトのプロパティを更新します。|
|[assign アクション](../api/intune-devices-devicemanagementscript-assign.md)|なし|まだ文書化されていません|

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|id|文字列|デバイス管理スクリプトの一意識別子。|
|displayName|String|デバイス管理スクリプトの名前。|
|description|String|デバイス管理スクリプトの省略可能な説明です。|
|runSchedule|[runSchedule](../resources/intune-devices-runschedule.md)|スクリプトを実行する間隔を指定します。 定義されていない場合、スクリプトは1回だけ実行されます。|
|scriptContent|Binary|スクリプトの内容。|
|createdDateTime|DateTimeOffset|デバイス管理スクリプトが作成された日付と時刻。|
|lastModifiedDateTime|DateTimeOffset|デバイス管理スクリプトが最後に変更された日付と時刻。|
|runAsAccount|[runAsAccountType](../resources/intune-shared-runasaccounttype.md)|実行コンテキストの種類を示します。 可能な値は、`system`、`user` です。|
|enforceSignatureCheck|Boolean|スクリプト署名をチェックする必要があるかどうかを示します。|
|fileName|String|スクリプトファイル名。|
|roleScopeTagIds|文字列コレクション|この PowerShellScript インスタンスの範囲タグ Id のリスト。|
|runAs32Bit|Boolean|PowerShell スクリプトを32ビットとして実行する必要があるかどうかを示す値。|

## <a name="relationships"></a>リレーションシップ
|リレーションシップ|型|説明|
|:---|:---|:---|
|groupAssignments|[Devicemanagementscriptgroupassignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md)コレクション|デバイス管理スクリプトのグループ割り当てのリスト。|
|assignments|[deviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md)コレクション|デバイス管理スクリプトのグループ割り当てのリスト。|
|runSummary|[deviceManagementScriptRunSummary](../resources/intune-devices-devicemanagementscriptrunsummary.md)|デバイス管理スクリプトのサマリーを実行します。|
|deviceRunStates|[Devicemanagementscriptdevicestate](../resources/intune-devices-devicemanagementscriptdevicestate.md)コレクション|すべてのデバイスでこのスクリプトの実行状態のリスト。|
|userRunStates|[Devicemanagementscriptuserstate](../resources/intune-devices-devicemanagementscriptuserstate.md)コレクション|すべてのユーザーにわたるこのスクリプトの実行状態のリスト。|

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
  "fileName": "String",
  "roleScopeTagIds": [
    "String"
  ],
  "runAs32Bit": true
}
```



