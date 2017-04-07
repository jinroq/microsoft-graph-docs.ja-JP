# <a name="group-resource-type"></a>group リソース タイプ

Office 365 グループ、動的なグループ、またはセキュリティ グループのいずれかの Azure Active Directory グループを表します。[directoryObject](directoryobject.md) から継承します。


## <a name="methods"></a>メソッド

| メソッド       | 戻り値の型  |説明|
|:---------------|:--------|:----------|
|[グループを作成する](../api/group_post_groups.md) | [group](group.md) |新しいグループを作成します。Office 365 グループ、動的なグループ、またはセキュリティ グループのいずれにすることができます。|
|[グループを取得する](../api/group_get.md) | [group](group.md) |グループ オブジェクトのプロパティを読み取ります。|
|[グループを一覧表示する](../api/group_list.md) |[group](group.md) コレクション |グループ オブジェクトとそのプロパティを一覧表示します。|
|[グループを更新する](../api/group_update.md) | [group](group.md) |グループ オブジェクトのプロパティを更新します。 |
|[グループを削除する](../api/group_delete.md) | なし |グループ オブジェクトを削除します。 |
|[メンバーを追加する](../api/group_post_members.md) |なし| **members** ナビゲーション プロパティ (セキュリティ グループおよびメールが有効なセキュリティ グループでのみサポートされます) に投稿することによってこのグループにユーザーまたはグループを追加します。|
|[メンバーを一覧表示する](../api/group_list_members.md) |[directoryObject](directoryobject.md) コレクション| **members** ナビゲーション プロパティからこのグループの直接のメンバーであるユーザーおよびグループを取得します。|
|[メンバーを削除する](../api/group_delete_members.md) | なし |**members** ナビゲーション プロパティを使用して Office 365 のグループ、セキュリティ グループ、またはメールが有効なセキュリティ グループからメンバーを削除できます。ユーザーや他のグループを削除できます。 |
|[memberOf を一覧表示する](../api/group_list_memberof.md) |[directoryObject](directoryobject.md) コレクション| **memberOf** ナビゲーション プロパティからこのグループが直接のメンバーであるグループを取得します。|
|[所有者を追加する](../api/group_post_owners.md) |なし| **members** ナビゲーション プロパティ (セキュリティ グループおよびメールが有効なセキュリティ グループのみをサポート) に投稿することによってグループの新規所有者を追加します。|
|[所有者を一覧表示する](../api/group_list_owners.md) |[directoryObject](directoryobject.md) コレクション| **owners** ナビゲーション プロパティからグループの所有者を取得します。|
|[所有者を削除する](../api/group_delete_owners.md) | なし |**owners** ナビゲーション プロパティを使用して Office 365 のグループ、セキュリティ グループ、またはメールが有効なセキュリティ グループから所有者を削除します。|
|[checkMemberGroups](../api/group_checkmembergroups.md)|String collection|グループの一覧内のメンバーシップについてこのグループを確認します。この関数は、推移的です。|
|[getMemberGroups](../api/group_getmembergroups.md)|String collection|このグループがメンバーであるすべてのグループを返します。この関数は、推移的です。|
|[getMemberObjects](../api/group_getmemberobjects.md)|String collection|このグループがメンバーであるすべてのグループを返します。この関数は、推移的です。 |
|[イベントを作成する](../api/group_post_events.md) |[Event](event.md)| Event コレクションへの投稿によって、新しいイベントを作成します。|
|[イベントを一覧表示する](../api/group_list_events.md) |[Event](event.md) コレクション| Event オブジェクトのコレクションを取得します。|
|[calendarView を一覧表示する](../api/group_list_calendarview.md) |[Event](event.md) コレクション| 指定された時間枠のイベントのコレクションを取得します。|
|[会話を作成する](../api/group_post_conversations.md) |[Conversation](conversation.md)| Conversation コレクションに投稿することによって、新しい会話を作成します。|
|[会話を一覧表示する](../api/group_list_conversations.md) |[Conversation](conversation.md) コレクション| Conversation オブジェクトのコレクションを取得します。|
|[スレッドを一覧表示する](../api/group_list_threads.md) |[conversationThread](conversationthread.md) コレクション| グループのすべてのスレッドを取得します。|
|[acceptedSenders を一覧表示する](../api/group_list_acceptedsenders.md) |[directoryObject](directoryobject.md) コレクション| このグループの acceptedSenders リストに含まれるユーザーまたはグループの一覧を取得します。|
|[acceptedSender を追加する](../api/group_post_acceptedsenders.md) |[directoryObject](directoryobject.md)| acceptSenders コレクションにユーザーまたはグループを追加します。|
|[acceptedSender を削除する](../api/group_delete_acceptedsenders.md) |[directoryObject](directoryobject.md)| acceptedSenders コレクションからユーザーまたはグループを削除します。|
|[rejectedSender を追加する](../api/group_post_rejectedsenders.md) |[directoryObject](directoryobject.md)| rejectedSender コレクションに新しいユーザーまたはグループを追加します。|
|[rejectedSenders を一覧表示する](../api/group_list_rejectedsenders.md) |[directoryObject](directoryobject.md) コレクション| このグループの rejectedSenders リストに含まれるユーザーまたはグループの一覧を取得します。|
|[rejectedSender を削除する](../api/group_delete_rejectedsenders.md) |[directoryObject](directoryobject.md)| rejectedSender コレクションから新しいユーザーまたはグループを削除します。|
|[addFavorite](../api/group_addfavorite.md)|なし|現在のユーザーのお気に入りのグループ一覧にグループを追加します。Office 365 のグループのみをサポートします。|
|[removeFavorite](../api/group_removefavorite.md)|なし|現在のユーザーのお気に入りのグループ一覧からグループを削除します。Office 365 のグループのみをサポートします。|
|[subscribeByMail](../api/group_subscribebymail.md)|なし|isSubscribedByMail プロパティを **true** に設定します。現在のユーザーが電子メールの会話を受信できるようにします。Office 365 のグループのみをサポートします。|
|[unsubscribeByMail](../api/group_unsubscribebymail.md)|なし|isSubscribedByMail プロパティを **false** に設定します。現在のユーザーに対して電子メールでの会話の受信を無効にします。Office 365 のグループのみをサポートします。|
|[resetUnseenCount](../api/group_resetunseencount.md)|なし|現在のユーザーが最後の訪問以降見ていない、すべての投稿の unseenCount を 0 にリセットします。Office 365 のグループのみをサポートします。|


## <a name="properties"></a>プロパティ
| プロパティ       | 型    |説明|
|:---------------|:--------|:----------|
|allowExternalSenders|Boolean|既定値は **false** です。組織外部のユーザーがグループにメッセージを送信できるかどうかを示します。|
|autoSubscribeNewMembers|Boolean|既定値は **false** です。グループに追加された新しいメンバーが、電子メールの通知を受信するように自動的にサブスクライブされるかどうかを示します。グループの PATCH 要求でこのプロパティを設定できます。グループを作成する最初の POST 要求では設定しないでください。|
|description|String|グループに関するオプションの説明。 |
|displayName|String|グループの表示名。このプロパティは、グループの作成時の必須プロパティであり、更新時にクリアすることはできません。$filter および $orderby をサポートします。|
|groupTypes|String collection| 作成するグループの種類を指定します。使用可能な値は **Unified** (Office 365 のグループを作成する場合) または **DynamicMembership** (動的なグループを作成する場合) です。その他のグループの種類 (セキュリティが有効なグループやメールが有効なセキュリティ グループなど) の場合、このプロパティは設定しないでください。$filter をサポートします。|
|id|String|グループの一意の識別子。[directoryObject](directoryobject.md) から継承されます。キー。null 許容ではありません。読み取り専用です。|
|isSubscribedByMail|Boolean|既定値は **true** です。現在のユーザーが電子メールの会話を受信するように登録されているかどうかを示します。|
|メール|String|グループの SMTP アドレス (たとえば、"Serviceadmins@contoso.onmicrosoft.com")。読み取り専用です。$filter をサポートします。|
|mailEnabled|Boolean|メールが有効なグループであるかどうかを指定します。**securityEnabled** プロパティも **true** の場合、グループはメールが有効なセキュリティ グループになります。それ以外の場合は、Microsoft Exchange 配布グループになります。|
|mailNickname|String|グループの電子メール エイリアス。このプロパティは、グループの作成時に指定する必要があります。$filter をサポートします。|
|onPremisesLastSyncDateTime|DateTimeOffset|グループがオンプレミスのディレクトリと最後に同期した日時を示します。Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表し、必ず UTC 時間です。たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`読み取り専用です。$filter をサポートします。|
|onPremisesSecurityIdentifier|String|オンプレミスからクラウドに同期されたグループのオンプレミスのセキュリティ識別子 (SID) が含まれます。読み取り専用です。 |
|onPremisesSyncEnabled|Boolean|このグループがオンプレミスのディレクトリから同期される場合は **true**、このグループが最初にオンプレミスのディレクトリから同期されていて、今後は同期しない場合は **false**、このオブジェクトがオンプレミスのディレクトリから一度も同期されたことがない場合は **null**。読み取り専用です。$filter をサポートします。|
|proxyAddresses|String collection| 複数値プロパティのフィルター式には **any** 演算子が必要です。読み取り専用です。null 許容ではありません。$filter をサポートします。 |
|securityEnabled|Boolean|グループがセキュリティ グループであるかどうかを指定します。**mailEnabled** プロパティも true の場合、グループはメールが有効なセキュリティ グループになります。それ以外の場合は、セキュリティ グループになります。Office 365 グループの場合、**false** にする必要があります。$filter をサポートします。|
|unseenCount|Int32|現在のユーザーの最後のアクセス以降の投稿の非表示カウントです。|
|visibility|String| Office 365 グループの表示を指定します。使用可能な値は次のとおりです。**Private**、**Public**、または空 (**Public** として解釈されます)。|

## <a name="relationships"></a>リレーションシップ
| リレーションシップ | 型    |説明|
|:---------------|:--------|:----------|
|acceptedSenders|[directoryObject](directoryobject.md) コレクション|このグループで投稿または予定表のイベントを作成することが許可されているユーザーまたはグループの一覧。この一覧が空でない場合、ここに記載されているユーザーまたはグループだけが投稿を許可されます。|
|予定表|[calendar](calendar.md)|グループの予定表。読み取り専用です。|
|calendarView|[event](event.md) コレクション|予定表のカレンダー ビュー。読み取り専用です。|
|conversations|[conversation](conversation.md) コレクション|グループの会話。|
|createdOnBehalfOf|[directoryObject](directoryobject.md)| グループを作成したユーザー (またはアプリケーション)。注: ユーザーが管理者である場合、これは設定されません。読み取り専用です。|
|ドライブ|[drive](drive.md)|グループのドライブ。読み取り専用です。|
|events|[event](event.md) コレクション|グループの予定表イベント。|
|memberOf|[directoryObject](directoryobject.md) コレクション|このグループがメンバーとして含まれているグループ。HTTP メソッド:GET (すべてのグループでサポートされます)。読み取り専用です。Null 許容型。|
|members|[directoryObject](directoryobject.md) コレクション| このグループのメンバーであるユーザーとグループ。HTTP メソッド:GET (すべてのグループでサポートされます)、POST (Office 365 グループ、セキュリティ グループ、およびメールが有効なセキュリティ グループでサポートされます)、DELETE (Office 365 グループとセキュリティ グループでサポートされます)。Null 許容型。|
|owners|[directoryObject](directoryobject.md) コレクション|グループの所有者。所有者は、このオブジェクトの変更を許可されている管理者以外のユーザーです。10 人の所有者に制限されます。HTTP メソッド:GET (すべてのグループでサポートされます)、POST (Office 365 グループ、セキュリティ グループ、およびメールが有効なセキュリティ グループでサポートされます)、DELETE (Office 365 グループとセキュリティ グループでサポートされます)。Null 許容型。|
|写真|[profilePhoto](profilephoto.md)| グループのプロフィール写真 |
|rejectedSenders|[directoryObject](directoryobject.md) コレクション|このグループで投稿またはカレンダーのイベントを作成することが許可されていないグループの一覧。Null 許容型|
|スレッド|[conversationThread](conversationthread.md) コレクション| グループの会話スレッド。Null 許容型。|


## <a name="json-representation"></a>JSON 表記

以下は、リソースの JSON 表記です

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "acceptedSenders",
    "appRoleAssignments",
    "calendar",
    "calendarView",
    "conversations",
    "createdOnBehalfOf",
    "drive",
    "events",
    "memberOf",
    "members",
    "owners",
    "photo",
    "rejectedSenders",
    "threads"
  ],
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.group"
}-->

```json
{
  "allowExternalSenders": false,
  "autoSubscribeNewMembers": true,
  "description": "string",
  "displayName": "string",
  "groupTypes": ["string"],
  "id": "string (identifier)",
  "isSubscribedByMail": true,
  "mail": "string",
  "mailEnabled": true,
  "mailNickname": "string",
  "onPremisesLastSyncDateTime": "String (timestamp)",
  "onPremisesSecurityIdentifier": "string",
  "onPremisesSyncEnabled": true,
  "proxyAddresses": ["string"],
  "securityEnabled": true,
  "unseenCount": 1024,
  "visibility": "string",
  "acceptedSenders": [ { "@odata.type": "microsoft.graph.directoryObject"} ],
  "calendar": { "@odata.type": "microsoft.graph.calendar" },
  "calendarView": [{ "@odata.type": "microsoft.graph.event" }],
  "conversations": [ { "@odata.type": "microsoft.graph.conversation" }],
  "createdOnBehalfOf": { "@odata.type": "microsoft.graph.directoryObject" },
  "drive": { "@odata.type": "microsoft.graph.drive" },
  "events": [ { "@odata.type": "microsoft.graph.event" }],
  "memberOf": [ { "@odata.type": "microsoft.graph.directoryObject" } ],
  "members": [ { "@odata.type": "microsoft.graph.directoryObject" } ],
  "owners": [ { "@odata.type": "microsoft.graph.directoryObject" } ],
  "photo": { "@odata.type": "microsoft.graph.profilePhoto" },
  "rejectedSenders": [ { "@odata.type": "microsoft.graph.directoryObject" } ],
  "threads": [ { "@odata.type": "microsoft.graph.conversationThread" }]
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "group resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
