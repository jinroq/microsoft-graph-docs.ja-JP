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
# <a name="agenda-component-in-the-microsoft-graph-toolkit"></a><span data-ttu-id="aea88-103">Microsoft Graph ツールキットの議題コンポーネント</span><span class="sxs-lookup"><span data-stu-id="aea88-103">Agenda component in the Microsoft Graph Toolkit</span></span>

<span data-ttu-id="aea88-104">`mgt-agenda` Web コンポーネントは、ユーザーまたはグループの予定表のイベントを表します。</span><span class="sxs-lookup"><span data-stu-id="aea88-104">The `mgt-agenda` web component represents events in a user or group calendar.</span></span> <span data-ttu-id="aea88-105">既定では、現在の日付の現在サインインしているユーザーイベントが予定表に表示されます。</span><span class="sxs-lookup"><span data-stu-id="aea88-105">By default, the calendar displays the current signed in user events for the current day.</span></span> <span data-ttu-id="aea88-106">コンポーネントは、Microsoft Graph からイベントを返すエンドポイントを使用することもできます。</span><span class="sxs-lookup"><span data-stu-id="aea88-106">The component can also use any endpoint that returns events from Microsoft Graph.</span></span> 

## <a name="example"></a><span data-ttu-id="aea88-107">例</span><span class="sxs-lookup"><span data-stu-id="aea88-107">Example</span></span>

[<span data-ttu-id="aea88-108">jsfiddle の例</span><span class="sxs-lookup"><span data-stu-id="aea88-108">jsfiddle example</span></span>](https://jsfiddle.net/metulev/ojt2c7vp/)

```html
<mgt-agenda group-by-day></mgt-agenda>
```

![の計画-アジェンダ](./images/mgt-agenda.png)

## <a name="properties"></a><span data-ttu-id="aea88-110">プロパティ</span><span class="sxs-lookup"><span data-stu-id="aea88-110">Properties</span></span>

<span data-ttu-id="aea88-111">既定では、 `mgt-agenda`コンポーネントは`/me/calendarview`エンドポイントからイベントをフェッチし、現在の日付のイベントを表示します。</span><span class="sxs-lookup"><span data-stu-id="aea88-111">By default, the `mgt-agenda` component fetches events from the `/me/calendarview` endpoint and displays events for the current day.</span></span> <span data-ttu-id="aea88-112">この動作を変更するには、いくつかのプロパティを使用できます。</span><span class="sxs-lookup"><span data-stu-id="aea88-112">There are several properties you can use to change this behavior.</span></span>

| <span data-ttu-id="aea88-113">プロパティ</span><span class="sxs-lookup"><span data-stu-id="aea88-113">Property</span></span> | <span data-ttu-id="aea88-114">属性</span><span class="sxs-lookup"><span data-stu-id="aea88-114">Attribute</span></span> | <span data-ttu-id="aea88-115">説明</span><span class="sxs-lookup"><span data-stu-id="aea88-115">Description</span></span> |
| --- | --- | --- |
| `groupByDay` | `group-by-day` | <span data-ttu-id="aea88-116">既定でイベントをグループ化するブール値はグループ化されません。</span><span class="sxs-lookup"><span data-stu-id="aea88-116">A Boolean value to group events by day - by default events are not grouped.</span></span> |
| `date` | `date` | <span data-ttu-id="aea88-117">Microsoft Graph から取り出すイベントの開始日を表す文字列型 (string) の値を指定します。</span><span class="sxs-lookup"><span data-stu-id="aea88-117">A string that represents the start date of the events to fetch from Microsoft Graph.</span></span> <span data-ttu-id="aea88-118">Value は、属性が設定されている場合`event-query`には、日付の[コンストラクター](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Date) -値で解析できる形式である必要があります。</span><span class="sxs-lookup"><span data-stu-id="aea88-118">Value should be in a format that can be parsed by the [Date constructor](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Date) - value has no effect if `event-query` attribute is set.</span></span> |
| `days` | `days` | <span data-ttu-id="aea88-119">Microsoft Graph から取得する日数を指定します-既定値は3です。属性が`event-query`設定されている場合は効果がありません。</span><span class="sxs-lookup"><span data-stu-id="aea88-119">A number of days to fetch from Microsoft Graph - default is 3 - value has no effect if `event-query` attribute is set.</span></span> |
| `eventQuery` | `event-query` | <span data-ttu-id="aea88-120">Microsoft Graph からイベントを取得するときに使用する代替クエリを表す文字列。</span><span class="sxs-lookup"><span data-stu-id="aea88-120">A string that represents an alternative query to be used when fetching events from Microsoft Graph.</span></span> <span data-ttu-id="aea88-121">必要に応じて、デリゲートスコープを ( `|` `"/groups/GROUP-ID-GUID/calendar/calendarView | group.read.all"`) で区切り、文字列の末尾に追加します。</span><span class="sxs-lookup"><span data-stu-id="aea88-121">Optionally, add the delegated scope at the end of the string by delimiting it with `|` (`"/groups/GROUP-ID-GUID/calendar/calendarView | group.read.all"`).</span></span> |
| `events` | `events` | <span data-ttu-id="aea88-122">コンポーネントによってレンダリングされるイベントのリストを取得または設定するイベントの配列-このプロパティを使用して、コンポーネントによって読み込まれたイベントにアクセスします。</span><span class="sxs-lookup"><span data-stu-id="aea88-122">An array of events to get or set the list of events rendered by the component - use this property to access the events loaded by the component.</span></span> <span data-ttu-id="aea88-123">独自のイベントを読み込むには、この値を設定します。値が`date`開発`days`者に`event-query`よって設定されている場合、、、または属性は影響を与えません。</span><span class="sxs-lookup"><span data-stu-id="aea88-123">Set this value to load your own events - if value is set by developer, the `date`, `days`, or `event-query` attributes have no effect.</span></span> |

<span data-ttu-id="aea88-124">次の例では、コンポーネントの動作を変更して、特定の日付および最大3日間のデータをフェッチします。</span><span class="sxs-lookup"><span data-stu-id="aea88-124">The following example changes the behavior of the component to fetch data for a specific date and up to 3 days.</span></span>

```html
<mgt-agenda
  group-by-day
  date="May 7, 2019"
  days="3"
  ></mgt-agenda>
```

<span data-ttu-id="aea88-125">次の例では、コンポーネントの動作を変更して、特定のクエリからデータをフェッチします。</span><span class="sxs-lookup"><span data-stu-id="aea88-125">The following example changes the behavior of the component to fetch data from a specific query.</span></span>

```html
<mgt-agenda
  event-query="/me/events?orderby=start/dateTime"
  ></mgt-agenda>
```

## <a name="css-custom-properties"></a><span data-ttu-id="aea88-126">CSS カスタムプロパティ</span><span class="sxs-lookup"><span data-stu-id="aea88-126">CSS Custom properties</span></span>

<span data-ttu-id="aea88-127">コンポーネント`mgt-agenda`は、これらの CSS カスタムプロパティを定義します。</span><span class="sxs-lookup"><span data-stu-id="aea88-127">The `mgt-agenda` component defines these CSS custom properties</span></span>

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

<span data-ttu-id="aea88-128">詳細については、「[スタイルコンポーネント](../style.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="aea88-128">To learn more, see [styling components](../style.md).</span></span>

## <a name="templates"></a><span data-ttu-id="aea88-129">テンプレート</span><span class="sxs-lookup"><span data-stu-id="aea88-129">Templates</span></span>

<span data-ttu-id="aea88-130">コンポーネント`mgt-agenda`は、コンポーネントの特定の部分を置き換えることができるいくつかの[テンプレート](../templates.md)をサポートしています。</span><span class="sxs-lookup"><span data-stu-id="aea88-130">The `mgt-agenda` component supports several [templates](../templates.md) that allow you to replace certain parts of the component.</span></span> <span data-ttu-id="aea88-131">テンプレートを指定するには、 `<template>`コンポーネントの内部に要素を含め、 `data-type`値を次のいずれかに設定します。</span><span class="sxs-lookup"><span data-stu-id="aea88-131">To specify a template, include a `<template>` element inside of a component and set the `data-type` value to one of the following:</span></span>

| <span data-ttu-id="aea88-132">データ型</span><span class="sxs-lookup"><span data-stu-id="aea88-132">Data type</span></span> | <span data-ttu-id="aea88-133">データコンテキスト</span><span class="sxs-lookup"><span data-stu-id="aea88-133">Data context</span></span> | <span data-ttu-id="aea88-134">説明</span><span class="sxs-lookup"><span data-stu-id="aea88-134">Description</span></span> |
| --- | --- | --- |
| `default` | <span data-ttu-id="aea88-135">`events`: event オブジェクトのリスト</span><span class="sxs-lookup"><span data-stu-id="aea88-135">`events`: list of event objects</span></span> | <span data-ttu-id="aea88-136">既定のテンプレートでは、コンポーネント全体が独自のものに置き換えられます。</span><span class="sxs-lookup"><span data-stu-id="aea88-136">The default template replaces the entire component with your own.</span></span> |
| `event` | <span data-ttu-id="aea88-137">`event`: event オブジェクト</span><span class="sxs-lookup"><span data-stu-id="aea88-137">`event`: event object</span></span> | <span data-ttu-id="aea88-138">各イベントのレンダリングに使用するテンプレート。</span><span class="sxs-lookup"><span data-stu-id="aea88-138">The template used to render each event.</span></span> |
| `header` | <span data-ttu-id="aea88-139">`header`: string</span><span class="sxs-lookup"><span data-stu-id="aea88-139">`header`: string</span></span> | <span data-ttu-id="aea88-140">各日のヘッダーのレンダリングに使用するテンプレート。</span><span class="sxs-lookup"><span data-stu-id="aea88-140">The template used to render the header for each day.</span></span> |
| `other` | <span data-ttu-id="aea88-141">`event`: event オブジェクト</span><span class="sxs-lookup"><span data-stu-id="aea88-141">`event`: event object</span></span> | <span data-ttu-id="aea88-142">各イベントに対して追加のコンテンツをレンダリングするために使用するテンプレート。</span><span class="sxs-lookup"><span data-stu-id="aea88-142">The template used to render additional content for each event.</span></span> |
| `no-data` | <span data-ttu-id="aea88-143">データコンテキストが渡されない</span><span class="sxs-lookup"><span data-stu-id="aea88-143">No data context is passed</span></span> | <span data-ttu-id="aea88-144">イベントが使用できないときに使用するテンプレート。</span><span class="sxs-lookup"><span data-stu-id="aea88-144">The template used when no events are available.</span></span> |
| `loading` | <span data-ttu-id="aea88-145">データコンテキストが渡されない</span><span class="sxs-lookup"><span data-stu-id="aea88-145">No data context is passed</span></span> | <span data-ttu-id="aea88-146">データの読み込み時に使用されるテンプレート。</span><span class="sxs-lookup"><span data-stu-id="aea88-146">The template used when data is loading.</span></span> |

<span data-ttu-id="aea88-147">次の例は、テンプレートの`event`使用方法を示しています。</span><span class="sxs-lookup"><span data-stu-id="aea88-147">The following examples illustrates how to use the `event` template:</span></span>

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

<span data-ttu-id="aea88-148">詳細については、「 [templates](../templates.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="aea88-148">To learn more, see [templates](../templates.md).</span></span>

## <a name="graph-scopes"></a><span data-ttu-id="aea88-149">グラフの範囲</span><span class="sxs-lookup"><span data-stu-id="aea88-149">Graph scopes</span></span>

<span data-ttu-id="aea88-150">このコンポーネントは、次の Microsoft Graph Api とアクセス許可を使用します。</span><span class="sxs-lookup"><span data-stu-id="aea88-150">This component uses the following Microsoft Graph APIs and permissions:</span></span>

| <span data-ttu-id="aea88-151">リソース</span><span class="sxs-lookup"><span data-stu-id="aea88-151">resource</span></span> | <span data-ttu-id="aea88-152">アクセス許可/スコープ</span><span class="sxs-lookup"><span data-stu-id="aea88-152">permission/scope</span></span> |
| - | - |
| [<span data-ttu-id="aea88-153">/me/calendarview</span><span class="sxs-lookup"><span data-stu-id="aea88-153">/me/calendarview</span></span>](https://docs.microsoft.com/en-us/graph/api/calendar-list-calendarview?view=graph-rest-1.0) | `Calendars.Read` |

<span data-ttu-id="aea88-154">このコンポーネントを使用すると、別の Microsoft Graph クエリを指定して`/groups/{id}/calendar/calendarView`呼び出すことができます (など)。</span><span class="sxs-lookup"><span data-stu-id="aea88-154">The component allows you to specify a different Microsoft Graph query to call (such as `/groups/{id}/calendar/calendarView`).</span></span> <span data-ttu-id="aea88-155">この場合は、文字列の末尾にスコープを追加します。`|`</span><span class="sxs-lookup"><span data-stu-id="aea88-155">In this case, append the scope at the end of the string, delimited by `|`</span></span>

## <a name="authentication"></a><span data-ttu-id="aea88-156">認証</span><span class="sxs-lookup"><span data-stu-id="aea88-156">Authentication</span></span>

<span data-ttu-id="aea88-157">ログインコントロールは、[認証のドキュメント](./../providers.md)で説明されているグローバル認証プロバイダを活用します。</span><span class="sxs-lookup"><span data-stu-id="aea88-157">The login control leverages the global authentication provider described in the [authentication documentation](./../providers.md).</span></span> 

