---
title: deviceManagementIntentDeviceSettingStateSummary リソースの種類
description: 目的に対するデバイス設定状態の概要を表すエンティティ
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 20eb5e9ae2941d1762a7cad634c9e6f5b3f2c24e
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/11/2019
ms.locfileid: "33943425"
---
# <a name="devicemanagementintentdevicesettingstatesummary-resource-type"></a>deviceManagementIntentDeviceSettingStateSummary リソースの種類

> **重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

目的に対するデバイス設定状態の概要を表すエンティティ

## <a name="methods"></a>メソッド
|メソッド|戻り値の型|説明|
|:---|:---|:---|
|[リスト deviceManagementIntentDeviceSettingStateSummaries](../api/intune-deviceintent-devicemanagementintentdevicesettingstatesummary-list.md)|[deviceManagementIntentDeviceSettingStateSummary](../resources/intune-deviceintent-devicemanagementintentdevicesettingstatesummary.md)コレクション|[DeviceManagementIntentDeviceSettingStateSummary](../resources/intune-deviceintent-devicemanagementintentdevicesettingstatesummary.md)オブジェクトのプロパティとリレーションシップをリストします。|
|[DeviceManagementIntentDeviceSettingStateSummary を取得する](../api/intune-deviceintent-devicemanagementintentdevicesettingstatesummary-get.md)|[deviceManagementIntentDeviceSettingStateSummary](../resources/intune-deviceintent-devicemanagementintentdevicesettingstatesummary.md)|[DeviceManagementIntentDeviceSettingStateSummary](../resources/intune-deviceintent-devicemanagementintentdevicesettingstatesummary.md)オブジェクトのプロパティとリレーションシップを読み取ります。|
|[DeviceManagementIntentDeviceSettingStateSummary を作成する](../api/intune-deviceintent-devicemanagementintentdevicesettingstatesummary-create.md)|[deviceManagementIntentDeviceSettingStateSummary](../resources/intune-deviceintent-devicemanagementintentdevicesettingstatesummary.md)|新しい[deviceManagementIntentDeviceSettingStateSummary](../resources/intune-deviceintent-devicemanagementintentdevicesettingstatesummary.md)オブジェクトを作成します。|
|[DeviceManagementIntentDeviceSettingStateSummary の削除](../api/intune-deviceintent-devicemanagementintentdevicesettingstatesummary-delete.md)|None|[DeviceManagementIntentDeviceSettingStateSummary](../resources/intune-deviceintent-devicemanagementintentdevicesettingstatesummary.md)を削除します。|
|[DeviceManagementIntentDeviceSettingStateSummary の更新](../api/intune-deviceintent-devicemanagementintentdevicesettingstatesummary-update.md)|[deviceManagementIntentDeviceSettingStateSummary](../resources/intune-deviceintent-devicemanagementintentdevicesettingstatesummary.md)|[DeviceManagementIntentDeviceSettingStateSummary](../resources/intune-deviceintent-devicemanagementintentdevicesettingstatesummary.md)オブジェクトのプロパティを更新します。|

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|id|String|ID|
|settingName|String|設定の名前|
|compliantCount|Int32|準拠デバイスの数|
|conflictCount|Int32|競合しているデバイスの数|
|errorCount|Int32|エラー デバイスの数|
|nonCompliantCount|Int32|準拠していないデバイスの数|
|notApplicableCount|Int32|該当しないデバイスの数|
|remediatedCount|Int32|修復済みデバイスの数|

## <a name="relationships"></a>関係
なし

## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceManagementIntentDeviceSettingStateSummary"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementIntentDeviceSettingStateSummary",
  "id": "String (identifier)",
  "settingName": "String",
  "compliantCount": 1024,
  "conflictCount": 1024,
  "errorCount": 1024,
  "nonCompliantCount": 1024,
  "notApplicableCount": 1024,
  "remediatedCount": 1024
}
```




