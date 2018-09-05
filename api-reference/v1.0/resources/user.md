# <a name="user-resource-type"></a>ユーザー リソースの種類

Azure AD ユーザー アカウントを表します。[directoryObject](directoryobject.md) から継承します。

このリソースは以下をサポートしています。

- [拡張機能](../../../concepts/extensibility_overview.md)を使用して、カスタム プロパティに独自のデータを追加します。
- [デルタ](../api/user_delta.md)関数を提供することにより、[デルタ クエリ](../../../concepts/delta_query_overview.md)を使用して、増分の追加、削除、更新を追跡します。

## <a name="methods"></a>メソッド

| メソッド       | 戻り値の型  |説明|
|:---------------|:--------|:----------|
|[user のリスト](../api/user_list.md) |[user](user.md) コレクション| ユーザー オブジェクトのリストを取得します。|
|[ユーザーを作成する](../api/user_post_users.md) |[ユーザー](user.md)| 新しいユーザー オブジェクトを作成します。|
|[ユーザーを取得する](../api/user_get.md) | [ユーザー](user.md) |ユーザー オブジェクトのプロパティと関係を読み取ります。|
|[ユーザーを更新する](../api/user_update.md) | [ユーザー](user.md) |ユーザー オブジェクトを更新します。 |
|[ユーザーを削除する](../api/user_delete.md) | なし |ユーザー オブジェクトを削除します。 |
|[メッセージのリスト](../api/user_list_messages.md) |[Message](message.md) コレクション| サインインしているユーザーのメールボックス内のすべてのメッセージを取得します。|
|[メッセージを作成する](../api/user_post_messages.md) |[メッセージ](message.md)| メッセージ コレクションへの投稿により、新しいメッセージを作成します。|
|[mailFolders のリスト](../api/user_list_mailfolders.md) |[MailFolder](mailfolder.md) コレクション| サインイン中のユーザーのルート フォルダーからメール フォルダー コレクションを取得します。 |
|[mailFolder を作成する](../api/user_post_mailfolders.md) |[MailFolder](mailfolder.md)| mailFolder コレクションへの投稿により、新しい MailFolder を作成します。|
|[sendMail](../api/user_sendmail.md)|なし|要求本文に指定されたメッセージを送信します。|
|[イベントのリスト](../api/user_list_events.md) |[Event](event.md) コレクション| ユーザーのメールボックス内のイベント オブジェクトの一覧を取得します。一覧には、単一インスタンスの会議と定期的なマスターが含まれています。|
|[イベントを作成する](../api/user_post_events.md) |[イベント](event.md)| Event コレクションへの投稿によって、新しいイベントを作成します。|
|[カレンダーのリスト](../api/user_list_calendars.md) |[Calendar](calendar.md) コレクション| 予定表オブジェクトのコレクションを取得します。|
|[カレンダーを作成する](../api/user_post_calendars.md) |[カレンダー](calendar.md)| 予定表コレクションへの投稿により、新しい予定表を作成します。|
|[calendarGroups のリスト](../api/user_list_calendargroups.md) |[CalendarGroup](calendargroup.md) コレクション| CalendarGroup オブジェクトのコレクションを取得します。|
|[calendarGroup を作成する](../api/user_post_calendargroups.md) |[CalendarGroup](calendargroup.md)| calendarGroups コレクションへの投稿により、新しい CalendarGroup を作成します。|
|[calendarView のリスト](../api/user_list_calendarview.md) |[Event](event.md) コレクション| Event オブジェクトのコレクションを取得します。|
|[連絡先のリスト](../api/user_list_contacts.md) |[Contact](contact.md) コレクション| サインイン中のユーザーの既定の連絡先フォルダーから連絡先コレクションを取得します。|
|[連絡先を作成する](../api/user_post_contacts.md) |[連絡先](contact.md)| 連絡先コレクションに投稿することにより、新しい連絡先を作成します。|
|[contactFolders のリスト](../api/user_list_contactfolders.md) |[ContactFolder](contactfolder.md) コレクション| サインイン中のユーザーの既定の連絡先フォルダー内の連絡先フォルダーのコレクションを取得します。|
|[ContactFolder を作成する](../api/user_post_contactfolders.md) |[ContactFolder](contactfolder.md)| contactFolder コレクションに投稿することにより、新しい ContactFolder を作成します。|
|[directReports のリスト](../api/user_list_directreports.md) |[directoryObject](directoryobject.md) コレクション| そのユーザーの部下であるユーザーと連絡先を、directReports ナビゲーション プロパティから取得します。|
|[マネージャーのリスト](../api/user_list_manager.md) |[directoryObject](directoryobject.md) | そのユーザーの上司であるユーザーまたは連絡先を、マネージャー ナビゲーション プロパティから取得します。|
|[memberOf のリスト](../api/user_list_memberof.md) |[directoryObject](directoryobject.md) コレクション| そのユーザーが直接のメンバーであるグループおよびディレクトリ ロールを、memberOf ナビゲーション プロパティから取得します。|
|[ownedDevices のリスト](../api/user_list_owneddevices.md) |[directoryObject](directoryobject.md) コレクション| そのユーザーにより所有されているデバイスを、OwnedDevices ナビゲーション プロパティから取得します。|
|[ownedObjects のリスト](../api/user_list_ownedobjects.md) |[directoryObject](directoryobject.md) コレクション| そのユーザーにより所有されているディレクトリ オブジェクトを、ownedObjects ナビゲーション プロパティから取得します。|
|[registeredDevices のリスト](../api/user_list_registereddevices.md) |[directoryObject](directoryobject.md) コレクション| そのユーザーについて登録されているデバイスを、RegisteredDevices ナビゲーション プロパティから取得します。|
|[createdObjects のリスト](../api/user_list_createdobjects.md) |[directoryObject](directoryobject.md) コレクション| そのユーザーにより作成されたディレクトリ オブジェクトを、createdObjects ナビゲーション プロパティから取得します。|
|[assignLicense](../api/user_assignlicense.md)|[ユーザー](user.md)|ユーザーのサブスクリプションを追加または削除します。また、サブスクリプションに関連付けられている特定のプランを有効または無効にすることもできます。|
|[licenseDetails を一覧表示する](../api/user_list_licensedetails.md) |[licenseDetails](licensedetails.md) コレクション| licenseDetails オブジェクトのコレクションを取得します。|
|[checkMemberGroups](../api/user_checkmembergroups.md)|String コレクション|グループの一覧内のメンバーシップを確認します。チェックは推移的です。|
|[getMemberGroups](../api/user_getmembergroups.md)|String コレクション|ユーザーがメンバーであるすべてのグループを返します。チェックは推移的です。|
|[getMemberObjects](../api/user_getmemberobjects.md)|String コレクション| ユーザーがメンバーになっているすべてのグループとディレクトリ ロールを返します。チェックは推移的です。 |
|[reminderView](../api/user_reminderview.md)|[Reminder](reminder.md) コレクション|指定した開始時刻と終了時刻内の予定表のアラームの一覧を返します。|
|[デルタ](../api/user_delta.md)|user コレクション| ユーザーに対する増分の変更を取得します。 |
|**オープン拡張機能**| | |
|[オープン拡張機能を作成する](../api/opentypeextension_post_opentypeextension.md) |[openTypeExtension](opentypeextension.md)| オープン拡張機能を作成し、新規または既存のリソースにカスタム プロパティを追加します。|
|[オープン拡張機能を取得する](../api/opentypeextension_get.md) |[openTypeExtension](opentypeextension.md) コレクション| 拡張機能の名前で識別されるオープン拡張機能を取得します。|
|**スキーマ拡張機能**| | |
|[スキーマ拡張機能の値を追加する](../../../concepts/extensibility_schema_groups.md) || スキーマ拡張機能の定義を作成し、それを使用してカスタマイズされた種類のデータをリソースに追加します。|

## <a name="properties"></a>プロパティ

| プロパティ       | タイプ    |説明|
|:---------------|:--------|:----------|
|aboutMe|文字列|ユーザーが自分自身について記述する、フリー フォームのテキスト入力フィールド。|
|accountEnabled|ブーリアン| アカウントが有効な場合は **true**。そうでない場合は **false**。このプロパティは、ユーザーの作成時に必要です。$filter をサポートします。    |
|ageGroup|文字列|ユーザーの年齢グループを設定します。 指定できる値は、`null`、 `minor`、 `notAdult` 、`adult` です。 詳細については [法定年齢グループのプロパティの定義](#legal-age-group-property-definitions) を参照してください。 |
|assignedLicenses|[assignedLicense](assignedlicense.md) コレクション|ユーザーに割り当てられているライセンス。null 許容ではありません。            |
|assignedPlans|[assignedPlan](assignedplan.md) コレクション|ユーザーに割り当てられているプラン。読み取り専用です。null 許容ではありません。 |
|誕生日|DateTimeOffset|ユーザーの誕生日。Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表し、必ず UTC 時間です。たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。 `'2014-01-01T00:00:00Z'`|
|businessPhones|String コレクション|ユーザーの電話番号。注:文字列コレクションですが、このプロパティに設定できるのは 1 つの数字のみです。|
|都市|文字列|ユーザーがいる都市。$filter をサポートします。|
|companyName| 文字列 | ユーザーが関連付けられている会社名。 読み取り専用です。
|consentProvidedForMinor|文字列|未成年者の同意が得られたかどうかを設定します。 指定できる値は、`null`、 `granted`、 `denied` 、`notRequired` です。 詳細については [法定年齢グループのプロパティの定義](#legal-age-group-property-definitions) を参照してください。|
|country|文字列|ユーザーがいる国/地域。たとえば、「US (米国)」や「UK (英国)」です。$filter をサポートします。|
|部署|文字列|ユーザーが働いている部門の名前。$filter をサポートします。|
|displayName|文字列|アドレス帳に表示されるユーザーの名前。これは通常、ユーザーの名前、ミドルネームのイニシャル、姓の組み合わせです。このプロパティは、ユーザーの作成時に必須になります。更新時にクリアすることはできません。$filter および $orderby をサポートします。|
|givenName|文字列|ユーザーの名。$filter をサポートします。|
|hireDate|DateTimeOffset|ユーザーの採用日付。Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表し、必ず UTC 時間です。たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。 `'2014-01-01T00:00:00Z'`|
|id|文字列|ユーザーの一意の識別子。[directoryObject](directoryobject.md) から継承されます。キー。null 許容ではありません。読み取り専用です。|
|imAddresses|String コレクション|ユーザーのインスタント メッセージ ボイス オーバー IP (VOIP) セッション開始プロトコル (SIP) のアドレス。読み取り専用です。|
|興味関心|String コレクション|ユーザーが自分の関心事を記述する一覧。|
|jobTitle|文字列|ユーザーの役職。$filter をサポートします。|
|legalAgeGroupClassification|文字列| ユーザーの法定年齢グループを決定するために、エンタープライズ アプリケーションで使用されます。 このプロパティは、読み取り専用で、`ageGroup` プロパティと `consentProvidedForMinor` プロパティに基づいて計算されます。 指定できる値は、`null`、 `minorWithOutParentalConsent`、 `minorWithParentalConsent` 、`minorNoParentalConsentRequired`、`notAdult`、`adult`  です。 詳細については、[法定年齢グループのプロパティの定義](#legal-age-group-property-definitions) を参照してください。|
|mail|文字列|ユーザーの SMTP アドレス (たとえば、"jeff@contoso.onmicrosoft.com")。読み取り専用。$filter をサポートします。|
|mailboxSettings|[mailboxSettings](mailboxsettings.md)|サインイン ユーザーのプライマリ メールボックスの設定。着信メッセージに対する自動応答を送信するための設定、ロケール、タイム ゾーンを [取得](../api/user_get_mailboxsettings.md) または [更新](../api/user_update_mailboxsettings.md) できます。|
|mailNickname|文字列|ユーザーの電子メール エイリアス。ユーザーの作成時に、このプロパティを指定する必要があります。$filter をサポートします。|
|mobilePhone|文字列|ユーザーの主な携帯電話の番号。|
|mySite|文字列|ユーザーの個人用サイトの URL。|
|officeLocation|文字列|ユーザーの勤務先の場所。|
|onPremisesDomainName|文字列| 内部設置型の `domainFQDN` が含まれています。また、内部設置型のディレクトリから同期された dnsDomainName を呼び出します。 プロパティは、内部設置型のディレクトリを  Azure AD Connect 経由で直接 Azure Active Directory に同期しているお客様に対してのみ設定されます。 読み取り専用です。 |
|onPremisesExtensionAttributes|[OnPremisesExtensionAttributes](onpremisesextensionattributes.md)|ユーザーの extensionAttributes 1-15 を含みます。 個々 の拡張属性は、選択もフィルターも不可能なことに注意してください。  `onPremisesSyncEnabled` ユーザーでは、このプロパティのセットは内部設置型をマスタとし、読み取り専用となります。 クラウドのみのユーザー (`onPremisesSyncEnabled`が falseの場合) では、これらのプロパティは作成時または更新時に設定されることがあります。 |
|onPremisesImmutableId|文字列|このプロパティは、オンプレミスの Active Directory ユーザー アカウントを Azure AD ユーザー オブジェクトに関連付けるために使用します。Graph で新しいユーザー アカウントを作成するとき、ユーザーの **userPrincipalName** (UPN) プロパティにフェデレーション ドメインを使用する場合は、このプロパティを指定する必要があります。**重要:****$** と **_** の文字は、このプロパティを指定するときには使用できません。$filter をサポートします。                            |
|onPremisesLastSyncDateTime|DateTimeOffset|オブジェクトがオンプレミス ディレクトリと前回、同期された日時を示します。例："2013-02-16T03:04:54Z"Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表し、必ず UTC 時間です。たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`読み取り専用です。|
|onPremisesProvisioningErrors|[onPremisesProvisioningError](onpremisesprovisioningerror.md) コレクション| 事前設定中に Microsoft の同期製品を使用するときのエラーです。 |
|onPremisesSamAccountName|文字列| 内部設置型のディレクトリから同期された、内部設置型の `samAccountName` が含まれています。 プロパティは、内部設置型のディレクトリを  Azure AD Connect 経由で直接 Azure Active Directory に同期しているお客様に対してのみ設定されます。 読み取り専用です。 |
|onPremisesSecurityIdentifier|文字列|オンプレミスからクラウドに同期されたユーザーのオンプレミスのセキュリティ識別子 (SID) が含まれます。読み取り専用です。|
|onPremisesSyncEnabled|ブーリアン| このオブジェクトがオンプレミスのディレクトリから同期される場合は **true**、このオブジェクトが最初にオンプレミスのディレクトリから同期されていて、今後は同期しない場合は **false**、このオブジェクトがオンプレミスのディレクトリから 1 度も同期されたことがない場合は **null** (既定値)。読み取り専用 |
|onPremisesUserPrincipalName|文字列| 内部設置型のディレクトリから同期された、内部設置型の `userPrincipalName` が含まれています。 プロパティは、内部設置型のディレクトリを  Azure AD Connect 経由で直接 Azure Active Directory に同期しているお客様に対してのみ設定されます。 読み取り専用です。 |
|passwordPolicies|文字列|ユーザーのパスワード ポリシーを指定します。この値は列挙値であり、可能な 1 つの値は "DisableStrongPassword" です。この場合は、既定のポリシーより脆弱なパスワードを指定できます。"DisablePasswordExpiration" を指定することもできます。2 つを一緒に指定することもできます。例:"DisablePasswordExpiration, DisableStrongPassword"|
|passwordProfile|[PasswordProfile](passwordprofile.md)|ユーザーのパスワード プロファイルを指定します。プロファイルには、ユーザーのパスワードが含まれています。このプロパティは、ユーザーの作成時に必要です。プロファイルにあるパスワードは、**passwordPolicies** プロパティによって指定されている最小要件を満たす必要があります。既定では、強力なパスワードが必要です。|
|pastProjects|String コレクション|ユーザーが過去のプロジェクトを列挙する一覧。|
|postalCode|文字列|ユーザーの住所の郵便番号。郵便番号は、ユーザーの国/地域に固有です。アメリカ合衆国では、この属性には、ZIP コードが含まれます。|
|preferredLanguage|文字列|ユーザーが設定する言語。ISO 639-1 コードに従う必要があります。たとえば "en-US" です。|
|preferredName|文字列|ユーザーが設定する名前。|
|provisionedPlans|[ProvisionedPlan](provisionedplan.md) コレクション|ユーザーのために用意されたプラン。読み取り専用です。null 許容ではありません。 |
|proxyAddresses|String コレクション|例:`["SMTP: bob@contoso.com", "smtp: bob@sales.contoso.com"]` 複数値プロパティのフィルター式には、**任意の**演算子が必要です。読み取り専用。null 許容ではありません。$filter をサポートします。          |
|責任|String コレクション|ユーザーが自分の責任の範囲を列挙する一覧。|
|学歴|String コレクション|ユーザーが在籍した学校を列挙する一覧。|
|スキル|String コレクション|ユーザーが自分のスキルを列挙する一覧。|
|都道府県|文字列|ユーザーの住所の都道府県。$filter をサポートします。|
|streetAddress|文字列|ユーザーの勤務先の番地。|
|姓|文字列|ユーザーの姓。$filter をサポートします。|
|usageLocation|文字列|2 文字の国コード (ISO 規格 3166)国におけるサービスの利用可能性を確認することが法的に義務付けられているため、ライセンスを割り当てられるユーザーには必須です。例:"US"、"JP"、"GB"null 許容ではありません。$filter をサポートします。|
|userPrincipalName|文字列|ユーザーのユーザー プリンシパル名 (UPN)。UPN は、インターネット標準 RFC 822 に基づいた、インターネット スタイルのユーザーのログイン名です。規則では、これはユーザーの電子メール名にマップされる必要があります。一般的な形式は alias@domain です。このドメインは、検証済みドメインのテナントのコレクション内に存在している必要があります。このプロパティは、ユーザーの作成時に必要です。テナントの検証済みのドメインには、[organization](organization.md) の **verifiedDomains** プロパティからアクセスできます。$filter および $orderby をサポートします。
|userType|文字列|ディレクトリ内のユーザーの種類を分類するために使用する文字列値 (“Member”、“Guest” など)。$filter をサポートします。          |

### <a name="legal-age-group-property-definitions"></a>法定年齢グループのプロパティの定義

このセクションでは、Azure AD の管理者とエンタープライズ アプリケーションの開発者が、年齢に関連する規制を満たすために、3 つの年齢グループのプロパティ (`legalAgeGroupClassification`、 `ageGroup` および `consentProvidedForMinor`) をどのように使用するかを説明します。

例: キャメロンは、イギリスのホリーポートで、小学校のディレクトリ管理者をしています。 学年の初めに、キャメロンは、イギリスの年齢に関する規制に基づいて、未成年者の親から同意を得るための同意書を使用します。 親から同意を得ることで、未成年者のアカウントをホリーポートの学校が使用できるほか、マイクロソフトのアプリケーションで使用できます。 キャメロンは、すべてのアカウントを作成し、ageGroup を「未成年」に設定し、consentProvidedForMinor を「許可」に設定します。 そうすることで、キャメロンの生徒が使用するアプリケーションで、未成年者に不適切な機能を無効にできます。

#### <a name="legal-age-group-classification"></a>法定年齢グループの分類

この読み取り専用プロパティは、法定年齢グループに基づいてユーザーを適切に処理するために、エンタープライズ アプリケーションの開発者が使用します。 このプロパティは、ユーザーの `ageGroup` プロパティと `consentProvidedForMinor` のプロパティに基づいて計算されます。

| 値    | #  |説明|
|:---------------|:--------|:----------|
|null|0|既定値 "`ageGroup` なし" がユーザーに設定されています。|
|minorWithoutParentalConsent |1|(将来使用するために予約されています)|
|minorWithParentalConsent|2| ユーザーは、自分の国または地域の年齢に関連する規制に基づいて、未成年者と見なされ、アカウントの管理者が親か保護者から適切な同意を得ます。|
|adult|3|ユーザーは、自分の国または地域の年齢に関連する規制に基づいて成人と見なされます。|
|notAdult|4|ユーザーは、その他の年齢に関する規制のある国または地域 (アメリカ、イギリス、EU、韓国など) の出身で、ユーザーは (国または地域での規定通り) 未成年と成人の間の年齢です。 通常、規制対象国では、10 代の若者は `notAdult` と見なされます。|
|minorNoParentalConsentRequired|5|ユーザーは未成年者ですが、年齢に関する規制のない国または地域の出身です。|

#### <a name="age-group-and-minor-consent"></a>年齢グループおよび未成年者の同意

年齢グループ プロパティと未成年者の同意プロパティはオプション プロパティで、ユーザーの国または地域で定められている年齢に関する規制ルールに基づいて、アカウントが正しく使用されるように、Azure AD の管理者が使用します。

#### <a name="agegroup-property"></a>ageGroup プロパティ

| 値    | #  |説明|
|:---------------|:--------|:----------|
|null|0|既定値 "`ageGroup` なし" がユーザーに設定されています。|
|minor|1|ユーザーは未成年だと思われます。|
|notAdult|2|ユーザーは、法定規制のある国 (アメリカ、イギリス、EU、または韓国) の出身で、ユーザーの年齢は (国指定の) 子供の年齢の上限を超えており、(国や地域に基づく規制で定められた) 成人年齢の下限よりも低い年齢です。 そのため、基本的に、規制対象国では 10 代の若者は `notAdult` と見なされます。|
|adult|3|ユーザーは、大人として扱われる必要があります。|

#### <a name="consentprovidedforminor-property"></a>consentProvidedForMinor プロパティ

| 値    | #  |説明|
|:---------------|:--------|:----------|
|null|0|既定値 "`consentProvidedForMinor` なし" がユーザーに設定されています。|
|granted|1|アカウントのユーザーの同意を受けています。|
|denied|2|アカウントのユーザーの同意を得ていません。|
|不要|3|ユーザーは、同意を必要としない国や地域の出身です。|
 
## <a name="relationships"></a>関係

| リレーションシップ | 型   |説明|
|:---------------|:--------|:----------|
|アクティビティ|[userActivity](projectrome_activity.md) コレクション|デバイス間でのユーザーのアクティビティです。 読み取り専用です。 Null 許容型。|
|calendar|[カレンダー](calendar.md)|ユーザーの標準予定表。読み取り専用です。|
|calendarGroups|[CalendarGroup](calendargroup.md) コレクション|ユーザーの予定表グループ。読み取り専用です。Null 許容型。|
|calendarView|[Event](event.md) コレクション|予定表のカレンダー ビュー。読み取り専用です。Null 許容型。|
|カレンダー|[Calendar](calendar.md) コレクション|ユーザーの予定表。読み取り専用です。Null 許容型。|
|contactFolders|[ContactFolder](contactfolder.md) コレクション|ユーザーの連絡先フォルダー。読み取り専用です。Null 許容型。|
|連絡先|[Contact](contact.md) コレクション|ユーザーの連絡先。読み取り専用です。Null 許容型。|
|createdObjects|[directoryObject](directoryobject.md) コレクション|ユーザーによって作成されたディレクトリ オブジェクト。読み取り専用です。Null 許容型。|
|directReports|[directoryObject](directoryobject.md) コレクション|そのユーザーの部下であるユーザーと連絡先。(マネージャー プロパティがこのユーザーに設定されている、ユーザーと連絡先。)読み取り専用です。Null 許容型。 |
|ドライブ|[ドライブ](drive.md)|ユーザーの OneDrive。読み取り専用です。|
|drives|[drive](drive.md) コレクション| このユーザーが使用できるドライブのコレクション。読み取り専用です。 |
|イベント|[Event](event.md) コレクション|ユーザーのイベント。既定は、既定の予定表でイベントを表示します。読み取り専用です。Null 許容型。|
|拡張機能|[extension](extension.md) コレクション|ユーザーに対して定義されているオープン拡張機能のコレクション。読み取り専用です。Null 許容型。|
|inferenceClassification | [inferenceClassification](inferenceClassification.md) | 明示的な指定に基づく、ユーザーのメッセージの関連性の分類。明示的な指定は、推定される関連性や重要性より優先されます。 |
|licenseDetails|[licenseDetails](licensedetails.md) コレクション|このユーザーのライセンス詳細情報のコレクションです。 Null 許容型。|
|mailFolders|[MailFolder](mailfolder.md) コレクション| ユーザーのメール フォルダー。読み取り専用です。Null 許容型。|
|マネージャー|[directoryObject](directoryobject.md)|このユーザーの上司であるユーザーまたは連絡先。読み取り専用です。(HTTP メソッド:GET、PUT、DELETE)|
|memberOf|[directoryObject](directoryobject.md) コレクション|ユーザーがメンバーになっているグループとディレクトリ ロール。読み取り専用です。Null 許容型。|
|メッセージ|[Message](message.md) コレクション|メールボックスまたはフォルダー内のメッセージ。読み取り専用です。Null 許容型。|
|onenote|[Onenote](onenote.md)| 読み取り専用です。|
|outlook|[outlookUser](outlookuser.md)| 読み取り専用です。|
|ownedDevices|[directoryObject](directoryobject.md) コレクション|ユーザーが所有しているデバイス。読み取り専用です。Null 許容型。|
|ownedObjects|[directoryObject](directoryobject.md) コレクション|ユーザーが所有しているディレクトリ オブジェクト。読み取り専用です。Null 許容型。|
|people|[person](person.md) コレクション| ユーザーに関連する人。 読み取り専用です。 Null 許容型。
|photo|[profilePhoto](profilephoto.md)| ユーザーのプロフィール写真。読み取り専用です。|
|planner|[plannerUser](planneruser.md)| ユーザー用に存在する可能性のあるプランナー リソースへのエントリ ポイントです。 読み取り専用です。|
|registeredDevices|[directoryObject](directoryobject.md) コレクション|ユーザーについて登録されているデバイス。読み取り専用です。Null 許容型。|

## <a name="json-representation"></a>JSON 表記

以下は、リソースの JSON 表記です

<!--{
  "blockType": "resource",
  "baseType": "microsoft.graph.directoryObject",
  "openType": true,
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
    "registeredDevices"
  ],
  "@odata.type": "microsoft.graph.user",
  "@odata.annotations": [
    {
      "capabilities": {
        "changeTracking": true
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
      "property": "calendarGroups",
      "capabilities": {
        "changeTracking": false,
        "expandable": false,
        "searchable": false
      }
    },
    {
      "property": "calendars",
      "capabilities": {
        "changeTracking": false,
        "expandable": false,
        "searchable": false
      }
    },
    {
      "property": "calendarView",
      "capabilities": {
        "changeTracking": true,
        "deletable": false,
        "expandable": true,
        "insertable": false,
        "navigability": "single",
        "searchable": false,
        "updatable": false
      }
    },
    {
      "property": "contactFolders",
      "capabilities": {
        "changeTracking": true,
        "expandable": false,
        "searchable": false
      }
    },
    {
      "property": "contacts",
      "capabilities": {
        "changeTracking": true,
        "expandable": false
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
      "property": "inferenceClassification",
      "capabilities": {
        "changeTracking": false,
        "deletable": false,
        "expandable": false,
        "insertable": false,
        "searchable": false
      }
    },
    {
      "property": "mailFolders",
      "capabilities": {
        "changeTracking": true,
        "expandable": false,
        "searchable": false
      }
    },
    {
      "property": "messages",
      "capabilities": {
        "changeTracking": false,
        "expandable": false
      }
    },
    {
      "property": "people",
      "capabilities": {
        "changeTracking": false,
        "deletable": false,
        "expandable": false,
        "insertable": false,
        "updatable": false
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
    }
  ]
}-->

```json
{
  "aboutMe": "string",
  "accountEnabled": true,
  "ageGroup": "string",
  "assignedLicenses": [{"@odata.type": "microsoft.graph.assignedLicense"}],
  "assignedPlans": [{"@odata.type": "microsoft.graph.assignedPlan"}],
  "birthday": "String (timestamp)",
  "businessPhones": ["string"],
  "city": "string",
  "companyName": "string",
  "consentProvidedForMinor": "string",
  "country": "string",
  "department": "string",
  "displayName": "string",
  "givenName": "string",
  "hireDate": "String (timestamp)",
  "id": "string (identifier)",
  "imAddresses": ["string"],
  "interests": ["string"],
  "jobTitle": "string",
  "legalAgeGroupClassification": "string",
  "mail": "string",
  "mailboxSettings": {"@odata.type": "microsoft.graph.mailboxSettings"},
  "mailNickname": "string",
  "mobilePhone": "string",
  "mySite": "string",
  "officeLocation": "string",
  "onPremisesDomainName": "string",
  "onPremisesExtensionAttributes": {"@odata.type": "microsoft.graph.onPremisesExtensionAttributes"},
  "onPremisesImmutableId": "string",
  "onPremisesLastSyncDateTime": "String (timestamp)",
  "onPremisesProvisioningErrors": [{"@odata.type": "microsoft.graph.onPremisesProvisioningError"}],
  "onPremisesSamAccountName": "string",
  "onPremisesSecurityIdentifier": "string",
  "onPremisesSyncEnabled": true,
  "onPremisesUserPrincipalName": "string",
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
  "outlook": { "@odata.type": "microsoft.graph.outlookUser" },
  "ownedDevices": [ { "@odata.type": "microsoft.graph.directoryObject" } ],
  "ownedObjects": [ { "@odata.type": "microsoft.graph.directoryObject" } ],
  "photo": { "@odata.type": "microsoft.graph.profilePhoto" },
  "registeredDevices": [ { "@odata.type": "microsoft.graph.directoryObject" } ]
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
