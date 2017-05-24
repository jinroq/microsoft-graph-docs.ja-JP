# <a name="user-resource-type"></a>ユーザー リソースの種類

Azure AD ユーザー アカウントを表します。[directoryObject](directoryobject.md) から継承します。

このリソースは以下をサポートしています。
- [拡張機能](../../../concepts/extensibility_overview.md)を使用して、カスタム プロパティに独自のデータを追加します。
- [デルタ](../api/user_delta.md)関数を提供することにより、[デルタ クエリ](../../../concepts/delta_query_overview.md)を使用して、増分の追加、削除、更新を追跡します。

## <a name="methods"></a>メソッド

| メソッド       | 戻り値の型  |説明|
|:---------------|:--------|:----------|
|[Get user](../api/user_get.md) | [user](user.md) |ユーザー オブジェクトのプロパティと関係を読み取ります。|
|[Update user](../api/user_update.md) | [user](user.md) |ユーザー オブジェクトを更新します。 |
|[Delete user](../api/user_delete.md) | None |ユーザー オブジェクトを削除します。 |
|[List messages](../api/user_list_messages.md) |[Message](message.md) collection| サインインしているユーザーのメールボックス内のすべてのメッセージを取得します。|
|[Create Message](../api/user_post_messages.md) |[Message](message.md)| メッセージ コレクションへの投稿により、新しいメッセージを作成します。|
|[List mailFolders](../api/user_list_mailfolders.md) |[MailFolder](mailfolder.md) collection| サインイン中のユーザーのルート フォルダーからメール フォルダー コレクションを取得します。 |
|[Create mailFolder](../api/user_post_mailfolders.md) |[MailFolder](mailfolder.md)| mailFolder コレクションへの投稿により、新しい MailFolder を作成します。|
|[sendMail](../api/user_sendmail.md)|None|要求本文に指定されたメッセージを送信します。|
|[List events](../api/user_list_events.md) |[Event](event.md) collection| ユーザーのメールボックス内のイベント オブジェクトの一覧を取得します。一覧には、単一インスタンスの会議と定期的なマスターが含まれています。|
|[Create event](../api/user_post_events.md) |[Event](event.md)| Event コレクションへの投稿によって、新しいイベントを作成します。|
|[List calendars](../api/user_list_calendars.md) |[Calendar](calendar.md) collection| 予定表オブジェクトのコレクションを取得します。|
|[Create calendar](../api/user_post_calendars.md) |[Calendar](calendar.md)| 予定表コレクションへの投稿により、新しい予定表を作成します。|
|[List calendarGroups](../api/user_list_calendargroups.md) |[CalendarGroup](calendargroup.md) collection| CalendarGroup オブジェクトのコレクションを取得します。|
|[Create calendarGroup](../api/user_post_calendargroups.md) |[CalendarGroup](calendargroup.md)| calendarGroups コレクションへの投稿により、新しい CalendarGroup を作成します。|
|[List calendarView](../api/user_list_calendarview.md) |[Event](event.md) collection| Event オブジェクトのコレクションを取得します。|
|[List contacts](../api/user_list_contacts.md) |[Contact](contact.md) collection| サインイン中のユーザーの既定の連絡先フォルダーから連絡先コレクションを取得します。|
|[Create Contact](../api/user_post_contacts.md) |[Contact](contact.md)| 連絡先コレクションに投稿することにより、新しい連絡先を作成します。|
|[List contactFolders](../api/user_list_contactfolders.md) |[ContactFolder](contactfolder.md) collection| サインイン中のユーザーの既定の連絡先フォルダー内の連絡先フォルダーのコレクションを取得します。|
|[Create ContactFolder](../api/user_post_contactfolders.md) |[ContactFolder](contactfolder.md)| contactFolder コレクションに投稿することにより、新しい ContactFolder を作成します。|
|[List directReports](../api/user_list_directreports.md) |[directoryObject](directoryobject.md) collection| そのユーザーの部下であるユーザーと連絡先を、directReports ナビゲーション プロパティから取得します。|
|[List manager](../api/user_list_manager.md) |[directoryObject](directoryobject.md) | そのユーザーの上司であるユーザーまたは連絡先を、マネージャー ナビゲーション プロパティから取得します。|
|[List memberOf](../api/user_list_memberof.md) |[directoryObject](directoryobject.md) collection| そのユーザーが直接のメンバーであるグループおよびディレクトリ ロールを、memberOf ナビゲーション プロパティから取得します。|
|[List ownedDevices](../api/user_list_owneddevices.md) |[directoryObject](directoryobject.md) collection| そのユーザーにより所有されているデバイスを、OwnedDevices ナビゲーション プロパティから取得します。|
|[List ownedObjects](../api/user_list_ownedobjects.md) |[directoryObject](directoryobject.md) collection| そのユーザーにより所有されているディレクトリ オブジェクトを、ownedObjects ナビゲーション プロパティから取得します。|
|[List registeredDevices](../api/user_list_registereddevices.md) |[directoryObject](directoryobject.md) collection| そのユーザーについて登録されているデバイスを、RegisteredDevices ナビゲーション プロパティから取得します。|
|[List createdObjects](../api/user_list_createdobjects.md) |[directoryObject](directoryobject.md) collection| そのユーザーにより作成されたディレクトリ オブジェクトを、createdObjects ナビゲーション プロパティから取得します。|
|[assignLicense](../api/user_assignlicense.md)|[user](user.md)|ユーザーのサブスクリプションを追加または削除します。サブスクリプションに関連付けられている特定のプランを有効または無効にすることもできます。|
|[licenseDetails を一覧表示する](../api/user_list_licensedetails.md) |[licenseDetails](licensedetails.md) コレクション| licenseDetails オブジェクトのコレクションを取得します。| 
|[checkMemberGroups](../api/user_checkmembergroups.md)|String collection|グループの一覧内のメンバーシップを確認します。チェックは推移的です。|
|[getMemberGroups](../api/user_getmembergroups.md)|String collection|ユーザーがメンバーであるすべてのグループを返します。チェックは推移的です。|
|[getMemberObjects](../api/user_getmemberobjects.md)|String collection| ユーザーがメンバーになっているすべてのグループとディレクトリ ロールを返します。チェックは推移的です。 |
|[reminderView](../api/user_reminderview.md)|[Reminder](reminder.md) collection|指定した開始時刻と終了時刻内の予定表のアラームの一覧を返します。|
|[delta](../api/user_delta.md)|user コレクション| ユーザーに対する増分の変更を取得します。 |
|**オープン拡張機能**| | |
|[オープン拡張機能を作成する](../api/opentypeextension_post_opentypeextension.md) |[openTypeExtension](opentypeextension.md)| オープン拡張機能を作成し、新規または既存のリソースにカスタム プロパティを追加します。|
|[オープン拡張機能を取得する](../api/opentypeextension_get.md) |[openTypeExtension](opentypeextension.md) コレクション| 拡張機能の名前で識別されるオープン拡張機能を取得します。|
|**スキーマ拡張機能**| | |
|[スキーマ拡張機能の値を追加する](../../../concepts/extensibility_schema_groups.md) || スキーマ拡張機能の定義を作成し、それを使用してカスタマイズされた種類のデータをリソースに追加します。|



## <a name="properties"></a>プロパティ

| プロパティ       | 型    |説明|
|:---------------|:--------|:----------|
|aboutMe|String|ユーザーが自分自身について記述する、フリー フォームのテキスト入力フィールド。|
|accountEnabled|Boolean| アカウントが有効な場合は **true**。そうでない場合は **false**。このプロパティは、ユーザーの作成時に必要です。$filter をサポートします。    |
|assignedLicenses|[assignedLicense](assignedlicense.md) collection|ユーザーに割り当てられているライセンス。null 許容ではありません。            |
|assignedPlans|[assignedPlan](assignedplan.md) collection|ユーザーに割り当てられているプラン。読み取り専用です。null 許容ではありません。 |
|birthday|DateTimeOffset|ユーザーの誕生日。Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表し、必ず UTC 時間です。たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`|
|businessPhones|String コレクション|ユーザーの電話番号。注:文字列コレクションですが、このプロパティに設定できるのは 1 つの数字のみです。|
|city|String|ユーザーがいる都市。$filter をサポートします。|
|country|String|ユーザーがいる国/地域。たとえば、「US (米国)」や「UK (英国)」です。$filter をサポートします。|
|department|String|ユーザーが働いている部門の名前。$filter をサポートします。|
|displayName|String|アドレス帳に表示されるユーザーの名前。これは通常、ユーザーの名前、ミドルネームのイニシャル、姓の組み合わせです。このプロパティは、ユーザーの作成時に必須になります。更新時にクリアすることはできません。$filter および $orderby をサポートします。|
|givenName|String|ユーザーの名。$filter をサポートします。|
|hireDate|DateTimeOffset|ユーザーの採用日付。Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表し、必ず UTC 時間です。たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`|
|id|String|ユーザーの一意の識別子。[directoryObject](directoryobject.md) から継承されます。キー。null 許容ではありません。読み取り専用です。|
|imAddresses|String コレクション|ユーザーのインスタント メッセージ ボイス オーバー IP (VOIP) セッション開始プロトコル (SIP) のアドレス。読み取り専用です。|
|interests|String collection|ユーザーが自分の関心事を記述する一覧。|
|jobTitle|String|ユーザーの役職。$filter をサポートします。|
|mail|String|ユーザーの SMTP アドレス (たとえば、"jeff@contoso.onmicrosoft.com")。読み取り専用。$filter をサポートします。|
|mailboxSettings|[mailboxSettings](mailboxsettings.md)|サインイン ユーザーのプライマリ メールボックスの設定。着信メッセージに対する自動応答を送信するための設定、ロケール、タイム ゾーンを [取得](../api/user_get_mailboxsettings.md) または [更新](../api/user_update_mailboxsettings.md) できます。|
|mailNickname|String|ユーザーの電子メール エイリアス。ユーザーの作成時に、このプロパティを指定する必要があります。$filter をサポートします。|
|mobilePhone|String|ユーザーの主な携帯電話の番号。|
|mySite|String|ユーザーの個人用サイトの URL。|
|officeLocation|String|ユーザーの勤務先の場所。|
|onPremisesImmutableId|String|このプロパティは、オンプレミスの Active Directory ユーザー アカウントを Azure AD ユーザー オブジェクトに関連付けるために使用します。Graph で新しいユーザー アカウントを作成するとき、ユーザーの **userPrincipalName** (UPN) プロパティにフェデレーション ドメインを使用する場合は、このプロパティを指定する必要があります。**重要:****$** と **_** の文字は、このプロパティを指定するときには使用できません。$filter をサポートします。                            |
|onPremisesLastSyncDateTime|DateTimeOffset|オブジェクトがオンプレミス ディレクトリと前回、同期された日時を示します。例："2013-02-16T03:04:54Z"Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表し、必ず UTC 時間です。たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`読み取り専用です。|
|onPremisesSecurityIdentifier|String|オンプレミスからクラウドに同期されたユーザーのオンプレミスのセキュリティ識別子 (SID) が含まれます。読み取り専用です。|
|onPremisesSyncEnabled|Boolean| このオブジェクトがオンプレミスのディレクトリから同期される場合は **true**、このオブジェクトが最初にオンプレミスのディレクトリから同期されていて、今後は同期しない場合は **false**、このオブジェクトがオンプレミスのディレクトリから 1 度も同期されたことがない場合は **null** (既定値)。読み取り専用 |
|passwordPolicies|String|ユーザーのパスワード ポリシーを指定します。この値は列挙値であり、可能な 1 つの値は "DisableStrongPassword" です。この場合は、既定のポリシーより脆弱なパスワードを指定できます。"DisablePasswordExpiration" を指定することもできます。2 つを一緒に指定することもできます。例:"DisablePasswordExpiration, DisableStrongPassword"|
|passwordProfile|[PasswordProfile](passwordprofile.md)|ユーザーのパスワード プロファイルを指定します。プロファイルには、ユーザーのパスワードが含まれています。このプロパティは、ユーザーの作成時に必要です。プロファイルにあるパスワードは、**passwordPolicies** プロパティによって指定されている最小要件を満たす必要があります。既定では、強力なパスワードが必要です。|
|pastProjects|String collection|ユーザーが過去のプロジェクトを列挙する一覧。|
|postalCode|String|ユーザーの住所の郵便番号。郵便番号は、ユーザーの国/地域に固有です。アメリカ合衆国では、この属性には、ZIP コードが含まれます。|
|preferredLanguage|String|ユーザーが設定する言語。ISO 639-1 コードに従う必要があります。たとえば "en-US" です。|
|preferredName|String|ユーザーが設定する名前。|
|provisionedPlans|[ProvisionedPlan](provisionedplan.md) collection|ユーザーのために用意されたプラン。読み取り専用です。null 許容ではありません。 |
|proxyAddresses|String collection|例:`["SMTP: bob@contoso.com", "smtp: bob@sales.contoso.com"]` 複数値プロパティのフィルター式には、**任意の**演算子が必要です。読み取り専用。null 許容ではありません。$filter をサポートします。          |
|responsibilities|String collection|ユーザーが自分の責任の範囲を列挙する一覧。|
|schools|String collection|ユーザーが在籍した学校を列挙する一覧。|
|skills|String collection|ユーザーが自分のスキルを列挙する一覧。|
|state|String|ユーザーの住所の都道府県。$filter をサポートします。|
|streetAddress|String|ユーザーの勤務先の番地。|
|surname|String|ユーザーの姓。$filter をサポートします。|
|usageLocation|String|2 文字の国コード (ISO 規格 3166)国におけるサービスの利用可能性を確認することが法的に義務付けられているため、ライセンスを割り当てられるユーザーには必須です。例:"US"、"JP"、"GB"null 許容ではありません。$filter をサポートします。|
|userPrincipalName|String|ユーザーのユーザー プリンシパル名 (UPN)。UPN は、インターネット標準 RFC 822 に基づいた、インターネット スタイルのユーザーのログイン名です。規則では、これはユーザーの電子メール名にマップされる必要があります。一般的な形式は alias@domain です。このドメインは、検証済みドメインのテナントのコレクション内に存在している必要があります。このプロパティは、ユーザーの作成時に必要です。テナントの検証済みのドメインには、[organization](organization.md) の **verifiedDomains** プロパティからアクセスできます。$filter および $orderby をサポートします。
|userType|String|ディレクトリ内のユーザーの種類を分類するために使用する文字列値 (“Member”、“Guest” など)。$filter をサポートします。          |

## <a name="relationships"></a>リレーションシップ

| リレーションシップ | 型    |説明|
|:---------------|:--------|:----------|
|calendar|[Calendar](calendar.md)|ユーザーの標準予定表。読み取り専用です。|
|calendarGroups|[CalendarGroup](calendargroup.md) collection|ユーザーの予定表グループ。読み取り専用です。Null 許容型。|
|calendarView|[Event](event.md) collection|予定表のカレンダー ビュー。読み取り専用です。Null 許容型。|
|calendars|[Calendar](calendar.md) collection|ユーザーの予定表。読み取り専用です。Null 許容型。|
|contactFolders|[ContactFolder](contactfolder.md) collection|ユーザーの連絡先フォルダー。読み取り専用です。Null 許容型。|
|contacts|[Contact](contact.md) collection|ユーザーの連絡先。読み取り専用です。Null 許容型。|
|createdObjects|[directoryObject](directoryobject.md) collection|ユーザーによって作成されたディレクトリ オブジェクト。読み取り専用です。Null 許容型。|
|directReports|[directoryObject](directoryobject.md) collection|そのユーザーの部下であるユーザーと連絡先。(マネージャー プロパティがこのユーザーに設定されている、ユーザーと連絡先。)読み取り専用です。Null 許容型。 |
|drive|[drive](drive.md)|ユーザーの OneDrive。読み取り専用です。|
|drives|[drive](drive.md) コレクション | このユーザーが使用できるドライブのコレクション。読み取り専用です。 |
|events|[Event](event.md) コレクション|ユーザーのイベント。既定は、既定の予定表でイベントを表示します。読み取り専用です。Null 許容型。|
|extensions|[extension](extension.md) コレクション|ユーザーに対して定義されているオープン拡張機能のコレクション。読み取り専用です。Null 許容型。|
|inferenceClassification | [inferenceClassification](inferenceClassification.md) | 明示的な指定に基づく、ユーザーのメッセージの関連性の分類。明示的な指定は、推定される関連性や重要性より優先されます。 |
|mailFolders|[MailFolder](mailfolder.md) collection| ユーザーのメール フォルダー。読み取り専用です。Null 許容型。|
|manager|[directoryObject](directoryobject.md)|このユーザーの上司であるユーザーまたは連絡先。読み取り専用です。(HTTP メソッド:GET、PUT、DELETE)|
|memberOf|[directoryObject](directoryobject.md) collection|ユーザーがメンバーになっているグループとディレクトリ ロール。読み取り専用です。Null 許容型。|
|messages|[Message](message.md) コレクション|メールボックスまたはフォルダー内のメッセージ。読み取り専用です。Null 許容型。|
|onenote|[OneNote](onenote.md)| 読み取り専用です。|
|ownedDevices|[directoryObject](directoryobject.md) collection|ユーザーが所有しているデバイス。読み取り専用です。Null 許容型。|
|ownedObjects|[directoryObject](directoryobject.md) collection|ユーザーが所有しているディレクトリ オブジェクト。読み取り専用です。Null 許容型。|
|photo|[profilePhoto](profilephoto.md)| ユーザーのプロフィール写真。読み取り専用です。|
|registeredDevices|[directoryObject](directoryobject.md) コレクション|ユーザーについて登録されているデバイス。読み取り専用です。Null 許容型。|
|sites|[site](site.md) コレクション | このユーザーが使用できるサイトのコレクション。読み取り専用です。 |

## <a name="json-representation"></a>JSON 表記

以下は、リソースの JSON 表記です

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "appRoleAssignments",
    "calendar",
    "calendarGroups",
    "calendarView",
    "calendars",
    "contactFolders",
    "contacts",
    "createdObjects",
    "directReports",
    "drive",
    "events",
    "extensions",
    "joinedGroups",
    "mailFolders",
    "manager",
    "memberOf",
    "messages",
    "oauth2PermissionGrants",
    "onenote",
    "ownedDevices",
    "ownedObjects",
    "photo",
    "sites",
    "registeredDevices"
  ],
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.user"
}-->

```json
{
  "aboutMe": "string",
  "accountEnabled": true,
  "assignedLicenses": [{"@odata.type": "microsoft.graph.assignedLicense"}],
  "assignedPlans": [{"@odata.type": "microsoft.graph.assignedPlan"}],
  "birthday": "String (timestamp)",
  "businessPhones": ["string"],
  "city": "string",
  "companyName": "string",
  "country": "string",
  "department": "string",
  "displayName": "string",
  "givenName": "string",
  "hireDate": "String (timestamp)",
  "id": "string (identifier)",
  "interests": ["string"],
  "jobTitle": "string",
  "mail": "string",
  "mailboxSettings": {"@odata.type": "microsoft.graph.mailboxSettings"},
  "mailNickname": "string",
  "mobilePhone": "string",
  "mySite": "string",
  "officeLocation": "string",
  "onPremisesImmutableId": "string",
  "onPremisesLastSyncDateTime": "String (timestamp)",
  "onPremisesSecurityIdentifier": "string",
  "onPremisesSyncEnabled": true,
  "passwordPolicies": "string",
  "passwordProfile": {"@odata.type": "microsoft.graph.passwordProfile"},
  "pastProjects": ["string"],
  "postalCode": "string",
  "preferredLanguage": "string",
  "preferredName": "string",
  "provisionedPlans": [{"@odata.type": "microsoft.graph.provisionedPlan"}],
  "proxyAddresses": ["string"],
  "responsibilities": ["string"],
  "schools": ["string"],
  "skills": ["string"],
  "state": "string",
  "streetAddress": "string",
  "surname": "string",
  "usageLocation": "string",
  "userPrincipalName": "string",
  "userType": "string",

  "calendar": { "@odata.type": "microsoft.graph.calendar" },
  "calendarGroups": [{ "@odata.type": "microsoft.graph.calendarGroup" }],
  "calendarView": [{ "@odata.type": "microsoft.graph.event" }],
  "calendars": [ {"@odata.type": "microsoft.graph.calendar"} ],
  "contacts": [ { "@odata.type": "microsoft.graph.contact" } ],
  "contactFolders": [ { "@odata.type": "microsoft.graph.contactFolder" } ],
  "createdObjects": [ { "@odata.type": "microsoft.graph.directoryObject" } ],
  "directReports": [ { "@odata.type": "microsoft.graph.directoryObject" } ],
  "drive": { "@odata.type": "microsoft.graph.drive" },
  "drives": [ { "@odata.type": "microsoft.graph.drive" } ],
  "events": [ { "@odata.type": "microsoft.graph.event" } ],
  "inferenceClassification": { "@odata.type": "microsoft.graph.inferenceClassification" },
  "mailFolders": [ { "@odata.type": "microsoft.graph.mailFolder" } ],
  "manager": { "@odata.type": "microsoft.graph.directoryObject" },
  "memberOf": [ { "@odata.type": "microsoft.graph.directoryObject" } ],
  "messages": [ { "@odata.type": "microsoft.graph.message" } ],
  "ownedDevices": [ { "@odata.type": "microsoft.graph.directoryObject" } ],
  "photo": { "@odata.type": "microsoft.graph.profilePhoto" },
  "registeredDevices": [ { "@odata.type": "microsoft.graph.directoryObject" } ],
  "sites": [ {"@odata.type": "microsoft.graph.site" }]
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
  "description": "user resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
