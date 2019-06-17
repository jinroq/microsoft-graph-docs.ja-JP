---
title: 時間のスケジュールリソースの種類
description: 定期的なデバイス管理スクリプトの時間単位の実行スケジュール。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: aadd9f6e53288087cea5ee75a5f7cab2b2decbde
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/14/2019
ms.locfileid: "34995169"
---
# <a name="hourlyschedule-resource-type"></a>時間のスケジュールリソースの種類

> **重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

定期的なデバイス管理スクリプトの時間単位の実行スケジュール。


[Runschedule](../resources/intune-devices-runschedule.md)から継承します

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|interval|Int32|間隔 (時間単位)|

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





