---
title: shift リソースの種類
description: Shift は、スケジュールのスケジュールされた作業の単位です。
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType_
ms.openlocfilehash: f76cd25a36ba070d9fa8281f31a1520a0d7b4435
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36008349"
---
# <a name="shift-resource-type"></a>shift リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[スケジュール](schedule.md)に含まれるスケジュールされた作業の単位。 

## <a name="methods"></a>メソッド

| メソッド       | 戻り値の型  |説明|
|:---------------|:--------|:----------|
|[Shift を作成する](../api/schedule-post-shifts.md) | [制](shift.md) | 新しい `shift` を作成します。|
|[シフトの一覧表示](../api/schedule-list-shifts.md) | [shift](shift.md)コレクション | このスケジュール内の`shifts`のリストを取得します。|
|[Shift を取得する](../api/shift-get.md) | [制](shift.md) | ID で `shift` を取得します。|
|[Shift を置換する](../api/shift-put.md) | [制](shift.md) | `shift` を置き換えます。|
|[Shift を削除する](../api/shift-delete.md) | None | スケジュールから`shift`を削除します。|

## <a name="properties"></a>プロパティ
|名前          |型           |説明                                                                                                                                      |
|--------------|---------------|-------------------------------------------------------------------------------------------------------------------------------------------------|
| id            |`string`      |`shift` の ID。|
| userId            |`string`      |に割り当てられているユーザー `shift`の ID。 必須です。 |
| schedulingGroupId         |`string`      |`shift`が含まれるスケジュールグループの ID。 必須です。 |
| sharedShift   |[佐々木](shiftitem.md)  |従業員とマネージャーの両方`shift`に表示される共有バージョン。 必須です。 |
| draftShift        |[佐々木](shiftitem.md)        |この`shift`の下書きバージョンは、マネージャーが表示できます。 必須。 |
| createdDateTime       |`DateTimeOffset`        |最初に作成さ`shift`れたタイムスタンプ。 Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表します。これは常に UTC 時間です。 たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、'2014-01-01T00:00:00Z'.のようになります。 |
| lastModifiedDateTime      |`DateTimeOffset`        |最後に更新され`shift`たタイムスタンプ。 Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表します。これは常に UTC 時間です。 たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、'2014-01-01T00:00:00Z'.のようになります。 |
| lastModifiedBy        | [identitySet](identityset.md)        |この `shift` を最後に更新した ID。|

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
  "lastModifiedBy": {"@odata.type":"microsoft.graph.identitySet"},
  "sharedShift": {"@odata.type":"microsoft.graph.shiftItem"},
  "draftShift": {"@odata.type":"microsoft.graph.shiftItem"}
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
  "suppressions": []
}
-->
