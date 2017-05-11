# <a name="known-issues-with-microsoft-graph"></a>Microsoft Graph に関する既知の問題

この記事では、Microsoft Graph に関する既知の問題を説明します。最新の更新プログラムについては、「[Microsoft Graph 変更ログ](http://graph.microsoft.io/en-us/changelog)」を参照してください。

## <a name="graph-quick-start"></a>Graph のクイック スタート
2017 年 4 月 30 日 - クイック スタート フローにバグがあり、リダイレクト URL が Asp.Net MVC、Node.js、Angular、PHP、Python、Ruby に対して適切に構成されていません。現在、運用環境への修正プログラムの展開に向けて作業が進められています。この問題を回避するには、[入門のためのチュートリアル](https://developer.microsoft.com/en-us/graph/docs/get-started/get-started)を参照してください。 これは、5 月 3 日に解決されました。

## <a name="graph-explorer"></a>Graph エクスプローラー
サービスに関する問題が発生したため、Graph エクスプローラーへの Microsoft アカウント ログオンは無効になっています。問題の解決に取り組んでいます。準備が整い次第、このテキストは更新されます。更新日 - 5 月 3 日- この問題は解決されています。

Internet Explorer および Microsoft Edge でのサインインが機能していませんでした。この問題は 2017 年 2 月 2 日現在、解決されています。

## <a name="users"></a>ユーザー
#### <a name="no-instant-access-after-creation"></a>作成後にすぐにアクセスできない
ユーザーは、ユーザー エンティティの POST ですぐに作成できます。Office 365 サービスにアクセスするには、まず Office 365 ライセンスをユーザーに割り当てる必要があります。それでも、サービスが分散しているという性質上、Microsoft Graph API を介してこのユーザーがファイル、メッセージ、イベント エンティティを使用できるようになるまで 15 分かかる場合があります。この間、アプリには HTTP 404 エラー応答が送られてきます。 

#### <a name="photo-restrictions"></a>写真の制限
ユーザーのプロファイル写真の読み取りと更新は、ユーザーが受信トレイを持っている場合にのみ使用できます。さらに、以前 **thumbnailPhoto** プロパティを使用して (Office 365 統合 API のプレビュー、Azure AD Graph、AD 接続同期を使用して) 保存*された*いかなる写真も Microsoft Graph ユーザー写真プロパティを使用してアクセスできなくなります。写真の読み取りまたは更新が失敗すると、この例では次のエラーが発生します:

```javascript
    {
      "error": {
        "code": "ErrorNonExistentMailbox",
        "message": "The SMTP address has no mailbox associated with it."
      }
    }
```

 > **注**:GA 後すぐ、ユーザーが受信トレイを持たない場合でも、ユーザーのプロファイル写真の保存と取得が有効になり、このエラーは表示されなくなります。


#### <a name="adding-and-accessing-ics-based-calendars-in-users-mailbox"></a>ユーザーのメールボックスに ICS ベースの予定表を追加してアクセスする
現在、インターネット予定表購読 (ICS) に基づく予定表の部分的なサポートがあります。

* ユーザー インターフェイスを通して ICS ベースの予定表をユーザーのメールボックスに追加できますが、Microsoft Graph API を通してこれを行うことはできません。 
* [ユーザーの予定表の一覧表示](http://developer.microsoft.com/en-us/graph/docs/api-reference/v1.0/api/user_list_calendars)を行うと、ICS ベースの予定表を含む、ユーザーの既定の予定表のグループ、または指定した予定表のグループにある各[予定表](http://developer.microsoft.com/en-us/graph/docs/api-reference/v1.0/resources/calendar)の**名前**、**色**、**ID** のプロパティを取得できます。予定表リソースの ICS URL を保存したり、アクセスしたりすることはできません。
* また、ICS ベースの予定表の[イベントを一覧表示](http://developer.microsoft.com/en-us/graph/docs/api-reference/v1.0/api/calendar_list_events)することもできます。

#### <a name="using-delta-query"></a>デルタ クエリの使用
デルタ クエリの使用に関する既知の問題については、この記事の[「デルタ クエリ」セクション](#delta-query)を参照してください。

## <a name="groups"></a>グループ
#### <a name="policy"></a>ポリシー
Microsoft Graph を使用して Office 365 グループを作成および名前付けすると、Outlook Web App で構成されたすべての Office 365 のグループ ポリシーがバイパスされます。 

#### <a name="group-permission-scopes"></a>グループ アクセス許可のスコープ
Microsoft Graph では、グループ API にアクセスするために 2 つのアクセス許可のスコープ (*Group.Read.All* と *Group.ReadWrite.All*) を公開します。  
これらのアクセス許可のスコープは、管理者による同意が必要です (これがプレビューとの違いです)。将来的には、ユーザーが同意する新しいグループのためのスコープを追加する予定です。

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


#### <a name="adding-and-getting-attachments-of-group-posts"></a>グループの投稿の添付ファイルの追加と取得
現在のところ、グループの投稿への添付ファイルの[追加](http://developer.microsoft.com/en-us/graph/docs/api-reference/v1.0/api/post_post_attachments)、グループの投稿の添付ファイルの[一覧表示](http://developer.microsoft.com/en-us/graph/docs/api-reference/v1.0/api/post_list_attachments)と取得を行うと、"OData 要求がサポートされていません" というエラー メッセージが返されます。`/v1.0` と `/beta` の両方のバージョンに対する修正プログラムが準備されており、2016 年 1 月の終わりまでには一般に利用可能になると予測されます。


#### <a name="setting-the-allowexternalsenders-property"></a>allowExternalSenders プロパティの設定
現在、`/v1.0` と `/beta` の両方で、POST または PATCH 操作の際にグループの **allowExternalSenders** プロパティを設定できないという問題が発生しています。

#### <a name="using-delta-query"></a>デルタ クエリの使用
デルタ クエリの使用に関する既知の問題については、この記事の[「デルタ クエリ」セクション](#delta-query)を参照してください。

## <a name="contacts"></a>連絡先

#### <a name="organization-contacts-available-in-only-beta"></a>ベータ版でのみ利用可能な組織の連絡先
現在、個人用連絡先しかサポートされていません。組織の連絡先は現在 `/v1.0` でサポートされていませんが、`/beta` で参照できます。

#### <a name="default-contacts-folder"></a>既定の連絡先フォルダー

`/v1.0` バージョンでは、`GET /me/contactFolders` にユーザーの既定の連絡先フォルダーは含まれません。 

修正プログラムが用意される予定です。それまでは、回避策として次の[連絡先一覧表示](http://developer.microsoft.com/en-us/graph/docs/api-reference/v1.0/api/user_list_contacts)クエリと **parentFolderId** プロパティを使用して、既定の連絡先フォルダーのフォルダー ID を取得できます。

```
GET https://graph.microsoft.com/v1.0/me/contacts?$top=1&$select=parentFolderId
```
上記のクエリで、
1. `/me/contacts?$top=1` は既定の連絡先フォルダーの[連絡先](http://developer.microsoft.com/en-us/graph/docs/api-reference/v1.0/resources/contact)のプロパティを取得します。
2. `&$select=parentFolderId` を追加すると、連絡先の **parentFolderId** プロパティ (既定の連絡先フォルダーの ID) のみが返されます。


#### <a name="accessing-contacts-via-a-contact-folder-in-beta"></a>ベータ版の連絡先フォルダーから連絡先にアクセスする
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

## <a name="messages"></a>メッセージ
#### <a name="the-comment-parameter-for-creating-a-draft"></a>下書きを作成するためのコメント パラメーター
返信または転送用の下書きを作成するための**コメント** パラメーター ([createReply](../api-reference/v1.0/api/message_createreply.md)、[createReplyAll](../api-reference/v1.0/api/message_createreplyall.md)、[createForward](../api-reference/v1.0/api/message_createforward.md)) は、結果メッセージの下書き本文の一部にはなりません。  


## <a name="drives-files-and-content-streaming"></a>ドライブ、ファイルおよびコンテンツのストリーミング
* ユーザーが自分の個人用サイトにブラウザーでアクセスする前に、Microsoft Graph でユーザーの個人ドライブに初めてアクセスした場合、401 応答になります。

## <a name="functionality-available-only-in-office-365-rest-apis"></a>Office 365 REST API でのみ使用可能な機能

Microsoft Graph では一部の機能はまだ利用できません。探している機能が表示されない場合は、エンドポイント固有の [Office 365 REST API](https://msdn.microsoft.com/en-us/office/office365/api/api-catalog) を使用することができます。


#### <a name="batching"></a>バッチ処理
Microsoft Graph では、バッチ処理はサポートされていません。ただし、Outlook のベータ版のエンドポイントを使用して、[Outlook REST 呼び出しをバッチ処理](https://msdn.microsoft.com/en-us/office/office365/api/batch-outlook-rest-requests)することは可能です。 

#### <a name="availability-in-china"></a>中国での可用性
Microsoft Graph サービスは 21Vianet によって運営されています (中国でも使用可能になりました)。制限を含む詳細については、「[Microsoft Graph の独立したクラウド展開](http://developer.microsoft.com/en-us/graph/docs/overview/deployments)」をご覧ください。

#### <a name="service-actions-and-functions"></a>サービスのアクションと関数
`isMemberOf` と `getObjectsById` は、Microsoft Graph では使用できません

## <a name="microsoft-graph-permissions"></a>Microsoft Graph のアクセス許可
Microsoft Graph をサポートするアプリケーションと委任されたアクセス許可に関する最新情報は、「[アクセス許可のスコープ](http://developer.microsoft.com/en-us/graph/docs/authorization/permission_scopes)」を参照してください。さらに、`v1.0` には次の制限が適用されます:

|アクセス許可 |    アクセス許可の種類 | 制限 |    代替手段 |
|-----------|-----------------|------------|--------------|
|_User.ReadWrite_| Delegated    | 携帯電話番号を更新できません|    `Directory.AccessAsUser.All` も選択してください| 
|_User.ReadWrite.All_|    Delegated|    `User` では、ユーザーの HD 写真と拡張プロファイルのプロパティの更新以外の CRUD 操作を実行することはできません|    ユーザーの削除が必要な場合は `Directory.ReadWrite.All` や `Directory.AccessAsUser.All` も選択してください。|
|_User.Read.All_|    Application    |他のユーザーに対して読み取り操作を実行することはできません|    `Directory.Read.All` も選択してください|
| _User.ReadWrite.All_ |    Application |    `User` では、ユーザーの HD 写真と拡張プロファイルのプロパティの更新以外の CRUD 操作を実行することはできません |    `Directory.ReadWrite.All` も選択してください。**注**:ユーザーの削除を実行できなくなります。|
|_Group.Read.All_    | Application |    グループまたはグループ メンバーシップを列挙することはできません。Office グループのグループ コンテンツを読み取ることはできます	    | `Directory.Read.All` も選択してください |
|_Group.ReadWrite.All_    | Application    | グループまたはグループ メンバーシップを列挙したり、グループを作成したり、グループ メンバーシップの更新やグループの削除はできません。Office グループのグループ コンテンツの読み取りや更新はできます。	    | `Directory.ReadWrite.All` も選択してください。**注**:グループの削除を実行できなくなります。|

さらに、`/beta` には次の制限があります:

|アクセス許可 |    アクセス許可の種類 | 制限 |    代替手段 |
|-----------|-----------------|------------|--------------|
| _Group.ReadWrite.All_    | Delegated    | Office のグループでプランナーのタスクの読み取りおよび更新はできません	    | `Tasks.ReadWrite` も選択してください|
|_Tasks.ReadWrite_    | Delegated    | サインイン中のユーザーのタスクを読み取りまたは更新することはできません| `Group.ReadWrite.All` も選択してください|

## <a name="odata-related-limitations"></a>OData に関連する制限
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

  >  お客様からのフィードバックを重視しています。[スタック オーバーフロー](http://stackoverflow.com/questions/tagged/office365)でご連絡いただけます。質問には {MicrosoftGraph} と {office365} でタグ付けしてください。

## <a name="delta-query"></a>デルタ クエリ

ユーザーとグループのリレーションシップへの変更の追跡は、変更が追跡されている特定のリソース クラス内でのみサポートされます。たとえば、クライアントが*グループ*の変更を追跡し、*メンバー*のリレーションシップを選択している場合、クライアントは、それらのメンバーが*グループ*でもある場合、デルタ クエリ応答でメンバーシップの更新のみを受信します。つまり、ユーザーのグループ メンバーシップの追跡はまだサポートされていません。Microsoft Graph チームは、これは優先度の高いシナリオであると理解しておりますので、近日中に更新プログラムの配信を予定しています。
