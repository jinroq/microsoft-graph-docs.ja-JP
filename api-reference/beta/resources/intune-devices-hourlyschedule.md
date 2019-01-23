---
title: hourlySchedule リソースの種類
description: 定期的なデバイスの管理スクリプトのスケジュールを 1 時間ごとに実行します。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: cf62c11da0932f5f10b6cc7a76ccecfd1e74ee92
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29396827"
---
# <a name="hourlyschedule-resource-type"></a>hourlySchedule リソースの種類

> **重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。 実稼働アプリケーションでこれらの API を使用することは、サポートされていません。

> **注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

定期的なデバイスの管理スクリプトのスケジュールを 1 時間ごとに実行します。


[RunSchedule](../resources/intune-devices-runschedule.md)から継承します。

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|interval|Int32|間隔 (時間数単位)|

## <a name="relationships"></a>リレーションシップ
なし

## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.hourlySchedule"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.hourlySchedule",
  "interval": 1024
}
```




