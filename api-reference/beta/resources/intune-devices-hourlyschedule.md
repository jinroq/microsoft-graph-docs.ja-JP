---
title: hourlySchedule リソースの種類
description: 定期的なデバイスの管理スクリプトのスケジュールを 1 時間ごとに実行します。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 2f22cc44fdd9017ef6db6f014e4a9b756d46d034
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27811292"
---
# <a name="hourlyschedule-resource-type"></a>hourlySchedule リソースの種類

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

> **注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。

定期的なデバイスの管理スクリプトのスケジュールを 1 時間ごとに実行します。

[RunSchedule](../resources/intune-devices-runschedule.md)から継承します。

## <a name="properties"></a>プロパティ
|プロパティ|種類|説明|
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





