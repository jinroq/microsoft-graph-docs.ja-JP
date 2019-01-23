---
title: windowsUpdateState リソースの種類
description: まだ文書化されていません
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 20387d9e1fd9b84853a7bc097dfa08d128809358
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29430458"
---
# <a name="windowsupdatestate-resource-type"></a>windowsUpdateState リソースの種類

> **重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。 実稼働アプリケーションでこれらの API を使用することは、サポートされていません。

> **注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

まだ文書化されていません

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|id|String|これは、エンティティの Id です。|
|deviceId|String|デバイスの id です。|
|userId|String|ユーザーの id です。|
|deviceDisplayName|String|デバイスの表示名です。|
|userPrincipalName|String|ユーザー プリンシパル名です。|
|status|[windowsUpdateStatus](../resources/intune-deviceconfig-windowsupdatestatus.md)|Windows udpate の状態です。|
|qualityUpdateVersion|String|デバイスの品質の更新プログラムのバージョンです。|
|featureUpdateVersion|String|デバイスの現在の機能の更新バージョンです。|
|lastScanDateTime|DateTimeOffset|日付時刻を Windows Update エージェントは、スキャンが成功をしました。|
|lastSyncDateTime|DateTimeOffset|Microsoft Intune でデバイスが同期で最後の日に。|

## <a name="relationships"></a>リレーションシップ
なし

## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.WindowsUpdateState"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.WindowsUpdateState",
  "id": "String (identifier)",
  "deviceId": "String (identifier)",
  "userId": "String (identifier)",
  "deviceDisplayName": "String",
  "userPrincipalName": "String",
  "status": "String",
  "qualityUpdateVersion": "String",
  "featureUpdateVersion": "String",
  "lastScanDateTime": "String (timestamp)",
  "lastSyncDateTime": "String (timestamp)"
}
```


