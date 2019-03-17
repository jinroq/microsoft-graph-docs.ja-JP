---
title: shift リソースの種類
description: shift は、スケジュールのスケジュールされた作業の単位です。
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: c392bfb4a1691ab99d852febdda27cdf1c3b8044
ms.sourcegitcommit: 081cacecb4960aabc9e1011d12f06fe9ecf7d188
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/16/2019
ms.locfileid: "30657897"
---
# <a name="shift-resource-type"></a>shift リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[スケジュール](schedule.md)に含まれるスケジュールされた作業の単位。 

## <a name="methods"></a>メソッド

| メソッド       | 戻り値の型  |説明|
|:---------------|:--------|:----------|
|[shift を作成する](../api/schedule-post-shifts.md) | [制](shift.md) | 新しい`shift`を作成します。|
|[シフトの一覧表示](../api/schedule-list-shifts.md) | [shift](shift.md)コレクション | このスケジュール内の`shifts`のリストを取得します。|
|[shift を取得する](../api/shift-get.md) | [制](shift.md) | ID `shift`で取得します。|
|[shift を置換する](../api/shift-put.md) | [制](shift.md) | を`shift`置き換えます。|
|[shift を削除する](../api/shift-delete.md) | なし | スケジュールから`shift`を削除します。|

## <a name="properties"></a>プロパティ
|名前          |型           |説明                                                                                                                                      |
|--------------|---------------|-------------------------------------------------------------------------------------------------------------------------------------------------|
| id            |`string`      |の ID `shift`。|
| userId            |`string`      |に割り当てられているユーザー `shift`の ID。 必須。 |
| schedulingGroupId         |`string`      |`shift`が含まれるスケジュールグループの ID。 必須。 |
| sharedshift   |`[shiftItem](shiftitem.md)`  |従業員とマネージャーの両方`shift`に表示される共有バージョン。 必須。 |
| draftShift        |`[shiftItem](shiftitem.md)`        |この`shift`の下書きバージョンは、マネージャーが表示できます。 必須。 |
| createdDateTime       |`DateTimeOffset`        |最初に作成さ`shift`れたタイムスタンプ。 Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表し、必ず UTC 時間です。 たとえば、2014年1月1日午前0時 (UTC) は次のようになります。 ' 2014-01-01t00:00: 00z ' のようになります。 |
| lastModifiedDateTime      |`DateTimeOffset`        |最後に更新され`shift`たタイムスタンプ。 Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表し、必ず UTC 時間です。 たとえば、2014年1月1日午前0時 (UTC) は次のようになります。 ' 2014-01-01t00:00: 00z ' のようになります。 |
| lastModifiedBy        |`microsoft.graph.identitySet`        |最後に更新`shift`した id。|

## <a name="json-representation"></a>JSON 表記

以下は、リソースの JSON 表記です。

<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.shift"
}-->

```json
{
  "id": "SHFT_577b75d2-a927-48c0-a5d1-dc984894e7b8",
  "createdDateTime": "2019-03-14T04:32:51.451Z",
  "lastModifiedDateTime": "2019-03-14T05:32:51.451Z",
  "userId": "c5d0c76b-80c4-481c-be50-923cd8d680a1",
  "schedulingGroupId": "TAG_228940ed-ff84-4e25-b129-1b395cf78be0",
  "lastModifiedBy": {
    "application": null,
    "device": null,
    "conversation": null,
    "user": {
      "id": "366c0b19-49b1-41b5-a03f-9f3887bd0ed8",
      "displayName": "John Doe"
    }
  },
  "sharedShift": {
    "displayName": "Day shift",
    "notes": "Please do inventory as part of your shift.",
    "startDateTime": "2019-03-11T15:00:00Z",
    "endDateTime": "2019-03-12T00:00:00Z",
    "theme": "blue",
    "activities": [
      {
        "isPaid": true,
        "startDateTime": "2019-03-11T15:00:00Z",
        "endDateTime": "2019-03-11T15:15:00Z",
        "code": "",
        "displayName": "Lunch"
      }
    ]
  },
  "draftShift": {
    "displayName": "Day shift",
    "notes": "Please do inventory as part of your shift.",
    "startDateTime": "2019-03-11T15:00:00Z",
    "endDateTime": "2019-03-12T00:00:00Z",
    "theme": "blue",
    "activities": [
      {
        "isPaid": true,
        "startDateTime": "2019-03-11T15:00:00Z",
        "endDateTime": "2019-03-11T15:30:00Z",
        "code": "",
        "displayName": "Lunch"
      }
    ]
  }
}
```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "shift resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/shift.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
