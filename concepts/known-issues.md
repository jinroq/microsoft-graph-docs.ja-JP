---
title: Microsoft Graph に関する既知の問題
description: この記事では、Microsoft Graph に関する既知の問題について説明します。最新の更新プログラムについては、「Microsoft Graph の変更ログ」を参照してください。
author: ''
localization_priority: Priority
ms.openlocfilehash: 13bea7e626232caabb0eb58dc3b9eb7b6d458e9e
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36033258"
---
# <a name="known-issues-with-microsoft-graph"></a>Microsoft Graph に関する既知の問題

この記事では、Microsoft Graph に関する既知の問題について説明します。最新の更新プログラムについては、「[Microsoft Graph の変更ログ](changelog.md)」を参照してください。

## <a name="users"></a>ユーザー

### <a name="no-instant-access-after-creation"></a>作成後にすぐにアクセスできない

ユーザーは、ユーザー エンティティの POST ですぐに作成できます。Office 365 サービスにアクセスするには、まず Office 365 ライセンスをユーザーに割り当てる必要があります。それでも、サービスが分散しているという性質上、Microsoft Graph API を介してこのユーザーがファイル、メッセージ、イベント エンティティを使用できるようになるまで 15 分かかる場合があります。この間、アプリには HTTP 404 エラー応答が送られてきます。

### <a name="photo-restrictions"></a>写真の制限

ユーザーのプロフィール写真の読み取りと更新は、ユーザーがメールボックスを持っている場合にのみ使用できます。さらに、以前 **thumbnailPhoto** プロパティを使用して (Office 365 統合 API のプレビュー、または Azure AD Graph、AD 接続同期を使用して) 保存*された*いかなる写真も[ユーザー](/graph/api/resources/user?view=graph-rest-1.0) リソースの Microsoft Graph の**写真**プロパティを使用してアクセスできなくなります。写真の読み取りまたは更新が失敗すると、この例では次のエラーが発生します。

```javascript
    {
      "error": {
        "code": "ErrorNonExistentMailbox",
        "message": "The SMTP address has no mailbox associated with it."
      }
    }
```

### <a name="using-delta-query"></a>デルタ クエリの使用

デルタ クエリの使用に関する既知の問題については、この記事の[「デルタ クエリ」セクション](#delta-query)を参照してください。

## <a name="microsoft-teams"></a>Microsoft Teams

### <a name="get-teams-and-post-teams-are-not-supported"></a>GET /teams と POST /teams はサポート対象外

チームのリストを取得するには、「[すべてのチームのリスト](teams-list-all-teams.md)」と「[自分のチームのリスト](/graph/api/user-list-joinedteams?view=graph-rest-1.0)」を参照してください。
チームを作成するには、「[チームの作成](/graph/api/team-put-teams?view=graph-rest-1.0)」を参照してください。

### <a name="missing-teams-in-list-all-teams"></a>すべてのチームのリストに含まれないチームがある

過去に作成され、Microsoft Teams ユーザーに最近使用されていないチームの一部は、[すべてのチームのリスト](teams-list-all-teams.md)に含まれません。
新しいチームはリストに含まれます。
古いチームの一部には、**resourceProvisioningOptions** プロパティが存在しないものがあります。このプロパティには "Team" が含まれており、新しく作成され、Microsoft Teams 内でアクセスされたチームには設定されます。
将来的には、Microsoft Teams で開かれたことのない既存のチームに対しても、**resourceProvisioningOptions** が設定される予定です。

## <a name="groups"></a>グループ

### <a name="permissions-for-groups-and-microsoft-teams"></a>グループと Microsoft Teams のアクセス許可

Microsoft Graph では、グループと Microsoft Teams API にアクセスするために 2 つのアクセス許可 ([*Group.Read.All*](permissions-reference.md#group-permissions) と [*Group.ReadWrite.All*](permissions-reference.md#group-permissions)) を公開します。
これらのアクセス許可には、管理者による同意が必要です。
将来的には、ユーザーが同意するグループとチームのための新しいアクセス許可を追加する予定です。

また、コア グループの管理とマネージメントのための API だけが、委任されたアクセス許可とアプリ専用のアクセス許可によるアクセスをサポートします。グループ API の他のすべての機能は、委任されたアクセス許可のみサポートします。

委任されたアクセス許可およびアプリ専用のアクセス許可をサポートするグループの機能の例:

* グループの作成と削除
* グループの管理とマネージメントに関するグループ プロパティの取得と更新
* グループの[ディレクトリ設定](/graph/api/resources/directoryobject?view=graph-rest-1.0)、型、同期
* グループの所有者とメンバーシップ

委任されたアクセス許可だけをサポートするグループ機能の例:

* グループの会話、イベント、写真
* 外部の送信者、承認済みまたは拒否された送信者、グループのサブスクリプション
* ユーザーのお気に入り、見えないカウント

### <a name="policy"></a>ポリシー

Microsoft Graph を使用して Office 365 グループを作成および名前付けすると、Outlook Web App で構成されたすべての Office 365 のグループ ポリシーがバイパスされます。

### <a name="adding-and-getting-attachments-of-group-posts"></a>グループの投稿の添付ファイルの追加と取得

現在のところ、グループの投稿への添付ファイルの[追加](/graph/api/post-post-attachments?view=graph-rest-1.0)、グループの投稿の添付ファイルの[一覧表示](/graph/api/post-list-attachments?view=graph-rest-1.0)と取得を行うと、"OData 要求がサポートされていません" というエラー メッセージが返されます。`/v1.0` と `/beta` の両方のバージョンに対する修正プログラムが準備されており、2016 年 1 月の終わりまでには一般に利用可能になると予測されます。

### <a name="setting-the-allowexternalsenders-property"></a>allowExternalSenders プロパティの設定

現在、`/v1.0` と `/beta` の両方で、POST または PATCH 操作の際にグループの **allowExternalSenders** プロパティを設定できないという問題が発生しています。

### <a name="using-delta-query"></a>デルタ クエリの使用

デルタ クエリの使用に関する既知の問題については、この記事の[「デルタ クエリ」セクション](#delta-query)を参照してください。

## <a name="bookings"></a>予約

### <a name="errorexceededfindcountlimit-when-querying-bookingbusinesses"></a>bookingBusinesses のクエリ時の ErrorExceededFindCountLimit

組織が複数のビジネスを予約しており、要求を発行するアカウントが管理者でない場合に、`bookingBusinesses` のリストを取得しようとすると、次のエラー コードのエラーになります:

```json
{
  "error": {
    "code": "ErrorExceededFindCountLimit",
    "message":
      "The GetBookingMailboxes request returned too many results. Please specify a query to limit the results.",
  }
}
```

回避策としては、`query` パラメーターを含めることによって、要求から返されるビジネスのセットを制限できます。たとえば:

```
GET https://graph.microsoft.com/beta/bookingBusinesses?query=Fabrikam
```


## <a name="calendars"></a>予定表

### <a name="accessing-a-shared-calendar"></a>共有された予定表にアクセスする

別のユーザーによって共有されている予定表で、次の操作によってイベントにアクセスするとします。

```http
GET \users('{id}')\calendars('{id}')\events
```

エラー コード `ErrorInternalServerTransientError` で HTTP 500 を受け取る可能性があります。エラーが発生する理由は次のとおりです。

- 従来、予定表共有を実装するための 2 つの方法がありました。それらを区別するために、"古い" アプローチと "新しい" アプローチと呼びます。
- 新しいアプローチは、表示または編集のアクセス許可による予定表の共有に使用できますが、委任のアクセス許可には使用できません。
- 予定表が**新しい**アプローチによって共有されている場合のみ、予定表 REST API を使用して、共有された予定表を表示または編集できます。
- 予定表が**古い**アプローチによって共有されている場合、予定表 REST API を使用して、このような予定表を表示または編集することはできません。


予定表が表示または編集のアクセス許可で共有されていても、古いアプローチを使用している場合、エラーを回避して手動で予定表共有をアップグレードし、新しいアプローチを使用することができます。
時間の経過とともに、Outlook では共有されているすべての予定表が、委任アクセス許可で共有されている予定表を含め、新しいアプローチを使用できるように自動的にアップグレードされます。

新しいアプローチを使用できるように共有されている予定表を手動でアップグレードするには、以下の手順を実行します。
1.  受信者は、それまで共有されていた予定表を削除します。
2.  予定表の所有者は、Outlook on the web、iOS 版 Outlook または Android 版 Outlook で予定表を再共有します。
3.  受信者は Outlook on the web を使用して共有された予定表を再度受け取ります。(まもなくその他の Outlook クライアントも使用可能になります)
4.  受信者は、新しいアプローチを使用して iOS 版 Outlook または Android 版 Outlook で共有されている予定表を表示可能にすることで、予定表が正しく再共有されていることを確認します。

新しいアプローチで共有した予定表は、全く別の予定表のようにメールボックスで表示されます。共有された予定表では、予定表 REST API を使用して自分の予定表のようにイベントを表示または編集できます。次に例を示します。

```http
GET \me\calendars('{id}')\events
```

### <a name="adding-and-accessing-ics-based-calendars-in-users-mailbox"></a>ユーザーのメールボックスに ICS ベースの予定表を追加してアクセスする

現在、インターネット予定表購読 (ICS) に基づく予定表の部分的なサポートがあります。

* ユーザー インターフェイスを経由して ICS ベースの予定表をユーザーのメールボックスに追加できますが、Microsoft Graph API を経由してこれを行うことはできません。
* [ユーザーの予定表の一覧表示](/graph/api/user-list-calendars?view=graph-rest-1.0)を行うと、ICS ベースの予定表を含む、ユーザーの既定の予定表のグループ、または指定した予定表のグループにある各[予定表](/graph/api/resources/calendar?view=graph-rest-1.0)の**名前**、**色**、**ID** のプロパティを取得できます。予定表リソースの ICS URL を保存したり、アクセスしたりすることはできません。
* また、ICS ベースの予定表の[イベントを一覧表示](/graph/api/calendar-list-events?view=graph-rest-1.0)することもできます。

### <a name="onlinemeetingurl-property-support-for-microsoft-teams"></a>Microsoft Teams 向けの onlineMeetingUrl プロパティのサポート

現時点では、Skype 会議 [event](/graph/api/resources/event?view=graph-rest-1.0) の **onlineMeetingUrl** プロパティは、オンライン会議の URL を示します。 ただし、Microsoft Teams の会議イベントの onlineMeetingUrl プロパティは Null に設定します。

## <a name="calls-and-online-meetings"></a>通話とオンライン会議

> **注**: 通話とオンライン会議は現在プレビュー段階で、Microsoft Graph ベータ版のエンドポイントでのみ利用可能です。

- ナビゲーション パス `/applications/{id}` はサポートされていません。 グローバル アプリケーション ノードを経由したアプリケーションへの移動は、自分が所有者である場合でも、許可されていません。 `/app` ナビゲーションのみ使用してください。

## <a name="contacts"></a>連絡先

### <a name="organization-contacts-available-in-only-beta"></a>ベータ版でのみ利用可能な組織の連絡先

現在、個人用連絡先しかサポートされていません。組織の連絡先は現在 `/v1.0` でサポートされていませんが、`/beta` で参照できます。

### <a name="default-contacts-folder"></a>既定の連絡先フォルダー

`/v1.0` バージョンでは、`GET /me/contactFolders` にユーザーの既定の連絡先フォルダーは含まれません。

修正プログラムが用意される予定です。それまでは、回避策として次の[連絡先一覧表示](/graph/api/user-list-contacts?view=graph-rest-1.0)クエリと **parentFolderId** プロパティを使用して、既定の連絡先フォルダーのフォルダー ID を取得できます。

```http
GET https://graph.microsoft.com/v1.0/me/contacts?$top=1&$select=parentFolderId
```

上記のクエリで、

1. `/me/contacts?$top=1` は既定の連絡先フォルダーの[連絡先](/graph/api/resources/contact?view=graph-rest-1.0)のプロパティを取得します。
2. `&$select=parentFolderId` を追加すると、連絡先の **parentFolderId** プロパティ (既定の連絡先フォルダーの ID) のみが返されます。


### <a name="accessing-contacts-via-a-contact-folder-in-beta"></a>ベータ版の連絡先フォルダーから連絡先にアクセスする

以下の 2 つのシナリオで示されているように、`/beta` バージョンでは、REST 要求 URL で親フォルダーを指定して[連絡先](/graph/api/resources/contact?view=graph-rest-beta)にアクセスすることができないという問題が発生しています。

* ユーザーの最上位レベル [contactFolder](/graph/api/resources/contactfolder?view=graph-rest-beta) から連絡先にアクセスする。

```http
GET /me/contactfolders/{id}/contacts/{id}
GET /users/{id | userPrincipalName}/contactfolders/{id}/contacts/{id}
```

* **contactFolder** の子フォルダーに含まれている連絡先にアクセスする。次の例は、入れ子のレベルの 1 つを示していますが、連絡先は子の子などに入れることができます。

```http
GET /me/contactFolder/{id}/childFolders/{id}/.../contacts/{id}
GET /users/{id | userPrincipalName}/contactFolders/{id}/childFolders/{id}/contacts/{id}
```

あるいは、以下に示すように、ID を指定するだけで連絡先を[取得](/graph/api/contact-get?view=graph-rest-beta)することもできます。これは、`/beta` バージョンの GET /contacts が、ユーザーのメールボックス内のすべての連絡先に適用されるためです。

```http
GET /me/contacts/{id}
GET /users/{id | userPrincipalName}/contacts/{id}
```

## <a name="messages"></a>メッセージ

### <a name="the-comment-parameter-for-creating-a-draft"></a>下書きを作成するためのコメント パラメーター

返信または転送用の下書きを作成するための**コメント** パラメーター ([createReply](/graph/api/message-createreply?view=graph-rest-1.0)、[createReplyAll](/graph/api/message-createreplyall?view=graph-rest-1.0)、[createForward](/graph/api/message-createforward?view=graph-rest-1.0)) は、結果メッセージの下書き本文の一部にはなりません。

### <a name="get-messages-returns-chats-in-microsoft-teams"></a>Microsoft Teams でのメッセージ返信チャットの GET

V1 とベータ版の両方のエンドポイントで、`GET /users/id/messages` の応答には、チームまたはチャネルの範囲外で行われたユーザーの Microsoft Teams チャットが含まれています。 これらのチャット メッセージの件名は「IM」です。


## <a name="drives-files-and-content-streaming"></a>ドライブ、ファイルおよびコンテンツのストリーミング

* ユーザーが自分の個人用サイトにブラウザーでアクセスする前に、Microsoft Graph でユーザーの個人ドライブに初めてアクセスした場合、401 応答になります。

## <a name="query-parameter-limitations"></a>クエリ パラメーターの制限事項

* 複数の名前空間はサポートされていません。
* `$ref` の GET とキャストはユーザー、グループ、デバイス、サービス プリンシパル、アプリケーションではサポートされていません。
* `@odata.bind` はサポートされていません。つまり、開発者は **acceptedSenders** や **rejectedSenders** ナビゲーション プロパティをグループに適切に設定することができません。
* `@odata.id` は最低限のメタデータを使用する場合、非包含構造のナビゲーション (メッセージなど) には存在しません。
* `$expand`:
  * `nextLink` はサポートされていません
  * 1 レベルを超える展開はサポートされていません
  * 余分なパラメーターはサポートされていません (`$filter`、`$select`)
* `$filter`:
  * `/attachments` エンドポイントは、フィルターをサポートしていません。 存在する場合、`$filter` パラメーターは無視されます。
  * ワークロード間でのフィルターはサポートされていません。
* `$search`:
  * フルテキスト検索はメッセージなどのエンティティのサブセットに対してのみ使用できます。
  * ワークロード間での検索はサポートされていません。

## <a name="delta-query"></a>デルタ クエリ

* リレーションシップの追跡では、誤った OData コンテキストが返されることがあります。
* スキーマ拡張情報 (レガシー) は $select ステートメントをつけては返されず、$select なしで返されます。
* クライアントはオープン拡張機能または登録済みスキーマ拡張機能の変更を追跡できません。

## <a name="application-and-serviceprincipal-api-changes"></a>application API と servicePrincipal API の変更

現在開発中の [application](/graph/api/resources/application?view=graph-rest-beta) エンティティおよび [servicePrincipal](/graph/api/resources/serviceprincipal?view=graph-rest-beta) エンティティに対して変更点があります。現在の制限事項と開発中の API の機能の概要を次に示します。

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

## <a name="extensions"></a>拡張機能

### <a name="change-tracking-is-not-supported"></a>変更履歴はサポートされていません

変更の追跡 (デルタ クエリ) はオープン拡張機能またはスキーマ拡張機能のプロパティではサポートされていません。

### <a name="creating-a-resource-and-open-extension-at-the-same-time"></a>リソースとオープン拡張機能の同時作成

**管理単位**、**デバイス**、**グループ**、**組織**、または**ユーザー**のインスタンスを作成するのと同時に、オープン拡張機能を指定することはできません。最初にインスタンスを作成し、次にそのインスタンスの後続の ``POST`` 要求でオープン拡張機能データを指定する必要があります。

### <a name="creating-a-resource-instance-and-adding-schema-extension-data-at-the-same-time"></a>リソースのインスタンスを作成し、同時にスキーマ拡張機能データを追加します。

**連絡先**、**イベント**、**メッセージ**、**投稿**のインスタンスを作成する場合と同じ操作では、スキーマ拡張機能を指定できません。
リソースのインスタンスを作成してから、そのインスタンスに`PATCH` 操作を行い、スキーマ拡張機能とカスタム データを追加する必要があります。

### <a name="limit-of-100-schema-extension-property-values-allowed-per-resource-instance"></a>スキーマ拡張機能のプロパティ値はリソースのインスタンスごとに 100 に制限されています。

現在、**デバイス**、**グループ**、**ユーザー**などのディレクトリ リソースでは、1 つのリソース インスタンスで設定可能なスキーマ拡張機能のプロパティ値の合計数が 100 に制限されています。

### <a name="filtering-on-schema-extension-properties-not-supported-on-all-entity-types"></a>スキーマ拡張プロパティによるフィルター処理はすべてのエンティティ タイプでサポートされているわけではありません

スキーマ拡張プロパティによるフィルター処理 (`$filter` 式を使用する) は、Outlook エンティティ タイプ - **contact**、**event**、**message**、または **post** ではサポートされません。

## <a name="json-batching"></a>JSON バッチ処理

### <a name="no-nested-batch"></a>入れ子状のバッチ不可

JSON のバッチ要求には、入れ子になったバッチは一切含めることはできません。

### <a name="all-individual-requests-must-be-synchronous"></a>個々の要求はすべて同期要求とします。

バッチ要求に含まれるすべての要求は同期して実行する必要があります。存在する場合、`respond-async` の設定は無視されます。

### <a name="no-transactions"></a>トランザクション未対応

Microsoft Graph は現段階では個々の要求のトランザクション処理をサポートしていません。個々の要求で `atomicityGroup` プロパティを指定しても無視されます。

### <a name="uris-must-be-relative"></a>URI は相対 URI である必要があります。

バッチ要求では、必ず相対 URI を指定してください。Microsoft Graph はバッチ要求の URL に含まれているバージョン エンドポイントを使い、これらを絶対 URL に変換します。

### <a name="limit-on-batch-size"></a>バッチ サイズの制限

現段階では、JSON バッチ要求は 20 個までの個別要求に限られています。

### <a name="simplified-dependencies"></a>簡略化された依存関係

個々の要求は、他の個々の要求に依存することがあります。現在、各要求は他の要求一つだけに依存でき、以下のパターンのどれかにあてはまることが必要です。

1. 並行:依存する要求が `dependsOn` プロパティに指定されていない場合。
2. 直列:個々の要求のすべてが前の個々の要求に依存する場合。
3. 同列:`dependsOn` プロパティに依存を示した個々の要求のすべてが同じ依存を指定している場合。

JSON バッチ処理が完成に近づくにつれて、これらの制限は削除されます。

## <a name="cloud-solution-provider-apps"></a>クラウド ソリューション プロバイダー アプリ

### <a name="csp-apps-must-use-azure-ad-endpoint"></a>CSP アプリは Azure AD エンドポイントを使用する必要がある

クラウド ソリューション プロバイダー (CSP) のアプリケーションは、パートナー管理の顧客から Microsoft Graph を正常に呼び出すには、Azure AD (v1) のエンドポイントからトークンを取得する必要があります。現時点では、新しい Azure AD バージョン 2.0 エンドポイントからのトークン取得はサポートされていません。

### <a name="pre-consent-for-csp-apps-doesnt-work-in-some-customer-tenants"></a>CSP アプリの事前同意が一部の顧客テナントで機能しない

状況によっては、CSP アプリの事前同意が一部の顧客テナントで機能しない可能性があります。

- 代理アクセス許可を使用するアプリでは、新しい顧客テナントで初めてアプリを使用すると、サインイン後に次のエラーを受け取る可能性があります。`AADSTS50000: There was an error issuing a token`。
- アプリケーションのアクセス許可を使用するアプリでは、アプリはトークンを取得できますが、Microsoft Graph を呼び出すときに予期せずにアクセス拒否メッセージを受け取ります。

事前同意をすべての顧客テナントで機能させるために、できるだけ早くこの問題を解決するべく取り組んでいます。

それまでの間、開発とテストのブロックを解除するために次の回避策を取ってください。

>**注:** これは永続的なソリューションではなく、開発のブロックを解除するためのものです。前述の問題が解決されたら、この回避策は必要なくなります。解決された後にこの回避策を元に戻す必要はありません。

1. Azure AD v2 PowerShell セッションを開き、サインイン ウィンドウに、管理者資格情報を入力して `customer` テナントに接続します。Azure AD PowerShell V2 は、[ここ](https://www.powershellgallery.com/packages/AzureAD)からダウンロードし、インストールできます。

    ```PowerShell
    Connect-AzureAd -TenantId {customerTenantIdOrDomainName}
    ```

2. Microsoft Graph サービス プリンシパルを作成します。

    ```PowerShell
    New-AzureADServicePrincipal -AppId 00000003-0000-0000-c000-000000000000
    ```

## <a name="functionality-available-only-in-office-365-rest-or-azure-ad-graph-apis"></a>Office 365 REST と Azure AD Graph API でのみ使用可能な機能

Microsoft Graph では一部の機能はまだ利用できません。探している機能が表示されない場合は、エンドポイント固有の [Office 365 REST API](https://msdn.microsoft.com/office/office365/api/api-catalog) を使用することができます。Azure Active Directory において、Azure AD と Graph API を介してのみ使用可能な機能については、[Microsoft Graph または Azure AD Graph](https://dev.office.com/blogs/microsoft-graph-or-azure-ad-graph) のブログの投稿を参照してください。

