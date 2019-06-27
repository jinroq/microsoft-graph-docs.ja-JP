---
title: Microsoft Graph ツールキットの議題コンポーネント
description: この web コンポーネントは、ユーザーまたはグループの予定表のイベントを表すために使用されます。
localization_priority: Normal
author: nmetulev
ms.openlocfilehash: 8a91b20a48c1646fafd8cd7a287f037615024a73
ms.sourcegitcommit: 750c82f161a0f62bc2486995456ccd92ee5c7831
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/26/2019
ms.locfileid: "35243058"
---
# <a name="agenda-component-in-the-microsoft-graph-toolkit"></a>Microsoft Graph ツールキットの議題コンポーネント

`mgt-agenda` Web コンポーネントは、ユーザーまたはグループの予定表のイベントを表します。 既定では、現在の日付の現在サインインしているユーザーイベントが予定表に表示されます。 コンポーネントは、Microsoft Graph からイベントを返すエンドポイントを使用することもできます。 

## <a name="example"></a>例

[jsfiddle の例](https://jsfiddle.net/metulev/ojt2c7vp/)

```html
<mgt-agenda group-by-day></mgt-agenda>
```

![の計画-アジェンダ](./images/mgt-agenda.png)

## <a name="properties"></a>プロパティ

既定では、 `mgt-agenda`コンポーネントは`/me/calendarview`エンドポイントからイベントをフェッチし、現在の日付のイベントを表示します。 この動作を変更するには、いくつかのプロパティを使用できます。

| プロパティ | 属性 | 説明 |
| --- | --- | --- |
| `groupByDay` | `group-by-day` | 既定でイベントをグループ化するブール値はグループ化されません。 |
| `date` | `date` | Microsoft Graph から取り出すイベントの開始日を表す文字列型 (string) の値を指定します。 Value は、属性が設定されている場合`event-query`には、日付の[コンストラクター](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Date) -値で解析できる形式である必要があります。 |
| `days` | `days` | Microsoft Graph から取得する日数を指定します-既定値は3です。属性が`event-query`設定されている場合は効果がありません。 |
| `eventQuery` | `event-query` | Microsoft Graph からイベントを取得するときに使用する代替クエリを表す文字列。 必要に応じて、デリゲートスコープを ( `|` `"/groups/GROUP-ID-GUID/calendar/calendarView | group.read.all"`) で区切り、文字列の末尾に追加します。 |
| `events` | `events` | コンポーネントによってレンダリングされるイベントのリストを取得または設定するイベントの配列-このプロパティを使用して、コンポーネントによって読み込まれたイベントにアクセスします。 独自のイベントを読み込むには、この値を設定します。値が`date`開発`days`者に`event-query`よって設定されている場合、、、または属性は影響を与えません。 |

次の例では、コンポーネントの動作を変更して、特定の日付および最大3日間のデータをフェッチします。

```html
<mgt-agenda
  group-by-day
  date="May 7, 2019"
  days="3"
  ></mgt-agenda>
```

次の例では、コンポーネントの動作を変更して、特定のクエリからデータをフェッチします。

```html
<mgt-agenda
  event-query="/me/events?orderby=start/dateTime"
  ></mgt-agenda>
```

## <a name="css-custom-properties"></a>CSS カスタムプロパティ

コンポーネント`mgt-agenda`は、これらの CSS カスタムプロパティを定義します。

```css
mgt-agenda {
  --event-box-shadow: 0px 2px 8px rgba(0, 0, 0, 0.092);
  --event-margin: 0px 10px 14px 10px;
  --event-padding: 8px 0px;
  --event-background: #ffffff;
  --event-border: solid 2px rgba(0, 0, 0, 0);

  --agenda-header-margin: 40px 10px 14px 10px;
  --agenda-header-font-size: 24px;
  --agenda-header-color: #333333;

  --event-time-font-size: 12px;
  --event-time-color: #000000;

  --event-subject-font-size: 19px;
  --event-subject-color: #333333;

  --event-location-font-size: 12px;
  --event-location-color: #000000;
}
```

詳細については、「[スタイルコンポーネント](../style.md)」を参照してください。

## <a name="templates"></a>テンプレート

コンポーネント`mgt-agenda`は、コンポーネントの特定の部分を置き換えることができるいくつかの[テンプレート](../templates.md)をサポートしています。 テンプレートを指定するには、 `<template>`コンポーネントの内部に要素を含め、 `data-type`値を次のいずれかに設定します。

| データ型 | データコンテキスト | 説明 |
| --- | --- | --- |
| `default` | `events`: event オブジェクトのリスト | 既定のテンプレートでは、コンポーネント全体が独自のものに置き換えられます。 |
| `event` | `event`: event オブジェクト | 各イベントのレンダリングに使用するテンプレート。 |
| `header` | `header`: string | 各日のヘッダーのレンダリングに使用するテンプレート。 |
| `other` | `event`: event オブジェクト | 各イベントに対して追加のコンテンツをレンダリングするために使用するテンプレート。 |
| `no-data` | データコンテキストが渡されない | イベントが使用できないときに使用するテンプレート。 |
| `loading` | データコンテキストが渡されない | データの読み込み時に使用されるテンプレート。 |

次の例は、テンプレートの`event`使用方法を示しています。

```html
<mgt-agenda>
  <template data-type="event">
    <button class="eventButton">
      <div class="event-subject">{{ event.subject }}</div>
      <div data-for="attendee in event.attendees">
        <mgt-person
          person-query="{{ attendee.emailAddress.name }}"
          show-name
          show-email>
        </mgt-person>
      </div>
    </button>
  </template>
  <template data-type="no-data">
    There are no events found!
  </template>
</mgt-agenda>
```

詳細については、「 [templates](../templates.md)」を参照してください。

## <a name="graph-scopes"></a>グラフの範囲

このコンポーネントは、次の Microsoft Graph Api とアクセス許可を使用します。

| リソース | アクセス許可/スコープ |
| - | - |
| [/me/calendarview](https://docs.microsoft.com/en-us/graph/api/calendar-list-calendarview?view=graph-rest-1.0) | `Calendars.Read` |

このコンポーネントを使用すると、別の Microsoft Graph クエリを指定して`/groups/{id}/calendar/calendarView`呼び出すことができます (など)。 この場合は、文字列の末尾にスコープを追加します。`|`

## <a name="authentication"></a>認証

ログインコントロールは、[認証のドキュメント](./../providers.md)で説明されているグローバル認証プロバイダを活用します。 

