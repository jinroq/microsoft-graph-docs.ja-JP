---
title: devicemanagementscript リソースの種類
description: Intune は、登録済みの windows 10 Azure Active Directory 参加済みデバイスで Powershell スクリプトを実行する機能をお客様に提供します。 このスクリプトは、一度または定期的に実行できます。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 19e61bf994a21305b4cf081c593b8d46cbb7806f
ms.sourcegitcommit: f58ff560fa02ac95e296375c143b0922fb6a425c
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/19/2019
ms.locfileid: "30572419"
---
# <a name="devicemanagementscript-resource-type"></a>devicemanagementscript リソースの種類

> **重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

Intune は、登録済みの windows 10 Azure Active Directory 参加済みデバイスで Powershell スクリプトを実行する機能をお客様に提供します。 このスクリプトは、一度または定期的に実行できます。

## <a name="methods"></a>メソッド
|メソッド|戻り値の型|説明|
|:---|:---|:---|
|[devicemanagementscripts を一覧表示する](../api/intune-devices-devicemanagementscript-list.md)|[devicemanagementscript](../resources/intune-devices-devicemanagementscript.md)コレクション|[devicemanagementscript](../resources/intune-devices-devicemanagementscript.md)オブジェクトのプロパティとリレーションシップをリストします。|
|[devicemanagementscript の取得](../api/intune-devices-devicemanagementscript-get.md)|[deviceManagementScript](../resources/intune-devices-devicemanagementscript.md)|[devicemanagementscript](../resources/intune-devices-devicemanagementscript.md)オブジェクトのプロパティとリレーションシップを読み取ります。|
|[devicemanagementscript の作成](../api/intune-devices-devicemanagementscript-create.md)|[deviceManagementScript](../resources/intune-devices-devicemanagementscript.md)|新しい[devicemanagementscript](../resources/intune-devices-devicemanagementscript.md)オブジェクトを作成します。|
|[devicemanagementscript の削除](../api/intune-devices-devicemanagementscript-delete.md)|なし|[devicemanagementscript](../resources/intune-devices-devicemanagementscript.md)を削除します。|
|[devicemanagementscript の更新](../api/intune-devices-devicemanagementscript-update.md)|[deviceManagementScript](../resources/intune-devices-devicemanagementscript.md)|[devicemanagementscript](../resources/intune-devices-devicemanagementscript.md)オブジェクトのプロパティを更新します。|
|[assign アクション](../api/intune-devices-devicemanagementscript-assign.md)|なし|まだ文書化されていません|

## <a name="properties"></a>プロパティ
|プロパティ|種類|説明|
|:---|:---|:---|
|id|String|デバイス管理スクリプトの一意識別子。|
|displayName|String|デバイス管理スクリプトの名前。|
|description|String|デバイス管理スクリプトの省略可能な説明です。|
|runSchedule|[runSchedule](../resources/intune-devices-runschedule.md)|スクリプトを実行する間隔を指定します。 定義されていない場合、スクリプトは1回だけ実行されます。|
|scriptcontent|バイナリ|スクリプトの内容。|
|createdDateTime|DateTimeOffset|デバイス管理スクリプトが作成された日付と時刻。|
|lastModifiedDateTime|DateTimeOffset|デバイス管理スクリプトが最後に変更された日付と時刻。|
|runAsAccount|[runAsAccountType](../resources/intune-shared-runasaccounttype.md)|実行コンテキストの種類を示します。 可能な値は、`system`、`user` です。|
|enforceSignatureCheck|Boolean|スクリプト署名をチェックする必要があるかどうかを示します。|
|fileName|String|スクリプトファイル名。|
|roleScopeTagIds|String collection|この powershellscript インスタンスの範囲タグ id のリスト。|
|runAs32Bit|Boolean|PowerShell スクリプトを32ビットとして実行する必要があるかどうかを示す値。|

## <a name="relationships"></a>関係
|リレーションシップ|型|説明|
|:---|:---|:---|
|groupAssignments|[devicemanagementscriptgroupassignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md)コレクション|デバイス管理スクリプトのグループ割り当てのリスト。|
|assignments|[deviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md)コレクション|デバイス管理スクリプトのグループ割り当てのリスト。|
|runSummary|[deviceManagementScriptRunSummary](../resources/intune-devices-devicemanagementscriptrunsummary.md)|デバイス管理スクリプトのサマリーを実行します。|
|deviceRunStates|[devicemanagementscriptdevicestate](../resources/intune-devices-devicemanagementscriptdevicestate.md)コレクション|すべてのデバイスでこのスクリプトの実行状態のリスト。|
|userRunStates|[devicemanagementscriptuserstate](../resources/intune-devices-devicemanagementscriptuserstate.md)コレクション|すべてのユーザーにわたるこのスクリプトの実行状態のリスト。|

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




