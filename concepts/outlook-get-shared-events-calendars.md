# <a name="get-outlook-events-in-a-shared-or-delegated-calendar"></a>共有または委任された予定表に Outlook のイベントを取得する

Outlook では、お客様は他のユーザーと予定表を共有し、これらのユーザーは共有した予定表のイベントを表示または変更することができます。 また、お客様は、権限を委任し、会議出席依頼の受信や応答、または予定表のアイテムの作成や変更を代行してもらうこともできます。

Microsoft Graph では、他のユーザーと共有する予定表のイベントを取得したり、共有予定表自体を取得したりする機能がプログラムとしてサポートされています。 サポートは、委任された予定表にも適用されます。

たとえば、Garth が予定表を John と共有している場合、John は読み取りアクセスが可能になります。 John がアプリにサインインし、委任されたアクセス許可 (Calendars.Read.Shared または Calendars.ReadWrite.Share) を提供した場合、アプリでは、下記のようにして Garth の規定の予定表とその予定表にあるイベントにアクセスすることができます。

## <a name="get-an-event-in-the-shared-calendar"></a>共有予定表のイベントを取得する

Garth が共有している既定の予定表にある、特定のイベントを取得できます。

<!-- { "blockType": "ignored" } -->
```http
GET users/{Garth-userId | Garth-userPrincipalName}/calendar/events/{id}
```

正常に終了すると、HTTP 200 OK となり、[ Garth](../api-reference/v1.0/resources/event.md)  の規定の予定表から `{id}` によって識別されるイベント インスタンスを取得します。

## <a name="get-all-the-events-in-the-shared-calendar"></a>共有予定表のすべてのイベントを取得する

Garth が John  と共有している既定の予定表にあるすべてのイベントを取得します。

<!-- { "blockType": "ignored" } -->
```http
GET users/{Garth-userId | Garth-userPrincipalName}/calendar/events
```

正常に終了すると、HTTP 200 OK となり、Garth の規定の予定表の [event](../api-reference/v1.0/resources/event.md) インスタンスのコレクションを取得します。

## <a name="get-the-shared-calendar"></a>共有予定表を取得する

Garth が John と共有している既定の予定表を取得します。

<!-- { "blockType": "ignored" } -->
```http
GET users/{Garth-userId | Garth-userPrincipalName}/calendar
```

正常に終了すると、HTTP 200 OK となり、Garth の規定のフォルダーを表す [calendar](../api-reference/v1.0/resources/calendar.md) インスタンスを取得します。

Garth が、自分の規定の予定表へのアクセス権をさらに多く John  に委任していた場合、または Garth が自分のメールボックス全体を John に委任していた場合も、同じ GET 機能が適用されます。

Garth が John と規定の予定表を共有していない、またはメールボックスを John に委任していない場合、それらの GET 操作に Garth のユーザー ID またはユーザー プリンシパル名を指定すると、エラーが返されます。 


## <a name="next-steps"></a>次の手順

詳細情報:

- [Outlook カレンダーと統合する理由](outlook-calendar-concept-overview.md)
- Microsoft Graph v1.0 の[カレンダー API](../api-reference/v1.0/resources/calendar.md)