---
title: スケジュールリソースの種類
description: チーム内の schedulingGroups、シフト、timeoffreasons 各理由と timesoff のコレクション。
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: de3662fcf3c5a8e50493e365f6a10a8641a451df
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32563143"
---
# <a name="schedule-resource-type"></a>スケジュールリソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[チーム](../resources/team.md)内の[schedulingGroup](schedulinggroup.md)オブジェクト、 [shift](shift.md)オブジェクト、 [timeoffreason](timeoffreason.md)オブジェクト、および[timeoff](timeoff.md)オブジェクトのコレクションです。 

## <a name="methods"></a>メソッド

| メソッド       | 戻り値の型  |説明|
|:---------------|:--------|:----------|
|[スケジュールを作成または置換する](../api/team-put-schedule.md) | [スケジューリング](schedule.md) | を`schedule`作成または置換します。|
|[スケジュールを取得する](../api/schedule-get.md) | [スケジューリング](schedule.md) | を`schedule`取得します。|
|[share](../api/schedule-share.md) | なし | スケジュールメンバー `schedule`で時間範囲を共有します。|

## <a name="properties"></a>プロパティ
|名前                   |型           |説明                                                                                                                                      |
|-----------------------|---------------|-------------------------------------------------------------------------------------------------------------------------------------------------|
| id                    |`string`  |`schedule` の ID。|
| enabled               |`bool`    | スケジュールがチームに対して有効になっているかどうかを示します。 必須です。|
| timeZone              |`string`  | tz データベース形式を使用して、スケジュールチームのタイムゾーンを示します。 必須です。|
| provisionStatus       |`enum`    | スケジュールの準備の状態。 |
| provisionStatusCode   |`string`  | スケジュールプロビジョニングが失敗した理由に関する追加情報。 |


## <a name="relationships"></a>関係
|名前                   |型           |説明                                                                                                                                      |
|-----------------------|---------------|-------------------------------------------------------------------------------------------------------------------------------------------------|
| 移す   |`collection(shift)`  | スケジュールのシフト。 |
| timesoff   |`collection(timeOff)`  | スケジュールでオフにされた回数のインスタンス。 |
| timeoffreasons   |`collection(timeOffReason)`  | スケジュールで時間切れがある理由のセット。 |
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
  "suppressions": [
    "Error: /api-reference/beta/resources/schedule.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
