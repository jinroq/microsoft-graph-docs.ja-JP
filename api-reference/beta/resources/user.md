---
title: ユーザー リソースの種類
description: Azure AD ユーザー アカウントを表します。directoryObject から継承します。
author: dkershaw10
localization_priority: Priority
ms.prod: microsoft-identity-platform
ms.openlocfilehash: a9d3ca1c6f9c67cc2e41907dc22b9f1ec7d28b0a
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27972650"
---
# <a name="user-resource-type"></a>user リソースの種類

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

Azure AD ユーザー アカウントを表します。[directoryObject](directoryobject.md) から継承します。

このリソースは以下をサポートしています。

- [拡張機能](/graph/extensibility-overview)として、カスタム プロパティに独自のデータを追加します。
- [変更通知](/graph/webhooks)にサブスクライブします。
- [デルタ](../api/user-delta.md)関数を提供することにより、[デルタ クエリ](/graph/delta-query-overview)を使用して、増分の追加、削除、更新を追跡します。

## <a name="methods"></a>メソッド

| メソッド | 戻り値の型 | 説明 |
|:-------|:------------|:------------|
|[user のリスト](../api/user-list.md) |[user](user.md) コレクション| ユーザー オブジェクトのリストを取得します。|
|[ユーザーを作成する](../api/user-post-users.md) |[user](user.md)| 新しいユーザー オブジェクトを作成します。|
|[Get user](../api/user-get.md) | [user](user.md) |ユーザー オブジェクトのプロパティと関係を読み取ります。|
|[Update user](../api/user-update.md) | [user](user.md) |ユーザー オブジェクトを更新します。 |
|[Delete user](../api/user-delete.md) | なし |ユーザー オブジェクトを削除します。 |
|[List messages](../api/user-list-messages.md) |[Message](message.md) collection| サインインしているユーザーのメールボックス内のすべてのメッセージを取得します。|
|[Create Message](../api/user-post-messages.md) |[Message](message.md)| メッセージのコレクションへの投稿には、メッセージを作成します。|
|[List mailFolders](../api/user-list-mailfolders.md) |[MailFolder](mailfolder.md) collection| サインイン中のユーザーのルート フォルダーからメール フォルダー コレクションを取得します。 |
|[Create mailFolder](../api/user-post-mailfolders.md) |[MailFolder](mailfolder.md)| mailFolder コレクションへの投稿により、新しい MailFolder を作成します。|
|[sendMail](../api/user-sendmail.md)|None|要求本文に指定されたメッセージを送信します。|
|[List events](../api/user-list-events.md) |[Event](event.md) collection| ユーザーのメールボックス内のイベント オブジェクトの一覧を取得します。一覧には、単一インスタンスの会議と定期的なマスターが含まれています。|
|[イベントを作成する](../api/user-post-events.md) |[Event](event.md)| Event コレクションへの投稿によって、新しいイベントを作成します。|
|[List calendars](../api/user-list-calendars.md) |[Calendar](calendar.md) collection| 予定表オブジェクトのコレクションを取得します。|
|[Create calendar](../api/user-post-calendars.md) |[Calendar](calendar.md)| 予定表コレクションへの投稿により、新しい予定表を作成します。|
|[List calendarGroups](../api/user-list-calendargroups.md) |[CalendarGroup](calendargroup.md) collection| CalendarGroup オブジェクトのコレクションを取得します。|
|[Create calendarGroup](../api/user-post-calendargroups.md) |[CalendarGroup](calendargroup.md)| calendarGroups コレクションへの投稿により、新しい CalendarGroup を作成します。|
|[List calendarView](../api/user-list-calendarview.md) |[Event](event.md) collection| イベント オブジェクトのコレクションを取得します。|
|[List contacts](../api/user-list-contacts.md) |[Contact](contact.md) collection| サインイン中のユーザーの既定の連絡先フォルダーから連絡先コレクションを取得します。|
|[Create Contact](../api/user-post-contacts.md) |[Contact](contact.md)| 連絡先コレクションに投稿することにより、新しい連絡先を作成します。|
|[List contactFolders](../api/user-list-contactfolders.md) |[ContactFolder](contactfolder.md) collection| サインイン中のユーザーの既定の連絡先フォルダー内の連絡先フォルダーのコレクションを取得します。|
|[Create ContactFolder](../api/user-post-contactfolders.md) |[ContactFolder](contactfolder.md)| contactFolder コレクションに投稿することにより、新しい ContactFolder を作成します。|
|[List directReports](../api/user-list-directreports.md) |[directoryObject](directoryobject.md) collection| そのユーザーの部下であるユーザーと連絡先を、directReports ナビゲーション プロパティから取得します。|
|[List manager](../api/user-list-manager.md) |[directoryObject](directoryobject.md) | そのユーザーの上司であるユーザーまたは連絡先を、マネージャー ナビゲーション プロパティから取得します。|
|[List memberOf](../api/user-list-memberof.md) |[directoryObject](directoryobject.md) コレクション| グループ、ディレクトリの役割、およびユーザーが所属するグループのナビゲーション プロパティからの直接のメンバーになっている管理の単位を取得します。|
|[推移的な所属するグループ] ボックスの一覧](../api/user-list-transitivememberof.md) |[directoryObject](directoryobject.md) コレクション| グループ、ディレクトリの役割、およびメンバーであるユーザーの管理の単位を一覧表示します。 この操作では、推移的では、ユーザーの入れ子にされたメンバーであるグループが含まれています。 |
|[参加チームのリストを作成する](../api/user-list-joinedteams.md) |[グループ](group.md)コレクション| ユーザーが joinedTeams のナビゲーション プロパティからの直接のメンバーであるマイクロソフトのチームを取得します。|
|[List ownedDevices](../api/user-list-owneddevices.md) |[directoryObject](directoryobject.md) collection| そのユーザーにより所有されているデバイスを、OwnedDevices ナビゲーション プロパティから取得します。|
|[List ownedObjects](../api/user-list-ownedobjects.md) |[directoryObject](directoryobject.md) collection| そのユーザーにより所有されているディレクトリ オブジェクトを、ownedObjects ナビゲーション プロパティから取得します。|
|[List plannerTasks](../api/planneruser-list-tasks.md) |[plannerTask](plannertask.md) コレクション| ユーザーに割り当てられている plannerTasks を取得します。|
|[List registeredDevices](../api/user-list-registereddevices.md) |[directoryObject](directoryobject.md) collection| RegisteredDevices のナビゲーション プロパティからユーザーの登録されているデバイスを取得します。|
|[スコープ ロール メンバーシップの一覧](../api/user-list-scopedrolememberof.md) |[scopedRoleMembership](scopedrolemembership.md) コレクション| このユーザーの管理単位メンバーシップのスコープからロールを取得します。|
|[List createdObjects](../api/user-list-createdobjects.md) |[directoryObject](directoryobject.md) collection| そのユーザーにより作成されたディレクトリ オブジェクトを、createdObjects ナビゲーション プロパティから取得します。|
|[リスト agreementAcceptances](../api/user-list-agreementacceptances.md) | [agreementAcceptance](agreementacceptance.md)コレクション | 使用条件の一覧にユーザーの承認ステータスを取得します。|
|[assignLicense](../api/user-assignlicense.md)|[user](user.md)|ユーザーのサブスクリプションを追加または削除します。また、サブスクリプションに関連付けられている特定のプランを有効または無効にすることもできます。|
|[licenseDetails を一覧表示する](../api/user-list-licensedetails.md) |[licenseDetails](licensedetails.md) コレクション| licenseDetails オブジェクトのコレクションを取得します。|
|[checkMemberGroups](../api/user-checkmembergroups.md)|String コレクション|グループの一覧内のメンバーシップを確認します。チェックは推移的です。|
|[findmeetingtimes](../api/user-findmeetingtimes.md)|[meetingTimeCandidate](meetingtimecandidate.md)|検索の時間と場所を満たすためには、出席者の空き時間、場所、時間の制約に基づいています。|
|[findRoomLists](../api/user-findroomlists.md)|[emailaddress.md](emailaddress.md)コレクション | テナントで定義された部屋の一覧を取得します。|
|[findRooms](../api/user-findrooms.md)|[emailaddress.md](emailaddress.md)コレクション | すべての会議室ユーザーのテナントや、特定の場所] ボックスの一覧を取得します。 |
|[getMailTips](../api/user-getmailtips.md)|[mailTips](mailtips.md) コレクション|サインイン中のユーザーが利用できる、1 人または複数の受信者に対してのメール ヒントを返します。 |
|[getMemberGroups](../api/user-getmembergroups.md)|String コレクション|ユーザーがメンバーであるすべてのグループを返します。チェックは推移的です。|
|[getMemberObjects](../api/user-getmemberobjects.md)|String コレクション| すべてのグループ、ディレクトリの役割、およびメンバーであるユーザーの管理の単位を取得します。 チェック、推移的です。 |
|[invalidateAllRefreshTokens](../api/user-invalidateallrefreshtokens.md)| なし |**RefreshTokensValidFromDateTime**ユーザーのプロパティを現在の日付と時刻にリセットすることで、アプリケーションに発行されたすべてのユーザーの更新し、セッション トークンを無効にします。 これは、それらのアプリケーションをもう一度サインインするユーザーを強制します。|
|[reminderView](../api/user-reminderview.md)|[Reminder](reminder.md) collection|指定した開始時刻と終了時刻内の予定表のアラームの一覧を返します。|
|[delta](../api/user-delta.md)|user コレクション| ユーザーに対する増分の変更を取得します。 |
|[Outlook の識別子を変換します。](../api/user-translateexchangeids.md) |[convertIdResult リソースの種類](convertidresult.md)のコレクション| 形式との間、Outlook に関連するリソースの識別子を変換します。|
|**オープン拡張機能**| | |
|[オープン拡張機能を作成する](../api/opentypeextension-post-opentypeextension.md) |[openTypeExtension](opentypeextension.md)| オープン拡張機能を作成し、新規または既存のリソースにカスタム プロパティを追加します。|
|[オープン拡張機能を取得する](../api/opentypeextension-get.md) |[openTypeExtension](opentypeextension.md) コレクション| 拡張機能の名前で識別されるオープン拡張機能を取得します。|
|**スキーマ拡張機能**| | |
|[スキーマ拡張機能の値を追加する](/graph/extensibility-schema-groups) || スキーマ拡張機能の定義を作成し、それを使用してカスタマイズされた種類のデータをリソースに追加します。|

## <a name="properties"></a>プロパティ

| プロパティ       | 型    | 説明 |
|:---------------|:--------|:------------|
|aboutMe|String|ユーザーが自分自身について記述する、フリー フォームのテキスト入力フィールド。|
|accountEnabled|Boolean| アカウントが有効な場合は **true**。そうでない場合は **false**。このプロパティは、ユーザーの作成時に必要です。$filter をサポートします。    |
|ageGroup|String|ユーザーの年齢グループを設定します。 使用できる値: `null`、 `minor`、`notAdult`と`adult`。 詳細については[法律の年齢グループのプロパティの定義](#legal-age-group-property-definitions)を参照してください。 |
|assignedLicenses|[assignedLicense](assignedlicense.md) collection|ユーザーに割り当てられているライセンス。null 許容ではありません。            |
|assignedPlans|[assignedPlan](assignedplan.md) コレクション|ユーザーに割り当てられているプラン。読み取り専用です。null 許容ではありません。 |
|birthday|DateTimeOffset|ユーザーの誕生日。Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表し、必ず UTC 時間です。たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`|
|city|String|ユーザーがいる都市。$filter をサポートします。|
|companyName| String | ユーザーが関連付けられている会社名。 読み取り専用です。
|consentProvidedForMinor|String|未成年者の同意が取得されたかどうかを設定します。 使用できる値: `null`、 `granted`、`denied`と`notRequired`。 詳細については[法律の年齢グループのプロパティの定義](#legal-age-group-property-definitions)を参照してください。|
|country|String|国/地域のユーザーが存在します。たとえば、「米国」または「大阪府」です。 $filter をサポートします。|
|deletedDateTime|DateTimeOffset| 日付と時刻、ユーザーが削除されました。 |
|department|String|ユーザーが働いている部門の名前。$filter をサポートします。|
|displayName|String|アドレス帳に表示されるユーザーの名前。 この値は、通常、ユーザーの名、ミドル ネームの最初と最後の名の組み合わせです。 このプロパティはユーザーの作成時に必須です。更新時にクリアすることはできません。 $filter および $orderby をサポートします。|
|[社員コード]|String|組織がユーザーに割り当てられている従業員の識別子です。 $filter をサポートします。|
|externalUserState|String|[招待 API](../api/invitation-post.md)を使用してテナントに招待された外部ユーザーに対しては、このプロパティは、招待されたユーザーの招待の状態を表します。 'PendingAcceptance' または '' を招待するユーザーの状態は、または`null`の他のすべてのユーザー用です。 $Filter でサポートされている値をサポートしています。 例: `$filter=externalUserState eq 'PendingAcceptance'`。|
|externalUserStateChangeDateTime|String|ExternalUserState プロパティには、最新の変更のタイムスタンプを表示します。|
|変更を保存|String|ユーザーの fax 番号です。|
|givenName|String|ユーザーの名。$filter をサポートします。|
|hireDate|DateTimeOffset|ユーザーの採用日付。Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表し、必ず UTC 時間です。たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`|
|id|String|ユーザーの一意の識別子。[directoryObject](directoryobject.md) から継承されます。キー。null 許容ではありません。読み取り専用です。|
|interests|String コレクション|ユーザーが自分の関心事を記述する一覧。|
|jobTitle|String|ユーザーの役職。$filter をサポートします。|
|legalAgeGroupClassification|String| エンタープライズ ・ アプリケーションで使用すると、ユーザーの法的な年齢グループを決定します。 このプロパティは読み取り専用と演算に基づく`ageGroup`と`consentProvidedForMinor`のプロパティです。 使用できる値: `null`、 `minorWithOutParentalConsent`、 `minorWithParentalConsent`、 `minorNoParentalConsentRequired`、`notAdult`と`adult`。 参照してください詳細については[法律の年齢グループのプロパティの定義](#legal-age-group-property-definitions)。)|
|licenseAssignmentStates|[licenseAssignmentState](licenseassignmentstate.md)コレクション|このユーザーのライセンスの割り当ての状態です。 読み取り専用です。|
|mail|String|ユーザーの SMTP アドレス (たとえば、"jeff@contoso.onmicrosoft.com")。読み取り専用。$filter をサポートします。|
|mailboxSettings|[mailboxSettings](mailboxsettings.md)|サインイン ユーザーのプライマリ メールボックスの設定。 着信メッセージ、ロケール、およびタイム ゾーンへの自動返信を送信するため[の更新](../api/user-update-mailboxsettings.md)を[取得](../api/user-get-mailboxsettings.md)または設定ができます。|
|mailNickname|String|ユーザーの電子メール エイリアス。ユーザーの作成時に、このプロパティを指定する必要があります。$filter をサポートします。|
|mobilePhone|String|ユーザーの主な携帯電話の番号。|
|mySite|String|ユーザーの個人用サイトの URL。|
|officeLocation|String|ユーザーの勤務先の場所。|
|onPremisesDistinguishedName|String| オンプレミスの Active Directory が含まれています`distinguished name`または`DN`。 プロパティは Azure AD 接続経由で Active Directory を Azure に、オンプレミスのディレクトリが同期しているお客様に対してのみ設定されます。 読み取り専用です。 |
|onPremisesDomainName|String| 設置が含まれています`domainFQDN`、設置ディレクトリからの同期をとりますとも呼ばれます。 プロパティは Azure AD 接続経由で Active Directory を Azure に、オンプレミスのディレクトリが同期しているお客様に対してのみ設定されます。 読み取り専用です。 |
|onPremisesExtensionAttributes|[OnPremisesExtensionAttributes](onpremisesextensionattributes.md)|ユーザーの extensionAttributes 1-15 が含まれています。 個々 の拡張属性は、フィルターも選択可能なことに注意してください。 `onPremisesSyncEnabled`ユーザーは、この一連のプロパティは読み取り専用で、マスター設置します。 クラウド専用のユーザー (、`onPremisesSyncEnabled`は)、これらのプロパティは作成時に設定するか、更新します。 |
|onPremisesImmutableId|String|Azure AD ユーザー オブジェクトには、オンプレミス Active Directory ユーザー アカウントを関連付けるにはこのプロパティを使用します。 ユーザーのフェデレーション ドメインを使用している場合は、グラフに新しいユーザー アカウントを作成するときは、このプロパティを指定する必要があります`userPrincipalName`(UPN) のプロパティです。 **重要な:****$** 、このプロパティを指定する場合、 **_** 文字を使用できません。 $filter をサポートします。 |
|onPremisesLastSyncDateTime|DateTimeOffset|オブジェクトがオンプレミス ディレクトリと前回、同期された日時を示します。例："2013-02-16T03:04:54Z"Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表し、必ず UTC 時間です。たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`読み取り専用です。|
|onPremisesProvisioningErrors|[onPremisesProvisioningError](onpremisesprovisioningerror.md)コレクション| 提供処理中に同期の Microsoft 製品を使用するときのエラーです。 |
|onPremisesSamAccountName|String| 設置が含まれています`sAMAccountName`設置ディレクトリと同期します。 プロパティは Azure AD 接続経由で Active Directory を Azure に、オンプレミスのディレクトリが同期しているお客様に対してのみ設定されます。 読み取り専用です。 |
|onPremisesSecurityIdentifier|String|オンプレミスからクラウドに同期されたユーザーのオンプレミスのセキュリティ識別子 (SID) が含まれます。読み取り専用です。|
|onPremisesSyncEnabled|Boolean| このオブジェクトがオンプレミスのディレクトリから同期される場合は **true**、このオブジェクトが最初にオンプレミスのディレクトリから同期されていて、今後は同期しない場合は **false**、このオブジェクトがオンプレミスのディレクトリから 1 度も同期されたことがない場合は **null** (既定値)。読み取り専用 |
|onPremisesUserPrincipalName|String| 設置が含まれています`userPrincipalName`設置ディレクトリと同期します。 プロパティは Azure AD 接続経由で Active Directory を Azure に、オンプレミスのディレクトリが同期しているお客様に対してのみ設定されます。 読み取り専用です。 |
|otherMails|String| ユーザーの他の電子メール アドレスの一覧例: `["bob@contoso.com", "Robert@fabrikam.com"]`。 $filter をサポートします。|
|passwordPolicies|String|ユーザーのパスワード ポリシーを指定します。この値は列挙値であり、可能な 1 つの値は "DisableStrongPassword" です。この場合は、既定のポリシーより脆弱なパスワードを指定できます。"DisablePasswordExpiration" を指定することもできます。2 つを一緒に指定することもできます。例:"DisablePasswordExpiration, DisableStrongPassword"|
|passwordProfile|[PasswordProfile](passwordprofile.md)|ユーザーのパスワード プロファイルを指定します。プロファイルには、ユーザーのパスワードが含まれています。このプロパティは、ユーザーの作成時に必要です。プロファイルにあるパスワードは、**passwordPolicies** プロパティによって指定されている最小要件を満たす必要があります。既定では、強力なパスワードが必要です。|
|pastProjects|String コレクション|ユーザーが過去のプロジェクトを列挙する一覧。|
|postalCode|String|ユーザーの住所の郵便番号。郵便番号は、ユーザーの国/地域に固有です。アメリカ合衆国では、この属性には、ZIP コードが含まれます。|
|preferredDataLocation|String|ユーザーの希望するデータの場所です。 詳細については、[オンラインの複数の地域 OneDrive](https://docs.microsoft.com/sharepoint/dev/solution-guidance/multigeo-introduction)を参照してください。|
|preferredLanguage|String|ユーザーが設定する言語。ISO 639-1 コードに従う必要があります。たとえば "en-US" です。|
|preferredName|String|ユーザーが設定する名前。|
|provisionedPlans|[ProvisionedPlan](provisionedplan.md) コレクション|ユーザーのために用意されたプラン。読み取り専用です。null 許容ではありません。 |
|proxyAddresses|String コレクション|例:`["SMTP: bob@contoso.com", "smtp: bob@sales.contoso.com"]` 複数値プロパティのフィルター式には、**任意の**演算子が必要です。読み取り専用。null 許容ではありません。$filter をサポートします。          |
|refreshTokensValidFromDateTime|DateTimeOffset| トークンの更新やセッション トークン (セッション cookie) は、この時間が有効でないと、アプリケーションはトークンを取得するエラー、無効な更新やセッション トークンを使用して、委任されたアクセスを取得するとき (Api にアクセスする Microsoft のグラフなど) の前に発行されます。  このような場合は、アプリケーションが承認エンドポイントを要求することによって、新しい更新のトークンを取得する必要があります。 読み取り専用です。 リセットするには、 [invalidateAllRefreshTokens](../api/user-invalidateallrefreshtokens.md)を使用します。|
|responsibilities|String コレクション|ユーザーが自分の責任の範囲を列挙する一覧。|
|schools|String コレクション|ユーザーが在籍した学校を列挙する一覧。|
|showInAddressList|Boolean|**true の**場合、Outlook のグローバル アドレス一覧は、このユーザー、それ以外の場合は**false**を含める必要があります。 かどうかが設定されていないこのとして扱われます**場合は true**です。 招待マネージャーによって参加を要請するユーザー、このプロパティは**false**に設定されます。|
|skills|String コレクション|ユーザーが自分のスキルを列挙する一覧。|
|state|String|ユーザーの住所の都道府県。$filter をサポートします。|
|streetAddress|String|ユーザーの勤務先の番地。|
|surname|String|ユーザーの姓。$filter をサポートします。|
|usageLocation|String|2 文字の国コード (ISO 規格 3166)国におけるサービスの利用可能性を確認することが法的に義務付けられているため、ライセンスを割り当てられるユーザーには必須です。例:"US"、"JP"、"GB"null 許容ではありません。$filter をサポートします。|
|userPrincipalName|String|ユーザーのユーザー プリンシパル名 (UPN)。UPN は、インターネット標準 RFC 822 に基づいた、インターネット スタイルのユーザーのログイン名です。規則では、これはユーザーの電子メール名にマップされる必要があります。一般的な形式は alias@domain です。このドメインは、検証済みドメインのテナントのコレクション内に存在している必要があります。このプロパティは、ユーザーの作成時に必要です。テナントの検証済みのドメインには、[organization](organization.md) の **verifiedDomains** プロパティからアクセスできます。$filter および $orderby をサポートします。
|userType|String|「メンバー」および"Guest"など、ディレクトリ内のユーザーの種類を分類するために使用する文字列値。 $filter をサポートします。          |

### <a name="legal-age-group-property-definitions"></a>法的年齢グループのプロパティの定義

この説明では、どのように 3 つの年齢グループのプロパティ (`legalAgeGroupClassification`、`ageGroup`と`consentProvidedForMinor`) 時代に関連する規制を満たすために、Azure AD の管理者とエンタープライズ アプリケーションの開発者によって使用されます。

例: ある Cameron は、英国の Holyport で、小学生用のディレクトリの管理者です。 学校年度の開始時のマイナーの親が愛知県の年齢関連の規制に基づく承認を取得するのには来園者の書類を使用しました。 親から取得した同意は、Holyport の学校およびマイクロソフトのアプリケーションで使用される、マイナーのアカウントを使用できます。 ある Cameron は、すべてのアカウントを作成し、「小さな」に ageGroup と consentProvidedForMinor を「許可」に設定します。 自分の受講者が使用するアプリケーションでは、未成年者が適切ではないフィーチャーを抑制すること、です。

#### <a name="legal-age-group-classification"></a>法的年齢グループの分類

エンタープライズ アプリケーションの開発者がこの読み取り専用プロパティを使用して、年齢、法律に基づいて、ユーザーの適切に処理できるように。 ユーザーの基に計算、`ageGroup`と`consentProvidedForMinor`のプロパティです。

| 値   | # |説明|
|:---------------|:--------|:----------|
|null|0|既定値は no`ageGroup`ユーザー用に設定されています。|
|minorWithoutParentalConsent |1|(将来使用するために予約されています)|
|minorWithParentalConsent|2| ユーザーが自分の国の年齢関連の規制に基づき、マイナーと見なされます。 または地域、およびアカウントの管理者から入手して適切な同意、親か保護者です。|
|成人向けコンテンツ|3|ユーザーには、自分の国または地域の年齢関連の規制に基づく成人と見なされます。|
|notAdult|4|ユーザーから国または地域を持つその他の有効期間に関連する規制 (米国、英国、欧州連合または (韓国)) は、ユーザーの年齢を副専攻と成人向けの有効期間の間 (として規定に基づいて国や地域)。 通常、これは、10 代の若者と見なされます`notAdult`規制対象国にします。|
|minorNoParentalConsentRequired|5|ユーザーは、マイナーでは、国または地域の時代に関連する規制がないからです。|

#### <a name="age-group-and-minor-consent"></a>年齢グループおよびマイナーの同意

年齢グループおよびマイナーの同意のプロパティは、Azure AD の管理者アカウントの使用が正しく、年齢に関連する規制のルールに基づいてユーザーの国または地域を制御する処理を確実に使用する省略可能なプロパティです。

#### <a name="agegroup-property"></a>ageGroup プロパティ

| 値    | # |説明|
|:---------------|:--------|:----------|
|null|0|既定値は no`ageGroup`ユーザー用に設定されています。|
|マイナー|1|ユーザーが副専攻を検討してください。|
|notAdult|2|ユーザーは、米国、英国、欧州連合、または韓国の法律上の規制のある国からは)、ユーザーの年齢 (国) に子供の年齢の上限を超えると成人の年齢の下限よりも小さい (として規定に基づいて国や地域). として 10 代の若者が考慮されるように基本的には、`notAdult`規制対象国にします。|
|成人向けコンテンツ|3|ユーザーは、大人として扱われる必要があります。|

#### <a name="consentprovidedforminor-property"></a>consentProvidedForMinor プロパティ

| 値    | # |説明|
|:---------------|:--------|:----------|
|null|0|既定値は no`consentProvidedForMinor`ユーザー用に設定されています。|
|付与|1|アカウントのユーザーの同意を受けています。|
|denied|2|アカウントのユーザーの同意が取得されていません。|
|必要ありません。|3|ユーザーは、同意を必要としない場所です。|

## <a name="relationships"></a>リレーションシップ

| リレーションシップ | 型 |説明|
|:---------------|:--------|:----------|
|agreementAcceptances|[agreementAcceptance](agreementacceptance.md)コレクション| 使用の承認の状態のユーザーの条件です。 読み取り専用です。 Null 許容型。|
|予定表|[calendar](calendar.md)|ユーザーの標準予定表。読み取り専用です。|
|calendarGroups|[calendarGroup](calendargroup.md)コレクション|ユーザーの予定表グループ。読み取り専用です。Null 許容型。|
|calendarView|[event](event.md) コレクション|予定表のカレンダー ビュー。読み取り専用です。Null 許容型。|
|calendars|[calendar](calendar.md) collection|ユーザーの予定表。読み取り専用です。Null 許容型。|
|contactFolders|[contactFolder](contactfolder.md)コレクション|ユーザーの連絡先フォルダー。読み取り専用です。Null 許容型。|
|contacts|[contact](contact.md)コレクション|ユーザーの連絡先。読み取り専用です。Null 許容型。|
|createdObjects|[directoryObject](directoryobject.md) コレクション|ユーザーによって作成されたディレクトリ オブジェクト。読み取り専用です。Null 許容型。|
|directReports|[directoryObject](directoryobject.md) collection|そのユーザーの部下であるユーザーと連絡先。(マネージャー プロパティがこのユーザーに設定されている、ユーザーと連絡先。)読み取り専用です。Null 許容型。 |
|ドライブ|[drive](drive.md)|ユーザーの OneDrive。読み取り専用です。|
|events|[event](event.md) コレクション|ユーザーのイベント。既定は、既定の予定表でイベントを表示します。読み取り専用です。Null 許容型。|
|extensions|[extension](extension.md) コレクション|開いている拡張機能がユーザーの定義のコレクションです。 Null 許容型。|
|inferenceClassification|[inferenceClassification](inferenceclassification.md)| 明示的な指定に基づく、ユーザーのメッセージの関連性の分類。明示的な指定は、推定される関連性や重要性より優先されます。 |
|洞察|[情報](insights.md)のコレクション| 読み取り専用。Null 許容型。|
|joinedGroups|[group](group.md) コレクション| 読み取り専用。Null 許容型。|
|mailFolders|[mailFolder](mailfolder.md) コレクション| ユーザーのメール フォルダー。読み取り専用です。Null 許容型。|
|manager|[directoryObject](directoryobject.md)|このユーザーの上司であるユーザーまたは連絡先。読み取り専用です。(HTTP メソッド:GET、PUT、DELETE)|
|memberOf|[directoryObject](directoryobject.md) コレクション|ユーザーがメンバーになっているグループ、ディレクトリ ロール、および管理単位。読み取り専用。Null 許容型。|
|joinedTeams|[group](group.md) コレクション|ユーザーがのメンバーであるマイクロソフトのチームです。 読み取り専用です。 Null 許容型。|
|messages|[message](message.md) コレクション|メールボックスまたはフォルダー内のメッセージ。読み取り専用です。Null 許容型。|
|onenote|[OneNote](onenote.md)| 読み取り専用です。|
|outlook|[outlookUser](outlookuser.md)| 選択 Outlook サービス ユーザーが利用できます。 読み取り専用です。 Null 許容型。|
|ownedDevices|[directoryObject](directoryobject.md) コレクション|ユーザーが所有しているデバイス。読み取り専用です。Null 許容型。|
|ownedObjects|[directoryObject](directoryobject.md) コレクション|ユーザーが所有しているディレクトリ オブジェクト。読み取り専用です。Null 許容型。|
|people|[人](person.md)コレクション| 読み取り専用。ユーザーに最も関連のある人。コレクションは、ユーザーに対する関連 (ユーザーの通信、コラボレーション、およびビジネス リレーションシップによって決まる) を基準として配列されます。person は、メール、連絡先、およびソーシャル ネットワークのすべてからの情報の集約です。|
|photo|[profilePhoto](profilephoto.md)| ユーザーのプロフィール写真。読み取り専用です。|
|Photos|[Photo](photo.md) コレクション| 読み取り専用。Null 許容型。|
|プランナー|[plannerUser](planneruser.md)| 選択的プランナー サービス ユーザーが利用できます。 読み取り専用です。 Null 許容型。 |
|sharepoint|[sharepoint](sharepoint.md)| ユーザーの SharePoint サイトにアクセスします。読み取り専用。 |
|scopedRoleMemberOf|[scopedRoleMembership](scopedrolemembership.md) コレクション| このユーザーのスコープ役割の管理単位のメンバーシップ。 読み取り専用です。 Null 許容型。|
|settings|[設定](user-settings.md)コレクション| 読み取り専用。Null 許容型。|
|registeredDevices|[directoryObject](directoryobject.md) コレクション|ユーザーについて登録されているデバイス。読み取り専用です。Null 許容型。|

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
    "joinedTeams",
    "messages",
    "onenote",
    "oauth2PermissionGrants",
    "outlook",
    "ownedDevices",
    "ownedObjects",
    "photo",
    "registeredDevices"
  ],
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.user"
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
  "deletedDateTime": "String (timestamp)",
  "department": "string",
  "displayName": "string",
  "externalUserState": "PendingAcceptance",
  "externalUserStateChangeDateTime": "2018-11-12T01:13:13Z",
  "givenName": "string",
  "hireDate": "String (timestamp)",
  "id": "string (identifier)",
  "interests": ["string"],
  "jobTitle": "string",
  "legalAgeGroupClassification": "string",
  "licenseAssignmentStates": [{"@odata.type": "microsoft.graph.licenseAssignmentState"}],
  "mail": "string",
  "mailboxSettings": {"@odata.type": "microsoft.graph.mailboxSettings"},
  "mailNickname": "string",
  "mobilePhone": "string",
  "mySite": "string",
  "officeLocation": "string",
  "onPremisesExtensionAttributes": {"@odata.type": "microsoft.graph.onPremisesExtensionAttributes"},
  "onPremisesImmutableId": "string",
  "onPremisesLastSyncDateTime": "String (timestamp)",
  "onPremisesProvisioningErrors": [{"@odata.type": "microsoft.graph.onPremisesProvisioningError"}],
  "onPremisesSecurityIdentifier": "string",
  "onPremisesSyncEnabled": true,
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
  "insights": { "@odata.type": "microsoft.graph.officeGraphInsights" },
  "settings": { "@odata.type": "microsoft.graph.userSettings" },
  "events": [ { "@odata.type": "microsoft.graph.event" } ],
  "extensions": [ { "@odata.type": "microsoft.graph.extension" } ],
  "inferenceClassification": { "@odata.type": "microsoft.graph.inferenceClassification" },
  "mailFolders": [ { "@odata.type": "microsoft.graph.mailFolder" } ],
  "manager": { "@odata.type": "microsoft.graph.directoryObject" },
  "memberOf": [ { "@odata.type": "microsoft.graph.directoryObject" } ],
  "joinedTeams": [ { "@odata.type": "microsoft.graph.group" } ],
  "messages": [ { "@odata.type": "microsoft.graph.message" } ],
  "outlook": { "@odata.type": "microsoft.graph.outlookUser" },
  "ownedDevices": [ { "@odata.type": "microsoft.graph.directoryObject" } ],
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
  "section": "documentation",
  "tocPath": ""
}-->
