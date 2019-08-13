---
title: deviceManagementIntentDeviceStateSummary リソースの種類
description: 目的のデバイス状態の概要を表すエンティティ
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: d4dcbad68d83978d269108b2a9a1b18a246e0039
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36371419"
---
# <a name="devicemanagementintentdevicestatesummary-resource-type"></a>deviceManagementIntentDeviceStateSummary リソースの種類

> **重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

目的のデバイス状態の概要を表すエンティティ

## <a name="methods"></a>メソッド
|メソッド|戻り値の型|説明|
|:---|:---|:---|
|[DeviceManagementIntentDeviceStateSummary を取得する](../api/intune-deviceintent-devicemanagementintentdevicestatesummary-get.md)|[deviceManagementIntentDeviceStateSummary](../resources/intune-deviceintent-devicemanagementintentdevicestatesummary.md)|[DeviceManagementIntentDeviceStateSummary](../resources/intune-deviceintent-devicemanagementintentdevicestatesummary.md)オブジェクトのプロパティとリレーションシップを読み取ります。|
|[DeviceManagementIntentDeviceStateSummary の更新](../api/intune-deviceintent-devicemanagementintentdevicestatesummary-update.md)|[deviceManagementIntentDeviceStateSummary](../resources/intune-deviceintent-devicemanagementintentdevicestatesummary.md)|[DeviceManagementIntentDeviceStateSummary](../resources/intune-deviceintent-devicemanagementintentdevicestatesummary.md)オブジェクトのプロパティを更新します。|

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|id|String|ID|
|conflictCount|Int32|競合しているデバイスの数|
|errorCount|Int32|エラー デバイスの数|
|failedCount|Int32|失敗したデバイスの数|
|notApplicableCount|Int32|該当しないデバイスの数|
|notApplicablePlatformCount|Int32|プラットフォームとポリシーの不一致が原因で適用されていないデバイスの数|
|successCount|Int32|成功したデバイスの数|

## <a name="relationships"></a>リレーションシップ
なし

## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceManagementIntentDeviceStateSummary"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementIntentDeviceStateSummary",
  "id": "String (identifier)",
  "conflictCount": 1024,
  "errorCount": 1024,
  "failedCount": 1024,
  "notApplicableCount": 1024,
  "notApplicablePlatformCount": 1024,
  "successCount": 1024
}
```



