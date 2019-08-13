---
title: deviceHealthScript リソースの種類
description: Intune は、登録済みの windows 10 Azure Active Directory 参加済みデバイスで Powershell スクリプトを実行する機能をお客様に提供します。 このスクリプトは、一度または定期的に実行できます。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 8ccde92a3d69cae27bc1a62926e733bc903c978e
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36376107"
---
# <a name="devicehealthscript-resource-type"></a>deviceHealthScript リソースの種類

> **重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

Intune は、登録済みの windows 10 Azure Active Directory 参加済みデバイスで Powershell スクリプトを実行する機能をお客様に提供します。 このスクリプトは、一度または定期的に実行できます。


[Devicemanagementscript](../resources/intune-devices-devicemanagementscript.md)から継承します

## <a name="methods"></a>メソッド
|メソッド|戻り値の型|説明|
|:---|:---|:---|
|[リスト deviceHealthScripts](../api/intune-devices-devicehealthscript-list.md)|[deviceHealthScript](../resources/intune-devices-devicehealthscript.md)コレクション|[DeviceHealthScript](../resources/intune-devices-devicehealthscript.md)オブジェクトのプロパティとリレーションシップをリストします。|
|[DeviceHealthScript を取得する](../api/intune-devices-devicehealthscript-get.md)|[deviceHealthScript](../resources/intune-devices-devicehealthscript.md)|[DeviceHealthScript](../resources/intune-devices-devicehealthscript.md)オブジェクトのプロパティとリレーションシップを読み取ります。|
|[DeviceHealthScript を作成する](../api/intune-devices-devicehealthscript-create.md)|[deviceHealthScript](../resources/intune-devices-devicehealthscript.md)|新しい[deviceHealthScript](../resources/intune-devices-devicehealthscript.md)オブジェクトを作成します。|
|[DeviceHealthScript の削除](../api/intune-devices-devicehealthscript-delete.md)|None|[DeviceHealthScript](../resources/intune-devices-devicehealthscript.md)を削除します。|
|[DeviceHealthScript の更新](../api/intune-devices-devicehealthscript-update.md)|[deviceHealthScript](../resources/intune-devices-devicehealthscript.md)|[DeviceHealthScript](../resources/intune-devices-devicehealthscript.md)オブジェクトのプロパティを更新します。|

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|id|文字列|デバイス管理スクリプトの一意識別子。 [Devicemanagementscript](../resources/intune-devices-devicemanagementscript.md)から継承します|
|displayName|String|デバイス管理スクリプトの名前。 [Devicemanagementscript](../resources/intune-devices-devicemanagementscript.md)から継承します|
|description|String|デバイス管理スクリプトの省略可能な説明です。 [Devicemanagementscript](../resources/intune-devices-devicemanagementscript.md)から継承します|
|runSchedule|[runSchedule](../resources/intune-devices-runschedule.md)|スクリプトを実行する間隔を指定します。 定義されていない場合、スクリプトは[Devicemanagementscript](../resources/intune-devices-devicemanagementscript.md)から継承された後に実行されます|
|scriptContent|Binary|スクリプトの内容。 [Devicemanagementscript](../resources/intune-devices-devicemanagementscript.md)から継承します|
|createdDateTime|DateTimeOffset|デバイス管理スクリプトが作成された日付と時刻。 [Devicemanagementscript](../resources/intune-devices-devicemanagementscript.md)から継承します|
|lastModifiedDateTime|DateTimeOffset|デバイス管理スクリプトが最後に変更された日付と時刻。 [Devicemanagementscript](../resources/intune-devices-devicemanagementscript.md)から継承します|
|runAsAccount|[runAsAccountType](../resources/intune-shared-runasaccounttype.md)|実行コンテキストの種類を示します。 [Devicemanagementscript](../resources/intune-devices-devicemanagementscript.md)から継承されます。 可能な値は、`system`、`user` です。|
|enforceSignatureCheck|Boolean|スクリプト署名をチェックする必要があるかどうかを示します。 [Devicemanagementscript](../resources/intune-devices-devicemanagementscript.md)から継承します|
|fileName|String|スクリプトファイル名。 [Devicemanagementscript](../resources/intune-devices-devicemanagementscript.md)から継承します|
|roleScopeTagIds|文字列コレクション|この PowerShellScript インスタンスの範囲タグ Id のリスト。 [Devicemanagementscript](../resources/intune-devices-devicemanagementscript.md)から継承します|
|runAs32Bit|Boolean|PowerShell スクリプトを[Devicemanagementscript](../resources/intune-devices-devicemanagementscript.md)から継承した32ビットとして実行する必要があるかどうかを示す値。|
|complianceRule|[deviceHealthScriptComplianceRule](../resources/intune-devices-devicehealthscriptcompliancerule.md)|まだ文書化されていません|
|remediationScriptContent|Binary|まだ文書化されていません|
|runRemediationScript|ブール型 (Boolean)|まだ文書化されていません|

## <a name="relationships"></a>リレーションシップ
|リレーションシップ|型|説明|
|:---|:---|:---|
|groupAssignments|[Devicemanagementscriptgroupassignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md)コレクション|デバイス管理スクリプトのグループ割り当てのリスト。 [Devicemanagementscript](../resources/intune-devices-devicemanagementscript.md)から継承します|
|assignments|[deviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md)コレクション|デバイス管理スクリプトのグループ割り当てのリスト。 [Devicemanagementscript](../resources/intune-devices-devicemanagementscript.md)から継承します|
|runSummary|[deviceManagementScriptRunSummary](../resources/intune-devices-devicemanagementscriptrunsummary.md)|デバイス管理スクリプトのサマリーを実行します。 [Devicemanagementscript](../resources/intune-devices-devicemanagementscript.md)から継承します|
|deviceRunStates|[Devicemanagementscriptdevicestate](../resources/intune-devices-devicemanagementscriptdevicestate.md)コレクション|すべてのデバイスでこのスクリプトの実行状態のリスト。 [Devicemanagementscript](../resources/intune-devices-devicemanagementscript.md)から継承します|
|userRunStates|[Devicemanagementscriptuserstate](../resources/intune-devices-devicemanagementscriptuserstate.md)コレクション|すべてのユーザーにわたるこのスクリプトの実行状態のリスト。 [Devicemanagementscript](../resources/intune-devices-devicemanagementscript.md)から継承します|

## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceHealthScript"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceHealthScript",
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
  "runAs32Bit": true,
  "complianceRule": {
    "@odata.type": "microsoft.graph.deviceHealthScriptComplianceRule",
    "detectionType": "String",
    "operator": "String",
    "detectionValue": "String"
  },
  "remediationScriptContent": "binary",
  "runRemediationScript": true
}
```



