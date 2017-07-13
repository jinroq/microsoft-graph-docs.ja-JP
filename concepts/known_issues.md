# Microsoft Graph に関する既知の問題
<a id="known-issues-with-microsoft-graph" class="xliff"></a>

この記事では、Microsoft Graph に関する既知の問題について説明します。最新の更新プログラムについては、「[Microsoft Graph の変更ログ](changelog.md)」を参照してください。

## ユーザー
<a id="users" class="xliff"></a>

### 作成後にすぐにアクセスできない
<a id="no-instant-access-after-creation" class="xliff"></a>

ユーザーは、ユーザー エンティティの POST ですぐに作成できます。Office 365 サービスにアクセスするには、まず Office 365 ライセンスをユーザーに割り当てる必要があります。それでも、サービスが分散しているという性質上、Microsoft Graph API を介してこのユーザーがファイル、メッセージ、イベント エンティティを使用できるようになるまで 15 分かかる場合があります。この間、アプリには HTTP 404 エラー応答が送られてきます。

### 写真の制限
<a id="photo-restrictions" class="xliff"></a>

ユーザーのプロフィール写真の読み取りと更新は、ユーザーがメールボックスを持っている場合にのみ使用できます。さらに、以前 **thumbnailPhoto** プロパティを使用して (Office 365 統合 API のプレビュー、または Azure AD Graph、AD 接続同期を使用して) 保存*された*いかなる写真も[ユーザー](../api-reference/v1.0/resources/user.md) リソースの Microsoft Graph の**写真**プロパティを使用してアクセスできなくなります。写真の読み取りまたは更新が失敗すると、この例では次のエラーが発生します。

```javascript
    {
      "error": {
        "code": "ErrorNonExistentMailbox",
        "message": "The SMTP address has no mailbox associated with it."
      }
    }
```


### デルタ クエリの使用
<a id="using-delta-query" class="xliff"></a>

デルタ クエリの使用に関する既知の問題については、この記事の[「デルタ クエリ」セクション](#delta-query)を参照してください。

## グループと Microsoft Teams
<a id="groups-and-microsoft-teams" class="xliff"></a>

>**注**: Microsoft Teams は現在プレビュー段階で、Microsoft Graph ベータ版のエンドポイントでのみ利用可能です。

### ポリシー
<a id="policy" class="xliff"></a>

Microsoft Graph を使用して Office 365 グループを作成および名前付けすると、Outlook Web App で構成されたすべての Office 365 のグループ ポリシーがバイパスされます。 

### グループと Microsoft Teams のアクセス許可
<a id="permissions-for-groups-and-microsoft-teams" class="xliff"></a>

Microsoft Graph では、グループと Microsoft Teams API にアクセスするために 2 つのアクセス許可 (*Group.Read.All* と *Group.ReadWrite.All*) を公開します。これらのアクセス許可は、管理者による同意が必要です (これがプレビューとの違いです)。将来的には、ユーザーが同意するグループとチームのための新しいアクセス許可を追加する予定です。

また、コア グループの管理とマネージメントのための API だけが、委任されたアクセス許可とアプリ専用のアクセス許可によるアクセスをサポートします。グループ API の他のすべての機能は、委任されたアクセス許可のみサポートします。

委任されたアクセス許可およびアプリ専用のアクセス許可をサポートするグループの機能の例:

* グループの作成と削除
* グループの管理とマネージメントに関するグループ プロパティの取得と更新
* グループの[ディレクトリ設定](../api-reference/v1.0/resources/directoryobject.md)、型、同期
* グループの所有者とメンバーシップ


委任されたアクセス許可だけをサポートするグループ機能の例:

* グループの会話、イベント、写真
* 外部の送信者、承認済みまたは拒否された送信者、グループのサブスクリプション
* ユーザーのお気に入り、見えないカウント

### Microsoft Teams のチーム (プレビュー)
<a id="teams-in-microsoft-teams-preview" class="xliff"></a>

Microsoft Teams と Office 365 グループは、同じような機能を共有します。グループ API はすべてチームで使用できますが、Create group API は例外で、現在これを使ってのチーム作成はできません。将来的に、API リリースでこの機能がサポートされます。

### Microsoft Teams チャンネル (プレビュー)
<a id="microsoft-teams-channels-preview" class="xliff"></a>

現在のところ、チャンネルの読み込みと作成が可能ですが、更新と削除はできません。将来的に、API リリースでこの機能がサポートされます。

### Microsoft Teams チャット スレッドとチャット メッセージ (プレビュー)
<a id="microsoft-teams-chat-threads-and-chat-messages-preview" class="xliff"></a>

現時点では、チャンネルにチャット スレッドを作成できますが、既存のチャンネル スレッドを読み込む、または返信を付加することができません。また、チームまたはチャンネルの範囲外のユーザー間での読み取り、書き込みもできません。将来の API リリースでこの部分の機能がサポートされます。


### グループの投稿の添付ファイルの追加と取得
<a id="adding-and-getting-attachments-of-group-posts" class="xliff"></a>

現在のところ、グループの投稿への添付ファイルの[追加](http://developer.microsoft.com/en-us/graph/docs/api-reference/v1.0/api/post_post_attachments)、グループの投稿の添付ファイルの[一覧表示](http://developer.microsoft.com/en-us/graph/docs/api-reference/v1.0/api/post_list_attachments)と取得を行うと、"OData 要求がサポートされていません" というエラー メッセージが返されます。`/v1.0` と `/beta` の両方のバージョンに対する修正プログラムが準備されており、2016 年 1 月の終わりまでには一般に利用可能になると予測されます。

### allowExternalSenders プロパティの設定
<a id="setting-the-allowexternalsenders-property" class="xliff"></a>

現在、`/v1.0` と `/beta` の両方で、POST または PATCH 操作の際にグループの **allowExternalSenders** プロパティを設定できないという問題が発生しています。

### デルタ クエリの使用
<a id="using-delta-query" class="xliff"></a>

デルタ クエリの使用に関する既知の問題については、この記事の[「デルタ クエリ」セクション](#delta-query)を参照してください。


## 予定表
<a id="calendars" class="xliff"></a>

### ユーザーのメールボックスに ICS ベースの予定表を追加してアクセスする
<a id="adding-and-accessing-ics-based-calendars-in-users-mailbox" class="xliff"></a>

現在、インターネット予定表購読 (ICS) に基づく予定表の部分的なサポートがあります。

* ユーザー インターフェイスを経由して ICS ベースの予定表をユーザーのメールボックスに追加できますが、Microsoft Graph API を経由してこれを行うことはできません。
* [ユーザーの予定表の一覧表示](http://developer.microsoft.com/en-us/graph/docs/api-reference/v1.0/api/user_list_calendars)を行うと、ICS ベースの予定表を含む、ユーザーの既定の予定表のグループ、または指定した予定表のグループにある各[予定表](http://developer.microsoft.com/en-us/graph/docs/api-reference/v1.0/resources/calendar)の**名前**、**色**、**ID** のプロパティを取得できます。予定表リソースの ICS URL を保存したり、アクセスしたりすることはできません。
* また、ICS ベースの予定表の[イベントを一覧表示](http://developer.microsoft.com/en-us/graph/docs/api-reference/v1.0/api/calendar_list_events)することもできます。

### 共有された予定表にアクセスする
<a id="accessing-a-shared-calendar" class="xliff"></a>

別のユーザーによって共有されている予定表で、次の操作によってイベントにアクセスするとします。

```http
GET \users('{id}')\calendars('{id}')\events
```

エラー コード `ErrorInternalServerTransientError` で HTTP 500 を受け取る可能性があります。エラーが発生する理由は次のとおりです。

- 従来、予定表共有を実装するための 2 つの方法がありました。それらを区別するために、"古い" アプローチと "新しい" アプローチと呼びます。
- 新しいアプローチは、表示または編集のアクセス許可による予定表の共有に使用できますが、委任のアクセス許可には使用できません。 
- 予定表が**新しい**アプローチによって共有されている場合のみ、予定表 REST API を使用して、共有された予定表を表示または編集できます。 
- 予定表が**古い**アプローチによって共有されている場合、予定表 REST API を使用して、このような予定表を表示または編集することはできません。


予定表が表示または編集のアクセス許可で共有されていても、古いアプローチを使用している場合、エラーを回避して手動で予定表共有をアップグレードし、新しいアプローチを使用することができます。時間の経過とともに、Outlook では共有されているすべての予定表が、委任アクセス許可で共有されている予定表を含め、新しいアプローチを使用できるように自動的にアップグレードされます。 

新しいアプローチを使用できるように共有されている予定表を手動でアップグレードするには、以下の手順を実行します。
1.  受信者は、それまで共有されていた予定表を削除します。
2.  予定表の所有者は、Outlook on the web、iOS 版 Outlook または Android 版 Outlook で予定表を再共有します。
3.  受信者は Outlook on the web を使用して共有された予定表を再度受け取ります。(まもなくその他の Outlook クライアントも使用可能になります)
4.  受信者は、新しいアプローチを使用して iOS 版 Outlook または Android 版 Outlook で共有されている予定表を表示可能にすることで、予定表が正しく再共有されていることを確認します。

新しいアプローチで共有した予定表は、全く別の予定表のようにメールボックスで表示されます。共有された予定表では、予定表 REST API を使用して自分の予定表のようにイベントを表示または編集できます。次に例を示します。

```http
GET \me\calendars('{id}')\events
```


## 連絡先
<a id="contacts" class="xliff"></a>

### ベータ版でのみ利用可能な組織の連絡先
<a id="organization-contacts-available-in-only-beta" class="xliff"></a>

現在、個人用連絡先しかサポートされていません。組織の連絡先は現在 `/v1.0` でサポートされていませんが、`/beta` で参照できます。

### 既定の連絡先フォルダー
<a id="default-contacts-folder" class="xliff"></a>

`/v1.0` バージョンでは、`GET /me/contactFolders` にユーザーの既定の連絡先フォルダーは含まれません。 

修正プログラムが用意される予定です。それまでは、回避策として次の[連絡先一覧表示](http://developer.microsoft.com/en-us/graph/docs/api-reference/v1.0/api/user_list_contacts)クエリと **parentFolderId** プロパティを使用して、既定の連絡先フォルダーのフォルダー ID を取得できます。

```http
GET https://graph.microsoft.com/v1.0/me/contacts?$top=1&$select=parentFolderId
```

上記のクエリで、

1. `/me/contacts?$top=1` は既定の連絡先フォルダーの[連絡先](http://developer.microsoft.com/en-us/graph/docs/api-reference/v1.0/resources/contact)のプロパティを取得します。
2. `&$select=parentFolderId` を追加すると、連絡先の **parentFolderId** プロパティ (既定の連絡先フォルダーの ID) のみが返されます。


### ベータ版の連絡先フォルダーから連絡先にアクセスする
<a id="accessing-contacts-via-a-contact-folder-in-beta" class="xliff"></a>

以下の 2 つのシナリオで示されているように、`/beta` バージョンでは、REST 要求 URL で親フォルダーを指定して[連絡先](../api-reference/beta/resources/contact.md)にアクセスすることができないという問題が発生しています。

* ユーザーの最上位レベル [contactFolder](../api-reference/beta/resources/contactfolder.md) から連絡先にアクセスする。

```http
GET /me/contactfolders/{id}/contacts/{id}
GET /users/{id | userPrincipalName}/contactfolders/{id}/contacts/{id}
```

* **contactFolder** の子フォルダーに含まれている連絡先にアクセスする。次の例は、入れ子のレベルの 1 つを示していますが、連絡先は子の子などに入れることができます。

```http
GET /me/contactFolder/{id}/childFolders/{id}/.../contacts/{id}
GET /users/{id | userPrincipalName}/contactFolders/{id}/childFolders/{id}/contacts/{id}
```

あるいは、以下に示すように、ID を指定するだけで連絡先を[取得](../api-reference/beta/api/contact_get.md)することもできます。これは、`/beta` バージョンの GET /contacts が、ユーザーのメールボックス内のすべての連絡先に適用されるためです。

```http
GET /me/contacts/{id}
GET /users/{id | userPrincipalName}/contacts/{id}
```

## メッセージ
<a id="messages" class="xliff"></a>

### 下書きを作成するためのコメント パラメーター
<a id="the-comment-parameter-for-creating-a-draft" class="xliff"></a>

返信または転送用の下書きを作成するための**コメント** パラメーター ([createReply](../api-reference/v1.0/api/message_createreply.md)、[createReplyAll](../api-reference/v1.0/api/message_createreplyall.md)、[createForward](../api-reference/v1.0/api/message_createforward.md)) は、結果メッセージの下書き本文の一部にはなりません。  

## ドライブ、ファイルおよびコンテンツのストリーミング
<a id="drives-files-and-content-streaming" class="xliff"></a>

* ユーザーが自分の個人用サイトにブラウザーでアクセスする前に、Microsoft Graph でユーザーの個人ドライブに初めてアクセスした場合、401 応答になります。

## クエリ パラメーターの制限事項
<a id="query-parameter-limitations" class="xliff"></a>

* **$expand** の制限:
    * `nextLink` はサポートされていません
    * 1 レベルを超える展開はサポートされていません
    * 余分なパラメーターはサポートされていません (**$filter**、**$select**)
* 複数の名前空間はサポートされていません
* `$ref` の GET とキャストはユーザー、グループ、デバイス、サービス プリンシパル、アプリケーションではサポートされていません。
* `@odata.bind` はサポートされていません。つまり、開発者は `Accepted` や `RejectedSenders` を適切にグループに設定することができません。
* `@odata.id` は最低限のメタデータを使用する場合、非包含構造のナビゲーション (メッセージなど) には存在しません
* ワークロード間でのフィルター/検索は利用できません。 
* フルテキスト検索 (**$search** を使用した検索) はメッセージなどのいくつかのエンティティに対してのみ使用できます。

## デルタ クエリ
<a id="delta-query" class="xliff"></a>

* リレーションシップの追跡では、誤った OData コンテキストが返されることがあります。
* スキーマ拡張情報 (レガシー) は $select ステートメントをつけては返されず、$select なしで返されます。
* クライアントはオープン拡張機能または登録済みスキーマ拡張機能の変更を追跡できません。

## application API と servicePrincipal API の変更
<a id="application-and-serviceprincipal-api-changes" class="xliff"></a>

現在開発中の [application](../api-reference/beta/resources/application.md) エンティティおよび [servicePrincipal](../api-reference/beta/resources/serviceprincipal.md) エンティティに対して変更点があります。現在の制限事項と開発中の API の機能の概要を次に示します。

現在の制限事項:

* 一部のアプリケーション プロパティ (appRoles、addIns など) は、すべての変更が完了するまで利用できません。
* 登録できるのは、マルチ テナント アプリだけです。
* アプリの更新は、初期ベータ更新後に登録されたアプリに限定されます。
* Azure Active Directory ユーザーは、アプリの登録と所有者の追加を行えます。
* OpenID Connect と OAuth プロトコルをサポートします。
* アプリケーションへのポリシーの割り当てが失敗します。 
* アプリ ID を必要とする ownedObjects に対する操作 (たとえば、users/{id|userPrincipalName}/ownedObjects/{id}/...) が失敗します。

開発中:

* 単一テナント アプリを登録する機能。
* servicePrincipal に対する更新。
* 更新されたモデルへの既存の Azure AD アプリへの移行。
* appRoles、事前承認済みクライアント、オプションのクレーム、グループ メンバーシップのクレーム、ブランド化のサポート。
* Microsoft アカウント (MSA) ユーザーによるアプリの登録。
* SAML および WsFed プロトコルのサポート。

## 拡張機能
<a id="extensions" class="xliff"></a>

### 変更履歴はサポートされていません
<a id="change-tracking-is-not-supported" class="xliff"></a>

変更の追跡 (デルタ クエリ) はオープン拡張機能またはスキーマ拡張機能のプロパティではサポートされていません。

### リソースとオープン拡張機能の同時作成
<a id="creating-a-resource-and-open-extension-at-the-same-time" class="xliff"></a>

**管理単位**、**デバイス**、**グループ**、**組織**、または**ユーザー**のインスタンスを作成するのと同時に、オープン拡張機能を指定することはできません。最初にインスタンスを作成し、次にそのインスタンスの後続の ``POST`` 要求でオープン拡張機能データを指定する必要があります。

### スキーマ拡張機能のプロパティ値はリソースのインスタンスごとに 100 に制限されています。
<a id="limit-of-100-schema-extension-property-values-allowed-per-resource-instance" class="xliff"></a>

現在、**デバイス**、**グループ**、**ユーザー**などのディレクトリ リソースでは、1 つのリソース インスタンスで設定可能なスキーマ拡張機能のプロパティ値の合計数が 100 に制限されています。

## JSON バッチ処理
<a id="json-batching" class="xliff"></a>

### 入れ子状のバッチ不可
<a id="no-nested-batch" class="xliff"></a>

JSON のバッチ要求には、入れ子になったバッチは一切含めることはできません。

### 個々の要求はすべて同期要求とします。
<a id="all-individual-requests-must-be-synchronous" class="xliff"></a>

バッチ要求に含まれるすべての要求は同期して実行する必要があります。存在する場合、`respond-async` の設定は無視されます。

### トランザクション未対応
<a id="no-transactions" class="xliff"></a>

Microsoft Graph は現段階では個々の要求のトランザクション処理をサポートしていません。個々の要求で `atomicityGroup` プロパティを指定しても無視されます。

### URI は相対 URI である必要があります。
<a id="uris-must-be-relative" class="xliff"></a>

バッチ要求では、必ず相対 URI を指定してください。Microsoft Graph はバッチ要求の URL に含まれているバージョン エンドポイントを使い、これらを絶対 URL に変換します。

### バッチ サイズの制限
<a id="limit-on-batch-size" class="xliff"></a>

現段階では、JSON バッチ要求は 5 つまでの個別要求に限られています。JSON バッチ処理が完成に近づくにつれて、この制限を緩和します。

### 簡略化された依存関係
<a id="simplified-dependencies" class="xliff"></a>

個々の要求は、他の個々の要求に依存することがあります。現在、各要求は他の要求一つだけに依存でき、以下のパターンのどれかにあてはまることが必要です。

1. 並行:依存する要求が `dependsOn` プロパティに指定されていない場合。
2. 直列:個々の要求のすべてが前の個々の要求に依存する場合。
3. 同列:`dependsOn` プロパティに依存を示した個々の要求のすべてが同じ依存を指定している場合。

JSON バッチ処理が完成に近づくにつれて、これらの制限は削除されます。

## クラウド ソリューション プロバイダー アプリ
<a id="cloud-solution-provider-apps" class="xliff"></a>

### CSP アプリは Azure AD エンドポイントを使用する必要がある
<a id="csp-apps-must-use-azure-ad-endpoint" class="xliff"></a>

クラウド ソリューション プロバイダー (CSP) のアプリケーションは、パートナー管理の顧客から Microsoft Graph を正常に呼び出すには、Azure AD (v1) のエンドポイントからトークンを取得する必要があります。現時点では、新しい Azure AD バージョン 2.0 エンドポイントからのトークン取得はサポートされていません。

### CSP アプリの事前同意が一部の顧客テナントで機能しない
<a id="pre-consent-for-csp-apps-doesnt-work-in-some-customer-tenants" class="xliff"></a>

状況によっては、CSP アプリの事前同意が一部の顧客テナントで機能しない可能性があります。

- 代理アクセス許可を使用するアプリでは、新しい顧客テナントで初めてアプリを使用すると、サインイン後に次のエラーを受け取る可能性があります。`AADSTS50000: There was an error issuing a token`。
- アプリケーションのアクセス許可を使用するアプリでは、アプリはトークンを取得できますが、Microsoft Graph を呼び出すときに予期せずにアクセス拒否メッセージを受け取ります。

事前同意をすべての顧客テナントで機能させるために、できるだけ早くこの問題を解決するべく取り組んでいます。

それまでの間、開発とテストのブロックを解除するために次の回避策を取ってください。

>**注:**これは永続的なソリューションではなく、開発のブロックを解除するためのものです。前述の問題が解決されたら、この回避策は必要なくなります。解決された後にこの回避策を元に戻す必要はありません。

1. Azure AD v2 PowerShell セッションを開き、サインイン ウィンドウに、管理者資格情報を入力して `customer` テナントに接続します。Azure AD PowerShell V2 は、[ここ](https://www.powershellgallery.com/packages/AzureAD)からダウンロードし、インストールできます。

    ```PowerShell
    Connect-AzureAd -TenantId {customerTenantIdOrDomainName}
    ```

2. Microsoft Graph サービス プリンシパルを作成します。

    ```PowerShell
    New-AzureADServicePrincipal -AppId 00000003-0000-0000-c000-000000000000
    ```

## Office 365 REST と Azure AD Graph API でのみ使用可能な機能
<a id="functionality-available-only-in-office-365-rest-or-azure-ad-graph-apis" class="xliff"></a>

Microsoft Graph では一部の機能はまだ利用できません。探している機能が表示されない場合は、エンドポイント固有の [Office 365 REST API](https://msdn.microsoft.com/en-us/office/office365/api/api-catalog) を使用することができます。Azure Active Directory において、Azure AD と Graph API を介してのみ使用可能な機能については、[Microsoft Graph または Azure AD Graph](https://dev.office.com/blogs/microsoft-graph-or-azure-ad-graph) のブログの投稿を参照してください。

## フィードバック
<a id="feedback" class="xliff"></a>

> お客様からのフィードバックを重視しています。[スタック オーバーフロー](http://stackoverflow.com/questions/tagged/microsoftgraph)でご連絡いただけます。
