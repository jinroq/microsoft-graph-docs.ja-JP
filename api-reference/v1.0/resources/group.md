# <a name="group-resource-type"></a>group リソースの種類

Office 365 グループ、動的なグループ、セキュリティ グループのいずれかの Azure Active Directory (Azure AD) グループを表します。[directoryObject](directoryobject.md) から継承します。

このリソースは以下をサポートしています。

- [拡張機能](../../../concepts/extensibility_overview.md)を使用して、カスタム プロパティに独自のデータを追加します。
- [デルタ](../api/user_delta.md)関数を提供することにより、[デルタ クエリ](../../../concepts/delta_query_overview.md)を使用して、増分の追加、削除、更新を追跡します。


## <a name="methods"></a>メソッド

| メソッド       | 戻り値の型  |説明|
|:---------------|:--------|:----------|
|**グループの管理**| | |
|[グループを作成する](../api/group_post_groups.md) | [group](group.md) |新しいグループを作成します。 Office 365 グループ、動的なグループ、またはセキュリティ グループのいずれかにできます。|
|[グループを取得する](../api/group_get.md) | [group](group.md) |グループ オブジェクトのプロパティを読み取ります。|
|[グループを一覧表示する](../api/group_list.md) |[group](group.md) コレクション |グループ オブジェクトとそのプロパティを一覧表示します。|
|[グループを更新する](../api/group_update.md) | なし |グループ オブジェクトのプロパティを更新します。 |
|[グループを削除する](../api/group_delete.md) | なし |グループ オブジェクトを削除します。 |
|[delta](../api/group_delta.md)|group コレクション| グループに対する増分の変更を取得します。 |
|[groupLifecyclePolicies を一覧表示する](../api/group_list_grouplifecyclepolicies.md) |[groupLifecyclePolicy](grouplifecyclepolicy.md) コレクション| グループのライフサイクル ポリシーを一覧表示します。 |
|[更新する](../api/group_renew.md)|ブール値|グループの有効期限を更新します。 グループが更新されると、グループの有効期限はポリシーで定義された日数、延長されます。|
|[所有者を追加する](../api/group_post_owners.md) |なし| **owners** ナビゲーション プロパティ (セキュリティ グループおよびメールが有効なセキュリティ グループのみをサポート) に投稿することによってグループの新規所有者を追加します。|
|[所有者を一覧表示する](../api/group_list_owners.md) |[directoryObject](directoryobject.md) コレクション| **owners** ナビゲーション プロパティからグループの所有者を取得します。|
|[所有者を削除する](../api/group_delete_owners.md) | なし |**owners** ナビゲーション プロパティを使用して Office 365 のグループ、セキュリティ グループ、またはメールが有効なセキュリティ グループから所有者を削除します。|
|[メンバーを追加する](../api/group_post_members.md) |なし| **members** ナビゲーション プロパティ (セキュリティ グループおよびメールが有効なセキュリティ グループでのみサポートされます) に投稿することによってこのグループにユーザーまたはグループを追加します。|
|[メンバーを一覧表示する](../api/group_list_members.md) |[directoryObject](directoryobject.md) コレクション| **members** ナビゲーション プロパティからこのグループの直接のメンバーであるユーザーおよびグループを取得します。|
|[メンバーを削除する](../api/group_delete_members.md) | なし |**members** ナビゲーション プロパティを使用して Office 365 のグループ、セキュリティ グループ、またはメールが有効なセキュリティ グループからメンバーを削除できます。ユーザーや他のグループを削除できます。 |
|[checkMemberGroups](../api/group_checkmembergroups.md)|String コレクション|グループの一覧内のメンバーシップについてこのグループを確認します。この関数は、推移的です。|
|[getMemberGroups](../api/group_getmembergroups.md)|String コレクション|このグループがメンバーであるすべてのグループを返します。この関数は、推移的です。|
|[getMemberObjects](../api/group_getmemberobjects.md)|String コレクション|このグループがメンバーであるすべてのグループを返します。この関数は、推移的です。 |
|[設定を作成する](../api/groupsetting_post_groupsettings.md) | [groupSetting](groupsetting.md) |groupSettingTemplate に基づいて、設定オブジェクトを作成します。POST 要求は、テンプレートに定義されているすべての設定の settingValues を提供する必要があります。グループ固有のテンプレートにのみ、この操作を使用します。|
|[設定を取得する](../api/groupsetting_get.md) | [groupSetting](groupsetting.md) | 特定の設定オブジェクトのプロパティを参照します。 |
|[設定を一覧表示する](../api/groupsetting_list.md) | [groupSetting](groupsetting.md) コレクション | すべての設定オブジェクトのプロパティを一覧表示します。 |
|[設定を更新する](../api/groupsetting_update.md) | [groupSetting](groupsetting.md) | 設定オブジェクトを更新します。 |
|[設定を削除する](../api/groupsetting_delete.md) | なし | 設定オブジェクトを削除します。 |
|**予定表**| | |
|[イベントを作成する](../api/group_post_events.md) |[event](event.md)| event コレクションへの投稿によって、新しいイベントを作成します。|
|[イベントを取得する](../api/group_get_event.md) |[event](event.md)|event オブジェクトのプロパティを読み取ります。|
|[イベントを一覧表示する](../api/group_list_events.md) |[event](event.md) コレクション| event オブジェクトのコレクションを取得します。|
|[イベントを更新する](../api/group_update_event.md) |なし|event オブジェクトのプロパティを更新します。|
|[イベントを削除する](../api/group_delete_event.md) |なし|event オブジェクトを削除します。|
|[calendarView を一覧表示する](../api/group_list_calendarview.md) |[event](event.md) コレクション| 指定された時間枠のイベントのコレクションを取得します。|
|**会話**| | |
|[会話を作成する](../api/group_post_conversations.md) |[会話](conversation.md)| conversation コレクションに投稿して、新しい会話を作成します。|
|[会話を取得する](../api/group_get_conversation.md) |[会話](conversation.md)| conversation オブジェクトのプロパティを読み取ります。|
|[会話を一覧表示する](../api/group_list_conversations.md) |[conversation](conversation.md) コレクション| conversation オブジェクトのコレクションを取得します。|
|[会話を削除する](../api/group_delete_conversation.md) |なし|conversation オブジェクトを削除します。|
|[スレッドを取得する](../api/group_get_thread.md) |[conversationThread](conversationthread.md)| thread オブジェクトのプロパティを読み取ります。|
|[スレッドを一覧表示する](../api/group_list_threads.md) |[conversationThread](conversationthread.md) コレクション| グループのすべてのスレッドを取得します。|
|[スレッドを更新する](../api/group_update_thread.md) |なし| thread オブジェクトのプロパティを更新します。|
|[スレッドを削除する](../api/group_delete_thread.md) |なし| thread オブジェクトを削除します。|
|[acceptedSenders を一覧表示する](../api/group_list_acceptedsenders.md) |[directoryObject](directoryobject.md) コレクション| このグループの acceptedSenders リストに含まれるユーザーまたはグループの一覧を取得します。|
|[acceptedSender を追加する](../api/group_post_acceptedsenders.md) |[directoryObject](directoryobject.md)| acceptSenders コレクションにユーザーまたはグループを追加します。|
|[acceptedSender を削除する](../api/group_delete_acceptedsenders.md) |[directoryObject](directoryobject.md)| acceptedSenders コレクションからユーザーまたはグループを削除します。|
|[rejectedSenders を一覧表示する](../api/group_list_rejectedsenders.md) |[directoryObject](directoryobject.md) コレクション| このグループの rejectedSenders リストに含まれるユーザーまたはグループの一覧を取得します。|
|[rejectedSender を追加する](../api/group_post_rejectedsenders.md) |[directoryObject](directoryobject.md)| rejectedSender コレクションに新しいユーザーまたはグループを追加します。|
|[rejectedSender を削除する](../api/group_delete_rejectedsenders.md) |[directoryObject](directoryobject.md)| rejectedSender コレクションから新しいユーザーまたはグループを削除します。|
|[設定を作成する](../api/groupsetting_post_groupsettings.md) | [groupSetting](groupsetting.md) |groupSettingTemplate に基づいて、設定オブジェクトを作成します。POST 要求は、テンプレートに定義されているすべての設定の settingValues を提供する必要があります。グループ固有のテンプレートにのみ、この操作を使用します。|
|[設定を取得する](../api/groupsetting_get.md) | [groupSetting](groupsetting.md) | 特定の設定オブジェクトのプロパティを参照します。 |
|[設定を一覧表示する](../api/groupsetting_list.md) | [groupSetting](groupsetting.md) コレクション | すべての設定オブジェクトのプロパティを一覧表示します。 |
|[設定を更新する](../api/groupsetting_update.md) | なし | 設定オブジェクトを更新します。 |
|[設定を削除する](../api/groupsetting_delete.md) | なし | 設定オブジェクトを削除します。 |
|**オープン拡張機能**| | |
|[オープン拡張機能を作成する](../api/opentypeextension_post_opentypeextension.md) |[openTypeExtension](opentypeextension.md)| オープン拡張機能を作成し、新規または既存のリソースにカスタム プロパティを追加します。|
|[オープン拡張機能を取得する](../api/opentypeextension_get.md) |[openTypeExtension](opentypeextension.md) コレクション| 拡張機能の名前で識別されるオープン拡張機能を取得します。|
|**スキーマ拡張機能**| | |
|[スキーマ拡張機能の値を追加する](../../../concepts/extensibility_schema_groups.md) || スキーマ拡張機能の定義を作成し、それを使用してカスタムの型指定されたデータをリソースに追加します。|
|**その他のグループ リソース**| | |
|[写真を一覧表示する](../api/group_list_photos.md) |[profilePhoto](photo.md) コレクション| グループのプロファイル写真のコレクションを取得します。|
|[plannerPlans を一覧表示する](../api/plannergroup_list_plans.md) |[plannerPlan](plannerPlan.md) コレクション| グループが所有しているプランナーの計画を取得します。|
|**ユーザーの設定**| | |
|[addFavorite](../api/group_addfavorite.md)|なし|現在のユーザーのお気に入りのグループ一覧にグループを追加します。Office 365 のグループのみをサポートします。|
|[removeFavorite](../api/group_removefavorite.md)|なし|現在のユーザーのお気に入りのグループ一覧からグループを削除します。Office 365 のグループのみをサポートします。|
|[memberOf を一覧表示する](../api/group_list_memberof.md) |[directoryObject](directoryobject.md) コレクション| このユーザーが直接のメンバーであるグループおよび管理単位を、**memberOf** ナビゲーション プロパティから取得します。|
|[subscribeByMail](../api/group_subscribebymail.md)|なし|isSubscribedByMail プロパティを **true** に設定します。現在のユーザーが電子メールの会話を受信できるようにします。Office 365 のグループのみをサポートします。|
|[unsubscribeByMail](../api/group_unsubscribebymail.md)|なし|isSubscribedByMail プロパティを **false** に設定します。現在のユーザーに対して電子メールでの会話の受信を無効にします。Office 365 のグループのみをサポートします。|
|[resetUnseenCount](../api/group_resetunseencount.md)|なし|現在のユーザーが最後の訪問以降見ていない、すべての投稿の unseenCount を 0 にリセットします。Office 365 のグループのみをサポートします。|

## <a name="properties"></a>プロパティ
| プロパティ     | タイプ   |説明|
|:---------------|:--------|:----------|
|allowExternalSenders|ブール値|既定値は **false** です。組織外部のユーザーがグループにメッセージを送信できるかどうかを示します。|
|autoSubscribeNewMembers|ブール値|既定値は **false** です。グループに追加された新しいメンバーが、電子メールの通知を受信するように自動的にサブスクライブされるかどうかを示します。グループの PATCH 要求でこのプロパティを設定できます。グループを作成する最初の POST 要求では設定しないでください。|
|classification|文字列|グループの分類 (低、中、高程度の企業への影響など) を説明します。このプロパティの有効な値は、[テンプレート定義](groupsettingtemplate.md)に基づいて ClassificationList [設定](groupsetting.md)値を作成することによって定義されます。|
|createdDateTime|DateTimeOffset| グループ作成時のタイムスタンプです。 値は変更できず、グループが作成されると自動的に設定されます。 Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表し、常に UTC 時間です。 たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'` 読み取り専用。 |
|description|文字列|グループに関するオプションの説明。 |
|displayName|文字列|グループの表示名。このプロパティは、グループの作成時の必須プロパティであり、更新時にクリアすることはできません。$filter および $orderby をサポートします。|
|groupTypes|文字列コレクション| 作成するグループの種類を指定します。使用可能な値は **Unified** (Office 365 のグループを作成する場合) または **DynamicMembership** (動的なグループを作成する場合) です。その他のグループの種類 (セキュリティが有効なグループやメールが有効なセキュリティ グループなど) の場合、このプロパティは設定しないでください。$filter をサポートします。|
|ID|文字列|グループの一意の識別子。[directoryObject](directoryobject.md) から継承されます。キー。null 許容ではありません。読み取り専用です。|
|isSubscribedByMail|ブール値|既定値は **true** です。現在のユーザーが電子メールの会話を受信するように登録されているかどうかを示します。|
|mail|文字列|グループの SMTP アドレス (たとえば、"Serviceadmins@contoso.onmicrosoft.com")。読み取り専用です。$filter をサポートします。|
|mailEnabled|ブール値|メールが有効なグループであるかどうかを指定します。**securityEnabled** プロパティも **true** の場合、グループはメールが有効なセキュリティ グループになります。それ以外の場合は、Microsoft Exchange 配布グループになります。|
|mailNickname|文字列|組織内で一意のグループのメール エイリアス。このプロパティは、グループの作成時に指定する必要があります。$filter をサポートします。|
|onPremisesLastSyncDateTime|DateTimeOffset|グループがオンプレミスのディレクトリと最後に同期した日時を示します。Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表し、必ず UTC 時間です。たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`読み取り専用です。$filter をサポートします。|
|onPremisesProvisioningErrors|[onPremisesProvisioningError](onpremisesprovisioningerror.md) コレクション| 事前設定中に Microsoft の同期製品を使用するときのエラーです。 |
|onPremisesSecurityIdentifier|文字列|オンプレミスからクラウドに同期されたグループのオンプレミスのセキュリティ識別子 (SID) が含まれます。読み取り専用です。 |
|onPremisesSyncEnabled|ブール値|このグループがオンプレミスのディレクトリから同期される場合は **true**、このグループが最初にオンプレミスのディレクトリから同期されていて、今後は同期しない場合は **false**、このオブジェクトがオンプレミスのディレクトリから一度も同期されたことがない場合は **null**。読み取り専用です。$filter をサポートします。|
|proxyAddresses|String コレクション| 複数値プロパティのフィルター式には **any** 演算子が必要です。読み取り専用です。null 許容ではありません。$filter をサポートします。 |
|renewedDateTime|DateTimeOffset| グループの最後の更新時のタイムスタンプです。 これは直接変更することはできず、[更新サービス アクション](../api/group_renew.md)経由でのみ更新されます。 Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表し、常に UTC 時間です。 たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'` 読み取り専用。|
|securityEnabled|ブール値|グループがセキュリティ グループであるかどうかを指定します。**mailEnabled** プロパティも true の場合、グループはメールが有効なセキュリティ グループになります。それ以外の場合は、セキュリティ グループになります。Office 365 グループの場合、**false** にする必要があります。$filter をサポートします。|
|unseenCount|Int32|現在のユーザーの最後のアクセス以降の投稿の非表示カウントです。|
|表示 / 非表示|文字列| Office 365 のグループの表示 / 非表示を指定します。 指定できる値は、**プライベート**、 **パブリック**、 **HiddenMembership**、または空 (これは、 **パブリック**として解釈されます) です。|

## <a name="relationships"></a>リレーションシップ
| リレーションシップ | 型   |説明|
|:---------------|:--------|:----------|
|acceptedSenders|[directoryObject](directoryobject.md) コレクション|このグループで投稿または予定表のイベントを作成することが許可されているユーザーまたはグループの一覧。この一覧が空でない場合、ここに記載されているユーザーまたはグループだけが投稿を許可されます。|
|calendar|[カレンダー](calendar.md)|グループの予定表。読み取り専用です。|
|calendarView|[event](event.md) コレクション|予定表のカレンダー ビュー。読み取り専用です。|
|conversations|[conversation](conversation.md) コレクション|グループの会話。|
|createdOnBehalfOf|[directoryObject](directoryobject.md)| グループを作成したユーザー (またはアプリケーション)。注: ユーザーが管理者である場合、これは設定されません。読み取り専用です。|
|drive|[drive](drive.md)|グループの既定のドライブです。 読み取り専用。|
|drives|[drive](drive.md) コレクション|グループのドライブ。 読み取り専用。|
|events|[event](event.md) コレクション|グループの予定表イベント。|
|extensions|[extension](extension.md) コレクション|グループに対して定義されているオープン拡張機能のコレクション。読み取り専用です。Null 許容型。|
|groupLifecyclePolicies|[groupLifecyclePolicy](groupLifecyclePolicy.md) コレクション|このグループのライフ サイクル ポリシーのコレクションです。 読み取り専用。 Null 許容型。|
|memberOf|[directoryObject](directoryobject.md) コレクション|このグループがメンバーとして含まれているグループ。HTTP メソッド:GET (すべてのグループでサポートされます)。読み取り専用です。Null 許容型。|
|members|[directoryObject](directoryobject.md) コレクション| このグループのメンバーであるユーザーとグループ。HTTP メソッド:GET (すべてのグループでサポートされます)、POST (Office 365 グループ、セキュリティ グループ、およびメールが有効なセキュリティ グループでサポートされます)、DELETE (Office 365 グループとセキュリティ グループでサポートされます)。Null 許容型。|
|onenote|[Onenote](onenote.md)| 読み取り専用。|
|owners|[directoryObject](directoryobject.md) コレクション|グループの所有者。所有者は、このオブジェクトの変更を許可されている管理者以外のユーザーです。10 人の所有者に制限されます。HTTP メソッド:GET (すべてのグループでサポートされます)、POST (Office 365 グループ、セキュリティ グループ、およびメールが有効なセキュリティ グループでサポートされます)、DELETE (Office 365 グループとセキュリティ グループでサポートされます)。Null 許容型。|
|photo|[profilePhoto](profilephoto.md)| グループのプロファイル写真 |
|photos|[profilePhoto](profilephoto.md) コレクション| グループが所有しているプロファイル写真。読み取り専用です。Null 許容型。|
|planner|[plannerGroup](plannergroup.md)| 統合グループに存在する可能性がある Planner リソースのエントリ ポイント。|
|rejectedSenders|[directoryObject](directoryobject.md) コレクション|このグループで投稿またはカレンダーのイベントを作成することが許可されていないグループの一覧。Null 許容型|
|設定|[groupSetting](groupsetting.md) コレクション| 読み取り専用。Null 許容型。|
|sites|[site](site.md) コレクション|このグループ内の SharePoint サイトの一覧。/sites/root を使用して既定のサイトにアクセスします。|
|スレッド|[conversationThread](conversationthread.md) コレクション| グループの会話スレッド。Null 許容型。|

## <a name="json-representation"></a>JSON 表記

リソースの JSON 表記を次に示します。

<!--{
  "blockType": "resource",
  "baseType": "microsoft.graph.directoryObject",
  "openType": true,
  "optionalProperties": [
    "acceptedSenders",
    "appRoleAssignments",
    "calendar",
    "calendarView",
    "conversations",
    "createdOnBehalfOf",
    "drive",
    "events",
    "extensions",
    "memberOf",
    "members",
    "onenote",
    "owners",
    "photo",
    "rejectedSenders",
    "threads"
  ],
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.group",
  "@odata.annotations": [
    {
      "capabilities": {
        "changeTracking": true
      }
    },
    {
      "property": "acceptedSenders",
      "capabilities": {
        "changeTracking": false,
        "expandable": false,
        "searchable": false,
        "updatable": false
      }
    },
    {
      "property": "calendar",
      "capabilities": {
        "changeTracking": false,
        "deletable": false,
        "expandable": false,
        "insertable": false,
        "searchable": false,
        "updatable": false
      }
    },
    {
      "property": "calendarView",
      "capabilities": {
        "changeTracking": true,
        "deletable": false,
        "expandable": false,
        "insertable": false,
        "searchable": false,
        "updatable": false
      }
    },
    {
      "property": "conversations",
      "capabilities": {
        "changeTracking": false,
        "expandable": false,
        "updatable": false
      }
    },
    {
      "property": "events",
      "capabilities": {
        "changeTracking": false,
        "expandable": false,
        "searchable": false
      }
    },
    {
      "property": "photo",
      "capabilities": {
        "changeTracking": false,
        "deletable": false,
        "expandable": false,
        "insertable": false,
        "searchable": false
      }
    },
    {
      "property": "photos",
      "capabilities": {
        "changeTracking": false,
        "deletable": false,
        "expandable": false,
        "insertable": false,
        "searchable": false,
        "updatable": false
      }
    },
    {
      "property": "rejectedSenders",
      "capabilities": {
        "changeTracking": false,
        "expandable": false,
        "searchable": false,
        "updatable": false
      }
    },
    {
      "property": "threads",
      "capabilities": {
        "changeTracking": false,
        "expandable": false,
        "searchable": false,
        "updatable": false
      }
    }
  ]
}-->

```json
{
  "allowExternalSenders": false,
  "autoSubscribeNewMembers": true,
  "classification": "string",
  "createdDateTime": "String (timestamp)",
  "description": "string",
  "displayName": "string",
  "groupTypes": ["string"],
  "id": "string (identifier)",
  "isSubscribedByMail": true,
  "mail": "string",
  "mailEnabled": true,
  "mailNickname": "string",
  "onPremisesLastSyncDateTime": "String (timestamp)",
  "onPremisesProvisioningErrors": [{"@odata.type": "microsoft.graph.onPremisesProvisioningError"}],
  "onPremisesSecurityIdentifier": "string",
  "onPremisesSyncEnabled": true,
  "proxyAddresses": ["string"],
  "renewedDateTime": "String (timestamp)",
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
  "sites": [ { "@odata.type": "microsoft.graph.site" } ],
  "threads": [ { "@odata.type": "microsoft.graph.conversationThread" }]
}

```

## <a name="see-also"></a>関連項目

- [拡張機能を使用してカスタム データをリソースに追加する](../../../concepts/extensibility_overview.md)
- [オープン拡張機能を使用してカスタム データをユーザーに追加する](../../../concepts/extensibility_open_users.md)
- [スキーマ拡張機能を使用したグループへのカスタム データの追加](../../../concepts/extensibility_schema_groups.md)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "group resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
