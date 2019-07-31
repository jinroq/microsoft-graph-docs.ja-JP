---
title: shiftActivity リソースの種類
description: Shift でのアクティビティを表します。
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType_
ms.openlocfilehash: 8acfb16235c90cf6067ad5fd6c5d8e82ae239f8d
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35965076"
---
# <a name="shiftactivity-resource-type"></a>shiftActivity リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[Shift](shift.md)でのアクティビティを表します。

## <a name="properties"></a>プロパティ
| プロパティ                         | 型                    | 説明                                                                                                                                                                        |
|------------------------------|-------------------------|---------------------------------------------------------------------------------------------|
| isPaid               | `bool`                  | を使用し`microsoft.graph.user`ている間に、活動に対し`shift`てを支払う必要があるかどうかを示します。 必須です。    |
| startDateTime               | `DateTimeOffset`                  | の開始日時`shiftActivity`。 Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表します。これは常に UTC 時間です。 たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、'2014-01-01T00:00:00Z'.のようになります。 必須です。 |
| endDateTime               | `DateTimeOffset`                  | の終了日時`shiftActivity`。 Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表します。これは常に UTC 時間です。 たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、'2014-01-01T00:00:00Z'.のようになります。 必須です。    |
| code               | `string`                  | の顧客定義コード`shiftActivity`。 必須です。    |
| displayName               | `string`                  | の名前`shiftActivity`。 必須。    |

## <a name="json-representation"></a>JSON 表記

以下は、リソースの JSON 表記です。

<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.shiftActivity"
}-->
```json
{
  "isPaid": true,
  "startDateTime": "2019-03-11T15:00:00Z",
  "endDateTime": "2019-03-11T15:15:00Z",
  "code": "",
  "displayName": "Lunch"
}
```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "shiftActivity resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
