---
title: deviceProtectionOverview リソースの種類
description: 特定のデバイスのハードウェア情報です。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 902e3a6062d2aa50c96c27eb9d542905bf9a029d
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29418989"
---
# <a name="deviceprotectionoverview-resource-type"></a>deviceProtectionOverview リソースの種類

> **重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。 実稼働アプリケーションでこれらの API を使用することは、サポートされていません。

> **注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

特定のデバイスのハードウェア情報です。

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|totalReportedDeviceCount|Int32|デバイスの合計数です。|
|inactiveThreatAgentDeviceCount|Int32|使用頻度の低い脅威エージェントの数とデバイス|
|unknownStateThreatAgentDeviceCount|Int32|不明な数として脅威エージェントの状態を持つデバイス。|
|pendingSignatureUpdateDeviceCount|Int32|古い署名の数を持つデバイス。|
|cleanDeviceCount|Int32|デバイス数をクリーニングします。|
|pendingFullScanDeviceCount|Int32|全体を走査する保留中のデバイスの数。|
|pendingRestartDeviceCount|Int32|再起動の保留中のデバイスの数。|
|pendingManualStepsDeviceCount|Int32|手作業で保留中のデバイスの数。|
|pendingOfflineScanDeviceCount|Int32|オフライン保留中のデバイス数をスキャンします。|
|criticalFailuresDeviceCount|Int32|障害の重要なデバイスの数。|

## <a name="relationships"></a>リレーションシップ
なし

## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceProtectionOverview"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceProtectionOverview",
  "totalReportedDeviceCount": 1024,
  "inactiveThreatAgentDeviceCount": 1024,
  "unknownStateThreatAgentDeviceCount": 1024,
  "pendingSignatureUpdateDeviceCount": 1024,
  "cleanDeviceCount": 1024,
  "pendingFullScanDeviceCount": 1024,
  "pendingRestartDeviceCount": 1024,
  "pendingManualStepsDeviceCount": 1024,
  "pendingOfflineScanDeviceCount": 1024,
  "criticalFailuresDeviceCount": 1024
}
```




