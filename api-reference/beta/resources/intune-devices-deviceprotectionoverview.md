---
title: deviceProtectionOverview リソースの種類
description: 特定のデバイスのハードウェア情報です。
author: tfitzmac
ms.openlocfilehash: e705324bfc611117657ec629f8770e76c69be28d
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27317053"
---
# <a name="deviceprotectionoverview-resource-type"></a>deviceProtectionOverview リソースの種類

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

> **注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。

特定のデバイスのハードウェア情報です。
## <a name="properties"></a>Properties
|プロパティ|種類|説明|
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





