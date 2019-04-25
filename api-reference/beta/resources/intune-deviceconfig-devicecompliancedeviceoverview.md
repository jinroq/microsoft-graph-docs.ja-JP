---
title: deviceComplianceDeviceOverview リソースの種類
description: まだ文書化されていません
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: fe7216986a4a64c242dd041cd4325f321d0c5956
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32567390"
---
# <a name="devicecompliancedeviceoverview-resource-type"></a>deviceComplianceDeviceOverview リソースの種類

> **重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

まだ文書化されていません

## <a name="methods"></a>メソッド
|メソッド|戻り値の型|説明|
|:---|:---|:---|
|[Get deviceComplianceDeviceOverview](../api/intune-deviceconfig-devicecompliancedeviceoverview-get.md)|[deviceComplianceDeviceOverview](../resources/intune-deviceconfig-devicecompliancedeviceoverview.md)|[deviceComplianceDeviceOverview](../resources/intune-deviceconfig-devicecompliancedeviceoverview.md) オブジェクトのプロパティとリレーションシップを読み取ります。|
|[Update deviceComplianceDeviceOverview](../api/intune-deviceconfig-devicecompliancedeviceoverview-update.md)|[deviceComplianceDeviceOverview](../resources/intune-deviceconfig-devicecompliancedeviceoverview.md)|[deviceComplianceDeviceOverview](../resources/intune-deviceconfig-devicecompliancedeviceoverview.md) オブジェクトのプロパティを更新します。|

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|id|String|エンティティのキー。|
|pendingCount|Int32|保留中のデバイスの数|
|notApplicableCount|Int32|該当しないデバイスの数|
|notApplicablePlatformCount|Int32|プラットフォームとポリシーの不一致が原因で適用されていないデバイスの数|
|successCount|Int32|成功したデバイスの数|
|errorCount|Int32|エラー デバイスの数|
|failedCount|Int32|失敗したデバイスの数|
|conflictCount|Int32|競合しているデバイスの数|
|lastUpdateDateTime|DateTimeOffset|最終更新時刻|
|configurationVersion|Int32|対象の概要に関するポリシーのバージョン|

## <a name="relationships"></a>関係
なし

## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceComplianceDeviceOverview"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceComplianceDeviceOverview",
  "id": "String (identifier)",
  "pendingCount": 1024,
  "notApplicableCount": 1024,
  "notApplicablePlatformCount": 1024,
  "successCount": 1024,
  "errorCount": 1024,
  "failedCount": 1024,
  "conflictCount": 1024,
  "lastUpdateDateTime": "String (timestamp)",
  "configurationVersion": 1024
}
```





