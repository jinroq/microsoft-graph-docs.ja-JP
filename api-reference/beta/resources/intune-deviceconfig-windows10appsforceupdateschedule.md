---
title: windows10AppsForceUpdateSchedule リソースの種類
description: アプリケーションの Windows 10 強制更新のスケジュール
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 3e0bd9b0963f8547b03243aa7ef791a351dc2b08
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29418835"
---
# <a name="windows10appsforceupdateschedule-resource-type"></a>windows10AppsForceUpdateSchedule リソースの種類

> **重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。 実稼働アプリケーションでこれらの API を使用することは、サポートされていません。

> **注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

アプリケーションの Windows 10 強制更新のスケジュール

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|startDateTime|DateTimeOffset|力の開始時刻を再起動します。|
|recurrence|[windows10AppsUpdateRecurrence](../resources/intune-deviceconfig-windows10appsupdaterecurrence.md)|定期的なスケジュールです。 可能な値は、`none`、`daily`、`weekly`、`monthly` です。|
|runImmediatelyIfAfterStartDateTime|Boolean|True の場合、タスクはすぐに実行させるまでは、他の次の反復の実行の場合です。|

## <a name="relationships"></a>リレーションシップ
なし

## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windows10AppsForceUpdateSchedule"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windows10AppsForceUpdateSchedule",
  "startDateTime": "String (timestamp)",
  "recurrence": "String",
  "runImmediatelyIfAfterStartDateTime": true
}
```




