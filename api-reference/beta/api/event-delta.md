---
title: 'イベント: デルタ'
description: 一連の追加、削除、または**予定表ビュー** (イベントの範囲) で更新されているイベントを取得します。
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: 384dd3eabf21685cf69cf2256493ad01bf4480f7
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27931784"
---
# <a name="event-delta"></a><span data-ttu-id="76a22-103">イベント: デルタ</span><span class="sxs-lookup"><span data-stu-id="76a22-103">event: delta</span></span>

> <span data-ttu-id="76a22-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="76a22-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="76a22-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="76a22-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="76a22-106">ユーザーの標準として設定されている予定表の**calendarView** において追加、削除、更新された一連のイベント (さまざまなイベント) を取得します。</span><span class="sxs-lookup"><span data-stu-id="76a22-106">Get a set of events that have been added, deleted, or updated in a **calendarView** (a range of events) of the user's primary calendar.</span></span>

<span data-ttu-id="76a22-p102">イベントの**デルタ**関数呼び出しは、ユーザーの標準として設定されている予定表のさまざまな日付に対する `GET /calendarview` 要求に似ていますが、これら 1 つ以上の呼び出しにおいて[状態トークン](/graph/delta-query-overview)を適切に適用することにより、そのカレンダー ビュー内における増分変化に対してクエリを実行できる点が異なります。これにより、標準として設定されている予定表のユーザー イベントのローカル格納の保守と同期を行う際に、サーバーからその予定表のイベントすべてを毎回フェッチする必要がなくなります。</span><span class="sxs-lookup"><span data-stu-id="76a22-p102">A **delta** function call for events is similar to a `GET /calendarview` request for a range of dates in the user's primary calendar, except that by appropriately applying [state tokens](/graph/delta-query-overview) in one or more of these calls, you can query for incremental changes in that calender view. This allows you to maintain and synchronize a local store of a user's events in the primary calendar, without having to fetch all the events of that calendar from the server every time.</span></span>

## <a name="permissions"></a><span data-ttu-id="76a22-109">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="76a22-109">Permissions</span></span>
<span data-ttu-id="76a22-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="76a22-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="76a22-112">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="76a22-112">Permission type</span></span>      | <span data-ttu-id="76a22-113">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="76a22-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="76a22-114">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="76a22-114">Delegated (work or school account)</span></span> | <span data-ttu-id="76a22-115">Calendars.Read、Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="76a22-115">Calendars.Read, Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="76a22-116">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="76a22-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="76a22-117">Calendars.Read、Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="76a22-117">Calendars.Read, Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="76a22-118">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="76a22-118">Application</span></span> | <span data-ttu-id="76a22-119">Calendars.Read、Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="76a22-119">Calendars.Read, Calendars.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="76a22-120">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="76a22-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/calendarView/delta?startDateTime={start_datetime}&endDateTime={end_datetime}
GET /users/<id>/calendarView/delta?startDateTime={start_datetime}&endDateTime={end_datetime}

```

## <a name="query-parameters"></a><span data-ttu-id="76a22-121">クエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="76a22-121">Query parameters</span></span>

<span data-ttu-id="76a22-p104">イベントの変化を追跡することにより、1 回以上の、一連の**デルタ**関数呼び出しが発生します。任意のクエリ パラメーター (`$deltatoken` と `$skiptoken` 以外) を使用する場合は、最初の**デルタ**要求でこれを指定する必要があります。Microsoft Graph は、応答で提供される `nextLink` または `deltaLink` の URL のトークン部分に指定したパラメーターを自動的にエンコードします。必要なクエリ パラメーターを前もって指定しておくだけで済みます。それ以降の要求では、前の応答で `nextLink` または `deltaLink` の URL に必要なパラメーターが既にエンコードされ、含まれているため、この URL をコピーして適用します。</span><span class="sxs-lookup"><span data-stu-id="76a22-p104">Tracking changes in events incurs a round of one or more **delta** function calls. If you use any query parameter (other than `$deltatoken` and `$skiptoken`), you must specify it in the initial **delta** request. Microsoft Graph automatically encodes any specified parameters into the token portion of the `nextLink` or `deltaLink` URL provided in the response. You only need to specify any desired query parameters once upfront. In subsequent requests, simply copy and apply the `nextLink` or `deltaLink` URL from the previous response, as that URL already includes the encoded, desired parameters.</span></span>


| <span data-ttu-id="76a22-127">クエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="76a22-127">Query parameter</span></span>      | <span data-ttu-id="76a22-128">種類</span><span class="sxs-lookup"><span data-stu-id="76a22-128">Type</span></span>   |<span data-ttu-id="76a22-129">説明</span><span class="sxs-lookup"><span data-stu-id="76a22-129">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="76a22-130">startDateTime</span><span class="sxs-lookup"><span data-stu-id="76a22-130">startDateTime</span></span>|<span data-ttu-id="76a22-131">String</span><span class="sxs-lookup"><span data-stu-id="76a22-131">String</span></span>|<span data-ttu-id="76a22-p105">時間範囲の開始日時は、ISO 8601 形式で表されます。例: "2015-11-08T19:00:00.0000000"。</span><span class="sxs-lookup"><span data-stu-id="76a22-p105">The start date and time of the time range, represented in ISO 8601 format. For example, "2015-11-08T19:00:00.0000000".</span></span>|
|<span data-ttu-id="76a22-134">endDateTime</span><span class="sxs-lookup"><span data-stu-id="76a22-134">endDateTime</span></span>|<span data-ttu-id="76a22-135">String</span><span class="sxs-lookup"><span data-stu-id="76a22-135">String</span></span>|<span data-ttu-id="76a22-p106">時間範囲の終了日時は、ISO 8601 形式で表されます。例: "2015-11-08T20:00:00.0000000"。</span><span class="sxs-lookup"><span data-stu-id="76a22-p106">The end date and time of the time range, represented in ISO 8601 format. For example, "2015-11-08T20:00:00.0000000".</span></span>|
| <span data-ttu-id="76a22-138">$deltatoken</span><span class="sxs-lookup"><span data-stu-id="76a22-138">$deltatoken</span></span> | <span data-ttu-id="76a22-139">文字列</span><span class="sxs-lookup"><span data-stu-id="76a22-139">string</span></span> | <span data-ttu-id="76a22-p107">同じカレンダー ビュー用の前の**デルタ**関数呼び出しの `deltaLink` URL で返された[状態トークン](/graph/delta-query-overview)で、その一連の変更追跡が完了したことを示します。このトークンを含む `deltaLink` URL 全体を、該当カレンダー ビュー用の次回の一連の変更追跡の最初の要求内に保存し、適用します。</span><span class="sxs-lookup"><span data-stu-id="76a22-p107">A [state token](/graph/delta-query-overview) returned in the `deltaLink` URL of the previous **delta** function call for the same calendar view, indicating the completion of that round of change tracking. Save and apply the entire `deltaLink` URL including this token in the first request of the next round of change tracking for that calendar view.</span></span>|
| <span data-ttu-id="76a22-142">$skiptoken</span><span class="sxs-lookup"><span data-stu-id="76a22-142">$skiptoken</span></span> | <span data-ttu-id="76a22-143">文字列</span><span class="sxs-lookup"><span data-stu-id="76a22-143">string</span></span> | <span data-ttu-id="76a22-144">前の**デルタ**関数呼び出しの `nextLink` URL 内で返された[状態トークン](/graph/delta-query-overview)で、同じカレンダー ビュー内に追跡されるべきさらなる変化があることを示しています。</span><span class="sxs-lookup"><span data-stu-id="76a22-144">A [state token](/graph/delta-query-overview) returned in the `nextLink` URL of the previous **delta** function call, indicating there are further changes to be tracked in the same calendar view.</span></span> |

<span data-ttu-id="76a22-p108">カレンダー ビューでデルタ クエリを実行する場合、`GET /calendarview` 要求で通常得られるプロパティのすべてを得られると予期します。この場合、`$select` はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="76a22-p108">When you do a delta query on a calendar view, expect to get all the properties you'd normally get from a `GET /calendarview` request. `$select` is not supported in this case.</span></span>


## <a name="request-headers"></a><span data-ttu-id="76a22-147">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="76a22-147">Request headers</span></span>
| <span data-ttu-id="76a22-148">名前</span><span class="sxs-lookup"><span data-stu-id="76a22-148">Name</span></span>       | <span data-ttu-id="76a22-149">型</span><span class="sxs-lookup"><span data-stu-id="76a22-149">Type</span></span> | <span data-ttu-id="76a22-150">説明</span><span class="sxs-lookup"><span data-stu-id="76a22-150">Description</span></span> |
|:---------------|:----------|:----------|
| <span data-ttu-id="76a22-151">Authorization</span><span class="sxs-lookup"><span data-stu-id="76a22-151">Authorization</span></span>  | <span data-ttu-id="76a22-152">string</span><span class="sxs-lookup"><span data-stu-id="76a22-152">string</span></span>  | <span data-ttu-id="76a22-p109">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="76a22-p109">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="76a22-155">Content-Type</span><span class="sxs-lookup"><span data-stu-id="76a22-155">Content-Type</span></span>  | <span data-ttu-id="76a22-156">string</span><span class="sxs-lookup"><span data-stu-id="76a22-156">string</span></span>  | <span data-ttu-id="76a22-p110">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="76a22-p110">application/json. Required.</span></span> |
| <span data-ttu-id="76a22-159">Prefer</span><span class="sxs-lookup"><span data-stu-id="76a22-159">Prefer</span></span> | <span data-ttu-id="76a22-160">文字列</span><span class="sxs-lookup"><span data-stu-id="76a22-160">string</span></span>  | <span data-ttu-id="76a22-p111">odata.maxpagesize={x}.省略可能。</span><span class="sxs-lookup"><span data-stu-id="76a22-p111">odata.maxpagesize={x}. Optional.</span></span> |
| <span data-ttu-id="76a22-163">Prefer</span><span class="sxs-lookup"><span data-stu-id="76a22-163">Prefer</span></span> | <span data-ttu-id="76a22-164">文字列</span><span class="sxs-lookup"><span data-stu-id="76a22-164">string</span></span> | <span data-ttu-id="76a22-p112">{タイム ゾーン}。省略可能。指定しない場合、UTC が使用されます。</span><span class="sxs-lookup"><span data-stu-id="76a22-p112">{Time zone}. Optional, UTC assumed if absent.</span></span>|

## <a name="response"></a><span data-ttu-id="76a22-167">応答</span><span class="sxs-lookup"><span data-stu-id="76a22-167">Response</span></span>

<span data-ttu-id="76a22-168">成功した場合、このメソッドは `200 OK` の応答コードと、応答本文で [イベント](../resources/event.md) コレクション オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="76a22-168">If successful, this method returns a `200 OK` response code and [event](../resources/event.md) collection object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="76a22-169">例</span><span class="sxs-lookup"><span data-stu-id="76a22-169">Example</span></span>
##### <a name="request"></a><span data-ttu-id="76a22-170">要求</span><span class="sxs-lookup"><span data-stu-id="76a22-170">Request</span></span>

<span data-ttu-id="76a22-171">次の例では、1 回の**デルタ**関数呼び出しを行い、応答本文中のイベントの最大数を 2 に制限する方法を示します。</span><span class="sxs-lookup"><span data-stu-id="76a22-171">The following example shows how to make a single **delta** function call, and limit the maximum number of events in the response body to 2.</span></span>

<span data-ttu-id="76a22-172">カレンダー ビュー内の変更を追跡するには、1 回以上の**デルタ**関数呼び出しを作成し、適切な[状態トークン](/graph/delta-query-overview)を使用して、前回のデルタ クエリ以降になされた一連の増分変更を取得します。</span><span class="sxs-lookup"><span data-stu-id="76a22-172">To track changes in a calendar view, you would make one or more **delta** function calls, with appropriate [state tokens](/graph/delta-query-overview), to get the set of incremental changes since the last delta query.</span></span>

<!-- {
  "blockType": "request",
  "name": "event_delta"
}-->
```http
GET https://graph.microsoft.com/beta/me/calendarview/delta?startdatetime={start_datetime}&enddatetime={end_datetime}

Prefer: odata.maxpagesize=2
```

##### <a name="response"></a><span data-ttu-id="76a22-173">応答</span><span class="sxs-lookup"><span data-stu-id="76a22-173">Response</span></span>
<span data-ttu-id="76a22-p113">要求が成功した場合、応答に含まれる状態トークンは、_スキップ トークン_ (_@odata.nextLink_ 応答ヘッダーに含まれる) か、_デルタ トークン_ (_@odata.deltaLink_ 応答ヘッダーに含まれる) のいずれかになります。前者はその回を続行する必要があることを示し、後者はその回のすべての変更の取得が完了したことを示します。</span><span class="sxs-lookup"><span data-stu-id="76a22-p113">If the request is successful, the response would include a state token, which is either a _skipToken_ (in an _@odata.nextLink_ response header) or a _deltaToken_ (in an _@odata.deltaLink_ response header). Respectively, they indicate whether you should continue with the round or you have completed getting all the changes for that round.</span></span>

<span data-ttu-id="76a22-176">以下の応答は、_@odata.nextLink_ 応答ヘッダーに含まれる _skipToken_ を示しています。</span><span class="sxs-lookup"><span data-stu-id="76a22-176">The response below shows a _skipToken_ in an _@odata.nextLink_ response header.</span></span>

<span data-ttu-id="76a22-p114">注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="76a22-p114">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.event",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 359

{
  "@odata.nextLink":"https://graph.microsoft.com/beta/me/calendarview/delta?$skiptoken={_skipToken_}",
  "value": [
    {
      "originalStartTimeZone": "originalStartTimeZone-value",
      "originalEndTimeZone": "originalEndTimeZone-value",
      "responseStatus": {
        "response": "response-value",
        "time": "datetime-value"
      },
      "uid": "iCalUId-value",
      "reminderMinutesBeforeStart": 99,
      "isReminderOn": true
    }
  ]
}
```

### <a name="see-also"></a><span data-ttu-id="76a22-179">関連項目</span><span class="sxs-lookup"><span data-stu-id="76a22-179">See also</span></span>

- [<span data-ttu-id="76a22-180">Microsoft Graph デルタ クエリ</span><span class="sxs-lookup"><span data-stu-id="76a22-180">Microsoft Graph delta query</span></span>](/graph/delta-query-overview)
- [<span data-ttu-id="76a22-181">フォルダー内のイベントへの増分の変更を取得する</span><span class="sxs-lookup"><span data-stu-id="76a22-181">Get incremental changes to events in a folder</span></span>](/graph/delta-query-events)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "event: delta",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
