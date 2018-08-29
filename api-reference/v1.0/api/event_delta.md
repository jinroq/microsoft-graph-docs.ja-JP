# <a name="event-delta"></a><span data-ttu-id="73177-101">イベント: デルタ</span><span class="sxs-lookup"><span data-stu-id="73177-101">event: delta</span></span>

<span data-ttu-id="73177-102">ユーザーの標準として設定されている予定表の**calendarView** において追加、削除、更新された一連のイベント (さまざまなイベント) を取得します。</span><span class="sxs-lookup"><span data-stu-id="73177-102">Get a set of events that have been added, deleted, or updated in a **calendarView** (a range of events) of the user's primary calendar.</span></span>

<span data-ttu-id="73177-p101">イベントの**デルタ**関数呼び出しは、ユーザーの標準として設定されている予定表のさまざまな日付に対する `GET /calendarview` 要求に似ていますが、これら 1 つ以上の呼び出しにおいて[状態トークン](../../../concepts/delta_query_overview.md)を適切に適用することにより、そのカレンダー ビュー内における増分変化に対してクエリを実行できる点が異なります。これにより、標準として設定されている予定表のユーザー イベントのローカル格納の保守と同期を行う際に、サーバーからその予定表のイベントすべてを毎回フェッチする必要がなくなります。</span><span class="sxs-lookup"><span data-stu-id="73177-p101">A **delta** function call for events is similar to a `GET /calendarview` request for a range of dates in the user's primary calendar, except that by appropriately applying [state tokens](../../../concepts/delta_query_overview.md) in one or more of these calls, you can query for incremental changes in that calender view. This allows you to maintain and synchronize a local store of a user's events in the primary calendar, without having to fetch all the events of that calendar from the server every time.</span></span>

## <a name="permissions"></a><span data-ttu-id="73177-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="73177-105">Permissions</span></span>
<span data-ttu-id="73177-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="73177-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>


|<span data-ttu-id="73177-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="73177-108">Permission type</span></span>      | <span data-ttu-id="73177-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="73177-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="73177-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="73177-110">Delegated (work or school account)</span></span> | <span data-ttu-id="73177-111">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="73177-111">Calendars.Read</span></span>    |
|<span data-ttu-id="73177-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="73177-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="73177-113">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="73177-113">Calendars.Read</span></span>    |
|<span data-ttu-id="73177-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="73177-114">Application</span></span> | <span data-ttu-id="73177-115">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="73177-115">Calendars.Read</span></span> |

## <a name="http-request"></a><span data-ttu-id="73177-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="73177-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/calendarView/delta?startDateTime={start_datetime}&endDateTime={end_datetime}
GET /users/{id}/calendarView/delta?startDateTime={start_datetime}&endDateTime={end_datetime}

```

### <a name="query-parameters"></a><span data-ttu-id="73177-117">クエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="73177-117">Query parameters</span></span>

<span data-ttu-id="73177-p103">イベントの変化を追跡することにより、1 回以上の、一連の**デルタ**関数呼び出しが発生します。任意のクエリ パラメーター (`$deltatoken` と `$skiptoken` 以外) を使用する場合は、最初の**デルタ**要求でこれを指定する必要があります。Microsoft Graph は、応答で提供される `nextLink` または `deltaLink` の URL のトークン部分に指定したパラメーターを自動的にエンコードします。必要なクエリ パラメーターを前もって指定しておくだけで済みます。それ以降の要求では、前の応答で `nextLink` または `deltaLink` の URL に必要なパラメーターが既にエンコードされ、含まれているため、この URL をコピーして適用します。</span><span class="sxs-lookup"><span data-stu-id="73177-p103">Tracking changes in events incurs a round of one or more **delta** function calls. If you use any query parameter (other than `$deltatoken` and `$skiptoken`), you must specify it in the initial **delta** request. Microsoft Graph automatically encodes any specified parameters into the token portion of the `nextLink` or `deltaLink` URL provided in the response. You only need to specify any desired query parameters once upfront. In subsequent requests, simply copy and apply the `nextLink` or `deltaLink` URL from the previous response, as that URL already includes the encoded, desired parameters.</span></span>


| <span data-ttu-id="73177-123">クエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="73177-123">Query parameter</span></span>      | <span data-ttu-id="73177-124">種類</span><span class="sxs-lookup"><span data-stu-id="73177-124">Type</span></span>   |<span data-ttu-id="73177-125">説明</span><span class="sxs-lookup"><span data-stu-id="73177-125">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="73177-126">startDateTime</span><span class="sxs-lookup"><span data-stu-id="73177-126">startDateTime</span></span>|<span data-ttu-id="73177-127">文字列</span><span class="sxs-lookup"><span data-stu-id="73177-127">String</span></span>|<span data-ttu-id="73177-p104">時間範囲の開始日時は、ISO 8601 形式で表されます。例: "2015-11-08T19:00:00.0000000"。</span><span class="sxs-lookup"><span data-stu-id="73177-p104">The start date and time of the time range, represented in ISO 8601 format. For example, "2015-11-08T19:00:00.0000000".</span></span>|
|<span data-ttu-id="73177-130">endDateTime</span><span class="sxs-lookup"><span data-stu-id="73177-130">endDateTime</span></span>|<span data-ttu-id="73177-131">文字列</span><span class="sxs-lookup"><span data-stu-id="73177-131">String</span></span>|<span data-ttu-id="73177-p105">時間範囲の終了日時は、ISO 8601 形式で表されます。例: "2015-11-08T20:00:00.0000000"。</span><span class="sxs-lookup"><span data-stu-id="73177-p105">The end date and time of the time range, represented in ISO 8601 format. For example, "2015-11-08T20:00:00.0000000".</span></span>|
| <span data-ttu-id="73177-134">$deltatoken</span><span class="sxs-lookup"><span data-stu-id="73177-134">$deltatoken</span></span> | <span data-ttu-id="73177-135">文字列</span><span class="sxs-lookup"><span data-stu-id="73177-135">string</span></span> | <span data-ttu-id="73177-p106">同じカレンダー ビュー用の前の**デルタ**関数呼び出しの `deltaLink` URL で返された[状態トークン](../../../concepts/delta_query_overview.md)で、その一連の変更追跡が完了したことを示します。このトークンを含む `deltaLink` URL 全体を、該当カレンダー ビュー用の次回の一連の変更追跡の最初の要求内に保存し、適用します。</span><span class="sxs-lookup"><span data-stu-id="73177-p106">A [state token](../../../concepts/delta_query_overview.md) returned in the `deltaLink` URL of the previous **delta** function call for the same calendar view, indicating the completion of that round of change tracking. Save and apply the entire `deltaLink` URL including this token in the first request of the next round of change tracking for that calendar view.</span></span>|
| <span data-ttu-id="73177-138">$skiptoken</span><span class="sxs-lookup"><span data-stu-id="73177-138">$skiptoken</span></span> | <span data-ttu-id="73177-139">文字列</span><span class="sxs-lookup"><span data-stu-id="73177-139">string</span></span> | <span data-ttu-id="73177-140">前の**デルタ**関数呼び出しの `nextLink` URL 内で返された[状態トークン](../../../concepts/delta_query_overview.md)で、同じカレンダー ビュー内に追跡されるべきさらなる変化があることを示しています。</span><span class="sxs-lookup"><span data-stu-id="73177-140">A [state token](../../../concepts/delta_query_overview.md) returned in the `nextLink` URL of the previous **delta** function call, indicating there are further changes to be tracked in the same calendar view.</span></span> |

<span data-ttu-id="73177-p107">カレンダー ビューでデルタ クエリを実行する場合、`GET /calendarview` 要求で通常得られるプロパティのすべてを得られると予期します。この場合、`$select` はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="73177-p107">When you do a delta query on a calendar view, expect to get all the properties you'd normally get from a `GET /calendarview` request. `$select` is not supported in this case.</span></span> 


## <a name="request-headers"></a><span data-ttu-id="73177-143">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="73177-143">Request headers</span></span>
| <span data-ttu-id="73177-144">名前</span><span class="sxs-lookup"><span data-stu-id="73177-144">Name</span></span>       | <span data-ttu-id="73177-145">型</span><span class="sxs-lookup"><span data-stu-id="73177-145">Type</span></span> | <span data-ttu-id="73177-146">説明</span><span class="sxs-lookup"><span data-stu-id="73177-146">Description</span></span> |
|:---------------|:----------|:----------|
| <span data-ttu-id="73177-147">承認</span><span class="sxs-lookup"><span data-stu-id="73177-147">Authorization</span></span>  | <span data-ttu-id="73177-148">文字列</span><span class="sxs-lookup"><span data-stu-id="73177-148">string</span></span>  | <span data-ttu-id="73177-p108">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="73177-p108">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="73177-151">コンテンツ タイプ</span><span class="sxs-lookup"><span data-stu-id="73177-151">Content-Type</span></span>  | <span data-ttu-id="73177-152">文字列</span><span class="sxs-lookup"><span data-stu-id="73177-152">string</span></span>  | <span data-ttu-id="73177-p109">アプリケーションまたは json。必須。</span><span class="sxs-lookup"><span data-stu-id="73177-p109">application/json. Required.</span></span> |
| <span data-ttu-id="73177-155">優先</span><span class="sxs-lookup"><span data-stu-id="73177-155">Prefer</span></span> | <span data-ttu-id="73177-156">文字列</span><span class="sxs-lookup"><span data-stu-id="73177-156">string</span></span>  | <span data-ttu-id="73177-p110">odata.maxpagesize={x}.省略可能。</span><span class="sxs-lookup"><span data-stu-id="73177-p110">odata.maxpagesize={x}. Optional.</span></span> |
| <span data-ttu-id="73177-159">優先</span><span class="sxs-lookup"><span data-stu-id="73177-159">Prefer</span></span> | <span data-ttu-id="73177-160">文字列</span><span class="sxs-lookup"><span data-stu-id="73177-160">string</span></span> | <span data-ttu-id="73177-p111">{タイム ゾーン}。省略可能。指定しない場合、UTC が使用されます。</span><span class="sxs-lookup"><span data-stu-id="73177-p111">{Time zone}. Optional, UTC assumed if absent.</span></span>|

## <a name="response"></a><span data-ttu-id="73177-163">応答</span><span class="sxs-lookup"><span data-stu-id="73177-163">Response</span></span>

<span data-ttu-id="73177-164">成功した場合、このメソッドは `200 OK` の応答コードと、応答本文で [イベント](../resources/event.md) コレクション オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="73177-164">If successful, this method returns a `200 OK` response code and [event](../resources/event.md) collection object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="73177-165">例</span><span class="sxs-lookup"><span data-stu-id="73177-165">Example</span></span>
##### <a name="request"></a><span data-ttu-id="73177-166">要求</span><span class="sxs-lookup"><span data-stu-id="73177-166">Request</span></span>

<span data-ttu-id="73177-167">次の例では、1 回の**デルタ**関数呼び出しを行い、応答本文中のイベントの最大数を 2 に制限する方法を示します。</span><span class="sxs-lookup"><span data-stu-id="73177-167">The following example shows how to make a single **delta** function call, and limit the maximum number of events in the response body to 2.</span></span>

<span data-ttu-id="73177-168">カレンダー ビュー内の変更を追跡するには、1 回以上の**デルタ**関数呼び出しを作成し、適切な[状態トークン](../../../concepts/delta_query_overview.md)を使用して、前回のデルタ クエリ以降になされた一連の増分変更を取得します。</span><span class="sxs-lookup"><span data-stu-id="73177-168">To track changes in a calendar view, you would make one or more **delta** function calls, with appropriate [state tokens](../../../concepts/delta_query_overview.md), to get the set of incremental changes since the last delta query.</span></span> 

<!-- {
  "blockType": "request",
  "name": "event_delta"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/calendarView/delta?startdatetime={start_datetime}&enddatetime={end_datetime}

Prefer: odata.maxpagesize=2
```

##### <a name="response"></a><span data-ttu-id="73177-169">応答</span><span class="sxs-lookup"><span data-stu-id="73177-169">Response</span></span>
<span data-ttu-id="73177-p112">要求が成功した場合、応答に含まれる状態トークンは、_スキップ トークン_ (_@odata.nextLink_ 応答ヘッダーに含まれる) か、_デルタ トークン_ (_@odata.deltaLink_ 応答ヘッダーに含まれる) のいずれかになります。前者はその回を続行する必要があることを示し、後者はその回のすべての変更の取得が完了したことを示します。</span><span class="sxs-lookup"><span data-stu-id="73177-p112">If the request is successful, the response would include a state token, which is either a _skipToken_ (in an _@odata.nextLink_ response header) or a _deltaToken_ (in an _@odata.deltaLink_ response header). Respectively, they indicate whether you should continue with the round or you have completed getting all the changes for that round.</span></span>

<span data-ttu-id="73177-172">以下の応答は、_@odata.nextLink_ 応答ヘッダーに含まれる _skipToken_ を示しています。</span><span class="sxs-lookup"><span data-stu-id="73177-172">The response below shows a _skipToken_ in an _@odata.nextLink_ response header.</span></span>

<span data-ttu-id="73177-p113">注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="73177-p113">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "@odata.nextLink":"https://graph.microsoft.com/v1.0/me/calendarView/delta?$skiptoken={_skipToken_}",
  "value": [
    {
      "originalStartTimeZone": "originalStartTimeZone-value",
      "originalEndTimeZone": "originalEndTimeZone-value",
      "responseStatus": {
        "response": "response-value",
        "time": "datetime-value"
      },
      "iCalUId": "iCalUId-value",
      "reminderMinutesBeforeStart": 99,
      "isReminderOn": true
    }
  ]
}
```

### <a name="see-also"></a><span data-ttu-id="73177-175">関連項目</span><span class="sxs-lookup"><span data-stu-id="73177-175">See also</span></span>

- [<span data-ttu-id="73177-176">デルタ クエリを使用して、Microsoft Graph データの変更を追跡する</span><span class="sxs-lookup"><span data-stu-id="73177-176">Use delta query to track changes in Microsoft Graph data</span></span>](../../../concepts/delta_query_overview.md)
- [<span data-ttu-id="73177-177">カレンダー内のイベントの増分の変更を取得する</span><span class="sxs-lookup"><span data-stu-id="73177-177">Get incremental changes to events in a calendar</span></span>](../../../concepts/delta_query_events.md)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "event: delta",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->