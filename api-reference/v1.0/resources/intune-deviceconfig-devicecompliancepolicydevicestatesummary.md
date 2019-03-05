---
title: deviceCompliancePolicyDeviceStateSummary リソースの種類
description: まだ文書化されていません
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 1c434009d1f34014a36e6871963051773aa2aab5
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/26/2019
ms.locfileid: "30256876"
---
# <a name="devicecompliancepolicydevicestatesummary-resource-type"></a>deviceCompliancePolicyDeviceStateSummary リソースの種類

> **注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

まだ文書化されていません

## <a name="methods"></a>メソッド
|メソッド|戻り値の型|説明|
|:---|:---|:---|
|[deviceCompliancePolicyDeviceStateSummary の取得](../api/intune-deviceconfig-devicecompliancepolicydevicestatesummary-get.md)|[deviceCompliancePolicyDeviceStateSummary](../resources/intune-deviceconfig-devicecompliancepolicydevicestatesummary.md)|[deviceCompliancePolicyDeviceStateSummary](../resources/intune-deviceconfig-devicecompliancepolicydevicestatesummary.md) オブジェクトのプロパティとリレーションシップを読み取ります。|
|[deviceCompliancePolicyDeviceStateSummary の更新](../api/intune-deviceconfig-devicecompliancepolicydevicestatesummary-update.md)|[deviceCompliancePolicyDeviceStateSummary](../resources/intune-deviceconfig-devicecompliancepolicydevicestatesummary.md)|[deviceCompliancePolicyDeviceStateSummary](../resources/intune-deviceconfig-devicecompliancepolicydevicestatesummary.md) オブジェクトのプロパティを更新します。|

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|inGracePeriodCount|Int32|解約猶予期間内のデバイスの数|
|configManagerCount|Int32|System Center Configuration Manager によってコンプライアンスが管理されているデバイスの数|
|id|String|エンティティのキー。|
|unknownDeviceCount|Int32|不明なデバイスの数|
|notApplicableDeviceCount|Int32|該当しないデバイスの数|
|compliantDeviceCount|Int32|準拠デバイスの数|
|remediatedDeviceCount|Int32|修復済みデバイスの数|
|nonCompliantDeviceCount|Int32|準拠していないデバイスの数|
|errorDeviceCount|Int32|エラー デバイスの数|
|conflictDeviceCount|Int32|競合デバイスの数|

## <a name="relationships"></a>リレーションシップ
なし

## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceCompliancePolicyDeviceStateSummary"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceCompliancePolicyDeviceStateSummary",
  "inGracePeriodCount": 1024,
  "configManagerCount": 1024,
  "id": "String (identifier)",
  "unknownDeviceCount": 1024,
  "notApplicableDeviceCount": 1024,
  "compliantDeviceCount": 1024,
  "remediatedDeviceCount": 1024,
  "nonCompliantDeviceCount": 1024,
  "errorDeviceCount": 1024,
  "conflictDeviceCount": 1024
}
```



