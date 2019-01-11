---
title: windowsProtectionState リソースの種類
description: デバイス保護の状態のエンティティです。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 5a21cc27039f3119836e0027b2558cadadab1b5d
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27884106"
---
# <a name="windowsprotectionstate-resource-type"></a>windowsProtectionState リソースの種類

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

> **注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。

デバイス保護の状態のエンティティです。
## <a name="methods"></a>メソッド
|メソッド|戻り値の型|説明|
|:---|:---|:---|
|[WindowsProtectionState を取得します。](../api/intune-devices-windowsprotectionstate-get.md)|[windowsProtectionState](../resources/intune-devices-windowsprotectionstate.md)|[WindowsProtectionState](../resources/intune-devices-windowsprotectionstate.md)オブジェクトのプロパティと関係を参照してください。|
|[WindowsProtectionState を更新します。](../api/intune-devices-windowsprotectionstate-update.md)|[windowsProtectionState](../resources/intune-devices-windowsprotectionstate.md)|[WindowsProtectionState](../resources/intune-devices-windowsprotectionstate.md)オブジェクトのプロパティを更新します。|

## <a name="properties"></a>プロパティ
|プロパティ|種類|説明|
|:---|:---|:---|
|ID|String|デバイス保護の状態のオブジェクトの一意の識別子です。 これは、デバイスのデバイス id|
|malwareProtectionEnabled|ブール型|マルウェア対策が有効になっているか|
|deviceState|[windowsDeviceHealthState](../resources/intune-devices-windowsdevicehealthstate.md)|コンピューターの状態 (などのクリーンな保留中の完全なスキャンまたは再起動の保留中など)。 使用可能な値: `clean`、`fullScanPending`、`rebootPending`、`manualStepsPending`、`offlineScanPending`、`critical`。|
|realTimeProtectionEnabled|ブール型|リアルタイム保護を有効または無効ですか。|
|networkInspectionSystemEnabled|ブール型|ネットワーク検査システムが有効か無効か。|
|quickScanOverdue|ブール型|クイック スキャン、か期限切れですか。|
|fullScanOverdue|ブール型|完全なスキャンの期限切れかどうでしょうか。|
|signatureUpdateOverdue|ブール型|署名が期限切れかどうか。|
|rebootRequired|ブール型|しましたか。|
|fullScanRequired|ブール型|全体を走査するかが必要でしょうか。|
|engineVersion|String|現在のエンドポイントの保護エンジンのバージョン|
|signatureVersion|String|マルウェア定義の現在のバージョン|
|antiMalwareVersion|String|現在のバージョンのマルウェア対策|
|lastQuickScanDateTime|DateTimeOffset|最後のクイック スキャンの日時|
|lastFullScanDateTime|DateTimeOffset|最後のクイック スキャンの日時|
|lastQuickScanSignatureVersion|String|最後のクイック スキャンの署名バージョン|
|lastFullScanSignatureVersion|String|最後の完全なスキャンの署名バージョン|
|lastReportedDateTime|DateTimeOffset|最後のデバイスの状態が報告された時間|

## <a name="relationships"></a>リレーションシップ
|リレーションシップ|型|説明|
|:---|:---|:---|
|detectedMalwareState|[windowsDeviceMalwareState](../resources/intune-devices-windowsdevicemalwarestate.md)コレクション|マルウェアのデバイス ・ リスト|

## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.windowsProtectionState"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsProtectionState",
  "id": "String (identifier)",
  "malwareProtectionEnabled": true,
  "deviceState": "String",
  "realTimeProtectionEnabled": true,
  "networkInspectionSystemEnabled": true,
  "quickScanOverdue": true,
  "fullScanOverdue": true,
  "signatureUpdateOverdue": true,
  "rebootRequired": true,
  "fullScanRequired": true,
  "engineVersion": "String",
  "signatureVersion": "String",
  "antiMalwareVersion": "String",
  "lastQuickScanDateTime": "String (timestamp)",
  "lastFullScanDateTime": "String (timestamp)",
  "lastQuickScanSignatureVersion": "String",
  "lastFullScanSignatureVersion": "String",
  "lastReportedDateTime": "String (timestamp)"
}
```





