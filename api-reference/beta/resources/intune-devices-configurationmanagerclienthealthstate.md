---
title: configurationManagerClientHealthState リソースの種類
description: 構成マネージャー クライアントの正常性状態
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 55ba2b24df0d1d4c278f4785a310237c9c32cd9b
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29425828"
---
# <a name="configurationmanagerclienthealthstate-resource-type"></a>configurationManagerClientHealthState リソースの種類

> **重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。 実稼働アプリケーションでこれらの API を使用することは、サポートされていません。

> **注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

構成マネージャー クライアントの正常性状態

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|state|[configurationManagerClientState](../resources/intune-devices-configurationmanagerclientstate.md)|現在の構成マネージャー クライアントの状態です。 可能な値は、`unknown`、`installed`、`healthy`、`installFailed`、`updateFailed`、`communicationError` です。|
|errorCode|Int32|障害状態のエラー コード。|
|lastSyncDateTime|DateTimeOffset|Datetime/fo オプション最後の同期の構成マネージャーの管理をポイントします。|

## <a name="relationships"></a>リレーションシップ
なし

## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.configurationManagerClientHealthState"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.configurationManagerClientHealthState",
  "state": "String",
  "errorCode": 1024,
  "lastSyncDateTime": "String (timestamp)"
}
```




