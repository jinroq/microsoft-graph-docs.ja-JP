---
title: schedulingGroup リソースの種類
description: スケジュール内のメンバーの論理グループ (通常は役割による)。
author: nkramer
localization_priority: Priority
ms.prod: microsoft-teams
ms.openlocfilehash: 644a9492e47979241ccab3f0e69eb90407eb2647
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32562953"
---
# <a name="schedulinggroup-resource-type"></a>schedulingGroup リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[スケジュール](schedule.md)内のメンバーの論理グループ (通常は役割による)。 

## <a name="methods"></a>メソッド

| メソッド       | 戻り値の型  |Description|
|:---------------|:--------|:----------|
|[schedulingGroup を作成する](../api/schedule-post-schedulinggroups.md) | [schedulingGroup](schedulinggroup.md) | 新しい `schedulingGroup` を作成します。|
|[List schedulingGroups](../api/schedule-list-schedulinggroups.md) | [schedulingGroup](schedulinggroup.md) コレクション | スケジュール内の `schedulingGroups` のリストを取得します。|
|[Get schedulingGroup](../api/schedulinggroup-get.md) | [schedulingGroup](schedulinggroup.md) | ID で `schedulingGroup` を取得します。|
|[Replace schedulingGroup](../api/schedulinggroup-put.md) | [schedulingGroup](schedulinggroup.md) | `schedulingGroup` を置き換えます。|
|[Delete schedulingGroup](../api/schedulinggroup-delete.md) | なし | `schedulingGroup` を非アクティブとしてマークします。|

## <a name="properties"></a>プロパティ
|名前          |型           |説明                                                                                 |
|--------------|---------------|--------------------------------------------------------------------------------------------|
| id            | `string`      |`schedulingGroup` の ID。|
| displayName   | `string`      | `schedulingGroup` の表示名。 必須。 |
| isActive          |`bool`      | 新しくエンティティを作成する場合や、既存のエンティティを更新する場合に `schedulingGroup` を使用できるかどうかを示します。 必須。 |
| UserIds       | `collection(string)`    |  `schedulingGroup` のメンバーであるユーザー ID のリスト。 必須。 |
| createdDateTime       |`DateTimeOffset`        |この `schedulingGroup` が最初に作成されたときのタイムスタンプ。 Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表します。これは常に UTC 時間です。 たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、'2014-01-01T00:00:00Z'.のようになります。 |
| lastModifiedDateTime      |`DateTimeOffset`        |この `schedulingGroup` の最終更新日のタイムスタンプ。 Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表します。これは常に UTC 時間です。 たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、'2014-01-01T00:00:00Z'.のようになります。 |
| lastModifiedBy        |`microsoft.graph.identitySet`        |この `schedulingGroup` を最後に更新した ID。|

## <a name="json-representation"></a>JSON 表記

以下は、リソースの JSON 表記です。

<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.schedulingGroup"
}-->

```json
{
  "id": "TAG_f914d037-00a3-4ba4-b712-ef178cbea263",
  "createdDateTime": "2019-03-12T22:10:38.242Z",
  "lastModifiedDateTime": "2019-03-12T22:10:38.242Z",
  "displayName": "Cashiers",
  "isActive": true,
  "userIds": [
    "c5d0c76b-80c4-481c-be50-923cd8d680a1",
    "2a4296b3-a28a-44ba-bc66-0274b9b95851"
  ],
  "lastModifiedBy": {
    "application": null,
    "device": null,
    "conversation": null,
    "user": {
      "id": "366c0b19-49b1-41b5-a03f-9f3887bd0ed8",
      "displayName": "John Doe"
    }
  }
}
```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "schedulingGroup resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/schedulinggroup.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
