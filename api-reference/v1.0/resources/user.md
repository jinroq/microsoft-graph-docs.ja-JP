---
title: user リソースの種類
description: Azure AD ユーザー アカウントを表します。directoryObject から継承します。
author: dkershaw10
localization_priority: Priority
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: d0a4f11a1dd9db580ba5c3a5f9a2981cd21fd157
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36033517"
---
# <a name="user-resource-type"></a>user リソースの種類

Azure AD ユーザー アカウントを表します。[directoryObject](directoryobject.md) から継承します。

このリソースは以下をサポートしています。

- [拡張機能](/graph/extensibility-overview)として、カスタム プロパティに独自のデータを追加します。
- [変更通知](/graph/webhooks)を受信します。
- [デルタ](../api/user-delta.md)関数を提供することにより、[デルタ クエリ](/graph/delta-query-overview)を使用して、増分の追加、削除、更新を追跡します。

## <a name="methods"></a>メソッド

| メソッド       | 戻り値の型  |説明|
|:---------------|:--------|:----------|
|[user のリスト](../api/user-list.md) |[user](user.md) コレクション| ユーザー オブジェクトのリストを取得します。|
|[ユーザーを作成する](../api/user-post-users.md) |[user](user.md)| 新しいユーザー オブジェクトを作成します。|
|[Get user](../api/user-get.md) | [user](user.md) |ユーザー オブジェクトのプロパティと関係を読み取ります。|
|[Update user](../api/user-update.md) | [user](user.md) |ユーザー オブジェクトを更新します。 |
|[Delete user](../api/user-delete.md) | None |ユーザー オブジェクトを削除します。 |
|[List messages](../api/user-list-messages.md) |[message](message.md) コレクション| サインインしているユーザーのメールボックス内のすべてのメッセージを取得します。|
|[メッセージの作成](../api/user-post-messages.md) |[message](message.md)| メッセージ コレクションへの投稿により、新しいメッセージを作成します。|
|[mailFolders を一覧表示する](../api/user-list-mailfolders.md) |[mailFolder](mailfolder.md) コレクション| サインイン中のユーザーのルート フォルダーからメール フォルダー コレクションを取得します。 |
|[Create mailFolder](../api/user-post-mailfolders.md) |[mailFolder](mailfolder.md)| mailFolder コレクションへの投稿により、新しい MailFolder を作成します。|
|[sendMail](../api/user-sendmail.md)|None|要求本文に指定されたメッセージを送信します。|
|[List events](../api/user-list-events.md) |[event](event.md) コレクション| ユーザーのメールボックス内のイベント オブジェクトの一覧を取得します。一覧には、単一インスタンスの会議と定期的なマスターが含まれています。|
|[Create event](../api/user-post-events.md) |[イベント](event.md)| Event コレクションへの投稿によって、新しいイベントを作成します。|
|[List calendars](../api/user-list-calendars.md) |[calendar](calendar.md) コレクション| 予定表オブジェクトのコレクションを取得します。|
|[Create calendar](../api/user-post-calendars.md) |[calendar](calendar.md)| 予定表コレクションへの投稿により、新しい予定表を作成します。|
|[List calendarGroups](../api/user-list-calendargroups.md) |[calendarGroup](calendargroup.md) コレクション| CalendarGroup オブジェクトのコレクションを取得します。|
|[Create calendarGroup](../api/user-post-calendargroups.md) |[calendarGroup](calendargroup.md)| calendarGroups コレクションへの投稿により、新しい CalendarGroup を作成します。|
|[List calendarView](../api/user-list-calendarview.md) |[event](event.md) コレクション| Event オブジェクトのコレクションを取得します。|
|[連絡先を一覧表示する](../api/user-list-contacts.md) |[contact](contact.md) コレクション| サインイン中のユーザーの既定の連絡先フォルダーから連絡先コレクションを取得します。|
|[Create contact](../api/user-post-contacts.md) |[contact](contact.md)| 連絡先コレクションに投稿することにより、新しい連絡先を作成します。|
|[List contactFolders](../api/user-list-contactfolders.md) |[contactFolder](contactfolder.md) コレクション| サインイン中のユーザーの既定の連絡先フォルダー内の連絡先フォルダーのコレクションを取得します。|
|[Create ContactFolder](../api/user-post-contactfolders.md) |[contactFolder](contactfolder.md)| contactFolder コレクションに投稿することにより、新しい ContactFolder を作成します。|
|[List directReports](../api/user-list-directreports.md) |[directoryObject](directoryobject.md) collection| そのユーザーの部下であるユーザーと連絡先を、directReports ナビゲーション プロパティから取得します。|
|[List manager](../api/user-list-manager.md) |[directoryObject](directoryobject.md) | そのユーザーの上司であるユーザーまたは連絡先を、マネージャー ナビゲーション プロパティから取得します。|
|[List memberOf](../api/user-list-memberof.md) |[directoryObject](directoryobject.md) collection| そのユーザーが直接のメンバーであるグループおよびディレクトリ ロールを、memberOf ナビゲーション プロパティから取得します。|
|[推移的な memberOf を一覧表示する](../api/user-list-transitivememberof.md) |[directoryObject](directoryobject.md) コレクション| ユーザーがメンバーになっているグループとディレクトリ ロールを一覧表示します。 この操作は推移的で、このユーザーが入れ子のメンバーになっているグループが含まれます。 |
|[LownedDevices を一覧表示する](../api/user-list-owneddevices.md) |[directoryObject](directoryobject.md) collection| そのユーザーにより所有されているデバイスを、OwnedDevices ナビゲーション プロパティから取得します。|
|[List ownedObjects](../api/user-list-ownedobjects.md) |[directoryObject](directoryobject.md) collection| そのユーザーにより所有されているディレクトリ オブジェクトを、ownedObjects ナビゲーション プロパティから取得します。|
|[List registeredDevices](../api/user-list-registereddevices.md) |[directoryObject](directoryobject.md) collection| そのユーザーについて登録されているデバイスを、RegisteredDevices ナビゲーション プロパティから取得します。|
|[List createdObjects](../api/user-list-createdobjects.md) |[directoryObject](directoryobject.md) collection| そのユーザーにより作成されたディレクトリ オブジェクトを、createdObjects ナビゲーション プロパティから取得します。|
|[assignLicense](../api/user-assignlicense.md)|[user](user.md)|ユーザーのサブスクリプションを追加または削除します。また、サブスクリプションに関連付けられている特定のプランを有効または無効にすることもできます。|
|[licenseDetails を一覧表示する](../api/user-list-licensedetails.md) |[licenseDetails](licensedetails.md) コレクション| licenseDetails オブジェクトのコレクションを取得します。|
|[checkMemberGroups](../api/user-checkmembergroups.md)|String collection|グループの一覧内のメンバーシップを確認します。チェックは推移的です。|
|[delta](../api/user-delta.md)|user コレクション| ユーザーに対する増分の変更を取得します。 |
|[getMemberGroups](../api/user-getmembergroups.md)|String collection|ユーザーがメンバーであるすべてのグループを返します。チェックは推移的です。|
|[getMemberObjects](../api/user-getmemberobjects.md)|String collection| ユーザーがメンバーになっているすべてのグループとディレクトリ ロールを返します。チェックは推移的です。 |
|[reminderView](../api/user-reminderview.md)|[Reminder](reminder.md) collection|指定した開始時刻と終了時刻内の予定表のアラームの一覧を返します。|
|[revokeSignInSessions](../api/user-revokesigninsessions.md)| なし |**signInSessionsValidFromDateTime** ユーザー プロパティを現在の日時にリセットすることで、アプリケーションに発行されたすべての更新トークンとセッション トークンを失効にします。 これによりユーザーは、強制的にアプリケーションに再度サインインさせられます。|
|**オープン拡張機能**| | |
|[オープン拡張機能を作成する](../api/opentypeextension-post-opentypeextension.md) |[openTypeExtension](opentypeextension.md)| オープン拡張機能を作成し、新規または既存のリソースにカスタム プロパティを追加します。|
|[オープン拡張機能を取得する](../api/opentypeextension-get.md) |[openTypeExtension](opentypeextension.md) コレクション| 拡張機能の名前で識別されるオープン拡張機能を取得します。|
|**スキーマ拡張機能**| | |
|[スキーマ拡張機能の値を追加する](/graph/extensibility-schema-groups) || スキーマ拡張機能の定義を作成し、それを使用してカスタマイズされた種類のデータをリソースに追加します。|

## <a name="properties"></a>プロパティ

| プロパティ       | 型    |説明|
|:---------------|:--------|:----------|
|aboutMe|String|ユーザーが自分自身について記述する、フリー フォームのテキスト入力フィールド。|
|accountEnabled|Boolean| アカウントが有効な場合は **true**。そうでない場合は **false**。このプロパティは、ユーザーの作成時に必要です。$filter をサポートします。    |
|ageGroup|String|ユーザーの年齢グループを設定します。 使用できる値: `null`、`minor`、`notAdult`、および `adult`。 詳細については、「[法的年齢グループ プロパティの定義](#legal-age-group-property-definitions)」を参照してください。 |
|assignedLicenses|[assignedLicense](assignedlicense.md) collection|ユーザーに割り当てられているライセンス。null 許容ではありません。            |
|assignedPlans|[assignedPlan](assignedplan.md) collection|ユーザーに割り当てられているプラン。読み取り専用です。null 許容ではありません。 |
|birthday|DateTimeOffset|ユーザーの誕生日。Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表し、必ず UTC 時間です。たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`|
|businessPhones|String collection|ユーザーの電話番号。注:文字列コレクションですが、このプロパティに設定できるのは 1 つの数字のみです。|
|city|String|ユーザーがいる都市。$filter をサポートします。|
|companyName | String | ユーザーが関連付けられている会社名。 このプロパティは、外部ユーザーが所属する会社を記述するのに役立ちます。 |
|consentProvidedForMinor|String|未成年者について同意を得ているかどうかを設定します。 使用できる値: `null`、`granted`、`denied`、および `notRequired`。 詳細については、「[法的年齢グループ プロパティの定義](#legal-age-group-property-definitions)」を参照してください。|
|country|String|ユーザーがいる国/地域。たとえば、「US (米国)」や「UK (英国)」です。$filter をサポートします。|
|createdDateTime | DateTimeOffset |ユーザー オブジェクトの作成日です。 |
|department|String|ユーザーが働いている部門の名前。$filter をサポートします。|
|displayName|String|アドレス帳に表示されるユーザーの名前。これは通常、ユーザーの名前、ミドルネームのイニシャル、姓の組み合わせです。このプロパティは、ユーザーの作成時に必須になります。更新時にクリアすることはできません。$filter および $orderby をサポートします。|
|employeeId|String|組織によりユーザーに割り当てられた従業員 ID。 $filter をサポートします。|
|faxNumber|String|ユーザーの Fax 番号。|
|givenName|String|ユーザーの名。$filter をサポートします。|
|hireDate|DateTimeOffset|ユーザーの採用日付。Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表し、必ず UTC 時間です。たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`|
|id|String|ユーザーの一意の識別子。[directoryObject](directoryobject.md) から継承されます。キー。null 許容ではありません。読み取り専用です。|
|imAddresses|String collection|ユーザーのインスタント メッセージ ボイス オーバー IP (VOIP) セッション開始プロトコル (SIP) のアドレス。読み取り専用です。|
|interests|String collection|ユーザーが自分の関心事を記述する一覧。|
|isResourceAccount|Boolean| ユーザーがリソース アカウントの場合は **true**、それ以外の場合は **false**。 Null 値は **false** とみなされます。|
|jobTitle|String|ユーザーの役職。$filter をサポートします。|
|legalAgeGroupClassification|String| エンタープライズ アプリケーションで使用され、ユーザーの法的年齢グループを示します。 このプロパティは読み取り専用であり、`ageGroup` プロパティと `consentProvidedForMinor` プロパティに基づいて計算されます。 使用できる値: `null`、`minorWithOutParentalConsent`、`minorWithParentalConsent`、`minorNoParentalConsentRequired`、`notAdult`、および `adult`。 詳細については、「[法的年齢グループ プロパティの定義](#legal-age-group-property-definitions)」を参照してください。|
|licenseAssignmentStates|[licenseAssignmentState](licenseassignmentstate.md) コレクション|このユーザーへのライセンス割り当ての状態です。 読み取り専用です。|
|mail|String|ユーザーの SMTP アドレス (たとえば、"jeff@contoso.onmicrosoft.com")。読み取り専用。$filter をサポートします。|
|mailboxSettings|[mailboxSettings](mailboxsettings.md)|サインイン ユーザーのプライマリ メールボックスの設定。着信メッセージに対する自動応答を送信するための設定、ロケール、タイム ゾーンを [取得](../api/user-get-mailboxsettings.md) または [更新](../api/user-update-mailboxsettings.md) できます。|
|mailNickname|String|ユーザーの電子メール エイリアス。ユーザーの作成時に、このプロパティを指定する必要があります。$filter をサポートします。|
|mobilePhone|String|ユーザーの主な携帯電話の番号。|
|mySite|String|ユーザーの個人用サイトの URL。|
|officeLocation|String|ユーザーの勤務先の場所。|
|onPremisesDistinguishedName|String| オンプレミスの Active Directory `distinguished name` または `DN` が含まれています。 このプロパティは、オンプレミス ディレクトリを Azure AD Connect 経由で Azure Active Directory と同期する顧客の場合にのみ読み込まれます。 読み取り専用です。 |
|onPremisesDomainName|String| オンプレミス ディレクトリから同期されたオンプレミス `domainFQDN` (dnsDomainName とも呼ばれます) が含まれています。 このプロパティは、オンプレミス ディレクトリを Azure AD Connect 経由で Azure Active Directory と同期する顧客の場合にのみ読み込まれます。 読み取り専用です。 |
|onPremisesExtensionAttributes|[onPremisesExtensionAttributes](onpremisesextensionattributes.md)|ユーザーの extensionAttribute 1 ～ 15 が含まれています。 個々の拡張属性は選択もフィルター処理もできないことに注意してください。 `onPremisesSyncEnabled` ユーザーの場合、この一連のプロパティはマスターされており、読み取り専用です。 クラウド専用ユーザー (`onPremisesSyncEnabled` が false) の場合、これらのプロパティは作成時または更新時に設定される可能性があります。 |
|onPremisesImmutableId|String|このプロパティは、オンプレミスの Active Directory ユーザー アカウントを Azure AD ユーザー オブジェクトに関連付けるために使用します。 Graph で新しいユーザー アカウントを作成するとき、ユーザーの **userPrincipalName** (UPN) プロパティにフェデレーション ドメインを使用する場合は、このプロパティを指定する必要があります。 **重要:** **$** と **\_** の文字は、このプロパティを指定するときには使用できません。 $filter をサポートします。                            |
|onPremisesLastSyncDateTime|DateTimeOffset|オブジェクトがオンプレミス ディレクトリと前回、同期された日時を示します。例："2013-02-16T03:04:54Z"Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表し、必ず UTC 時間です。たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`読み取り専用です。|
|onPremisesProvisioningErrors|[onPremisesProvisioningError](onpremisesprovisioningerror.md) コレクション| Microsoft 同期製品のプロビジョニング中に発生するエラーです。 |
|onPremisesSamAccountName|String| オンプレミス ディレクトリから同期されたオンプレミス `samAccountName` が含まれています。 このプロパティは、オンプレミス ディレクトリを Azure AD Connect 経由で Azure Active Directory と同期する顧客の場合にのみ読み込まれます。 読み取り専用です。 |
|onPremisesSecurityIdentifier|String|オンプレミスからクラウドに同期されたユーザーのオンプレミスのセキュリティ識別子 (SID) が含まれます。読み取り専用です。|
|onPremisesSyncEnabled|Boolean| このオブジェクトがオンプレミスのディレクトリから同期される場合は **true**、このオブジェクトが最初にオンプレミスのディレクトリから同期されていて、今後は同期しない場合は **false**、このオブジェクトがオンプレミスのディレクトリから 1 度も同期されたことがない場合は **null** (既定値)。読み取り専用 |
|onPremisesUserPrincipalName|String| オンプレミス ディレクトリから同期されたオンプレミス `userPrincipalName` が含まれています。 このプロパティは、オンプレミス ディレクトリを Azure AD Connect 経由で Azure Active Directory と同期する顧客の場合にのみ読み込まれます。 読み取り専用です。 |
|otherMails|String| ユーザーの追加のメール アドレスの一覧 (例: `["bob@contoso.com", "Robert@fabrikam.com"]`)。 $filter をサポートします。|
|passwordPolicies|String|ユーザーのパスワード ポリシーを指定します。この値は列挙値であり、可能な 1 つの値は "DisableStrongPassword" です。この場合は、既定のポリシーより脆弱なパスワードを指定できます。"DisablePasswordExpiration" を指定することもできます。2 つを一緒に指定することもできます。例:"DisablePasswordExpiration, DisableStrongPassword"|
|passwordProfile|[passwordProfile](passwordprofile.md)|ユーザーのパスワード プロファイルを指定します。プロファイルには、ユーザーのパスワードが含まれています。このプロパティは、ユーザーの作成時に必要です。プロファイルにあるパスワードは、**passwordPolicies** プロパティによって指定されている最小要件を満たす必要があります。既定では、強力なパスワードが必要です。|
|pastProjects|String collection|ユーザーが過去のプロジェクトを列挙する一覧。|
|postalCode|String|ユーザーの住所の郵便番号。郵便番号は、ユーザーの国/地域に固有です。アメリカ合衆国では、この属性には、ZIP コードが含まれます。|
|preferredDataLocation|String|ユーザーの優先されるデータの場所。 詳細については、「[OneDrive Online Multi-Geo](https://docs.microsoft.com/sharepoint/dev/solution-guidance/multigeo-introduction)」を参照してください。|
|preferredLanguage|String|ユーザーが設定する言語。ISO 639-1 コードに従う必要があります。たとえば "en-US" です。|
|preferredName|String|ユーザーが設定する名前。|
|provisionedPlans|[ProvisionedPlan](provisionedplan.md) コレクション|ユーザーのために用意されたプラン。読み取り専用です。null 許容ではありません。 |
|proxyAddresses|String collection|例:`["SMTP: bob@contoso.com", "smtp: bob@sales.contoso.com"]` 複数値プロパティのフィルター式には、**任意の**演算子が必要です。読み取り専用。null 許容ではありません。$filter をサポートします。          |
|responsibilities|String collection|ユーザーが自分の責任の範囲を列挙する一覧。|
|schools|String collection|ユーザーが在籍した学校を列挙する一覧。|
|showInAddressList|Boolean|Outlook グローバル アドレス一覧にこのユーザーが含まれている必要がある場合は **true**、それ以外の場合は **false**。 設定されていない場合は、**true** として扱われます。 招待マネージャーから招待されたユーザーの場合、このプロパティは **false** に設定されます。|
|skills|String collection|ユーザーが自分のスキルを列挙する一覧。|
|signInSessionsValidFromDateTime|DateTimeOffset| この時点よりも前に発行された更新トークンとセッション トークン (セッション Cookie) はすべて無効であり、アプリケーションが無効な更新トークンまたはセッション トークンを使用して (Microsoft Graph などの API にアクセスする目的で) 代理アクセス トークンを取得しようとすると、エラーが発生します。  この状況が発生した場合、アプリケーションは承認エンドポイントに対してリクエストを発行して新しいトークンを取得する必要があります。 読み取り専用です。 [revokeSignInSessions](../api/user-revokesigninsessions.md) を使用して再設定します。|
|state|String|ユーザーの住所の都道府県。$filter をサポートします。|
|streetAddress|String|ユーザーの勤務先の番地。|
|surname|String|ユーザーの姓。$filter をサポートします。|
|usageLocation|String|2 文字の国コード (ISO 規格 3166)国におけるサービスの利用可能性を確認することが法的に義務付けられているため、ライセンスを割り当てられるユーザーには必須です。例:"US"、"JP"、"GB"null 許容ではありません。$filter をサポートします。|
|userPrincipalName|String|ユーザーのユーザー プリンシパル名 (UPN)。UPN は、インターネット標準 RFC 822 に基づいた、インターネット スタイルのユーザーのログイン名です。規則では、これはユーザーの電子メール名にマップされる必要があります。一般的な形式は alias@domain です。このドメインは、検証済みドメインのテナントのコレクション内に存在している必要があります。このプロパティは、ユーザーの作成時に必要です。テナントの検証済みのドメインには、[organization](organization.md) の **verifiedDomains** プロパティからアクセスできます。$filter および $orderby をサポートします。
|userType|String|ディレクトリ内のユーザーの種類を分類するために使用する文字列値 (“Member”、“Guest” など)。$filter をサポートします。          |

### <a name="legal-age-group-property-definitions"></a>法的年齢グループ プロパティの定義

ここでは、Azure AD 管理者とエンタープライズ アプリケーション開発者が 3 つの年齢グループ プロパティ (`legalAgeGroupClassification`、`ageGroup`、および `consentProvidedForMinor`) を使用して年齢関連の規制に準拠する方法を説明します。

例: Cameron は英国の Holyport にある小学校でディレクトリを管理する管理者です。 学年の始まりに、英国の年齢関連の規制に基づき、入学書類を使用して未成年者の保護者から同意を得ます。 保護者から取得した同意により、未成年者のアカウントを Holyport スクールと Microsoft アプリが使用することが許可されます。 次に Cameron はすべてのアカウントを作成し、ageGroup を "minor" に、consentProvidedForMinor を "granted" に設定します。 これにより、生徒が使用するアプリケーションでは未成年に適していない機能が非表示になります。

#### <a name="legal-age-group-classification"></a>法的年齢グループの分類

この読み取り専用プロパティは、エンタープライズ アプリケーション開発者が、ユーザーの法的年齢グループに基づいてそのユーザーを適切に処理できるようにするために使用します。 ユーザーの `ageGroup` および `consentProvidedForMinor` プロパティに基づいて計算されます。

| 値    | #  |説明|
|:---------------|:--------|:----------|
|null|0|既定値。ユーザーに `ageGroup` が設定されていません。|
|minorWithoutParentalConsent |1|(将来使用するために予約されています)|
|minorWithParentalConsent|2| 当該国または地域の年齢関連規制に基づいてユーザーが未成年と判断され、アカウントの管理者が保護者から適切な同意を得ています。|
|adult|3|当該国または地域の年齢関連規制に基づいて成人と判断されたユーザー。|
|notAdult|4|追加の年齢関連規制がある国または地域 (米国、英国、欧州連合、韓国など) にいるユーザーであり、ユーザーの年齢が未成年と成人の間です (国または地域での規定に基づく)。 通常、規制対象の国では 10 代の若者は `notAdult` とみなされます。|
|minorNoParentalConsentRequired|5|ユーザーは未成年ですが、年齢関連の規制のない国または地域にいます。|

#### <a name="age-group-and-minor-consent"></a>年齢グループと未成年の同意

年齢グループと未成年の同意のプロパティはオプションであり、Azure AD 管理者はこれらのプロパティを使用して、ユーザーの国または地域で施行されている年齢関連の規制に基づいてアカウントの使用が正しく処理されるようにします。

#### <a name="agegroup-property"></a>ageGroup プロパティ

| 値    | #  |説明|
|:---------------|:--------|:----------|
|null|0|既定値。ユーザーに `ageGroup` が設定されていません。|
|minor|1|ユーザーは未成年として扱われます。|
|notAdult|2|ユーザーは法的規制のある国 (米国、英国、欧州連合、または韓国) におり、ユーザーの年齢は未成年者の年齢の上限 (国に応じて異なる) を超えているが成人の年齢の下限 (国または地域に基づき規定されている) 未満です。 したがって基本的に 10 代の若者は規制対象の国では `notAdult` とみなされます。|
|adult|3|ユーザーは成人として扱われます。|

#### <a name="consentprovidedforminor-property"></a>consentProvidedForMinor プロパティ

| 値    | #  |説明|
|:---------------|:--------|:----------|
|null|0|既定値。ユーザーに `consentProvidedForMinor` が設定されていません。|
|granted|1|ユーザーがアカウントを所有することについて同意が得られています。|
|denied|2|ユーザーがアカウントを所有することについて同意が得られていません。|
|notRequired|3|ユーザーは、同意を必要としない場所にいます。|

## <a name="relationships"></a>リレーションシップ

| リレーションシップ | 型   |説明|
|:---------------|:--------|:----------|
|アクティビティ|[userActivity](projectrome-activity.md) コレクション|デバイス間におけるユーザーのアクティビティ。 読み取り専用です。 Null 許容型。|
|予定表|[calendar](calendar.md)|ユーザーの標準予定表。読み取り専用です。|
|calendarGroups|[calendarGroup](calendargroup.md) コレクション|ユーザーの予定表グループ。読み取り専用です。Null 許容型。|
|calendarView|[event](event.md) コレクション|予定表のカレンダー ビュー。読み取り専用です。Null 許容型。|
|calendars|[calendar](calendar.md) コレクション|ユーザーの予定表。読み取り専用です。Null 許容型。|
|contactFolders|[contactFolder](contactfolder.md) コレクション|ユーザーの連絡先フォルダー。読み取り専用です。Null 許容型。|
|contacts|[contact](contact.md) コレクション|ユーザーの連絡先。読み取り専用です。Null 許容型。|
|createdObjects|[directoryObject](directoryobject.md) collection|ユーザーによって作成されたディレクトリ オブジェクト。読み取り専用です。Null 許容型。|
|directReports|[directoryObject](directoryobject.md) collection|そのユーザーの部下であるユーザーと連絡先。(マネージャー プロパティがこのユーザーに設定されている、ユーザーと連絡先。)読み取り専用です。Null 許容型。 |
|drive|[drive](drive.md)|ユーザーの OneDrive。読み取り専用です。|
|drives|[drive](drive.md) コレクション| このユーザーが使用できるドライブのコレクション。読み取り専用です。 |
|イベント|[event](event.md) コレクション|ユーザーのイベント。既定では、既定の予定表でイベントが表示されます。読み取り専用です。Null 許容型。|
|extensions|[extension](extension.md) コレクション|ユーザーに対して定義されているオープン拡張機能のコレクション。読み取り専用です。Null 許容型。|
|inferenceClassification | [inferenceClassification](inferenceclassification.md) | 明示的な指定に基づく、ユーザーのメッセージの関連性の分類。明示的な指定は、推定される関連性や重要性より優先されます。 |
|licenseDetails|[licenseDetails](licensedetails.md) コレクション|このユーザーのライセンスの詳細のコレクション。 読み取り専用です。|
|mailFolders|[mailFolder](mailfolder.md) コレクション| ユーザーのメール フォルダー。読み取り専用です。Null 許容型。|
|manager|[directoryObject](directoryobject.md)|このユーザーの上司であるユーザーまたは連絡先。読み取り専用です。(HTTP メソッド:GET、PUT、DELETE)|
|memberOf|[directoryObject](directoryobject.md) collection|ユーザーがメンバーになっているグループとディレクトリ ロール。読み取り専用です。Null 許容型。|
|messages|[message](message.md) コレクション|メールボックスまたはフォルダー内のメッセージ。読み取り専用です。Null 許容型。|
|onenote|[onenote](onenote.md)| 読み取り専用です。|
|outlook|[outlookUser](outlookuser.md)| 読み取り専用です。|
|ownedDevices|[directoryObject](directoryobject.md) collection|ユーザーが所有しているデバイス。読み取り専用です。Null 許容型。|
|ownedObjects|[directoryObject](directoryobject.md) collection|ユーザーが所有しているディレクトリ オブジェクト。読み取り専用です。Null 許容型。|
|people|[person](person.md) コレクション| ユーザーに関連のある人物です。 読み取り専用です。 Null 許容型。
|photo|[profilePhoto](profilephoto.md)| ユーザーのプロフィール写真。読み取り専用です。|
|planner|[plannerUser](planneruser.md)| ユーザーに存在する可能性がある Planner リソースのエントリ ポイントです。 読み取り専用です。|
|registeredDevices|[directoryObject](directoryobject.md) collection|ユーザーについて登録されているデバイス。読み取り専用です。Null 許容型。|

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
  "employeeId": "string",
  "faxNumber" : "string",
  "givenName": "string",
  "hireDate": "String (timestamp)",
  "id": "string (identifier)",
  "imAddresses": ["string"],
  "interests": ["string"],
  "isResourceAccount": false,
  "jobTitle": "string",
  "legalAgeGroupClassification": "string",
  "licenseAssignmentStates": [{"@odata.type": "microsoft.graph.licenseAssignmentState"}],
  "mail": "string",
  "mailboxSettings": {"@odata.type": "microsoft.graph.mailboxSettings"},
  "mailNickname": "string",
  "mobilePhone": "string",
  "mySite": "string",
  "officeLocation": "string",
  "onPremisesDistinguishedName": "string",
  "onPremisesDomainName": "string",
  "onPremisesExtensionAttributes": {"@odata.type": "microsoft.graph.onPremisesExtensionAttributes"},
  "onPremisesImmutableId": "string",
  "onPremisesLastSyncDateTime": "String (timestamp)",
  "onPremisesProvisioningErrors": [{"@odata.type": "microsoft.graph.onPremisesProvisioningError"}],
  "onPremisesSamAccountName": "string",
  "onPremisesSecurityIdentifier": "string",
  "onPremisesSyncEnabled": true,
  "onPremisesUserPrincipalName": "string",
  "otherMails": "string",
  "passwordPolicies": "string",
  "passwordProfile": {"@odata.type": "microsoft.graph.passwordProfile"},
  "pastProjects": ["string"],
  "postalCode": "string",
  "preferredDataLocation": "string",
  "preferredLanguage": "string",
  "preferredName": "string",
  "provisionedPlans": [{"@odata.type": "microsoft.graph.provisionedPlan"}],
  "proxyAddresses": ["string"],
  "responsibilities": ["string"],
  "schools": ["string"],
  "showInAddressList": true,
  "signInSessionsValidFromDateTime": "String (timestamp)",
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

- [拡張機能を使用してカスタム データをリソースに追加する](/graph/extensibility-overview)
- [オープン拡張機能を使用してカスタム データをユーザーに追加する](/graph/extensibility-open-users)
- [スキーマ拡張機能を使用したグループへのカスタム データの追加](/graph/extensibility-schema-groups)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "user resource",
  "keywords": "",
  "suppressions" : [
     "Warning: /api-reference/v1.0/resources/user.md/microsoft.graph.user:
      Property 'createdDateTime' found in markdown table but not in resource definition."
  ],
  "section": "documentation",
  "tocPath": ""
}-->
