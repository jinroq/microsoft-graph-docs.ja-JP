---
title: deviceProtectionOverview リソースの種類
description: 特定のデバイスのハードウェア情報。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: bcae979d81034155b715a634476b8dc4aa7a9c4a
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36369956"
---
# <a name="deviceprotectionoverview-resource-type"></a>deviceProtectionOverview リソースの種類

> **重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

特定のデバイスのハードウェア情報。

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|totalReportedDeviceCount|Int32|デバイスの合計数。|
|inactiveThreatAgentDeviceCount|Int32|脅威エージェント数が非アクティブなデバイス|
|unknownStateThreatAgentDeviceCount|Int32|不明な数の脅威エージェントの状態を持つデバイス。|
|pendingSignatureUpdateDeviceCount|Int32|署名数が古いデバイス。|
|cleanDeviceCount|Int32|デバイス数をクリーニングします。|
|pendingFullScanDeviceCount|Int32|保留中のフルスキャンデバイス数。|
|pendingRestartDeviceCount|Int32|保留中の再起動デバイス数。|
|pendingManualStepsDeviceCount|Int32|保留中の手動手順デバイス数。|
|pendingOfflineScanDeviceCount|Int32|保留中のオフラインスキャンデバイス数。|
|criticalFailuresDeviceCount|Int32|重大なエラーデバイス数。|

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



