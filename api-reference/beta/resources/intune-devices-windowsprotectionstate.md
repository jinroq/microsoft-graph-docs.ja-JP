---
title: windowsProtectionState リソースの種類
description: デバイス保護状態エンティティ。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 793cd54995fdac06f53e78c0ffdd4d16dd1c51d4
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35999333"
---
# <a name="windowsprotectionstate-resource-type"></a>windowsProtectionState リソースの種類

> **重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

デバイス保護状態エンティティ。

## <a name="methods"></a>メソッド
|メソッド|戻り値の型|説明|
|:---|:---|:---|
|[WindowsProtectionState の取得](../api/intune-devices-windowsprotectionstate-get.md)|[windowsProtectionState](../resources/intune-devices-windowsprotectionstate.md)|[Windowsprotectionstate](../resources/intune-devices-windowsprotectionstate.md)オブジェクトのプロパティとリレーションシップを読み取ります。|
|[WindowsProtectionState の更新](../api/intune-devices-windowsprotectionstate-update.md)|[windowsProtectionState](../resources/intune-devices-windowsprotectionstate.md)|[Windowsprotectionstate](../resources/intune-devices-windowsprotectionstate.md)オブジェクトのプロパティを更新します。|

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|id|String|デバイス保護状態オブジェクトの一意の識別子。 これはデバイスのデバイス id です|
|malwareProtectionEnabled|Boolean|マルウェア対策が有効になっているか、または使用できない|
|deviceState|[windowsDeviceHealthState](../resources/intune-devices-windowsdevicehealthstate.md)|コンピューターの状態 (クリーンスキャンまたは保留中の再起動など)。 使用可能な値: `clean`、`fullScanPending`、`rebootPending`、`manualStepsPending`、`offlineScanPending`、`critical`。|
|realTimeProtectionEnabled|Boolean|リアルタイム保護が有効になっているかどうか。|
|networkInspectionSystemEnabled|Boolean|ネットワーク検査システムが有効になっているかどうか。|
|quickScanOverdue 超過|Boolean|クイックスキャンの期限が過ぎたかどうか。|
|fullScanOverdue|Boolean|完全スキャンの期限が過ぎたかどうか。|
|signatureUpdateOverdue|Boolean|署名が古くなっているかどうか|
|rebootRequired|Boolean|再起動が必要かどうか|
|fullScanRequired|Boolean|フルスキャンが必要かどうか。|
|engineVersion|String|現在のエンドポイント保護エンジンのバージョン|
|signatureVersion|String|現在のマルウェア定義バージョン|
|antiMalwareVersion|String|現在のマルウェア対策バージョン|
|lastQuickScanDateTime|DateTimeOffset|最後のクイックスキャンの日時|
|lastFullScanDateTime|DateTimeOffset|最後のクイックスキャンの日時|
|lastQuickScanSignatureVersion|String|最終クイックスキャン署名バージョン|
|lastFullScanSignatureVersion|String|前回のフルスキャン署名バージョン|
|lastReportedDateTime|DateTimeOffset|前回のデバイス正常性の状態が報告された時刻|

## <a name="relationships"></a>リレーションシップ
|リレーションシップ|型|説明|
|:---|:---|:---|
|detectedMalwareState|[windowsDeviceMalwareState](../resources/intune-devices-windowsdevicemalwarestate.md)コレクション|デバイスマルウェアの一覧|

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





