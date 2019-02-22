---
title: windowsprotectionstate リソースの種類
description: デバイス保護状態エンティティ。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: eebf798a41e5cbab27fab849cdead8a288a782e2
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/21/2019
ms.locfileid: "30148315"
---
# <a name="windowsprotectionstate-resource-type"></a>windowsprotectionstate リソースの種類

> **重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

デバイス保護状態エンティティ。

## <a name="methods"></a>メソッド
|メソッド|戻り値の型|説明|
|:---|:---|:---|
|[windowsprotectionstate の取得](../api/intune-devices-windowsprotectionstate-get.md)|[windowsProtectionState](../resources/intune-devices-windowsprotectionstate.md)|[windowsprotectionstate](../resources/intune-devices-windowsprotectionstate.md)オブジェクトのプロパティとリレーションシップを読み取ります。|
|[windowsprotectionstate の更新](../api/intune-devices-windowsprotectionstate-update.md)|[windowsProtectionState](../resources/intune-devices-windowsprotectionstate.md)|[windowsprotectionstate](../resources/intune-devices-windowsprotectionstate.md)オブジェクトのプロパティを更新します。|

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|id|String|デバイス保護状態オブジェクトの一意の識別子。 これはデバイスのデバイス id です|
|malwareProtectionEnabled|ブール値|マルウェア対策が有効になっているか、または使用できない|
|devicestate|[windowsdevicehealthstate](../resources/intune-devices-windowsdevicehealthstate.md)|コンピューターの状態 (クリーンスキャンまたは保留中の再起動など)。 使用可能な値: `clean`、`fullScanPending`、`rebootPending`、`manualStepsPending`、`offlineScanPending`、`critical`。|
|realTimeProtectionEnabled|ブール値|リアルタイム保護が有効になっているかどうか。|
|networkInspectionSystemEnabled|ブール値|ネットワーク検査システムが有効になっているかどうか。|
|quickscanoverdue 超過|ブール値|クイックスキャンの期限が過ぎたかどうか。|
|fullscanoverdue|ブール値|完全スキャンの期限が過ぎたかどうか。|
|signatureupdateoverdue|ブール値|署名が古くなっているかどうか|
|rebootRequired|ブール値|再起動が必要かどうか|
|fullscanrequired|ブール値|フルスキャンが必要かどうか。|
|engineVersion|String|現在のエンドポイント保護エンジンのバージョン|
|signatureversion|String|現在のマルウェア定義バージョン|
|antiMalwareVersion|String|現在のマルウェア対策バージョン|
|lastquickscandatetime|DateTimeOffset|最後のクイックスキャンの日時|
|lastfullscandatetime|DateTimeOffset|最後のクイックスキャンの日時|
|lastquickscansignatureversion|String|最終クイックスキャン署名バージョン|
|lastfullscansignatureversion|String|前回のフルスキャン署名バージョン|
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




