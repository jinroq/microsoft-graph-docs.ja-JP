---
title: ユーザーの代わりにアクセスを取得する
description: Microsoft Graph を使用してユーザーの代理としてリソースを読み取り/書き込みするには、Azure AD からアクセス トークンを取得し、Microsoft Graph に送信する要求にトークンを添付する必要があります。
author: jackson-woods
localization_priority: Priority
ms.prod: microsoft-identity-platform
ms.openlocfilehash: d87b419276a33c4cdc79cf7569590c6377730e1e
ms.sourcegitcommit: c74195b8725c3f28bb3bded43c855261590a0cec
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/06/2019
ms.locfileid: "36775554"
---
# <a name="get-access-on-behalf-of-a-user"></a>ユーザーの代わりにアクセスを取得

Microsoft Graph を使用してユーザーの代理としてリソースを読み取り/書き込みするには、Microsoft ID プラットフォームからアクセス トークンを取得し、Microsoft Graph に送信する要求にトークンを添付する必要があります。アクセス トークンの取得に使用する認証フローは、開発しているアプリの種類と、OpenID Connect を使用してユーザーがアプリにサインインするかどうかによって異なります。ネイティブ アプリ、モバイル アプリ、一部の Web アプリで使用される一般的なフローの 1 つに、OAuth 2.0 認証コードの付与フローがあります。このトピックでは、このフローの使用例について説明します。

## <a name="authentication-and-authorization-steps"></a>認証および承認の手順

OAuth 2.0 認証コードの付与フローを使用して Microsoft ID プラットフォームのエンドポイントからアクセス トークンを取得する際に必要な基本手順は次のとおりです。

1. Azure AD にアプリを登録する。
2. 承認を取得する。
3. アクセス トークンを取得する。
4. アクセス トークンを使用して Microsoft Graph を呼び出す。
5. 更新トークンを使用して新しいアクセス トークンを取得する。

## <a name="1-register-your-app"></a>1.アプリを登録する

Microsoft ID プラットフォームのエンドポイントを使用するには、Azure [アプリ登録ポータル](https://go.microsoft.com/fwlink/?linkid=2083908)でアプリを登録する必要があります。アプリを登録するには、Microsoft アカウントのほか、職場または学校のアカウントを使用できます。

OAuth 2.0 認証コードの付与フローを使用するようにアプリを構成するには、アプリの登録時に次の値を保存する必要があります。

- アプリ登録ポータルによって割り当てられたアプリケーション (クライアント) ID。
- クライアント (アプリケーション) シークレット。パスワードか、公開鍵や秘密鍵のペア (証明書) のいずれか。 ネイティブ アプリの場合、これは必須ではありません。
- Azure AD からの応答を受信するためのリダイレクト URI (または応答 URL)。

Azure portal でアプリを構成する手順については、「[アプリを登録する](./auth-register-app-v2.md)」を参照してください。

## <a name="2-get-authorization"></a>2. 承認を取得する

多くの OpenID Connect および OAuth 2.0 フローのアクセス トークンを取得するための最初の手順は、ユーザーを Microsoft ID プラットフォームの `/authorize` エンドポイントにリダイレクトすることです。 Azure AD はユーザーをサインインし、アプリの要求するアクセス許可にユーザーが同意していることを確認します。 承認コードの付与フローでは、同意が得られた後、Azure AD が authorization_code をアプリに返します。アプリは、このコードを Microsoft ID プラットフォームの `/token` エンドポイントでアクセス トークンと引き換えることができます。

### <a name="authorization-request"></a>承認要求

`/authorize` エンドポイントへの要求例を次に示します。

Microsoft ID プラットフォームのエンドポイントでは、`scope` パラメーターによってアクセス許可が要求されます。 この例では、要求された Microsoft Graph のアクセス許可は_User.Read_と _Mail.Read_ です。これにより、アプリはサインインしたユーザーのプロファイルとメールを読むことができます。 _offline\_access_ アクセス許可が要求されるので、アプリは更新トークンを取得できます。更新トークンは、現在のトークンが期限切れになったときに新しいアクセス トークンを取得するために使用できます。

```
// Line breaks for legibility only

https://login.microsoftonline.com/{tenant}/oauth2/v2.0/authorize?
client_id=6731de76-14a6-49ae-97bc-6eba6914391e
&response_type=code
&redirect_uri=http%3A%2F%2Flocalhost%2Fmyapp%2F
&response_mode=query
&scope=offline_access%20user.read%20mail.read
&state=12345
```

| パラメーター |  | 説明 |
| --- | --- | --- |
| tenant |必須出席者 |要求のパスで `{tenant}` 値を使用して、アプリケーションにサインインできるユーザーを制御できます。許可される値は、Microsoft のアカウントと職場または学校のアカウントの両方に `common`、職場または学校のアカウントのみに `organizations`、Microsoft のアカウントのみに `consumers`。また、テナント ID やドメイン名などのテナント識別子が含まれています。詳細については、[プロトコルの基本情報](https://docs.microsoft.com/azure/active-directory/develop/active-directory-v2-protocols#endpoints)を参照してください。 |
| client_id |必須 |[登録ポータル](https://go.microsoft.com/fwlink/?linkid=2083908)によってアプリに割り当てられたアプリケーション ID。 |
| response_type |必須 |認可コードのフローに `code` を含める必要があります。 |
| redirect_uri |推奨 |アプリの redirect_uri。アプリが認証応答を送受信できる場所。アプリ登録ポータルに登録した redirect_uri のいずれかと正確に一致する必要があります。ただし、URL エンコードされている必要があります。ネイティブとモバイル アプリの場合は、既定値の `https://login.microsoftonline.com/common/oauth2/nativeclient` を使用する必要があります。 |
| スコープ |必須出席者 |ユーザーが同意する必要がある Microsoft Graph のアクセス許可のスペースで区切った一覧。これには OpenID スコープも含まれている場合があります。 |
| response_mode |推奨 |結果のトークンをアプリに送信するために使用するメソッドを指定します。`query` または `form_post` にできます。 |
| state |推奨 |トークン応答でも返される要求に含まれている値。任意のコンテンツの文字列にすることができます。ランダムに生成された一意の値は、通常、[クロスサイト リクエスト フォージェリ攻撃を防止する](https://tools.ietf.org/html/rfc6749#section-10.12)ために使用されます。state は、使用していたページまたはビューなど、認証要求が発生する前の、アプリでのユーザーの状態に関する情報をエンコードするためにも使用されます。 |

> **重要**:Microsoft Graph では、アプリケーションのアクセス許可と委任されたアクセス許可という 2 種類のアクセス許可を公開しています。サインインしたユーザーが実行するアプリの場合は、`scope` パラメーターで、委任されたアクセス許可を要求します。これらのアクセス許可は、サインインしたユーザーの権限をアプリに委任し、Microsoft Graph を呼び出したときに、サインインしたユーザーとして動作できるようにします。Microsoft Graph で使用できるアクセス許可の詳細については、「[アクセス許可のリファレンス](./permissions-reference.md)」を参照してください。

### <a name="consent-experience"></a>同意エクスペリエンス

この時点で、ユーザーは Microsoft で認証するための資格情報の入力を求められます。 Microsoft ID プラットフォーム v2.0 エンドポイントは、ユーザーが `scope` クエリ パラメーターに示されているアクセス許可に同意したことを確認します。  ユーザーがこれらのアクセス許可のいずれかに同意していない場合と、管理者が組織内のすべてのユーザーに代わって同意していない場合は、必要なアクセス許可に同意するよう求められます。  

次は Microsoft アカウント ユーザーの同意ダイアログ ボックスの例です。

![Microsoft アカウントの同意ダイアログ](./images/v2-consumer-consent.png)

> **試してみましょう** Microsoft アカウントや Azure AD の職場または学校のアカウントを所有している場合は、次のリンクをクリックして試してみてください。サインイン後、ブラウザーは `https://localhost/myapp/` にリダイレクトされ、アドレスバーに `code` が表示されます。
>
> <a href="https://login.microsoftonline.com/common/oauth2/v2.0/authorize?client_id=6731de76-14a6-49ae-97bc-6eba6914391e&response_type=code&redirect_uri=http%3A%2F%2Flocalhost%2Fmyapp%2F&response_mode=query&scope=offline_access%20user.read%20mail.read&state=12345" target="_blank">https://login.microsoftonline.com/common/oauth2/v2.0/authorize...</a>

### <a name="authorization-response"></a>承認応答

ユーザーがアプリがリクエストした権限に同意した場合、応答には `code` パラメーターに承認コードが含まれます。以前の要求に対して成功した応答の例を次に示します。要求の `response_mode` パラメーターが `query` に設定されているため、応答はリダイレクト URL のクエリ文字列で返されます。

```
GET https://localhost/myapp/?
code=M0ab92efe-b6fd-df08-87dc-2c6500a7f84d
&state=12345
```

| パラメーター | 説明 |
| --- | --- |
| code |アプリが要求した authorization_code。アプリは、認証コードを使用してターゲット リソースのアクセス トークンを要求できます。authorization_code は非常に短期間であり、通常は約 10 分後に期限が切れます。 |
| state |state パラメーターが要求に含まれている場合は、同じ値が応答に表示されます。アプリは要求と応答の state 値が同じであることを確認する必要があります。 |

## <a name="3-get-a-token"></a>3.トークンを取得する

アプリは前の手順で受け取った承認 `code` を使用して、`/token` エンドポイントに `POST` 要求を送信することにより、アクセス トークンを要求します。

### <a name="token-request"></a>トークン要求

```
// Line breaks for legibility only

POST /{tenant}/oauth2/v2.0/token HTTP/1.1
Host: https://login.microsoftonline.com
Content-Type: application/x-www-form-urlencoded

client_id=6731de76-14a6-49ae-97bc-6eba6914391e
&scope=user.read%20mail.read
&code=OAAABAAAAiL9Kn2Z27UubvWFPbm0gLWQJVzCTE9UkP3pSx1aXxUjq3n8b2JRLk4OxVXr...
&redirect_uri=http%3A%2F%2Flocalhost%2Fmyapp%2F
&grant_type=authorization_code
&client_secret=JqQX2PNo9bpM0uEihUPzyrh    // NOTE: Only required for web apps
```

| パラメーター |  | 説明 |
| --- | --- | --- |
| tenant |必須出席者 |要求のパスで `{tenant}` 値を使用して、アプリケーションにサインインできるユーザーを制御できます。許可される値は、Microsoft のアカウントと職場または学校のアカウントの両方に `common`、職場または学校のアカウントのみに `organizations`、Microsoft のアカウントのみに `consumers`。また、テナント ID やドメイン名などのテナント識別子が含まれています。詳細については、[プロトコルの基本情報](https://docs.microsoft.com/azure/active-directory/develop/active-directory-v2-protocols#endpoints)を参照してください。 |
| client_id |必須 |[登録ポータル](https://go.microsoft.com/fwlink/?linkid=2083908)によってアプリに割り当てられたアプリケーション ID。 |
| grant_type |必須 |認可コードのフローの `authorization_code` になる必要があります。 |
| scope |必須出席者 |スコープのスペースで区切られた一覧。この区間で要求されたスコープは、最初の (承認) 区間で要求されたスコープと同じか、サブセットである必要があります。この要求で指定されたスコープが複数のリソース サーバーにまたがる場合、v2.0 エンドポイントは最初のスコープで指定されたリソースのトークンを返します。 |
| code |必須 |フローの最初の区間で取得した authorization_code。 |
| redirect_uri |必須 |authorization_code の取得に使用されたものと同じ redirect_uri 値。 |
| client_secret |Web アプリに必須。 |アプリのアプリ登録ポータルで作成したアプリケーション シークレット。client_secrets はデバイスに確実に保存できないため、ネイティブ アプリでは使用しないでください。Web アプリと Web API に必須。これには、サーバー側に client_secret を安全に保存する機能があります。 |

### <a name="token-response"></a>トークンの応答

アクセス トークンはアプリに対して不透明ですが、応答には、そのアクセス トークンが `scope` パラメーターに適しているアクセス許可の一覧が含まれています。 

```
{
    "token_type": "Bearer",
    "scope": "user.read%20Fmail.read",
    "expires_in": 3600,
    "access_token": "eyJ0eXAiOiJKV1QiLCJhbGciOiJSUzI1NiIsIng1dCI6Ik5HVEZ2ZEstZnl0aEV1Q...",
    "refresh_token": "AwABAAAAvPM1KaPlrEqdFSBzjqfTGAMxZGUTdM0t4B4..."
}
```

| パラメーター | 説明 |
| --- | --- |
| token_type |トークンの種類の値を示します。Azure AD がサポートしている種類はベアラーのみです。 |
| scope |access_token が有効な Microsoft Graph のアクセス許可のスペースで区切った一覧。 |
| expires_in |アクセス トークンの有効期間 (秒単位)。 |
| access_token |要求されたアクセス トークン。アプリはこのトークンを、Microsoft Graph の呼び出しで使用できます。 |
| refresh_token |OAuth 2.0 の更新トークン。 アプリはこのトークンを使用して、現在のアクセス トークンの有効期限が切れた後、追加のアクセス トークンを取得します。  更新トークンは有効期限が長く、長期間にわたってリソースへのアクセスを保持するために使用できます。  詳細については、「[Azure Active Directory v2.0 トークン リファレンス](https://docs.microsoft.com/azure/active-directory/develop/active-directory-v2-tokens)」を参照してください。 |

## <a name="4-use-the-access-token-to-call-microsoft-graph"></a>4.アクセス トークンを使用して、Microsoft Graph を呼び出す

アクセス トークンの取得後は、そのトークンを使用して (トークンを要求の `Authorization` ヘッダーに含める)、Microsoft Graph を呼び出すことができます。次の要求は、サインインしたユーザーのプロファイルを取得します。

```
GET https://graph.microsoft.com/v1.0/me 
Authorization: Bearer eyJ0eXAiO ... 0X2tnSQLEANnSPHY0gKcgw
Host: graph.microsoft.com

```

正常な応答は次のようになります (一部の応答ヘッダーは削除されています)。

```
HTTP/1.1 200 OK
Content-Type: application/json;odata.metadata=minimal;odata.streaming=true;IEEE754Compatible=false;charset=utf-8
request-id: f45d08c0-6901-473a-90f5-7867287de97f
client-request-id: f45d08c0-6901-473a-90f5-7867287de97f
OData-Version: 4.0
Duration: 727.0022
Date: Thu, 20 Apr 2017 05:21:18 GMT
Content-Length: 407

{
    "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#users/$entity",
    "id":"12345678-73a6-4952-a53a-e9916737ff7f",
    "businessPhones":[
        "+1 555555555"
    ],
    "displayName":"Chris Green",
    "givenName":"Chris",
    "jobTitle":"Software Engineer",
    "mail":null,
    "mobilePhone":"+1 5555555555",
    "officeLocation":"Seattle Office",
    "preferredLanguage":null,
    "surname":"Green",
    "userPrincipalName":"ChrisG@contoso.onmicrosoft.com"
}
```

## <a name="5-use-the-refresh-token-to-get-a-new-access-token"></a>5.更新トークンを使用して新しいアクセス トークンを取得する

アクセス トークンの保存期間は短く、リソースへのアクセスを続行するには期限が切れた後で更新する必要があります。これは、`/token` エンドポイントに別の `POST` 要求を送信することで行うことができます。今回は、`code` の代わりに `refresh_token` を提供します。

### <a name="request"></a>要求

```
// Line breaks for legibility only

POST /common/oauth2/v2.0/token HTTP/1.1
Host: https://login.microsoftonline.com
Content-Type: application/x-www-form-urlencoded

client_id=6731de76-14a6-49ae-97bc-6eba6914391e
&scope=user.read%20mail.read
&refresh_token=OAAABAAAAiL9Kn2Z27UubvWFPbm0gLWQJVzCTE9UkP3pSx1aXxUjq...
&redirect_uri=http%3A%2F%2Flocalhost%2Fmyapp%2F
&grant_type=refresh_token
&client_secret=JqQX2PNo9bpM0uEihUPzyrh      // NOTE: Only required for web apps
```

| パラメーター |  | 説明 |
| --- | --- | --- |
| client_id |必須 |[登録ポータル](https://go.microsoft.com/fwlink/?linkid=2083908)によってアプリに割り当てられたアプリケーション ID。 |
| grant_type |必須 |`refresh_token` である必要があります。 |
| scope |必須出席者 |アクセス許可 (scope) のスペースで区切られた一覧。要求されたアクセス許可は、元の authorization_code 要求で要求されたアクセス許可と同じか、サブセットである必要があります。 |
| refresh_token |必須 |トークン要求の間に取得した refresh_token。 |
| redirect_uri |必須 |authorization_code の取得に使用されたものと同じ redirect_uri 値。 |
| client_secret |Web アプリに必須。 |アプリのアプリ登録ポータルで作成したアプリケーション シークレット。client_secrets はデバイスに確実に保存できないため、ネイティブ アプリでは使用しないでください。Web アプリと Web API に必須。これには、サーバー側に client_secret を安全に保存する機能があります。 |

### <a name="response"></a>応答

正常なトークン応答は、次のようになります。

```
{
    "access_token": "eyJ0eXAiOiJKV1QiLCJhbGciOiJSUzI1NiIsIng1dCI6Ik5HVEZ2ZEstZnl0aEV1Q...",
    "token_type": "Bearer",
    "expires_in": 3599,
    "scope": "user.read%20mail.read",
    "refresh_token": "AwABAAAAvPM1KaPlrEqdFSBzjqfTGAMxZGUTdM0t4B4...",
}
```
| パラメーター | 説明 |
| --- | --- |
| access_token |要求されたアクセス トークン。アプリはこのトークンを Microsoft Graph の呼び出しで使用できます。 |
| token_type |トークンの種類の値を示します。Azure AD がサポートしている種類はベアラーのみです。 |
| expires_in |アクセス トークンの有効期間 (秒単位)。 |
| scope |access_token が有効なアクセス許可 (scope)。 |
| refresh_token |新しい OAuth 2.0 の更新トークン。更新トークンを可能な限り長く有効にしておくために、古い更新トークンをこの新しく取得した更新トークンと置き換える必要があります。 |

## <a name="supported-app-scenarios-and-additional-resources"></a>サポートされているアプリのシナリオと追加のリソース

Microsoft Graph は、次に示す種類のアプリから、ユーザーの代わりに呼び出すことができます。

- [ネイティブ/モバイル アプリ](https://docs.microsoft.com/azure/active-directory/develop/scenario-mobile-overview)
- [Web アプリ](https://docs.microsoft.com/azure/active-directory/develop/scenario-web-app-call-api-overview)
- [シングル ページ アプリ (SPA)](https://docs.microsoft.com/azure/active-directory/develop/scenario-spa-overview)
- [バックエンド Web API](https://docs.microsoft.com/azure/active-directory/develop/scenario-web-app-call-api-overview): たとえば、ネイティブ アプリなどのクライアント アプリが Web API のバックエンドで機能を実装するシナリオなどの場合。 Microsoft ID プラットフォームのエンドポイントでは、クライアント アプリとバックエンドの Web API の両方に同じアプリケーション ID が必要です。

Microsoft ID プラットフォームのエンドポイントでサポートされているアプリのシナリオの詳細については、「[アプリのシナリオおよび認証フロー](https://docs.microsoft.com/azure/active-directory/develop/authentication-flows-app-scenarios)」を参照してください。

> **注**: スタンドアロンの Web API からの Microsoft Graph の呼び出しは、現在 Microsoft ID プラットフォームのエンドポイントではサポートされていません。 このシナリオでは、Azure AD エンドポイントを使用する必要があります。

Microsoft ID プラットフォームのエンドポイントからユーザーに代わって Microsoft Graph にアクセスする方法の詳細については、次を参照してください。

- プロトコルのドキュメントへのリンクや、さまざまな種類のアプリでの作業の開始についての記事は、「[Microsoft ID プラットフォームのエンドポイントのドキュメント](https://docs.microsoft.com/azure/active-directory/develop/active-directory-appmodel-v2-overview)」を参照してください。
- サポートされているアプリケーション タイプと認証フローの詳細な説明については、「[v2.0 アプリ タイプ](https://docs.microsoft.com/azure/active-directory/develop/v2-app-types)」を参照してください。
- 推奨される認証ライブラリ (Microsoft およびサード パーティ) と Microsoft ID プラットフォーム用サーバー ミドルウェアの詳細については、「[Azure Active Directory v2.0 認証ライブラリ](https://docs.microsoft.com/azure/active-directory/develop/active-directory-v2-libraries)」を参照してください。

## <a name="endpoint-considerations"></a>エンドポイントに関する考慮事項

Microsoft では引き続き Azure AD エンドポイントをサポートします。 Microsoft ID プラットフォームのエンドポイントと Azure AD のエンドポイントの使用には、[いくつかの違い](https://docs.microsoft.com/azure/active-directory/develop/azure-ad-endpoint-comparison)があります。 Azure AD エンドポイントを使用する場合:

- アプリには、プラットフォームごとのアプリケーション ID (クライアント ID) が必要です。
- アプリがマルチ テナント アプリの場合は、[Azure ポータル](https://portal.azure.com)でマルチ テナントとなるよう明示的に設定する必要があります。
- アプリに必要なすべてのアクセス許可を開発者が構成する必要があります。 Azure AD エンドポイントは、動的 (増分) の同意をサポートしていません。
- Azure AD エンドポイントは、承認とトークンの要求に `resource` パラメーターを使用して、アクセス許可が必要な Microsoft Graph などのリソースを指定します。エンドポイントは `scope` パラメーターをサポートしていません。
- Azure AD エンドポイントは、管理者の同意用に特定のエンドポイントを公開しません。その代わりに、アプリは承認要求で `prompt=admin_consent`パラメーターを使用して、組織の管理者の同意を取得します。詳細については、「[Azure Active Directory とアプリケーションの統合](https://docs.microsoft.com/azure/active-directory/develop/active-directory-integrating-applications)」の「**実行時の Azure AD 同意フレームワークのトリガー**」を参照してください。

Azure AD エンドポイントからユーザーに代わって Microsoft Graph にアクセスする方法の詳細については、次を参照してください。

- さまざまな種類のアプリで Microsoft ID プラットフォームのエンドポイントを使用する方法については、「[Microsoft ID プラットフォームの開発者向けドキュメント](https://docs.microsoft.com/azure/active-directory/develop/active-directory-developers-guide)」の「**はじめに**」リンクを参照してください。 ドキュメントには、Microsoft ID プラットフォームのエンドポイントでサポートされているさまざまな種類のアプリの概要トピック、クイックスタート、チュートリアル、コード サンプル、およびプロトコル ドキュメントへのリンクが含まれています。
- Microsoft ID プラットフォームのエンドポイントで使用可能な Microsoft Authentication Library (MSAL) およびサーバー ミドルウェアの詳細については、「[Microsoft Authentication Library](https://docs.microsoft.com/azure/active-directory/develop/msal-overview)」を参照してください。

