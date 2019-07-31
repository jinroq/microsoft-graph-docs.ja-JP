---
title: スケジュールリソースの種類
description: チーム内の schedulingGroups、シフト、timeOffReasons 各理由と timesOff のコレクション。
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType_
ms.openlocfilehash: a404c620b20cfcb69076ecc3bac25f907a12216c
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35965328"
---
# <a name="schedule-resource-type"></a>スケジュールリソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[チーム](../resources/team.md)内の[schedulingGroup](schedulinggroup.md)オブジェクト、 [Shift](shift.md)オブジェクト、 [Timeoffreason](timeoffreason.md)オブジェクト、および[timeoff](timeoff.md)オブジェクトのコレクションです。 

## <a name="methods"></a>メソッド

| メソッド       | 戻り値の型  |説明|
|:---------------|:--------|:----------|
|[スケジュールを作成または置換する](../api/team-put-schedule.md) | [schedule](schedule.md) | を`schedule`作成または置換します。|
|[スケジュールを取得する](../api/schedule-get.md) | [schedule](schedule.md) | を`schedule`取得します。|
|[share](../api/schedule-share.md) | None | スケジュールメンバー `schedule`で時間範囲を共有します。|

## <a name="properties"></a>プロパティ
|名前                   |型           |説明                                                                                                                                      |
|-----------------------|---------------|-------------------------------------------------------------------------------------------------------------------------------------------------|
| id                    |`string`  |`schedule` の ID。|
| enabled               |`bool`    | スケジュールがチームに対して有効になっているかどうかを示します。 必須です。|
| timeZone              |`string`  | Tz データベース形式を使用して、スケジュールチームのタイムゾーンを示します。 必須です。|
| provisionStatus       |`operationStatus`    | スケジュールの準備の状態。 使用可能な値`notStarted`は`running` `completed`、、 `failed`、です。 |
| provisionStatusCode   |`string`  | スケジュールプロビジョニングが失敗した理由に関する追加情報。 |


## <a name="relationships"></a>関係
|名前                   |型           |説明                                                                                                                                      |
|-----------------------|---------------|-------------------------------------------------------------------------------------------------------------------------------------------------|
| 移す   |`collection(shift)`  | スケジュールのシフト。 |
| timesOff   |`collection(timeOff)`  | スケジュールでオフにされた回数のインスタンス。 |
| timeOffReasons   |`collection(timeOffReason)`  | スケジュールで時間切れがある理由のセット。 |
| schedulingGroups   |`collection(schedulingGroup)`  | スケジュールに含まれるユーザーの論理グループ (通常は、役割別)。 |


## <a name="json-representation"></a>JSON 表記

以下は、リソースの JSON 表記です。

<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.schedule"
}-->

```json
{
  "id": "833fc4df-c88b-4398-992f-d8afcfe41df2",
  "enabled": true,
  "timeZone": "America/Chicago",
  "provisionStatus": "Completed",
  "provisionStatusCode": null
}
```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "schedule resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
