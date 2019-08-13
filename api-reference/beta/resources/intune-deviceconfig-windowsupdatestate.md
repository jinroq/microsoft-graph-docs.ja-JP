---
title: windowsUpdateState リソースの種類
description: まだ文書化されていません
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 47f2e2668634fed4d24d952d08b2b4a90f33c332
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36337679"
---
# <a name="windowsupdatestate-resource-type"></a>windowsUpdateState リソースの種類

> **重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

まだ文書化されていません

## <a name="methods"></a>メソッド
|メソッド|戻り値の型|説明|
|:---|:---|:---|
|[リスト windowsUpdateStates](../api/intune-deviceconfig-windowsupdatestate-list.md)|[windowsUpdateState](../resources/intune-deviceconfig-windowsupdatestate.md)コレクション|[WindowsUpdateState](../resources/intune-deviceconfig-windowsupdatestate.md)オブジェクトのプロパティとリレーションシップをリストします。|
|[WindowsUpdateState を取得する](../api/intune-deviceconfig-windowsupdatestate-get.md)|[windowsUpdateState](../resources/intune-deviceconfig-windowsupdatestate.md)|[WindowsUpdateState](../resources/intune-deviceconfig-windowsupdatestate.md)オブジェクトのプロパティとリレーションシップを読み取ります。|
|[WindowsUpdateState を作成する](../api/intune-deviceconfig-windowsupdatestate-create.md)|[windowsUpdateState](../resources/intune-deviceconfig-windowsupdatestate.md)|新しい[windowsUpdateState](../resources/intune-deviceconfig-windowsupdatestate.md)オブジェクトを作成します。|
|[WindowsUpdateState の削除](../api/intune-deviceconfig-windowsupdatestate-delete.md)|None|[WindowsUpdateState](../resources/intune-deviceconfig-windowsupdatestate.md)を削除します。|
|[WindowsUpdateState の更新](../api/intune-deviceconfig-windowsupdatestate-update.md)|[windowsUpdateState](../resources/intune-deviceconfig-windowsupdatestate.md)|[WindowsUpdateState](../resources/intune-deviceconfig-windowsupdatestate.md)オブジェクトのプロパティを更新します。|

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|id|文字列|これはエンティティの Id です。|
|deviceId|String|デバイスの id。|
|userId|String|ユーザーの id。|
|deviceDisplayName|String|デバイスの表示名。|
|userPrincipalName|String|ユーザープリンシパル名。|
|status|[windowsUpdateStatus](../resources/intune-deviceconfig-windowsupdatestatus.md)|Windows udpate 状態。 使用可能な値は、`upToDate`、`pendingInstallation`、`pendingReboot`、`failed` です。|
|qualityUpdateVersion|String|デバイスの品質更新プログラムのバージョン。|
|featureUpdateVersion|String|デバイスの現在の機能更新バージョン。|
|lastScanDateTime|DateTimeOffset|Windows Update エージェントがスキャンに成功した日時。|
|lastSyncDateTime|DateTimeOffset|デバイスと Microsoft Intune との同期が最後に実行された日時。|

## <a name="relationships"></a>リレーションシップ
なし

## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.windowsUpdateState"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsUpdateState",
  "id": "String (identifier)",
  "deviceId": "String",
  "userId": "String",
  "deviceDisplayName": "String",
  "userPrincipalName": "String",
  "status": "String",
  "qualityUpdateVersion": "String",
  "featureUpdateVersion": "String",
  "lastScanDateTime": "String (timestamp)",
  "lastSyncDateTime": "String (timestamp)"
}
```



