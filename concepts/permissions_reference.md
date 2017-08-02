# <a name="microsoft-graph-permissions-reference"></a>Microsoft Graph のアクセス許可のリファレンス 
Microsoft Graph は、アプリがアクセスするリソース (ユーザー、グループ、メールなど) を制御する詳細なアクセス許可を公開しています。開発者は、アプリが要求する Microsoft Graph のアクセス許可を決定します。そのアクセス許可に同意するかどうかは、アプリにサインインするときに、ユーザー (場合によっては管理者) が決定します。ユーザーが同意すると、アプリは、そのアプリが必要としているリソースと API にアクセスできるようになります。サインインしているユーザーを必要としないアプリの場合、アクセス許可は、アプリのインストール時またはサインアップ時に管理者が事前に同意できます。 

## <a name="delegated-permissions-application-permissions-and-effective-permissions"></a>委任されたアクセス許可、アプリケーションのアクセス許可、有効なアクセス許可
Microsoft Graph には、「**委任されたアクセス許可**」と「**アプリケーションのアクセス許可**」という 2 種類のアクセス許可があります。 

- **委任されたアクセス許可**は、サインインしているユーザーが存在するアプリで使用します。これに該当するアプリの場合は、ユーザーまたは管理者がアプリの要求するアクセス許可に同意します。アプリには、Microsoft Graph の呼び出し時に、サインインしているユーザーとして動作するためのアクセス許可が委任されます。一部の委任されたアクセス許可は非管理ユーザーの同意によって付与されますが、高度な特権が付与されるアクセス許可には管理者の同意が必要になります。  

- **アプリケーションのアクセス許可**は、サインインしているユーザーが存在しないアプリで使用します。たとえば、バックグラウンド サービスやデーモンなどのアプリです。アプリケーションのアクセス許可は、管理者のみが同意できます。 

_有効なアクセス許可_は、アプリが Microsoft Graph に要求を出すときに付与されるアクセス許可です。アプリに付与される委任されたアクセス許可とアプリケーションのアクセス許可の相違点について理解することに加えて、Microsoft Graph の呼び出し時の有効なアクセス許可についても理解することが重要です。

- 委任されたアクセス許可の場合、アプリの_有効なアクセス許可_は、アプリに付与されている委任されたアクセス許可 (同意によって付与) と現在サインインしているユーザーの特権が重なる範囲に収まる最小権限になります。サインインしているユーザーよりも高い特権がアプリに付与されることはありません。組織では、サインインしているユーザーの特権は、ポリシーで決まることもあれば、1 つ以上の管理者ロールに含まれるメンバーシップで決まることもあります。管理者ロールの詳細については、「[Azure Active Directory での管理者ロールの割り当て](https://docs.microsoft.com/en-us/azure/active-directory/active-directory-assign-admin-roles)」を参照してください。<br/><br/>たとえば、委任されたアクセス許可として _User.ReadWrite.All_ がアプリに付与されているとします。通常、このアクセス許可は、組織内のすべてのユーザーのプロファイルを読み取り、更新するためのアクセス許可をアプリに付与します。サインインしているユーザーが全体管理者の場合、アプリは、組織内のすべてのユーザーのプロファイルを更新できるようになります。ただし、サインインしているユーザーが管理者ロールに含まれていない場合、アプリは、そのサインインしているユーザーのプロファイルのみを更新できるようになります。組織内の他のユーザーのプロファイルは更新できません。これは、アプリが代理するアクセス許可を持つユーザーに、そのような権限が付与されていないためです。
  
- アプリケーションのアクセス許可の場合、アプリの_有効なアクセス許可_は、そのアクセス許可が暗示する完全なレベルの権限になります。たとえば、アプリケーションのアクセス許可として _User.ReadWrite.All_ が付与されているアプリは、組織内のすべてのユーザーのプロファイルを更新できます。 

### <a name="microsoft-graph-permission-names"></a>Microsoft Graph のアクセス許可名
Microsoft Graph のアクセス許可名は、「_リソース.操作.制約_」という簡単なパターンに従います。たとえば、_User.Read_ ではサインインしているユーザーのプロファイルを読み取るためのアクセス許可を付与し、_User.ReadWrite_ ではサインインしているユーザーのプロファイルを読み取りおよび変更するためのアクセス許可を付与します。また、_Mail.Send_ ではサインインしているユーザーの代わりにメールを送信するためのアクセス許可を付与します。 

名前の_制約_要素は、ディレクトリ内でアプリがアクセスする可能性のある範囲を決定します。現在、Microsoft Graph は次に示す制約をサポートしています。 

* **All**: ディレクトリ内にある指定した種類のすべてのリソースに対して操作を実行するためのアクセス許可をアプリに付与します。たとえば、_User.Read.All_ は、ディレクトリ内のすべてのユーザーのプロファイルを読み取るための特権をアプリに付与することになります。 
* **Shared**: サインインしているユーザーと共有している別のユーザーのリソースに対して操作を実行するためアクセス許可をアプリに付与します。この制約は、主に Outlook のリソース (メール、カレンダー、連絡先など) に使用されます。たとえば、_Mail.Read.Shared_ は、サインインしているユーザーのメールボックス内のメールを読み取る特権に加えて、サインインしているユーザーと共有している組織内の別のユーザーのメールボックス内のメールも読み取る特権を付与します。
* **AppFolder**: OneDrive の専用フォルダー内でファイルを読み取りおよび書き込みするためのアクセス許可をアプリに付与します。この制約は、[ファイルのアクセス許可](#files-permissions)でのみ公開され、Microsoft アカウントでのみ有効です。
* **制限なし**が指定されると、アプリは、サインインしているユーザーが所有するリソースに限定した操作を実行するようになります。たとえば、_User.Read_ ではサインインしているユーザーのプロファイルのみを読み取る特権を付与し、_Mail.Read_ ではサインインしているユーザーのメールボックス内のメールのみを読み取るアクセス許可を付与します。

> **注**:委任されたシナリオでは、アプリに付与される有効なアクセス許可が、組織内のサインインしているユーザーの特権によって制限されることがあります。
> 

### <a name="microsoft-accounts-and-work-or-school-accounts"></a>Microsoft アカウントと職場または学校アカウント

すべてのアクセス許可が、Microsoft アカウントと職場または学校アカウントの両方で有効になるわけではない点に注意してください。それぞれのアクセス許可グループの「**備考**」を確認して、特定のアクセス許可が Microsoft アカウントと職場または学校アカウントのどちらで有効になるか、または両方で有効になるかを判断してください。 

### <a name="user-and-group-search-limitations-for-guest-users-in-organizations"></a>組織のゲスト ユーザーに対するユーザーとグループの検索の制限事項

ユーザーとグループの検索機能を使用すると、`/users` または `/groups` リソース セットに対するクエリ (例: `https://graph.microsoft.com/v1.0/users`) を実行して、アプリで組織のディレクトリ内のユーザーまたはグループを検索できるようになります管理者とユーザーは、どちらもこの機能を使用でますが、ゲスト ユーザーは使用できません。サインインしているユーザーがゲスト ユーザーの場合、アプリに付与されたアクセス許可に応じて、特定のユーザーまたはグループのプロファイルを読み取ることはできますが (例: `https://graph.microsoft.com/v1.0/users/241f22af-f634-44c0-9a15-c8cd2cea5531`)、複数のリソースを返す可能性のある `/users` または `/groups` リソース セットに対するクエリは実行できません。適切なアクセス許可があるアプリは、ナビゲーション プロパティのリンク (たとえば、`/users/{id}/directReports` や `/groups/{id}/members`) に従って取得するユーザーまたはグループのプロファイルの読み取りが可能になります。

---

## <a name="calendars-permissions"></a>カレンダーのアクセス許可

#### <a name="delegated-permissions"></a>委任されたアクセス許可

|   アクセス許可    |  表示文字列   |  説明 | 管理者の同意の要不要 |
|:-----------------------------|:-----------------------------------------|:-----------------|:-----------------|
| _Calendars.Read_ |    ユーザーのカレンダーの読み取り  | アプリは、ユーザーの予定表内のイベントを読み取ることができます。| 不要 |
| _Calendars.Read.Shared_ |    ユーザーのカレンダーと共有のカレンダーの読み取り | ユーザーがアクセスできるすべてのカレンダー (委任されたカレンダーと共有のカレンダーを含む) のイベントをアプリで読み取りできるようにします。 | 不要 |
| _Calendars.ReadWrite_ |    ユーザーのカレンダーへのフル アクセス  | ユーザーのカレンダー内のイベントをアプリで作成、読み取り、更新、削除できるようにします。 | 不要 |
| _Calendars.ReadWrite.Shared_ |    ユーザーのカレンダーと共有のカレンダーの読み取りと書き込み | アプリで、ユーザーがアクセス許可を得ているすべてのカレンダー内のイベントを作成、読み取り、更新、および削除できるようにします。これには、委任されたカレンダーと共有のカレンダーが含まれます。| 不要 |

#### <a name="application-permissions"></a>アプリケーションのアクセス許可

|   アクセス許可    |  表示文字列   |  説明 | 管理者の同意の要不要 |
|:-----------------------------|:-----------------------------------------|:-----------------|:-----------------|
| _Calendars.Read_ |    すべてのメールボックスにあるカレンダーの読み取り  | サインインしているユーザーなしで、すべてのカレンダーのイベントをアプリで読み取れるようにします。| 必要 |
| _Calendars.ReadWrite_ |    すべてのメールボックスにあるカレンダーの読み取りと書き込み | サインインしているユーザーなしで、すべての予定表のイベントをアプリで作成、読み取り、更新、および削除できるようにします。| 必要 |

### <a name="remarks"></a>注釈

_Calendars.Read.Shared_ および _Calendars.ReadWrite.Shared_ は、職場または学校アカウントでのみ有効です。その他すべてのアクセス許可は、Microsoft アカウントと職場または学校アカウントのどちらでも有効です。

### <a name="example-usage"></a>使用例

#### <a name="delegated"></a>委任

* _Calendars.Read_: ユーザーのカレンダーについて、2017 年 4 月 23 日から 2017 年 4 月 29 日までのイベントを取得します (`GET /me/calendarView?startDateTime=2017-04-23T00:00:00&endDateTime=2017-04-29T00:00:00`)。
* _Calendars.Read.Shared_: すべての出席者が出席可能な会議の日時を検索します (`POST /users/{id|userPrincipalName}/findMeetingTimes`)。
* _Calendars.ReadWrite_: ユーザーの予定表にイベントを追加します (`POST /me/events`)。

#### <a name="application"></a>アプリケーション

* _Calendars.Read_: bob@contoso.com が編成した会議室のカレンダーのイベントを検索します (`GET /users/{id | userPrincipalName}/events?$filter=organizer/emailAddress/address eq 'bob@contoso.com'`)。
* _Calendars.Read_: ユーザーのカレンダーにある 5 月のイベントをすべてリストします (`GET /users/{id | userPrincipalName}/calendarView?startDateTime=2017-05-01T00:00:00&endDateTime=2017-06-01T00:00:00`)
* _Calendars.ReadWrite_: 承認済みの休暇について、ユーザーのカレンダーにイベントを追加します (`POST /users/{id | userPrincipalName}/events`)。
* _Calendars.Send_: メッセージを送信します (`POST /users/{id | userPrincipalName}/sendCalendars`)。


より複雑な複数のアクセス許可を伴うシナリオについては、「[アクセス許可のシナリオ](#permission-scenarios)」を参照してください。

---

## <a name="contacts-permissions"></a>連絡先のアクセス許可

#### <a name="delegated-permissions"></a>委任されたアクセス許可

|   アクセス許可    |  表示文字列   |  説明 | 管理者の同意の要不要 |
|:-----------------------------|:-----------------------------------------|:-----------------|:-----------------|
| _Contacts.Read_ |    ユーザーの連絡先の読み取り  | アプリは、ユーザーの連絡先を読み取ることができます。 | 不要 |
| _Contacts.Read.Shared_ |    ユーザーの連絡先と共有の連絡先の読み取り | アプリで、ユーザー自身の連絡先と共有の連絡先を含む、ユーザーがアクセス許可を得ている連絡先を読み取ることができるようにします。 | 不要 |
| _Contacts.ReadWrite_ |    ユーザーの連絡先へのフル アクセス  | アプリで、ユーザーの連絡先の作成、読み取り、更新、削除を行えるようにします。 | 不要 |
| _Contacts.ReadWrite.Shared_ |    ユーザーの連絡先と共有の連絡先の読み取りと書き込み | アプリで、ユーザー自身の連絡先と共有の連絡先を含むユーザーがアクセス許可を得ている連絡先の作成、読み取り、更新、削除を行えるようにします。| 不要 |

#### <a name="application-permissions"></a>アプリケーションのアクセス許可

|   アクセス許可    |  表示文字列   |  説明 | 管理者の同意の要不要 |
|:-----------------------------|:-----------------------------------------|:-----------------|:-----------------|
| _Contacts.Read_ |    すべてのメールボックスにある連絡先の読み取り | サインインしているユーザーなしで、すべてのメールボックス内のすべての連絡先をアプリで読み取りできるようにします。 | 必要 |
| _Contacts.ReadWrite_ |    すべてのメールボックスにある連絡先の読み取りと書き込み  |サインインしているユーザーなしで、すべてのメールボックス内のすべての連絡先をアプリで作成、読み取り、更新、および削除できるようにします。| 必要 |

### <a name="remarks"></a>備考
Microsoft アカウントでは、委任されたアクセス許可の _Contacts.Read_ および _Contacts.ReadWrite_ のみが有効です。 

### <a name="example-usage"></a>使用例
#### <a name="delegated"></a>委任

* _Contacts.Read_: サインインしているユーザーの最上位レベルの連絡先フォルダーの 1 つから連絡先を読み取ります (`GET /me/contactfolders/{Id}/contacts/{id}`)。
* _Contacts.ReadWrite_: サインインしているユーザーの連絡先のうち、1 つの連絡先の写真を更新します (`PUT /me/contactfolders/{contactFolderId}/contacts/{id}/photo/$value`)。 
* _Contacts.ReadWrite_: サインインしているユーザーのルート フォルダーに連絡先を追加します (`POST /me/contacts`)。

#### <a name="application"></a>アプリケーション

* _Contacts.Read_: 組織内の任意のユーザーの最上位レベルの 1 つのフォルダーから連絡先を読み取ります (`GET /users/{id | userPrincipalName}/contactfolders/{Id}/contacts/{id}`)。 
* _Contacts.ReadWrite_: 組織内の任意のユーザーの連絡先の写真を更新します (`PUT /user/{id | userPrincipalName}/contactfolders/{contactFolderId}/contacts/{id}/photo/$value`)。 
* _Contacts.ReadWrite_: 組織内の任意のユーザーのルート フォルダーに連絡先を追加します (`POST /users/{id | userPrincipalName}/contacts`)。

より複雑な複数のアクセス許可を伴うシナリオについては、「[アクセス許可のシナリオ](#permission-scenarios)」を参照してください。

---

## <a name="device-permissions"></a>デバイス アクセス許可

#### <a name="delegated-permissions"></a>委任されたアクセス許可

|   アクセス許可    |  表示文字列   |  説明 | 管理者の同意が必要 |
|:-----------------------------|:-----------------------------------------|:-----------------|:-----------------|
| _Device.Read_ | ユーザー デバイスの読み取り | サインインしているユーザーの代わりに、アプリでユーザーのデバイスの一覧を読み取ることができるようにします。 | いいえ |
| _Device.Command_ | ユーザーのデバイスとの通信 | サインインしているユーザーの代わりに、アプリで、別のアプリを起動するか、ユーザーのデバイス上にある別のアプリと通信できるようにします。 | いいえ |


#### <a name="application-permissions"></a>アプリケーションのアクセス許可

|   アクセス許可    |  表示文字列   |  説明 | 管理者の同意の要不要 |
|:-----------------------------|:-----------------------------------------|:-----------------|:-----------------|
| _Device.ReadWrite.All_ | デバイスの読み取りと書き込み | アプリで、サインインしているユーザーなしで、すべてのデバイス プロパティの読み取りと書き込みができるようにします。デバイスの作成、デバイスの削除、デバイスの代替セキュリティ識別子の更新はできません。 | 必要 |

### <a name="remarks"></a>備考

委任されたアクセス許可の _Device.Read_ と _Device.Command_ は、個人用の Microsoft アカウントに対してのみ有効です。

### <a name="example-usage"></a>使用例
#### <a name="application"></a>アプリケーション

* _Device.ReadWrite.All_: 組織内のすべての登録済デバイスを読み取ります (`GET /devices`)。

より複雑な複数のアクセス許可を伴うシナリオについては、「[アクセス許可のシナリオ](#permission-scenarios)」を参照してください。

---

## <a name="microsoft-intune-device-management-permissions"></a>Microsoft Intune デバイス管理のアクセス許可

#### <a name="delegated-permissions"></a>委任されたアクセス許可

なし。

#### <a name="application-permissions"></a>アプリケーションのアクセス許可

|   アクセス許可    |  表示文字列   |  説明 | 管理者の同意の要不要 |
|:-----------------------------|:-----------------------------------------|:-----------------|:-----------------|
| _DeviceManagementServiceConfiguration.Read.All_ | Microsoft Intune 構成の読み取り (プレビュー) | アプリで、デバイスの登録やサード パーティのサービスの接続構成を含む Microsoft Intune サービスのプロパティを読み取れるようにします。 | 必要 |
| _DeviceManagementServiceConfiguration.ReadWrite.All_ | Microsoft Intune 構成の読み取りおよび書き込み (プレビュー) | アプリで、デバイスの登録やサード パーティのサービスの接続構成を含む Microsoft Intune サービスのプロパティを読み書きできるようにします。 | 必要 |
| _DeviceManagementConfiguration.Read.All_ | Microsoft Intune のデバイスの構成とポリシーの読み取り (プレビュー) | アプリで、Microsoft Intune で管理されるデバイス構成のプロパティおよびデバイスのコンプライアンス ポリシーとそのポリシーのグループへの割り当てを読み取れるようにします。 | 必要 |
| _DeviceManagementConfiguration.ReadWrite.All_ | Microsoft Intune のデバイスの構成とポリシーの読み取りおよび書き込み (プレビュー) | アプリで、Microsoft Intune で管理されるデバイスの構成のプロパティおよびデバイスのコンプライアンス ポリシーとそのポリシーのグループへの割り当てを読み書きできるようにします。 | 必要 |
| _DeviceManagementApps.Read.All_ | Microsoft Intune アプリの読み取り (プレビュー) | アプリで、Microsoft Intune で管理されるアプリ、アプリの構成、アプリ保護ポリシーについて、プロパティ、グループの割り当て、状態を読み取れるようにします。 | 必要 |
| _DeviceManagementApps.ReadWrite.All_ | Microsoft Intune アプリの読み取りおよび書き込み (プレビュー) | アプリで、Microsoft Intune で管理されるアプリ、アプリの構成、アプリ保護ポリシーについて、プロパティ、グループの割り当て、状態を読み書きできるようにします。 | 必要 |
| _DeviceManagementRBAC.Read.All_ | Microsoft Intune RBAC の設定の読み取り (プレビュー) | アプリで、Microsoft Intune のロール ベースのアクセス制御 (RBAC) の設定に関連するプロパティを読み取れるようにします。 | 必要 |
| _DeviceManagementRBAC.ReadWrite.All_ | Microsoft Intune RBAC の設定の読み取りおよび書き込み (プレビュー) | アプリで、Microsoft Intune のロール ベースのアクセス制御 (RBAC) の設定に関連するプロパティを読み書きできるようにします。 | 必要 |
| _DeviceManagementManagedDevices.Read.All_ | Microsoft Intune デバイスの読み取り (プレビュー) | アプリで、Microsoft Intune で管理されるデバイスのプロパティを読み取れるようにします。 | 必要 |
| _DeviceManagementManagedDevices.ReadWrite.All_ | Microsoft Intune デバイスの読み取りおよび書き込み (プレビュー) | アプリで、Microsoft Intune で管理されるデバイスのプロパティを読み書きできるようにします。リモート ワイプやデバイスの所有者のパスワードのリセットなど、影響の大きい操作は許可されません。 | 必要 |
| _DeviceManagementManagedDevices.PrivilegedOperations.All_ | Microsoft Intune デバイスでユーザーに影響を与えるリモート操作を実行する (プレビュー) | アプリで、デバイスのワイプや Microsoft Intune で管理されるデバイスのパスコードのリセットなど、影響の大きいリモート操作を実行できるようにします。 | 必要 |

### <a name="remarks"></a>注釈
> **注:**Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。

これらのアクセス許可は、職場または学校アカウントでのみ有効です。

### <a name="example-usage"></a>使用例
#### <a name="application"></a>アプリケーション

* _DeviceManagementServiceConfiguration.Read.All_: Intune サブスクリプションの現在の状態を確認します (`GET /deviceManagement/subscriptionState`)。
* _DeviceManagementServiceConfiguration.ReadWrite.All_: 新しい条項および条件を作成します (`POST /deviceManagement/termsAndConditions`)
* _DeviceManagementConfiguration.Read.All_: デバイス構成の状態を検索します (`GET /deviceManagement/deviceConfigurations/{id}/deviceStatuses`)
* _DeviceManagementConfiguration.ReadWrite.All_: デバイス コンプライアンス ポリシーをグループに割り当てます (`POST deviceCompliancePolicies/{id}/assign`)
* _DeviceManagementApps.Read.All_: Intune に公開したすべての Windows ストア アプリを検索します (`GET /deviceAppManagement/mobileApps?$filter=isOf('microsoft.graph.windowsStoreApp')`)
* _DeviceManagementApps.ReadWrite.All_: 新しいアプリケーションを公開します (`POST /deviceAppManagement/mobileApps`)
* _DeviceManagementRBAC.Read.All_: ロールの割り当てを名前で検索します (`GET /deviceManagement/roleAssignments?$filter=displayName eq 'My Role Assignment'`)
* _DeviceManagementRBAC.ReadWrite.All_: 新しいカスタム ロールを作成します (`POST /deviceManagement/roleDefinitions`)
* _DeviceManagementManagedDevices.Read.All_: 管理対象デバイスを名前で検索します (`GET /managedDevices/?$filter=deviceName eq 'My Device'`)
* _DeviceManagementManagedDevices.ReadWrite.All_: 管理対象デバイスを削除します (`DELETE /managedDevices/{id}`)
* _DeviceManagementManagedDevices.PrivilegedOperations.All_: ユーザーの管理対象デバイスのパスコードをリセットします (`POST /managedDevices/{id}/resetPasscode`)。

より複雑な複数のアクセス許可を伴うシナリオについては、「[アクセス許可のシナリオ](#permission-scenarios)」を参照してください。

---

## <a name="directory-permissions"></a>ディレクトリのアクセス許可

#### <a name="delegated-permissions"></a>委任されたアクセス許可

|   アクセス許可    |  表示文字列   |  説明 | 管理者の同意の要不要 |
|:-----------------------------|:-----------------------------------------|:-----------------|:-----------------|
| _Directory.Read.All_           |     ディレクトリ データの読み取り                     | アプリで、ユーザー、グループ、アプリなどの組織のディレクトリ内のデータを読み取ることができるようにします。 | 必要 |
| _Directory.ReadWrite.All_      |     ディレクトリ データの読み取りおよび書き込み           | アプリで、ユーザーやグループなどの組織のディレクトリ内のデータを読み書きできるようにします。アプリでユーザーまたはグループの削除や、ユーザー パスワードのリセットはできません。 | はい |
| _Directory.AccessAsUser.All_   |     ディレクトリに対するサインインしたユーザーと同じアクセス  | サインインしているユーザーと同じように、アプリでディレクトリ内の情報にアクセスできるようにします。| 必要 |

#### <a name="application-permissions"></a>アプリケーションのアクセス許可

|   アクセス許可    |  表示文字列   |  説明 | 管理者の同意の要不要 |
|:-----------------------------|:-----------------------------------------|:-----------------|:-----------------|
| _Directory.Read.All_ | ディレクトリ データの読み取り | サインインしているユーザーなしで、ユーザー、グループ、アプリなどの組織のディレクトリ内のデータをアプリで読み取りできるようにします。 | 必要 |
| _Directory.ReadWrite.All_ | ディレクトリ データの読み取りおよび書き込み | アプリで、サインインしているユーザーなしで、ユーザー、グループなどの組織のディレクトリ内のデータを読み取りと書き込みができるようにします。ユーザーまたはグループの削除はできません。 | 必要 |

### <a name="remarks"></a>備考
ディレクトリのアクセス許可は、Microsoft アカウントではサポートされていません。 

 ディレクトリのアクセス許可は、組織内のディレクトリ リソース ([ユーザー](../api-reference/v1.0/resources/user.md)、[グループ](../api-reference/v1.0/resources/group.md)、[デバイス](../api-reference/v1.0/resources/device.md)など) に対する最上位レベルの特権を提供します。また、その他のディレクトリ ソースへのアクセスを排他的に制御します。このリソースには、[組織の連絡先](../api-reference/beta/resources/orgcontact.md)、[スキーマ拡張 API](../api-reference/beta/resources/schemaextension.md)、[Privileged Identity Management (PIM) API](../api-reference/beta/resources/privilegedidentitymanagement_root.md) などに加え、v1.0 およびベータの API リファレンス ドキュメントの **Azure Active Directory** ノードにリストされる多数のリソースや API があります。これには、管理単位、ディレクトリ ロール、ディレクトリ設定など多くのものが含まれます。 

_Directory.ReadWrite.All_ アクセス許可は、次に示す特権を付与します。

- すべてのディレクトリ リソースの完全な読み取り (宣言されたプロパティとナビゲーション プロパティの両方) 
- ユーザーの作成と更新
- ユーザー (会社管理者以外) の無効化と有効化
- ユーザーの代替セキュリティ ID の設定 (管理者以外)
- グループの作成と更新
- グループ メンバーシップの管理
- グループ所有者の更新
- ライセンス割り当ての管理
- アプリケーションのスキーマ拡張の定義
- **注**:ユーザーのパスワードをリセットする権限はありません
- **注**:リソース (ユーザーまたはグループを含む) を削除する権限はありません
- **注**:具体的には、上記の一覧に示されていないリソースの作成と更新が除外されます。これには、application、oAauth2Permissiongrant、appRoleAssignment、device、servicePrincipal、organization、domains などが含まれます。
 

### <a name="example-usage"></a>使用例
#### <a name="delegated"></a>委任
* _Directory.Read.All_: 組織内のすべての管理単位をリストします (`GET /beta/administrativeUnits`)
* _Directory.ReadWrite.All_: ディレクトリ ロールにメンバーを追加します (`POST /directoryRoles/{id}/members/$ref`)

#### <a name="application"></a>アプリケーション
* _Directory.Read.All_: ディレクトリ ロールと管理単位を含むユーザーのメンバーシップをすべてリストします (`GET /beta/users/{id}/memberOf`)
* _Directory.Read.All_: サービス プリンシパルを含むグループ メンバーをすべてリストします (`GET /beta/groups/{id}/members`)
* _Directory.ReadWrite.All_: グループに所有者を追加します (`POST /groups/{id}/owners/$ref`)


より複雑な複数のアクセス許可を伴うシナリオについては、「[アクセス許可のシナリオ](#permission-scenarios)」を参照してください。

---

## <a name="files-permissions"></a>ファイルのアクセス許可

#### <a name="delegated-permissions"></a>委任されたアクセス許可

|   アクセス許可    |  表示文字列   |  説明 | 管理者の同意の要不要 |
|:-----------------------------|:-----------------------------------------|:-----------------|:-----------------|
| _Files.Read_ |    ユーザー ファイルの読み取り | アプリで、サインインしているユーザーのファイルを読み取れるようにします。| 不要 |
| _Files.Read.All_ | ユーザーがアクセスできるすべてのファイルの読み取り | アプリで、サインしているユーザーがアクセスできるすべてのファイルを読み取ることができるようにします。 | 不要 |
| _Files.ReadWrite_ |   ユーザー ファイルへのフル アクセスを持つ | アプリで、サインインしているユーザーのファイルを読み取り、作成、更新、および削除できるようにします。 | 不要 |
| _Files.ReadWrite.All_ | ユーザーがアクセスできるすべてのファイルへのフル アクセス | アプリで、サインインしているユーザーがアクセス可能なすべてのファイルを読み取り、作成、更新、および削除できるようにします。 | 不要 |
| _Files.ReadWrite.AppFolder_ | アプリケーションのフォルダーへのフル アクセス (プレビュー) | (プレビュー) アプリで、アプリケーションのフォルダー内のファイルを読み取り、作成、更新、および削除できるようにします。 | 不要 |
| _Files.Read.Selected_ |    ユーザーが選んだファイルの読み取り (プレビュー) | **Microsoft Graph の限定的なサポート (「備考」を参照)** <br/> (プレビュー) ユーザーが選んだファイルをアプリで読み取りできるようにします。アプリは、ユーザーがファイルを選んでから数時間後までアクセス許可を持ちます。 | いいえ |
| _Files.ReadWrite.Selected_ |    ユーザーが選んだファイルの読み取りと書き込み (プレビュー) | **Microsoft Graph の限定的なサポート (「備考」を参照)** <br/> (プレビュー) ユーザーが選んだファイルをアプリで読み書きできるようにします。アプリは、ユーザーがファイルを選んでから数時間後までアクセス許可を持ちます。 | いいえ |

#### <a name="application-permissions"></a>アプリケーションのアクセス許可

|   アクセス許可    |  表示文字列   |  説明 | 管理者の同意の要不要 |
|:-----------------------------|:-----------------------------------------|:-----------------|:-----------------|
| _Files.Read.All_ | すべてのサイト コレクションにおけるファイルの読み取り (プレビュー) | (プレビュー) サインインしているユーザーなしで、すべてのサイト コレクション内のすべてのファイルをアプリで読み取れるようにします。 | 必要 |
| _Files.ReadWrite.All_ | すべてのサイト コレクションにおけるファイルの読み取りと書き込み (プレビュー) | **Microsoft Graph の限定的なサポート** <br/> (プレビュー) サインインしているユーザーなしで、すべてのサイトコレクション内のすべてのファイルをアプリで読み取り、作成、更新、および削除できるようにします。 | 必要 |

### <a name="remarks"></a>注釈

委任されたアクセス許可の Files.Read、Files.ReadWrite、Files.Read.All、および Files.ReadWrite.All は、個人用の Microsoft アカウントと職場または学校アカウントの両方で有効です。個人用アカウントの場合、Files.Read および Files.ReadWrite はサインインしているユーザーと共有しているファイルへのアクセスも許可される点に注意してください。 

委任されたアクセス許可の Files.Read.Selected および Files.ReadWrite.Selected は、職場または学校アカウントでのみ有効です。また、[Office 365 ファイル ハンドラー (v1.0)](https://msdn.microsoft.com/office/office365/howto/using-cross-suite-apps) を使用している場合にのみ公開されます。これらは、Microsoft Graph API を直接呼び出すために使用しないでください。 

委任されたアクセス許可の Files.ReadWrite.AppFolder は、個人用アカウントでのみ有効です。また、OneDrive の[特殊フォルダーを取得する](../api-reference/v1.0/api/drive_special.md) Microsoft Graph API で [App Root 特殊フォルダー](https://dev.onedrive.com/items/special_folders.htm)にアクセスする場合に使用します。

アプリケーションアクセス許可の Files.ReadWrite.All は、OneDrive の[再開可能なアップロード セッションを作成する ](../api-reference/v1.0/api/item_createuploadsession.md) Microsoft Graph API では、まだサポートされていません。近日中にフル サポートされる予定です。 

### <a name="example-usage"></a>使用例
#### <a name="delegated"></a>委任

* _Files.Read_: サインインしているユーザーの OneDrive に保存されているファイルを読み取ります (`GET /me/drive/root/children`)
* _Files.Read.All_: サインインしているユーザーと共有しているファイルを読み取ります (`GET /me/drive/root/sharedWithMe`)
* _Files.ReadWrite_: サインインしているユーザーの OneDrive にファイルを書き込みます (`PUT /me/drive/root/children/filename.txt/content`)
* _Files.ReadWrite.All_: ユーザーと共有するファイルを書き込みます (`PUT /users/rgregg@contoso.com/drive/root/children/file.txt/content`)
* _Files.ReadWrite.AppFolder_: OneDrive 内のアプリのフォルダーにファイルを書き込みます (`PUT /me/drive/special/approot/children/file.txt/content`)

より複雑な複数のアクセス許可を伴うシナリオについては、「[アクセス許可のシナリオ](#permission-scenarios)」を参照してください。

---

## <a name="group-permissions"></a>グループのアクセス許可

#### <a name="delegated-permissions"></a>委任されたアクセス許可

|   アクセス許可    |  表示文字列   |  説明 | 管理者の同意の要不要 |
|:-----------------------------|:-----------------------------------------|:-----------------|:-----------------|
| _Group.Read.All_ |    すべてのグループの読み取り | アプリで、サインインしているユーザーの代わりに、グループを一覧表示し、グループのプロパティとすべてのグループ メンバーシップを読み取ることができるようにします。アプリで、サインインしているユーザーがアクセスできるすべてのグループの予定表、会話、ファイル、およびその他のグループのコンテンツを読み取ることができるようにします。 | 必要 |
| _Group.ReadWrite.All_ |    すべてのグループの読み取りと書き込み| アプリで、サインインしているユーザーの代わりに、グループを作成したり、すべてのグループのプロパティとメンバーシップを読み取ったりできるようにします。さらに、グループの所有者が自身のグループを管理できるよう、またグループ メンバーがグループのコンテンツを更新できるようにします。 | 必要 |

#### <a name="application-permissions"></a>アプリケーションのアクセス許可

|   アクセス許可    |  表示文字列   |  説明 | 管理者の同意の要不要 |
|:-----------------------------|:-----------------------------------------|:-----------------|:-----------------|
| _Group.Read.All_ | すべてのグループの読み取り | アプリで、サインインしているユーザーなしで、すべてのグループのメンバーシップを読み取れるようにします。すべてのグループ API が、アプリ専用のアクセス許可を使用したアクセスをサポートするわけではないことに注意してください。例については、「[既知の問題](../concepts/known_issues.md)」を参照してください。 | 必要 |
| _Group.ReadWrite.All_ | すべてのグループの読み取りと書き込み | アプリで、グループの作成、グループ メンバーシップの読み取りと更新、グループの削除ができるようにします。これらの操作はすべて、サインインしているユーザーなしで、アプリで実行できます。すべてのグループ API が、アプリ専用のアクセス許可を使用したアクセスをサポートするわけではないことに注意してください。例については、「[既知の問題](../concepts/known_issues.md)」を参照してください。| 必要 |


### <a name="remarks"></a>備考

グループ機能は、Microsoft アカウントではサポートされません。 

Office 365 グループの場合は、グループのアクセス許可により、グループのコンテンツ (会話、ファイル、メモなど) へのアクセスがアプリに許可されます。また、グループのアクセス許可は、[Microsoft Planner](../api-reference/beta/resources/planner_overview.md) のリソースと API へのアクセスを制御するためにも使用されます。

アプリケーションのアクセス許可については、サポートされる API についていくつかの制限があります。詳細については、「[既知の問題](../concepts/known_issues.md)」を参照してください。

場合によっては、アプリは一部のグループ プロパティ (`member` や `memberOf` など) の読み取りに[ディレクトリのアクセス許可](#directory-permissions)を必要とすることがあります。たとえば、グループにメンバーとして 1 つ以上の [servicePrincipals](../api-reference/beta/resources/serviceprincipal.md) が含まれている場合、アプリは _Directory.\*_ アクセス許可のいずれかによって付与されるサービス プリンシパルを読み取るための有効なアクセス許可が必要になります。このアクセス許可がない場合、Microsoft Graph はエラーを返します (委任されたアクセス許可の場合、サインインしているユーザーも、サービス プリンシパルを読み取るために、組織内の十分な権限が必要です)。同様のガイダンスは、[administrativeUnits](../api-reference/beta/resources/administrativeunit.md) を返す `memberOf` プロパティにも当てはまります。

### <a name="example-usage"></a>使用例
#### <a name="delegated"></a>委任

* _Group.Read.All_: サインインしているユーザーがメンバーになっているすべての Office 365 グループを読み取ります (`GET /me/memberOf/$/microsoft.graph.group?$filter=groupTypes/any(a:a%20eq%20'unified')`)。
* _Group.Read.All_: すべての Office 365 グループ コンテンツ (会話など) を読み取ります (`GET /groups/{id}/conversations`)。
* _Group.ReadWrite.All_: グループ プロパティ (photo など) を更新します (`PUT /groups/{id}/photo/$value`)。
* _Group.ReadWrite.All_: グループ メンバーを更新します (`POST /groups/{id}/members/$ref`)。注:これには、メンバーとして追加するユーザーを読み取るための _User.ReadBasic.All_ も必要になります。

#### <a name="application"></a>アプリケーション

* _Group.Read.All_: 名前が 'Sales' で始まるグループをすべて検索します (`GET /groups?$filter=startswith(displayName,'Sales')`)。
* _Group.ReadWrite.All_: デーモン サービスにより、Office 365 グループの予定表に新しいイベントを作成します (`POST /groups/{id}/events`)。

より複雑な複数のアクセス許可を伴うシナリオについては、「[アクセス許可のシナリオ](#permission-scenarios)」を参照してください。

---

## <a name="identity-risk-event-permissions"></a>ID リスク イベントのアクセス許可

#### <a name="delegated-permissions"></a>委任されたアクセス許可

|   アクセス許可    |  表示文字列   |  説明 | 管理者の同意の要不要 |
|:-----------------------------|:-----------------------------------------|:-----------------|:-----------------|
| _IdentityRiskEvent.Read.All_ |   ID リスク イベント情報の読み取り  | アプリで、サインインしているユーザーの代わりに、組織内のすべてのユーザーの ID リスク イベント情報を読み取れるようにします。 | 必要 |

#### <a name="application-permissions"></a>アプリケーションのアクセス許可

|   アクセス許可    |  表示文字列   |  説明 | 管理者の同意の要不要 |
|:-----------------------------|:-----------------------------------------|:-----------------|:-----------------|
| _IdentityRiskEvent.Read.All_ |   ID リスク イベント情報の読み取り | サインインしているユーザーなしで、組織内のすべてのユーザーの ID リスク イベント情報をアプリで読み取れるようにします。 | 必要 |


### <a name="remarks"></a>注釈

_IdentityRiskEvent.Read.All_ は、職場または学校アカウントでのみ有効です。委任されたアクセス許可があるアプリの場合、ID リスク情報を読み取るには、サインインしているユーザーが「全体管理者」、「セキュリティ管理者」、または「セキュリティ閲覧者」のいずれかの管理者ロールのメンバーになっている必要があります。管理者ロールの詳細については、「[Azure Active Directory での管理者ロールの割り当て](https://docs.microsoft.com/azure/active-directory/active-directory-assign-admin-roles)」を参照してください。

### <a name="example-usage"></a>使用例
#### <a name="delegated-and-application"></a>委任およびアプリケーション
次に示す使用法は、委任されたアクセス許可とアプリケーションのアクセス許可のどちらでも有効です。

* テナント内のすべてのユーザーに対して生成されたすべてのリスク イベントを読み取ります (`GET /beta/identityRiskEvents`)
* Dorknet ボンネットで生成されたマルウェア リスク イベントを読み取ります (`GET /beta/malwareRiskEvents?$filter=malwareName eq 'Dorkbot'`)
* 最新の 50 件のリスク イベントを読み取ります (`GET /beta/identityRiskEvents?$orderBy=riskEventDateTime desc&top=50`)
 
より複雑な複数のアクセス許可を伴うシナリオについては、「[アクセス許可のシナリオ](#permission-scenarios)」を参照してください。

---

## <a name="mail-permissions"></a>メールのアクセス許可

#### <a name="delegated-permissions"></a>委任されたアクセス許可

|   アクセス許可    |  表示文字列   |  説明 | 管理者の同意の要不要 |
|:-----------------------------|:-----------------------------------------|:-----------------|:-----------------|
| _Mail.Read_ |    ユーザー メールの読み取り | アプリで、ユーザー メールボックス内のメールを読み取ることができるようにします。 | 不要 |
| _Mail.ReadWrite_ |    ユーザーのメールの読み取りおよび書き込みアクセス許可 | アプリで、ユーザー メールボックス内のメールの作成、読み取り、更新、削除を行えるようにします。メールを送信するためのアクセス許可は含まれません。| いいえ |
| _Mail.Read.Shared_ |    ユーザーのメールと共有のメールの読み取り | アプリで、ユーザー自身のメールと共有のメールを含む、ユーザーがアクセス許可を得ているメールを読み取れるようにします。 | 不要 |
| _Mail.ReadWrite.Shared_ |    ユーザーのメールと共有のメールの読み取りと書き込み | アプリで、ユーザー自身のメールと共有のメールを含むユーザーがアクセス許可を得ているメールの作成、読み取り、更新、削除を行えるようにします。メールを送信するためのアクセス許可は含まれません。 | 不要 |
| _Mail.Send_ |    ユーザーからのメールとして送信 | アプリで、組織内のユーザーとしてメールを送信できるようにします。 | 不要 |
| _Mail.Send.Shared_ |    他のユーザーに代わってメールを送信 | アプリで、他のユーザーの代理としての送信を含め、サインインしているユーザーとしてメールを送信できるようにします。 | 不要 |
| _MailboxSettings.Read_ |  ユーザーのメールボックス設定の読み取り | ユーザーのメールボックス設定をアプリで読み取れるようにします。メールを送信するためのアクセス許可は含まれません。 | いいえ |
| _MailboxSettings.ReadWrite_ |  ユーザーのメールボックス設定の読み取りと書き込み | アプリで、ユーザーのメールボックス設定の作成、読み取り、更新、削除を行えるようにします。メールを送信するためのアクセス許可は含まれません。 | いいえ |

#### <a name="application-permissions"></a>アプリケーションのアクセス許可

|   アクセス許可    |  表示文字列   |  説明 | 管理者の同意の要不要 |
|:-----------------------------|:-----------------------------------------|:-----------------|:-----------------|
| _Mail.Read_       |    すべてのメールボックスにあるメールの読み取り | サインインしているユーザーなしで、すべてのメールボックス内のメールをアプリで読み取れるようにします。| 必要 |
| _Mail.ReadWrite_ |    すべてのメールボックスにあるメールの読み取りと書き込み | サインインしているユーザーなしで、アプリですべてのメールボックス内のメールの作成、読み取り、更新、削除を行えるようにします。メールを送信するためのアクセス許可は含まれません。 | 必要 |
| _Mail.Send_ |    任意のユーザーからのメールを送信 | サインインしているユーザーなしで、任意のユーザーとしてアプリでメールを送信できるようにします。 | 必要 | 
| _MailboxSettings.Read_ |  すべてのユーザーのメールボックス設定の読み取り | サインインしているユーザーなしで、ユーザーのメールボックス設定をアプリで読み取れるようにします。メールを送信するためのアクセス許可は含まれません。 | いいえ |
| _MailboxSettings.ReadWrite_ | ユーザーのすべてのメールボックス設定の読み取りと書き込み  | サインインしているユーザーなしで、アプリでユーザーのメールボックス設定の作成、読み取り、更新、削除を行えるようにします。メールを送信するためのアクセス許可は含まれません。 | はい |

### <a name="remarks"></a>注釈

_Mail.Read.Shared_、_Mail.ReadWrite.Shared_、および _Mail.Send.Shared_ は、職場または学校アカウントでのみ有効です。その他すべてのアクセス許可は、Microsoft アカウントと職場または学校アカウントのどちらでも有効です。

アクセス許可の _Mail.Send_ または _Mail.Send.Shared_ があるアプリは、対応するアクセス許可の _Mail.ReadWrite_ または _Mail.ReadWrite.Shared_ を使用しない場合でも、メールの送信とユーザーの [送信済みアイテム] フォルダーへのコピーが可能になります。

### <a name="example-usage"></a>使用例

#### <a name="delegated"></a>委任

* _Mail.Read_: ユーザーのメールボックス内のメッセージを `receivedDateTime` で並べ替えてリストします (`GET /me/mailfolders/inbox/messages?$orderby=receivedDateTime DESC`)。
* _Mail.Read.Shared_: サインインしているユーザーと受信トレイを共有しているユーザーのメールボックス内にある添付ファイル付きのメッセージをすべて検索します (`GET /users{id | userPrincipalName}/mailfolders/inbox/messages?$filter=hasAttachments eq true`)。
* _Mail.ReadWrite_: メッセージに既読のマークを付けます (`PATCH /me/messages/{id}`)。
* _Mail.Send_: メッセージを送信します (`POST /me/sendmail`)。
* _MailboxSettings.ReadWrite_: ユーザーの自動応答を更新します (`PATCH /me/mailboxSettings`)。

#### <a name="application"></a>アプリケーション

* _Mail.Read_: bob@contoso.com からメッセージを検索します (`GET /users/{id | userPrincipalName}/messages?$filter=from/emailAddress/address eq 'bob@contoso.com'`)。
* _Mail.ReadWrite_: `Expense Reports` という名前の受信トレイに新しいフォルダーを作成します (`POST /users/{id | userPrincipalName}/mailfolders`)。
* _Mail.Send_: メッセージを送信します (`POST /users/{id | userPrincipalName}/sendmail`)。
* _MailboxSettings.Read_: ユーザーのメールボックスの既定のタイムゾーンを取得します (`GET /users/{id | userPrincipalName}/mailboxSettings/timeZone`)


より複雑な複数のアクセス許可を伴うシナリオについては、「[アクセス許可のシナリオ](#permission-scenarios)」を参照してください。

---

## <a name="member-permissions"></a>メンバーのアクセス許可

#### <a name="delegated-permissions"></a>委任されたアクセス許可

なし。

#### <a name="application-permissions"></a>アプリケーションのアクセス許可

|   アクセス許可    |  表示文字列   |  説明 | 管理者の同意の要不要 |
|:-----------------------------|:-----------------------------------------|:-----------------|:-----------------|
| _Member.Read.Hidden_ | すべての非表示のメンバーシップの読み取り | サインインしているユーザーなしで、非表示のグループのメンバーシップと管理単位をアプリで読み取れるようにします。 | 必要 |

### <a name="remarks"></a>注釈
一部の Office 365 グループのメンバーシップは非表示にできます。これは、そのメンバーを表示できるのは、そのグループのメンバーのみになるということです。この機能は、部外者にはグループのメンバーシップを隠すことを要求する組織の規制に従う際に役立ちます (たとえば、クラスに登録した学生を表す Office 365 グループなど)。

### <a name="example-usage"></a>使用例

#### <a name="application"></a>アプリケーション

* _Member.Read.Hidden_: メンバーシップが非表示になっている管理単位のメンバーを読み取ります (`GET /administrativeUnits/{id}/members`)。
* _Member.Read.Hidden_: メンバーシップが非表示になっているグループのメンバーを読み取ります (`GET /groups/{id}/members`)。

より複雑な複数のアクセス許可を伴うシナリオについては、「[アクセス許可のシナリオ](#permission-scenarios)」を参照してください。

---

## <a name="notes-permissions"></a>メモのアクセス許可
#### <a name="delegated-permissions"></a>委任されたアクセス許可

|   アクセス許可    |  表示文字列   |  説明 | 管理者の同意の要不要 |
|:-----------------------------|:-----------------------------------------|:-----------------|:-----------------|
| _Notes.Read_ |    ユーザーの OneNote ノートブックの読み取り | サインインしているユーザーの代わりに、アプリで OneNote ノートブックとセクションのタイトルの読み取りと、新しいページ、ノートブック、セクションの作成を実行できるようにします。 | 不要 |
| _Notes.Create_ |    ユーザーの OneNote ノートブックの作成 | サインインしているユーザーの代わりに、アプリで OneNote ノートブックとセクションのタイトルの読み取りと、新しいページ、ノートブック、セクションの作成を実行できるようにします。| 不要 |
| _Notes.ReadWrite_ |    ユーザーの OneNote ノートブックの読み取りと書き込み | サインインしているユーザーの代わりに、アプリで OneNote ノートブックの読み取り、共有、および変更を実行できるようにします。 | 不要 |
| _Notes.Read.All_ |    ユーザーがアクセスできるすべての OneNote ノートブックの読み取り | サインインしているユーザーがアクセスできる組織内の OneNote ノートブックをアプリで読み取れるようにします。 | 不要 |
| _Notes.ReadWrite.All_ |    ユーザーがアクセスできるすべての OneNote ノートブックの読み取りと書き込み | サインインしているユーザーがアクセスできる組織内の OneNote ノートブックの読み取り、共有、および変更をアプリで実行できるようにします。| 不要 |
| _Notes.ReadWrite.CreatedByApp_ |    ノートブックへの限定的なアクセス (非推奨) | **非推奨** <br/>使用しないでください。このアクセス許可によって付与される特権はありません。 | なし |

#### <a name="application-permissions"></a>アプリケーションのアクセス許可

|   アクセス許可    |  表示文字列   |  説明 | 管理者の同意の要不要 |
|:-----------------------------|:-----------------------------------------|:-----------------|:-----------------|
| _Notes.Read.All_ |    すべての OneNote ノートブックの読み取り | サインインしているユーザーなしで、組織内のすべての OneNote ノートブックをアプリで読み取れるようにします。 | 必要 |
| _Notes.ReadWrite.All_ |    すべての OneNote ノートブックの読み取りと書き込み | サインインしているユーザーなしで、組織内のすべての OneNote ノートブックをアプリで読み取り、共有、および変更できるようにします。| 必要 |


### <a name="remarks"></a>注釈
_Notes.Read.All_ および _Notes.ReadWrite.All_ は、職場または学校アカウントでのみ有効です。その他すべてのアクセス許可は、Microsoft アカウントと職場または学校アカウントのどちらでも有効です。

_Notes.Create_ のアクセス許可があるアプリは、サインインしているユーザーの OneNote ノートブック階層の表示と、OneNote コンテンツ (ノートブック、セクション グループ、セクション、ページなど) の作成を実行できます。

また、_Notes.ReadWrite_ および _Notes.ReadWrite.All_ によって、アプリはサインインしているユーザーがアクセス可能な OneNote コンテンツのアクセス許可を変更することもできるようになります。 

職場または学校アカウントの場合、_Notes.Read.All_ および _Notes.ReadWrite.All_ により、アプリは、サインインしているユーザーが組織内でアクセス許可を持つ別のユーザーの OneNote コンテンツにアクセスできるようになります。

### <a name="example-usage"></a>使用例
#### <a name="delegated"></a>委任

* _Notes.Create_: サインインしているユーザー用に新しいノートブックを作成します (`POST /me/onenote/notebooks`)。
* _Notes.Read_: サインインしているユーザーのノートブックを読み取ります (`GET /me/onenote/notebooks`)。
* _Notes.Read.All_: サインインしているユーザーが組織内でアクセス可能なすべてのノートブックを取得します (`GET /me/onenote/notebooks?includesharednotebooks=true`)。
* _Notes.ReadWrite_: サインインしているユーザーのページを更新します (`PATCH /me/onenote/pages/{id}/$value`)。
* _Notes.ReadWrite.All_: サインインしているユーザーが組織内でアクセス可能な別のユーザーのノートブックにページを作成します (`POST /users/{id}/onenote/pages`)。

#### <a name="application"></a>アプリケーション

* _Notes.Read.All_: グループ内のすべてのユーザーのノートブックを読み取ります (`GET /groups/{id}/onenote/notebooks`)。
* _Notes.ReadWrite.All_: 組織内の任意のユーザーのノートブックのページを更新します (`PATCH /users/{id}/onenote/pages/{id}/$value`)。

より複雑な複数のアクセス許可を伴うシナリオについては、「[アクセス許可のシナリオ](#permission-scenarios)」を参照してください。

---

## <a name="openid-permissions"></a>OpenID のアクセス許可

#### <a name="delegated-permissions"></a>委任されたアクセス許可

|   アクセス許可    |  表示文字列   |  説明 | 管理者の同意の要不要 |
|:-----------------------------|:-----------------------------------------|:-----------------|:-----------------|
| _email_ |    ユーザーのメール アドレスの表示 | ユーザーのプライマリ電子メール アドレスをアプリで読み取れるようにします。 | 不要 |
| _offline_access_ |    ユーザーのデータへの常時アクセス | 現在アプリを使用していない場合も、アプリでユーザー データの読み取りと更新ができるようにします。| 不要 |
| _openid_ |    ユーザーのサインイン | ユーザーが職場または学校アカウントでアプリにサインインできるようにします。またアプリで、ユーザーの基本的なプロファイル情報を読み取れるようにします。| 不要 |
| _profile_ |    ユーザーの基本プロファイルの表示 | ユーザーの基本プロファイル (名前、写真、ユーザー名) をアプリで確認できるようにします。| 不要 |

#### <a name="application-permissions"></a>アプリケーションのアクセス許可

なし。

### <a name="remarks"></a>注釈
これらのアクセス許可を使用すると、Azure AD の承認とトークン要求で返される成果物を指定できます。これらは Azure AD v1.0 エンドポイントと v2.0 エンドポイントでは異なる方法でサポートされます。

Azure AD (v1.0) エンドポイントでは、_openid_ アクセス許可のみが使用されます。これを承認要求で *scope* パラメーターに指定して、ユーザーがアプリにサインインするときに OpenID Connect プロトコルを使用する場合に ID トークンが返されるようにします。詳細については、「[OpenID Connect と Azure Active Directory を使用する Web アプリケーションへのアクセスの承認](https://docs.microsoft.com/azure/active-directory/develop/active-directory-protocols-openid-connect-code)」を参照してください。ID トークンが正常に返されるようにするには、アプリを登録するときに _User.Read_ アクセス許可も必ず構成します。 

Azure AD v2.0 エンドポイントでは、_scope_ パラメーターで_offline\_access_ アクセス許可を指定して、OAuth 2.0 または OpenID Connect プロトコルを使用するときに明示的に更新トークンを要求します。OpenID Connect では、_openid_ アクセス許可を指定して ID トークンを要求します。_email_ アクセス許可、_profile_ アクセス許可、あるいはその両方で ID トークンに追加の要求が返されるように指定できます。v2.0 エンドポイントでは、ID トークンを返すよう _User.Read_ を指定する必要はありません。詳細については、「[OpenID Connect のスコープ](https://docs.microsoft.com/azure/active-directory/develop/active-directory-v2-scopes#openid-connect-scopes)」を参照してください。

> **重要**Microsoft Authentication Library (MSAL) では現在、承認要求およびトークン要求に既定で _offline\_access_、_openid_、_profile_、_email_ が指定されています。つまり、既定では、これらのアクセス許可を明示的に指定すると、Azure AD ではエラーが返される場合があります。
>  

---

## <a name="people-permissions"></a>People のアクセス許可

#### <a name="delegated-permissions"></a>委任されたアクセス許可

|   アクセス許可    |  表示文字列   |  説明 | 管理者の同意の要不要 |
|:-----------------------------|:-----------------------------------------|:-----------------|:-----------------|
| _People.Read_ |    ユーザーに関係する連絡先リストの読み取り (プレビュー) | アプリで、サインインしているユーザーの関連する人に関するランク付けされたリストを読み取れるようにします。リストには、個人の連絡先、ソーシャル ネットワーキングの連絡先、組織のディレクトリ、最近 (メール、Skype などで) 通信した人が含まれます。| 不要 |

#### <a name="application-permissions"></a>アプリケーションのアクセス許可

なし。

### <a name="remarks"></a>備考


### <a name="example-usage"></a>使用例
#### <a name="delegated"></a>委任


より複雑な複数のアクセス許可を伴うシナリオについては、「[アクセス許可のシナリオ](#permission-scenarios)」を参照してください。

---

## <a name="reports-permissions"></a>レポートのアクセス許可

#### <a name="delegated-permissions"></a>委任されたアクセス許可

なし。

#### <a name="application-permissions"></a>アプリケーションのアクセス許可

|   アクセス許可    |  表示文字列   |  説明 | 管理者の同意の要不要 |
|:-----------------------------|:-----------------------------------------|:-----------------|:-----------------|
| _Reports.Read.All_ | すべての利用状況レポートの読み取り | アプリで、サインインしているユーザーなしで、すべてのサービス利用状況レポートの読み取りができるようにします。利用状況レポートを提供するサービスには、Office 365 と Azure Active Directory が含まれます。 | 必要 |

### <a name="remarks"></a>備考
レポートのアクセス許可は、職場または学校アカウントでのみ有効です。 

### <a name="example-usage"></a>使用例

#### <a name="application"></a>アプリケーション

* _Reports.Read.All_: 7 日間の期間で電子メール アプリの利用状況詳細レポートを読み取ります (`GET /reports/EmailAppUsage(view='Detail',period='D7')/content`)
* _Reports.Read.All_: '2017-01-01' の日付で電子メールのアクティビティ詳細レポートを読み取ります (`GET /reports/EmailActivity(view='Detail',data='2017-01-01')/content`)。
* _Reports.Read.All_: Office 365 ライセンス認証詳細レポートを読み取ります (`GET /reports/Office365Activations(view='Detail')/content`)

より複雑な複数のアクセス許可を伴うシナリオについては、「[アクセス許可のシナリオ](#permission-scenarios)」を参照してください。

---

## <a name="sites-permissions"></a>サイトのアクセス許可

#### <a name="delegated-permissions"></a>委任されたアクセス許可

|   アクセス許可    |  表示文字列   |  説明 | 管理者の同意の要不要 |
|:-----------------------------|:-----------------------------------------|:-----------------|:-----------------|
| _Sites.Read.All_ |    すべてのサイト コレクションに含まれる項目の読み取り | サインインしているユーザーの代わりに、すべてのサイト コレクションに含まれるドキュメントおよびリスト アイテムをアプリケーションで読み取りできるようにします。 | 不要 |
| _Sites.ReadWrite.All_ |    すべてのサイト コレクション内のアイテムの読み取りおよび書き込み | サインインしているユーザーの代わりに、すべてのサイト コレクションに含まれるドキュメントとリスト アイテムをアプリケーションで編集または削除できるようにします。 | 不要 |

#### <a name="application-permissions"></a>アプリケーションのアクセス許可

なし。

### <a name="remarks"></a>備考
サイトのアクセス許可は、職場または学校アカウントでのみ有効です。

### <a name="example-usage"></a>使用例
#### <a name="delegated"></a>委任

* _Sites.Read.All_: SharePoint ルート サイトのリストを読み取ります (`GET /beta/sharePoint/site/lists`)
* _Sites.ReadWrite.All_: SharePoint リストに新しいリスト アイテムを作成します (`POST /beta/sharePoint/site/lists/123/items`)


より複雑な複数のアクセス許可を伴うシナリオについては、「[アクセス許可のシナリオ](#permission-scenarios)」を参照してください。

---

## <a name="tasks-permissions"></a>タスクのアクセス許可

#### <a name="delegated-permissions"></a>委任されたアクセス許可

|   アクセス許可    |  表示文字列   |  説明 | 管理者の同意の要不要 |
|:-----------------------------|:-----------------------------------------|:-----------------|:-----------------|
| _Tasks.Read_ | ユーザー タスクの読み取り | アプリで、ユーザー タスクを読み取れるようにします。 | 不要 |
| _Tasks.Read.Shared_ | ユーザー タスクと共有のタスクの読み取り | アプリで、ユーザー自身のタスクと共有のタスクを含む、ユーザーがアクセス許可を得ているタスクを読み取れるようにします。 | 不要 |
| _Tasks.ReadWrite_ |    ユーザーのタスクとコンテナーの作成、読み取り、更新および削除 | タスクとコンテナー (およびコンテナー内のタスク) のうち、サインインしているユーザーに割り当てられたもの、またはサインインしているユーザーと共有するものをアプリで作成、読み取り、更新および削除できるようにします。| 不要 |
| _Tasks.ReadWrite.Shared_ | ユーザー タスクと共有のタスクの読み取りと書き込み | アプリで、ユーザー自身のタスクと共有のタスクを含むユーザーがアクセス許可を得ているタスクの作成、読み取り、更新、削除を行えるようにします。 | 不要 |

#### <a name="application-permissions"></a>アプリケーションのアクセス許可

なし。

### <a name="remarks"></a>注釈
_タスク_のアクセス許可は、Outlook タスクのアクセスを制御するために使用します。Microsoft Planner のタスクは、[_グループ_のアクセス許可](#group-permissions)で制御します。

_共有_のアクセス許可は、現時点では職場または学校アカウントでのみサポートされます。_共有_のアクセス許可がある場合でも、共有コンテンツを所有するユーザーが、そのコンテンツにアクセスするユーザーに、フォルダー内のコンテンツを変更するアクセス許可を付与していないと、読み取りと書き込みが失敗することがあります。

### <a name="example-usage"></a>使用例
#### <a name="delegated"></a>委任

* _Tasks.Read_: ユーザーのメールボックス内のすべてのタスクを取得します (`GET /me/outlook/tasks`)。
* _Tasks.Read.Shared_: 組織内の別のユーザーによって共有されているフォルダー内のタスクにアクセスします (`Get /users{id|userPrincipalName}/outlook/taskfolders/{id}/tasks`)。
* _Tasks.ReadWrite_: ユーザーの既定のタスク フォルダーにイベントを追加します (`POST /me/outook/tasks`)。
* _Tasks.Read_: ユーザーのメールボックス内にある未完了のタスクをすべて取得します (`GET /users/{id | userPrincipalName}/outlook/tasks?$filter=status ne 'completed'`)。
* _Tasks.ReadWrite_: ユーザーのメールボックス内のタスクを更新します (`PATCH /users/{id | userPrincipalName}/outlook/tasks/id`)。
* _Tasks.ReadWrite.Shared_: 別のユーザーの代わりにタスクを完了します (`POST /users/{id | userPrincipalName}/outlook/tasks/id/complete`)。

より複雑な複数のアクセス許可を伴うシナリオについては、「[アクセス許可のシナリオ](#permission-scenarios)」を参照してください。

---

## <a name="user-permissions"></a>ユーザーのアクセス許可

#### <a name="delegated-permissions"></a>委任されたアクセス許可

|   アクセス許可    |  表示文字列   |  説明 | 管理者の同意の要不要 |
|:-----------------------------|:-----------------------------------------|:-----------------|:-----------------|
| _User.Read_       |    サインインとユーザー プロファイルの読み取り | ユーザーがアプリにサインインできるようにします。またサインインしているユーザーのプロファイルをアプリで読み取ることができるようにします。また、サインインしているユーザーの基本会社情報をアプリで読み取れるようにします。| なし |
| _User.ReadWrite_ |    ユーザーのプロファイルの読み取りおよび書き込みアクセス許可 | アプリはユーザーのプロファイルを読み取ることができます。また、アプリはユーザーの代わりにプロファイル情報を更新することもできます。 | いいえ |
| _User.ReadBasic.All_ |    すべてのユーザーの基本プロファイルの読み取り | アプリで、サインインしているユーザーの代わりに、組織内の他のユーザーのプロファイル プロパティの基本的なセットを読み取れるようにします。これには表示名、氏名、メール アドレス、写真が含まれます。 | いいえ |
| _User.Read.All_  |     すべてのユーザーの完全なプロファイルの読み取り           | アプリで、サインインしているユーザーの代わりに、組織内の他のユーザーのプロファイル プロパティ、部下、および上司の完全なセットを読み取れるようにします。 | 必要 |
| _User.ReadWrite.All_ |     すべてのユーザーの完全なプロファイルの読み取りと書き込み | アプリで、サインインしているユーザーの代わりに、組織内の他のユーザーのプロファイル プロパティ、部下、上司の完全なセットを読み書きできるようにします。また、サインインしているユーザーの代わりに、アプリでユーザーの作成および削除ができるようにするとともに、パスワードのリセットもできるようにします。 | はい |
| _User.Invite.All_  |     組織へのゲスト ユーザーの招待 | サインインしているユーザーの代わりに、アプリで組織にゲスト ユーザーを招待できるようにします。 | はい |
| _UserTimelineActivity.Write.CreatedByApp_  |     ユーザーのタイムラインにアプリのアクティビティを書き込む | アプリがサインイン ユーザーのアプリ アクティビティ情報を Microsoft タイムラインに報告することを許可します。 | いいえ |

#### <a name="application-permissions"></a>アプリケーションのアクセス許可

|   アクセス許可    |  表示文字列   |  説明 | 管理者の同意の要不要 |
|:-----------------------------|:-----------------------------------------|:-----------------|:-----------------|
| _User.Read.All_ |    すべてのユーザーの完全なプロファイルの読み取り | サインインしているユーザーなしで、アプリで組織内の他のユーザーのプロファイル プロパティ、グループ メンバーシップ、部下、上司の完全なセットを読み取ることができるようにします。| 必要 |
| _User.ReadWrite.All_ |   すべてのユーザーの完全なプロファイルの読み取りと書き込み | サインインしているユーザーなしで、組織内の別のユーザーのプロファイル プロパティ、グループ メンバーシップ、部下、上司の完全なセットをアプリで読み書きできるようにします。また、アプリで非管理ユーザーの作成と削除もできるようにします。ユーザーのパスワードのリセットはできません。 | はい |
| _User.Invite.All_  |     組織へのゲスト ユーザーの招待 | サインインしているユーザーなしで、ゲスト ユーザーをアプリで組織に招待できるようにします。 | 必要 |

### <a name="remarks"></a>注釈

Microsoft アカウントで有効なアクセス許可は、_User.Read_、_User.ReadWrite_、および _UserTimelineActivity.Write.CreatedByApp_ のみです。職場または学校アカウントについては、_UserTimelineActivity.Write.CreatedByApp_ を除くすべてのアクセス許可が有効です。

_User.Read_ のアクセス許可があるアプリは、[組織](../api-reference/v1.0/resources/organization.md)リソースを通じて職場または学校アカウントでサインインしているユーザーの基本会社情報を読み取ることもできます。使用可能なプロパティは、id、displayName、および verifiedDomains です。

職場または学校アカウントの場合は、完全なプロファイルに[ユーザー](../api-reference/v1.0/resources/user.md) リソースの宣言されたプロパティがすべて含まれます。既定では、読み取り時に制限された数のプロパティのみが返されます。既定のセットに含まれていないプロパティを読み取るには、`$select` を使用します。既定のプロパティは、次のとおりです。

- displayName
- givenName
- jobTitle
- mail
- mobilePhone
- officeLocation
- preferredLanguage
- surname
- userPrincipalName

 委任されたアクセス許可の _User.ReadWrite_ および _User.Readwrite.All_ により、アプリは、次に示す職場または学校アカウントのプロファイル プロパティを更新できるようになります。

- aboutMe
- birthday
- hireDate
- interests
- mobilePhone
- mySite
- pastProjects
- photo
- preferredName
- responsibilities
- schools
- skills

アプリケーションのアクセス許可の _User.ReadWrite.All_ があるアプリは、職場または学校アカウントのすべての宣言されたプロパティ (パスワードを除く) を更新できるようになります。

職場または学校アカウントの直属の部下 (`directReports`) または上司 (`manager`) を読み取りまたは書き込みするには、アプリに _User.Read.All_ (読み取り専用) または _User.ReadWrite.All_ が付与されている必要があります。

_User.ReadBasic.All_ アクセス許可では、基本プロファイルと呼ばれる限定されたプロパティのセットにアプリのアクセスを制限します。これは、完全なプロファイルには機密性の高い情報が含まれている可能性があるためです。基本プロパティには、次に示すプロパティのみが含まれています。 

- displayName
- givenName
- mail
- photo
- surname
- userPrincipalName

ユーザーのグループ メンバーシップ (`memberOf`) を読み取るには、アプリに [_Group.Read.All_](#group-permissions) または [_Group.ReadWrite.All_](#group-permissions) のどちらかが付与されている必要があります。ただし、ユーザーに [directoryRole](../api-reference/v1.0/resources/directoryrole.md) または [administrativeUnit](../api-reference/beta/resources/administrativeunit.md) のメンバーシップもある場合、アプリにはそれらのリソースを読み取るための有効なアクセス許可も必要になります。このアクセス許可がない場合、Microsoft Graph はエラーを返します。つまり、アプリは[ディレクトリのアクセス許可](#directory-permissions)も必要とし、委任されたアクセス許可の場合は、サインインしているユーザーにも組織内でディレクトリ ロールと管理単位にアクセスするための十分な特権も必要とするということです。 

### <a name="example-usage"></a>使用例
#### <a name="delegated"></a>委任

* _User.Read_: サインインしているユーザーの完全なプロファイルを読み取ります (`GET /me`)。
* _User.ReadWrite_: サインインしているユーザーの写真を更新します (`PUT /me/photo/$value`)。
* _User.ReadBasic.All_: 名前が "David" で始まるユーザーをすべて検索します (`GET /users?$filter=startswith(displayName,'David')`)。
* _User.Read.All_: ユーザーの上司を読み取ります (`GET /user/{id | userPrincipalName}/manager`)。


#### <a name="application"></a>アプリケーション

* _User.Read.All_: デルタ クエリによってすべてのユーザーとリレーションシップを読み取ります (`GET /beta/users/delta?$select=displayName,givenName,surname`)。
* _User.ReadWrite.All_: 組織内の任意のユーザーの写真を更新します (`PUT /user/{id | userPrincipalName}/photo/$value`)。

より複雑な複数のアクセス許可を伴うシナリオについては、「[アクセス許可のシナリオ](#permission-scenarios)」を参照してください。

---

## <a name="permission-scenarios"></a>アクセス許可のシナリオ

ここでは、組織内の[ユーザー](../api-reference/v1.0/resources/user.md) リソースと[グループ](../api-reference/v1.0/resources/group.md) リソースを対象とした、いくつかの一般的なシナリオを示します。この表には、シナリオごとに必要になる特定の操作を実行するために、アプリが必要とするアクセス許可を示しています。場合によっては、特定の操作をアプリが実行できるかどうかは、アクセス許可が、アプリケーションのアクセス許可か、委任されたアクセス許可かによって決まります。委任されたアクセス許可の場合、アプリの有効なアクセス許可は、サインインしているユーザーの組織内の特権にも依存します。詳細については、「[委任されたアクセス許可、アプリケーションのアクセス許可、有効なアクセス許可](#delegated-permissions-application-permissions-and-effective-permissions)」を参照してください。

### <a name="access-scenarios-on-the-user-resource"></a>ユーザー リソースに対するアクセスのシナリオ

| **ユーザーが関与するアプリ タスク**   |  **必要なアクセス許可** | **アクセス許可文字列** |
|:-------------------------------|:---------------------|:---------------|
| アプリの目的は、人材選択画面への表示などのために、他のユーザーの基本情報 (表示名と写真のみ) を読み取ること   | _User.ReadBasic.All_  |  すべてのユーザーの基本プロファイルの読み取り |
| アプリの目的は、サインインしているユーザーの完全なユーザー プロファイルを読み取ること (直属の部下や上司を表示するなど)     | _User.Read_ | サインインを有効にし、ユーザー プロファイルを読み取ります|
| アプリの目的は、すべてのユーザーの完全なユーザー プロファイルを読み取ること  | _User.Read.All_ |  すべてのユーザーの完全なプロファイルの読み取り   |
| アプリの目的は、サインインしているユーザーのファイル、メール、カレンダー情報を読み取ること  | _User.Read_, _Files.Read_, _Mail.Read_, _Calendars.Read_ | サインインの有効化とユーザー プロファイルの読み取り、ユーザー ファイルの読み取り、ユーザー メールの読み取り、ユーザーのカレンダーの読み取り |
| アプリの目的は、サインインしているユーザー (自分) のファイルと、サインインしているユーザー (自分) が他のユーザーから共有してもらっているファイルを読み取ること | _User.Read_, _Files.Read_, _Sites.Read.All_ | サインインを有効にし、ユーザー プロファイルを読み取ります、ユーザー ファイルの読み取り、すべてのサイト コレクションにあるアイテムの読み取り |
| アプリの目的は、サインインしているユーザーの完全なユーザー プロファイルを読み書きすること   | _User.ReadWrite_ | ユーザーのプロファイルの読み取りおよび書き込みアクセス許可 |
| アプリの目的は、すべてのユーザーの完全なユーザー プロファイルを読み書きすること    | _User.ReadWrite.All_ | すべてのユーザーの完全なプロファイルの読み取りと書き込み |
| アプリの目的は、サインインしているユーザーのファイル、メール、カレンダー情報を読み書きすること    | _User.ReadWrite_, _Files.ReadWrite_, _Mail.ReadWrite_, _Calendars.ReadWrite_  |  ユーザーのプロファイルの読み取りおよび書き込みアクセス許可、ユーザーのプロファイルの読み取りおよび書き込みアクセス許可、ユーザーのメールの読み取りおよび書き込みアクセス許可、ユーザーのカレンダーへのフル アクセス |
   

### <a name="access-scenarios-on-the-group-resource"></a>グループ リソースに対するアクセスのシナリオ
    
| **グループが関与するアプリ タスク**  |  **必要なアクセス許可** |  **アクセス許可文字列** |
|:-------------------------------|:---------------------|:---------------|
| アプリの目的は、グループ選択画面への表示などのために、基本グループ情報 (表示名と写真など) を読み取ることです。  | _Group.Read.All_  | すべてのグループの読み取り|
| アプリの目的は、ファイルや会話を含むすべての公開の Office 365 グループ内のすべてのコンテンツを読み取ることです。グループ メンバーを表示することも必要です。  |  _Group.Read.All_、_User.ReadBasic.All_ | すべてのグループの読み取り、すべてのユーザーの基本プロファイルの読み取り |
| アプリの目的は、ファイルや会話を含むすべての公開の Office 365 グループ内のすべてのコンテンツを読み書きすることです。グループ メンバーを表示し、グループ メンバーを更新できる必要もあります (サインイン ユーザーがグループの所有者である場合)。  |     _Group.ReadWrite.All_、_User.ReadBasic.All_ |  すべてのグループの読み取りと書き込み、すべてのユーザーの基本プロファイルの読み取り |
| アプリの目的は、ユーザーが公開の Office 365 グループに参加できるようにすることです。ユーザーが、特定のグループを検索し、一覧表から選択できるようにします。ユーザーは選択した任意のグループに追加されます。    |   _Group.ReadWrite.All_、_User.Read_ | すべてのグループの読み取りと書き込み、サインインとユーザー プロファイルの読み取り |
| アプリの目的は、Microsoft Graph を使用してグループを作成することです。 |    _Group.ReadWrite.All_ | すべてのグループの読み取りと書き込み|
