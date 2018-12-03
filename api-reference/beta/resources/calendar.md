---
title: calendar リソース型
description: イベントのコンテナーである予定表です。 ユーザーの予定表、または Office 365 グループの既定の予定表のいずれかを指定できます。
ms.openlocfilehash: 90be98acace678b45626f812150362dfeed1f52d
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27074234"
---
# <a name="calendar-resource-type"></a>calendar リソース型

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

イベントのコンテナーである予定表です。 [ユーザー](user.md)の予定表、または Office 365 [グループ](group.md)の既定の予定表のいずれかを指定できます。

> **注:** ユーザーの予定表、グループ予定表と対話できるように、いくつかの小さな違いがあります。

 - の[calendarGroup](calendargroup.md)のユーザーの予定表のみを整理することができます。
 - Outlook は、グループのためのすべての会議出席依頼を自動的に受け入れます。 ユーザーの予定表のみの[承諾](../api/event-accept.md)、[仮承諾](../api/event-tentativelyaccept.md)、または会議出席依頼を[辞退する](../api/event-decline.md)ことをがします。
  - Outlook は、グループのイベントのアラームをサポートしていません。 [再通知](../api/event-snoozereminder.md)や[アラーム](reminder.md)を[消す](../api/event-dismissreminder.md)をユーザーの予定表のみにできます。

## <a name="methods"></a>メソッド

| メソッド       | 戻り値の型  |説明|
|:---------------|:--------|:----------|
|[予定表を一覧表示する](../api/user-list-calendars.md)|[calendar](calendar.md) collection|ユーザーのすべての予定表を取得するか、既定またはその他の特定の予定表グループの予定表を取得します。|
|[予定表を作成する](../api/user-post-calendars.md) |[calendar](calendar.md)| 既定の予定表グループまたはユーザーの特定の予定表グループに予定表を作成します。|
|[予定表を取得する](../api/calendar-get.md) | [calendar](calendar.md) |**予定表**オブジェクトのプロパティと関係を取得します。 ユーザーの予定表、または Office 365 のグループの既定の予定表のいずれかを指定できます。 |
|[更新する](../api/calendar-update.md) | [calendar](calendar.md)  |**予定表**オブジェクトのプロパティを更新します。 ユーザーの予定表、または Office 365 のグループの既定の予定表のいずれかを指定できます。 |
|[削除する](../api/calendar-delete.md) | なし |予定表オブジェクトを削除します。 |
|[calendarView を一覧表示する](../api/calendar-list-calendarview.md) |[event](event.md) コレクション| ユーザーの標準として設定されている予定表 `(../me/calendarview)` または特定の予定表から、時間範囲で定義したカレンダー ビューのイベントの発生、例外、および単一インスタンスを取得します。|
|[イベントを一覧表示する](../api/calendar-list-events.md) |[event](event.md) コレクション| 予定表のイベント一覧を取得します。一覧には、単一インスタンスの会議と定期的なマスターが含まれています。|
|[イベントを作成する](../api/calendar-post-events.md) |[event](event.md)| 既定または指定した予定表で新しいイベントを作成します。|
|[findMeetingTimes](../api/user-findmeetingtimes.md) |[meetingTimeSuggestionsResult](meetingtimesuggestionsresult.md) |会議の時間と開催者と出席者の可用性、および時間や場所の制約に基づいて場所をお勧めします。 |
|[getSchedule (プレビュー)](../api/calendar-getschedule.md) |[scheduleInformation](scheduleinformation.md)コレクション|コレクションの空き時間情報の可用性の情報をユーザー、配布リスト、または、リソースの指定された時間を取得します。 |
|[単一値の拡張プロパティを作成する](../api/singlevaluelegacyextendedproperty-post-singlevalueextendedproperties.md) |[calendar](calendar.md)  |新規または既存の予定表に、1 つ以上の単一値の拡張プロパティを作成します。   |
|[単一値の拡張プロパティを持つ予定表を取得する](../api/singlevaluelegacyextendedproperty-get.md)  | [calendar](calendar.md) | `$expand` または `$filter` を使用して、単一値の拡張プロパティを含む予定表を取得します。 |
|[複数値の拡張プロパティを作成する](../api/multivaluelegacyextendedproperty-post-multivalueextendedproperties.md) | [calendar](calendar.md) | 新規または既存の予定表に、1 つ以上の複数値の拡張プロパティを作成します。  |
|[複数値の拡張プロパティを持つ予定表を取得する](../api/multivaluelegacyextendedproperty-get.md)  | [calendar](calendar.md) | `$expand` を使用して、複数値の拡張プロパティを含む予定表を取得します。 |

## <a name="properties"></a>プロパティ
| プロパティ     | 型   |説明|
|:---------------|:--------|:----------|
|canEdit |ブール値 |ユーザーが予定表に書き込むことができる場合は true、それ以外の場合は false です。予定表を作成したユーザーの場合は、このプロパティは true です。予定表を共有していて、書き込みアクセスが付与されているユーザーの場合も、このプロパティは true です。 |
|canShare |ブール値 |ユーザーに予定表を共有するためのアクセス許可がある場合は true、それ以外の場合は false です。予定表を作成したユーザーのみがその予定表を共有できます。 |
|canViewPrivateItems |ブール値 |ユーザーがプライベートとしてマークされている予定表アイテムを読み取れることができる場合は true、それ以外の場合は false です。 |
|changeKey|String|予定表オブジェクトのバージョンを識別します。予定表を変更するたびに changeKey も変更されます。これにより、Exchange は正しいバージョンのオブジェクトに変更を適用できます。読み取り専用。|
|color|String|UI で予定表を他の予定表から区別するための配色テーマを指定します。プロパティ値は次のとおりです。薄い青=0、薄い緑=1、薄いオレンジ=2、薄い灰色=3、薄い黄=4、薄い青緑=5、薄いピンク=6、薄い茶色=7、薄い赤=8、最大色=9、自動=-1|
|hexColor|String|カレンダーを表す色。 色は、6 桁、3 バイトの 16 進数で表されます。 各バイトは、FF を 16 進数で 00 の範囲で、色の赤、緑、および青のコンポーネントの 1 つを表します。 |
|id|String|グループの一意識別子。読み取り専用です。|
|isDefaultCalendar|Boolean|この予定表がユーザーの既定の予定表であれば True、そうでなければ False。|
|IsShared |Boolean |True を設定すると、ユーザーがカレンダーを共有、他のユーザーでは、false それ以外の場合。 予定表を作成したユーザーのみが共有できるため、 **isShared**と**isSharedWithMe**が同じユーザーの場合はできません。 |
|isSharedWithMe |Boolean |ユーザーが予定表を共有している場合は true、それ以外の場合は false です。予定表の所有者の場合は、このプロパティは常に false です。  |
|名前|String|予定表の名前。|
|owner |[emailAddress](emailaddress.md) | 設定すると、これは予定表を作成または追加したユーザーを表します。ユーザーが作成または追加した予定表の場合、**owner** プロパティがユーザーに設定されます。ユーザーと共有されている予定表の場合は、**owner** プロパティがその予定表をユーザーと共有した人に設定されます。 |

## <a name="relationships"></a>関係
| リレーションシップ | 型   |説明|
|:---------------|:--------|:----------|
|calendarView|[event](event.md) コレクション|予定表のカレンダー ビュー。ナビゲーション プロパティ。読み取り専用。|
|events|[event](event.md) コレクション|予定表内のイベント。ナビゲーション プロパティ。読み取り専用。|
|multiValueExtendedProperties|[multiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md) collection| 予定表に定義された、複数値の拡張プロパティのコレクション。読み取り専用。Null 許容型。|
|singleValueExtendedProperties|[singleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md) collection| 予定表に定義された、単一値の拡張プロパティのコレクション。読み取り専用。Null 許容型。|

## <a name="json-representation"></a>JSON 表記

以下は、リソースの JSON 表記です

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "calendarView",
    "events",
    "multiValueExtendedProperties",
    "singleValueExtendedProperties"
  ],
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.calendar"
}-->

```json
{
  "canEdit": "boolean",
  "canShare": "boolean",
  "canViewPrivateItems": "boolean",
  "changeKey": "string",
  "color": "String",
  "hexColor": "String",
  "id": "string (identifier)",
  "isDefaultCalendar": "boolean",
  "isShared": "boolean",
  "isSharedWithMe": "boolean",
  "name": "string",
  "owner": {"@odata.type": "microsoft.graph.emailAddress"}
}

```
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "calendar resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
