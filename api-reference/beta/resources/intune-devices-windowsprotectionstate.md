---
title: windowsprotectionstate リソースの種類
description: デバイス保護状態エンティティ。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 9ecdc3ab743502ff4aef78fa8923248399ce16f4
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/11/2019
ms.locfileid: "31803102"
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
|malwareProtectionEnabled|Boolean|マルウェア対策が有効になっているか、または使用できない|
|devicestate|[windowsdevicehealthstate](../resources/intune-devices-windowsdevicehealthstate.md)|コンピューターの状態 (クリーンスキャンまたは保留中の再起動など)。 可能な値は `clean`、`fullScanPending`、`rebootPending`、`manualStepsPending`、`offlineScanPending`、`critical` です。|
|realTimeProtectionEnabled|Boolean|リアルタイム保護が有効になっているかどうか。|
|networkInspectionSystemEnabled|Boolean|ネットワーク検査システムが有効になっているかどうか。|
|quickscanoverdue 超過|Boolean|クイックスキャンの期限が過ぎたかどうか。|
|fullscanoverdue|Boolean|完全スキャンの期限が過ぎたかどうか。|
|signatureupdateoverdue|Boolean|署名が古くなっているかどうか|
|rebootRequired|Boolean|再起動が必要かどうか|
|fullscanrequired|Boolean|フルスキャンが必要かどうか。|
|engineVersion|文字列|現在のエンドポイント保護エンジンのバージョン|
|signatureversion|文字列|現在のマルウェア定義バージョン|
|antiMalwareVersion|文字列|現在のマルウェア対策バージョン|
|lastquickscandatetime|DateTimeOffset|最後のクイックスキャンの日時|
|lastfullscandatetime|DateTimeOffset|最後のクイックスキャンの日時|
|lastquickscansignatureversion|文字列|最終クイックスキャン署名バージョン|
|lastfullscansignatureversion|文字列|前回のフルスキャン署名バージョン|
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





