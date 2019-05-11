---
title: deviceManagementIntent リソースの種類
description: デバイスに設定を適用する目的を表すエンティティ
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 976a13bb8ac542e67ebdd0422669cd866cc70af6
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/11/2019
ms.locfileid: "33943446"
---
# <a name="devicemanagementintent-resource-type"></a>deviceManagementIntent リソースの種類

> **重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

デバイスに設定を適用する目的を表すエンティティ

## <a name="methods"></a>メソッド
|メソッド|戻り値の型|説明|
|:---|:---|:---|
|[DeviceManagementIntents を一覧表示する](../api/intune-deviceintent-devicemanagementintent-list.md)|[Devicemanagementintent](../resources/intune-deviceintent-devicemanagementintent.md)コレクション|[Devicemanagementintent](../resources/intune-deviceintent-devicemanagementintent.md)オブジェクトのプロパティとリレーションシップをリストします。|
|[DeviceManagementIntent の取得](../api/intune-deviceintent-devicemanagementintent-get.md)|[deviceManagementIntent](../resources/intune-deviceintent-devicemanagementintent.md)|[Devicemanagementintent](../resources/intune-deviceintent-devicemanagementintent.md)オブジェクトのプロパティとリレーションシップを読み取ります。|
|[DeviceManagementIntent の作成](../api/intune-deviceintent-devicemanagementintent-create.md)|[deviceManagementIntent](../resources/intune-deviceintent-devicemanagementintent.md)|新しい[Devicemanagementintent](../resources/intune-deviceintent-devicemanagementintent.md)オブジェクトを作成します。|
|[DeviceManagementIntent の削除](../api/intune-deviceintent-devicemanagementintent-delete.md)|None|[Devicemanagementintent](../resources/intune-deviceintent-devicemanagementintent.md)を削除します。|
|[DeviceManagementIntent の更新](../api/intune-deviceintent-devicemanagementintent-update.md)|[deviceManagementIntent](../resources/intune-deviceintent-devicemanagementintent.md)|[Devicemanagementintent](../resources/intune-deviceintent-devicemanagementintent.md)オブジェクトのプロパティを更新します。|
|[updateSettings アクション](../api/intune-deviceintent-devicemanagementintent-updatesettings.md)|なし|まだ文書化されていません|
|[migrateToTemplate アクション](../api/intune-deviceintent-devicemanagementintent-migratetotemplate.md)|なし|まだ文書化されていません|
|[assign アクション](../api/intune-deviceintent-devicemanagementintent-assign.md)|なし|まだ文書化されていません|

## <a name="properties"></a>プロパティ
|プロパティ|種類|説明|
|:---|:---|:---|
|id|文字列|インテント ID|
|displayName|String|ユーザーが指定した表示名|
|description|String|ユーザーが指定した説明|
|isAssigned|Boolean|目的がユーザーに割り当てられているかどうかを表します。|
|lastModifiedDateTime|DateTimeOffset|目的が最後に変更された日時|
|templateId|String|この目的が作成されたテンプレートの ID (存在する場合)|

## <a name="relationships"></a>関係
|リレーションシップ|型|説明|
|:---|:---|:---|
|settings|[Devicemanagementsettinginstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)コレクション|適用されるすべての設定のコレクション|
|categories|[Devicemanagementintentsettingcategory](../resources/intune-deviceintent-devicemanagementintentsettingcategory.md)コレクション|目的内のカテゴリ設定のコレクション|
|assignments|[Devicemanagementintentassignment](../resources/intune-deviceintent-devicemanagementintentassignment.md)コレクション|割り当てのコレクション|
|deviceSettingStateSummaries|[deviceManagementIntentDeviceSettingStateSummary](../resources/intune-deviceintent-devicemanagementintentdevicesettingstatesummary.md)コレクション|目的内のすべての設定について、対応する状態に属するデバイスの設定とその状態、およびそれらの状態のコレクション。|
|deviceStates|[Devicemanagementintentdevicestate](../resources/intune-deviceintent-devicemanagementintentdevicestate.md)コレクション|目的が適用されているすべてのデバイスの状態のコレクション|
|userStates|[Devicemanagementintentuserstate](../resources/intune-deviceintent-devicemanagementintentuserstate.md)コレクション|目的が適用されているすべてのユーザーの状態のコレクション|
|deviceStateSummary|[deviceManagementIntentDeviceStateSummary](../resources/intune-deviceintent-devicemanagementintentdevicestatesummary.md)|目的が適用されているすべてのデバイスについて、対応する状態に属するデバイスの状態と数の概要|
|userStateSummary|[deviceManagementIntentUserStateSummary](../resources/intune-deviceintent-devicemanagementintentuserstatesummary.md)|目的が適用されているすべてのユーザーについて、対応する状態に属するユーザーの状態と数の概要|

## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceManagementIntent"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementIntent",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String",
  "isAssigned": true,
  "lastModifiedDateTime": "String (timestamp)",
  "templateId": "String"
}
```




