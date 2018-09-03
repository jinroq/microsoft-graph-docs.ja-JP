# <a name="outlook-calendar-api-overview"></a>Outlook カレンダー API の概要

Outlook カレンダーは、Office 365 の Outlook メッセージング ハブの一部です。Outlook メッセージング ハブを使うと、メールや連絡先の管理、組織内のユーザーに関する情報の検索、オンライン会話の開始、ファイルの共有、およびグループでの共同作業ができます。

## <a name="why-integrate-with-outlook-calendar"></a>Outlook カレンダーと統合する理由

### <a name="reach-hundreds-of-millions-of-customers-and-build-rich-scenarios"></a>何億というユーザーに達する豊富なシナリオの構築

何百万人ものユーザーが、効果的な通信や作業を可能にする統合ハブの一部として、Outlook カレンダーを利用しています。 そのようなユーザーは、会議の設定、メール管理、連絡先や他のユーザーに関する情報の検索、会話やオンライン会議の開始などを、Web 上であれ、モバイル端末やデスクトップであれ、すべて 1 つの場所で実行できます。 Microsoft Graph は、これらのユーザーのカレンダー、メール、連絡先にアプリを接続するだけでなく、アプリを使って [Microsoft 365 の長所と統合](overview-major-services.md)し、生産性とコラボレーションの向上につながるさまざまなシナリオをサポートすることができます。

### <a name="automate-appointment-organization-and-calendaring"></a>自動予約機構とカレンダーの作成

多くのユーザーは、Outlook による仕事予定、家族や個人の活動時間の整理方法を好んで利用しています。 Microsoft Graph REST API は、操作感がこのカスタマー エクスペリエンスとよく似ており、アプリを使ったイベントの作成、管理、応答を次のように自然に行えます。

- Outlook では、ユーザーは仕事、家族、その他の用途に合わせてそれぞれカレンダーを作成し、カレンダー グループでそれらを整理できます。 **誕生日**や**休日**に関する無料のカレンダーを有効にして、連絡先の誕生日や地元の祝日を忘れないようにできます。 スポーツ チームやテレビ番組のカレンダーなど、関心に応じてカレンダーを追加できます。 ユーザーは、カレンダーを選択およびオーバーレイして、同じビューでイベントを確認できます。 カレンダー API を使うと、[カレンダー グループ](../api-reference/v1.0/resources/calendargroup.md)内の[カレンダー](../api-reference/v1.0/resources/calendar.md)を同様に整理し、ユーザーのメールボックスにある他の**カレンダー**と同じように関心のあるカレンダーを操作できます。 

- Outlook ユーザーは、イベント、メッセージ、連絡先、タスク、グループ投稿に対して、一貫した方法でカテゴリを適用でき、データの整理と検出機能を拡充できます。 カレンダー API を使うと、[カテゴリに関するユーザーのマスター リストにアクセスして定義](../api-reference/v1.0/api/outlookuser_post_mastercategories.md)できるので、クリエイティブなシナリオがさらに豊富になります。 たとえば、スポーツ クラブではスポーツ トーナメントを整理し、競技種目ごとに色分類項目を別個に指定してメールやイベントを区別するアプリを提供できます。 思いがけない予定変更など、予定間際のニュースでも、そのようなイベントやメールに**重要度**プロパティをアプリで設定して、ユーザーに通知できます。

- カレンダー フォルダーでは、1 回きりの[イベント](../api-reference/v1.0/resources/event.md)を[作成](../api-reference/v1.0/api/user_post_events.md)および[更新](../api-reference/v1.0/api/event_update.md)できるだけでなく、[定期的なイベントをスケジュールして管理](outlook-schedule-recurring-events.md)することもできます。 ユーザーは[会議出席依頼](../api-reference/v1.0/resources/eventmessage.md)に回答でき、関連付けられている**イベント** ナビゲーション プロパティを使用すると、[アラーム](../api-reference/v1.0/resources/reminder.md)の[再通知](../api-reference/v1.0/api/event_snoozereminder.md)や[解除](../api-reference/v1.0/api/event_dismissreminder.md)もできます。


### <a name="help-customers-stay-synchronized-and-navigate-their-day"></a>同期維持と予定日の操作に関するユーザー支援機能

カレンダー API を使うと、次に示すように、予定日の操作や生産性の向上が容易になります。

<!-- change link to notifications to the concept topic once it's created. In general, try staying in the conceptual level in these overview topics, if conceptual topics are available for the link destination. 
-->

- [変更通知](../api-reference/v1.0/resources/webhooks.md)を受信登録し、ユーザーのカレンダー内の[イベントに対する変更を追跡](delta_query_events.md)することにより、アプリのローカル ストアの同期を維持できます。
- 軽量な[通知ビュー](../api-reference/v1.0/api/user_reminderview.md)に基づいて、ユーザーの予定一覧を表示できます。 
- ユーザーは、会議の[承諾](../api-reference/v1.0/api/event_accept.md)や出席を **webLink** プロパティを介してオンラインで行うことができます。webLink プロパティにより、会議は Outlook on the web で開催されます。
- ユーザーは、会議の[仮承諾](../api-reference/v1.0/api/event_tentativelyaccept.md)または[辞退](../api-reference/v1.0/api/event_decline.md)を外出中でも回答できます。

### <a name="enhance-collaboration"></a>コラボレーションの強化

- Outlook では、ユーザーどうしでカレンダーを共有でき、カレンダーの内容の読み取り、書き込み、削除に関するアクセス許可を付与できます。 また、ユーザーは自分の代わりに別のユーザーが会議出席依頼に返信するように、カレンダーに指定できます。 あるユーザーの代理をする共有アクションや委任アクションをプログラムを使用して開始することはできませんが、一連のプロパティ (**canEdit**、**canShare**、**canViewPrivateItems**、**isShared**、**isSharedWithMe**) を使用すると、共有ステータスを確認し、共有カレンダーや委任されたカレンダーに関するシナリオを有効にできます。
- カレンダー API を利用することにより、サインイン ユーザー、またはサインイン ユーザーとカレンダーを共有または委任しているユーザーの予定表アイテムを取得できます。 たとえば、Garth がカレンダーを John と共有している場合、または Garth が John にアクセスを委任している場合、John からの[アクセス許可委任](permissions_reference.md#delegated-permissions-application-permissions-and-effective-permissions)があれば、Garth の共有カレンダーとその内容にも読み取りアクセスが可能になります。
- ** Office 365 グループを使用すると、グループ メンバーの共同作業や、グループでの会話やカレンダーへのアクセスが、Outlook で直接行うことができます。 グループ カレンダーとユーザー カレンダーに細かな違いがいくつかあることを除けば、カレンダー API を使用することで、ユーザー カレンダーとほぼ同様にグループ カレンダーを操作できます。 詳細については、[calendar](../api-reference/v1.0/resources/calendar.md) リソースをご覧ください。

** 職場または学校のアカウントで Outlook カレンダーに特に適用可能な機能を示します。


### <a name="schedule-smart"></a>スマートなスケジュール設定

Outlook とカレンダー API には、イベントのスケジュールに便利な機能が豊富に用意されています。

- Outlook カレンダーのアプリ設定により、ユーザーは、フライト、ホテル、食事の予約などのメールや請求書からイベントを自動で追加できます。 追加されたイベントは、ユーザーのメールボックスにある他の [event](../api-reference/v1.0/resources/event.md) オブジェクトと同様に操作できるので、Outlook のこの機能に基づいてクリエイティブなシナリオを構築できます。
- ** Outlook では、会議室の予約も、出席者を**イベント**に追加するのと同じほど簡単に行えます。 カレンダー API では、会議室が [emailAddress](../api-reference/v1.0/resources/emailaddress.md) オブジェクトとして表されます。 テナントで利用可能な[会議室を取得 (プレビュー) ](../api-reference/beta/api/user_findrooms.md)したり、[会議室リストを取得 (プレビュー) ](../api-reference/beta/api/user_findroomlists.md)することができます。 特定の会議室での会議を主催するには、その会議室を** イベント**の** 場所**プロパティに割り当てます。
- * * 一定期間の[ユーザーとリソースの空き状況の情報を検索する (プレビュー) ](outlook-get-free-busy-schedule.md)することができます。 そして、このデータを使用してリソース プランニングやイベントのスケジューリングなど、さまざまなシナリオに適用することができます。 
- ** 最適な時間に会議をスケジューリングしなければならないような場合は、[findMeetingTimes を使用して可能な時間や集合する場所を特定する](findmeetingtimes_example.md)ことを検討してください。 [FindMeetingTimes](../api-reference/v1.0/api/user_findmeetingtimes.md) 関数は、出席者の空き時間状況、会議室や日時に関する希望、およびユーザーが指定した他の制約事項を考慮します。 最初の試行で全員参加可能な会議日時が返されない場合は、理由を確認してから条件を変更し、もう一度 **findMeetingTimes** を呼び出してください。


### <a name="teleconference-across-multiple-locations-and-time-zones"></a>複数の場所とタイム ゾーンをまたぐ電話会議

グローバル化に伴い、現代のビジネス会議には、出席者がさまざまな場所やタイム ゾーンから参加していることも少なくありません。 カレンダー API を使用してそのような会議を管理する方法を次に示します。

- Outlook の例として、ユーザーが組織する会議に、シアトルの会議室、パリのコーヒー ショップ、中国のホーム オフィスから出席者が参加するケースが考えられます。 プログラムを使用すると、[location](../api-reference/v1.0/resources/location.md) オブジェクトのコレクションであるイベントの**場所**プロパティで、このレベルの詳細を**場所**ごとに **displayName** と **locationType** で反映できます。 [例](../api-reference/v1.0/api/event_get.md#request-2)をご覧ください。
- Outlook では、柔軟にイベントを組織し、イベントの開始日時と終了日時ごとにタイム ゾーンを指定できます。 このような柔軟性をサポートするため、既定では、カレンダー API は**イベント**の**開始**日時と**終了**日時を UTC で返し、用意されている **originalStartTimeZone** プロパティと **originalEndTimeZone** プロパティで、イベントの作成時に使用されたタイム ゾーンを示します。 
- 代わりに、`Prefer: outlook.timezone="{time zone name}"` ヘッダーを指定して、GET イベント操作が**開始**日時と**終了**日時を指定したタイム ゾーンで返すようにすることもできます。 タイム ゾーン名は、この[リスト](../api-reference/v1.0/resources/datetimetimezone.md)にあるものだけでなく、Windows でサポートされている任意の名前を使用できます。 ヘッダーの使用[例](../api-reference/v1.0/api/event_get.md#request-1)をご覧ください。`Prefer`


### <a name="take-advantage-of-social-intelligence-and-other-developer-conveniences-in-microsoft-graph"></a>Microsoft Graph でのソーシャル インテリジェンス、および開発者向けのその他の便利な機能の活用

Microsoft Graph では、[people API](people_example.md) を使用し、ユーザーの通信パターンやコラボレーション パターン、ビジネス上の関係に基づく [人物データ](../api-reference/v1.0/resources/person.md)に接続できます。 ユーザー選択などのコントロールを実装し、ユーザーの代わりに会議を組織するときに、ユーザーに関係のある人物を提案できます。

アプリ データを外部データ ストアに保存および管理する際、オーバーヘッドを保存します。 Microsoft Graph では、各リソース インスタンスごとに、カスタム アプリ データを[オープン拡張機能](extensibility_overview.md#open-extensions)として保存できます。 データを入力する必要がある場合、または入力されたスキーマを共有できるようにする場合は、カスタム アプリ データを[スキーマ拡張機能](extensibility_overview.md#schema-extensions)に保存できます。


## <a name="next-steps"></a>次の手順

- [Graph Explorer](https://developer.microsoft.com/graph/graph-explorer/?request=me%2Fevents&version=v1.0) でカレンダー サンプル クエリを選択して試行します。
- 以下について調べます。
  - [開催可能な会議日時を Outlook カレンダーで検索する](findmeetingtimes_example.md)
  - [繰り返される予定を Outlook で定期的なイベントとしてスケジュール設定する](outlook-schedule-recurring-events.md)
- Outlook [カレンダー API](../api-reference/v1.0/resources/calendar.md) リファレンスを確認します。

<!-- Replace the last item with the calendar API overview when it's published.
-->
