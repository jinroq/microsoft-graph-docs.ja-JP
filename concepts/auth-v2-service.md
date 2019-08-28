---
title: ユーザーなしでアクセスを取得
description: 一部のアプリでは、ユーザーの代わりに独自の ID を使用して Microsoft Graph を呼び出します。 多くの場合、これらは、サインインしたユーザーが存在しないサーバー上で実行される、バックグラウンド サービスかデーモンです。
author: jackson-woods
localization_priority: Priority
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 106d1f79917427e68df4dcc738fb5720c3dd5ad8
ms.sourcegitcommit: 0329bbcd5f1b09a2a6c5f935a30c4560b6eed492
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/27/2019
ms.locfileid: "36633735"
---
# <a name="get-access-without-a-user"></a>ユーザーなしでアクセスを取得

一部のアプリでは、ユーザーの代わりに独自の ID を使用して Microsoft Graph を呼び出します。多くの場合、これらは、サインインしたユーザーが存在しないサーバー上で実行される、バックグラウンド サービスかデーモンです。この種のアプリの例として、夜間に起動して実行される電子メール アーカイブ サービスがあります。場合によっては、サインインしているユーザーが存在するアプリでも、独自の ID で Microsoft Graph を呼び出す必要があります。たとえば、サインインしたユーザーが所有している組織内の特権よりも高い特権を必要とする機能をアプリが使用する必要がある場合があります。  

独自の ID で Microsoft Graph を呼び出すアプリは、OAuth 2.0 [クライアント資格情報の付与フロー](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-client-creds-grant-flow)を使用して、Azure AD からアクセス トークンを取得します。このトピックでは、サービスを構成し、OAuth クライアント資格情報の付与フローを使用して、アクセス トークンを取得する基本的な手順について説明します。

## <a name="authentication-and-authorization-steps"></a>認証および承認の手順

サービスを構成し、サービスが独自の ID で Microsoft Graph を呼び出すために使用できる Microsoft ID プラットフォームのエンドポイントからトークンを取得するために必要となる、基本的な手順は次のとおりです。

1. アプリを登録する。
2. アプリで Microsoft Graph のアクセス許可を構成する。
3. 管理者の同意を取得する。
4. アクセス トークンを取得する。
5. アクセス トークンを使用して、Microsoft Graph を呼び出す。

## <a name="1-register-your-app"></a>1.アプリを登録する

Microsoft ID プラットフォームのエンドポイントで認証するには、まずアプリを [Azure アプリ登録ポータル](https://go.microsoft.com/fwlink/?linkid=2083908) で登録する必要があります。アプリを登録するには、Microsoft アカウントのほか、職場または学校のアカウントを使用できます。

独自の ID で Microsoft Graph を呼び出すサービスの場合は、Web プラットフォーム用のアプリを登録して、次の値をコピーする必要があります。

- Azure アプリ登録ポータルが割り当てたアプリケーション ID。
- クライアント (アプリケーション) シークレット。パスワードか、公開鍵や秘密鍵のペア (証明書) のいずれか。
- トークンの応答を受け取るためのサービスのリダイレクト URL。
- アプリに管理者の同意を要求する機能が実装されている場合は、サービスが管理者の同意の応答を受信するためのリダイレクト URL。  

Azure アプリ登録ポータルを使用してアプリを構成する手順については、「[アプリを登録する](./auth-register-app-v2.md)」を参照してください。

OAuth 2.0 クライアント資格情報の付与フローでは、Azure AD が割り当てたアプリケーション ID と、ポータルを使用して作成したアプリケーション シークレットを使用して、アプリが Microsoft ID プラットフォーム`/token`のエンドポイントで直接認証されます。

## <a name="2-configure-permissions-for-microsoft-graph"></a>2.Microsoft Graph のアクセス許可を構成する

独自の ID で Microsoft Graph を呼び出すアプリの場合、Microsoft Graph はアプリケーションのアクセス許可を公開します (Microsoft Graph は、ユーザーに代わって Microsoft Graph を呼び出すアプリの委任されたアクセス許可も公開できます)。アプリに必要なアプリケーションのアクセス許可は、アプリを登録する時点で事前に構成します。アプリケーションのアクセス許可には常に管理者の同意が必要です。管理者は、組織にアプリがインストールされるときに [Azure ポータル](https://portal.azure.com)を使用してこれらのアクセス許可に同意するか、構成済みのアクセス許可に管理者が同意することによりアプリでサインアップ エクスペリエンスを提供することができます。管理者の同意が Azure AD によって記録されると、アプリは再度同意を要求する必要なしにトークンを要求できます。Microsoft Graph で使用できるアクセス許可の詳細については、「[アクセス許可のリファレンス](./permissions-reference.md)」を参照してください。

[Azure アプリ登録ポータル](https://go.microsoft.com/fwlink/?linkid=2083908)でアプリのアプリケーション アクセス許可を構成するには、アプリケーションの [**API アクセス許可**] ページで [**アクセス許可を追加**]、[**Microsoft Graph**] の順に選択し、[**アプリケーションのアクセス許可**] でアプリに必要なアクセス許可を選択します。

次のスクリーンショットは、Microsoft Graph のアプリケーションのアクセス許可に対する **[アクセス許可の選択]** ダイアログ ボックスを示しています。

![Microsoft Graph のアプリケーションのアクセス許可に対する [アクセス許可の選択] ダイアログ。](./images/auth-v2/v2-application-permissions.png)

> **注**: アプリで必要になるアクセス許可の、最低限の権限セットを構成することをお勧めします。これにより、アクセス許可の長大なリストに同意を求めるものよりも快適なエクスペリエンスを管理者に提供できます。

## <a name="3-get-administrator-consent"></a>3.管理者の同意を取得する

管理者に任せて [Azure ポータル](https://portal.azure.com)でアプリケーションに必要なアクセス許可を付与することができます。ただし、多くの場合、Microsoft ID プラットフォーム`/adminconsent`のエンドポイントを使用して管理者にサインアップ エクスペリエンスを提供するほうが優れた選択肢になります。 

> **重要**:構成済みのアクセス許可に変更を加える場合は常に、管理者の同意プロセスも繰り返す必要があります。 アプリ登録ポータルで行われた変更は、テナント管理者が同意を再適用するまで反映されません。

### <a name="request"></a>要求

```
// Line breaks are for legibility only.

GET https://login.microsoftonline.com/{tenant}/adminconsent
?client_id=6731de76-14a6-49ae-97bc-6eba6914391e
&state=12345
&redirect_uri=https://localhost/myapp/permissions
```

| パラメーター     | 条件   | 説明 
|:--------------|:------------|:------------
| tenant        | 必須    | アクセス許可の要求元のディレクトリ テナント。これは、GUID またはフレンドリ名の形式で指定できます。ユーザーが所属しているテナントがわからないときに、そのユーザーを任意のテナントでサインインさせる場合は、`common` を使用します。
| client_id     | 必須    | [Azure アプリ登録ポータル](https://go.microsoft.com/fwlink/?linkid=2083908)がアプリに割り当てたアプリケーション ID。
| redirect_uri  | 必須    | アプリが処理するために応答を送信するリダイレクト URI。URL でエンコードされている必要があることを除き、ポータルに登録したリダイレクト URI のいずれかに完全に一致する必要があります。また追加のパス セグメントを含めることができます。
| state         | 推奨 | トークン応答でも返される、要求に含まれている値。任意のコンテンツの文字列にすることができます。state は、使用していたページまたはビューなど、認証要求が発生する前の、アプリでのユーザーの状態に関する情報をエンコードするために使用されます。

### <a name="administrator-consent-experience"></a>管理者の同意エクスペリエンス

`/adminconsent` エンドポイントへの要求では、Azure AD はテナント管理者のみがサインインして要求を完了できるように強制します。管理者は、アプリ登録ポータルでユーザーがアプリに対して要求したすべてのアプリケーションのアクセス許可を承認するよう求められます。

Azure AD が管理者に提示する同意ダイアログの例を次に示します。

![管理者の同意ダイアログ。](./images/admin-consent.png)

### <a name="response"></a>応答

管理者がアプリケーションのアクセス許可を承認した場合、成功応答は次のようになります。

```
// Line breaks are for legibility only.

GET https://localhost/myapp/permissions
?tenant=a8990e1f-ff32-408a-9f8e-78d3b9139b95&state=12345
&admin_consent=True
```

| パラメーター     | 説明
|:--------------|:------------
| tenant        | 要求されたアクセス許可をアプリケーションに付与したディレクトリ テナント (GUID 形式)。
| state         | トークン応答でも返される、要求に含まれている値。任意のコンテンツの文字列にすることができます。state は、使用していたページまたはビューなど、認証要求が発生する前の、アプリでのユーザーの状態に関する情報をエンコードするために使用されます。
| admin_consent | **true** に設定します。


> **お試しください**:次の要求をブラウザーに貼り付けて、これを試してみることができます。Azure AD テナントのグローバル管理者としてサインインすると、アプリの管理者の同意ダイアログ ボックスが表示されます。(これは、前述の同意ダイアログ ボックスのスクリーンショットのアプリとは別のアプリになります。)
> 
> https://login.microsoftonline.com/common/adminconsent?client_id=6731de76-14a6-49ae-97bc-6eba6914391e&state=12345&redirect_uri=https://localhost/myapp/permissions 

## <a name="4-get-an-access-token"></a>4. アクセス トークンを取得する

OAuth 2.0 クライアント資格情報の付与フローでは、アプリの登録時に保存したアプリケーション ID とアプリケーション シークレットの値を使用して、Microsoft ID プラットフォーム`/token`のエンドポイントからアクセス トークンを直接要求します。

トークン要求の `scope` パラメーターの値として `https://graph.microsoft.com/.default` を渡すことにより、事前構成済みのアクセス許可を指定します。詳細については、次のトークン要求の `scope` パラメーターの説明を参照してください。

### <a name="token-request"></a>トークン要求

POST 要求を `/token` ID プラットフォームに送信して、アクセス トークンを取得します。

```
// Line breaks are for legibility only.

POST https://login.microsoftonline.com/{tenant}/oauth2/v2.0/token HTTP/1.1
Host: login.microsoftonline.com
Content-Type: application/x-www-form-urlencoded

client_id=535fb089-9ff3-47b6-9bfb-4f1264799865
&scope=https%3A%2F%2Fgraph.microsoft.com%2F.default
&client_secret=qWgdYAmab0YSkuL1qKv5bPX
&grant_type=client_credentials
```

| パラメーター     | 条件 | 説明 
|:--------------|:----------|:------------
| tenant        | 必須  | アクセス許可の要求元のディレクトリ テナント。これは、GUID またはフレンドリ名の形式で指定できます。
| client_id     | 必須  | アプリの登録時に [Azure アプリ登録ポータル](https://go.microsoft.com/fwlink/?linkid=2083908)が割り当てたアプリケーション ID。
| スコープ         | 必須  | この要求で `scope` パラメーターに渡される値は、必要なリソースのリソース識別子 (アプリケーション ID の URI) になっている必要があります (`.default` サフィックス付き)。 Microsoft Graph の場合、値は `https://graph.microsoft.com/.default` です。 この値は、アプリに構成した全アプリケーションのアクセス許可のうち、使用するリソースに関連付けられているアクセス許可のトークンを発行するように Microsoft ID プラットフォームに通知します。
| client_secret | 必須  | アプリケーション登録ポータルでアプリ用に生成したアプリケーション シークレット。
| grant_type    | 必須  | `client_credentials` である必要があります。

#### <a name="token-response"></a>トークンの応答

成功応答は、次のようになります。

```json
{
  "token_type": "Bearer",
  "expires_in": 3599,
  "access_token": "eyJ0eXAiOiJKV1QiLCJhbGciOiJSUzI1NiIsIng1dCI6Ik1uQ19WWmNBVGZNNXBP..."
}
```

| パラメーター     | 説明
|:--------------|:------------
| access_token  | 要求されたアクセス トークン。アプリはこのトークンを Microsoft Graph の呼び出しで使用できます。
| token_type    | トークンの種類の値を示します。Azure AD がサポートしている種類は `bearer` のみです。
| expires_in    | アクセス トークンの有効期間 (秒単位)。

## <a name="5-use-the-access-token-to-call-microsoft-graph"></a>5.アクセス トークンを使用して、Microsoft Graph を呼び出す

アクセス トークンの取得後は、そのトークンを使用して (トークンを要求の `Authorization` ヘッダーに含める)、Microsoft Graph を呼び出すことができます。次の要求は、特定のユーザーのプロファイルを取得します。この API を呼び出すには、アプリに _User.Read.All_ アクセス許可が必要です。

```
GET https://graph.microsoft.com/v1.0/users/12345678-73a6-4952-a53a-e9916737ff7f
Authorization: Bearer eyJ0eXAiO ... 0X2tnSQLEANnSPHY0gKcgw
Host: graph.microsoft.com
```
正常な応答は次のようになります (一部の応答ヘッダーは削除されています)。

```http
HTTP/1.1 200 OK
Content-Type: application/json;odata.metadata=minimal;odata.streaming=true;IEEE754Compatible=false;charset=utf-8
request-id: f45d08c0-6901-473a-90f5-7867287de97f
client-request-id: f45d08c0-6901-473a-90f5-7867287de97f
OData-Version: 4.0
Duration: 309.0273
Date: Wed, 26 Apr 2017 19:53:49 GMT
Content-Length: 407
```

```json
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

## <a name="supported-app-scenarios-and-resources"></a>サポートされているアプリのシナリオとリソース

独自の ID で Microsoft Graph を呼び出すアプリは、次に示す 2 つのカテゴリのいずれかに分類されます。

- サインインしたユーザーが存在しないサーバーで実行される[バックグラウンド サービス (デーモン)](https://docs.microsoft.com/azure/active-directory/develop/scenario-daemon-overview)。
- サインインしたユーザーは存在するが、独自の ID でも Microsoft Graph を呼び出すアプリ (たとえば、ユーザーの特権よりも高い特権を必要とする機能を使用するため)。

独自の ID で Microsoft Graph を呼び出すアプリは、OAuth 2.0 クライアントの認証情報の付与を使用して Azure AD で認証し、トークンを取得します。 Microsoft ID プラットフォームのエンドポイントの場合は、次のリソースを使用して、このシナリオについてさらに詳しく調べることができます。

- エラーへの対応を含む、クライアント資格情報の付与フローの完全な処理については、「[Azure Active Directory v2.0 と OAuth 2.0 クライアント資格情報フロー](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-client-creds-grant-flow)」を参照してください。
- サービスから Microsoft Graph を呼び出すサンプルについては、GitHub の「[v2.0 デーモンのサンプル](https://github.com/Azure-Samples/active-directory-dotnet-daemon-v2)」を参照してください。
- 推奨される Microsoft ライブラリとサード パーティ製認証ライブラリの詳細については、「[Microsoft ID プラットフォームの認証ライブラリ](https://docs.microsoft.com/azure/active-directory/develop/reference-v2-libraries)」を参照してください。

## <a name="endpoint-considerations"></a>エンドポイントに関する考慮事項

Microsoft では引き続き Azure AD エンドポイントをサポートします。 Microsoft ID プラットフォームのエンドポイントと Azure AD のエンドポイントの使用には、[いくつかの違い](https://docs.microsoft.com/azure/active-directory/develop/azure-ad-endpoint-comparison)があります。 Azure AD エンドポイントを使用する場合:

- アプリがマルチ テナント アプリの場合は、[Microsoft Azure portal](https://portal.azure.com) でマルチ テナントとなるよう明示的に設定する必要があります。
- 管理者の同意エンドポイント (`/adminconsent`) はありません。 その代わりに、認証要求に `prompt=admin_consent` パラメーターを追加することで、アプリは実行時に管理者の同意を要求できます。 詳細については、「[Azure Active Directory とアプリケーションの統合](https://docs.microsoft.com/azure/active-directory/develop/active-directory-integrating-applications)」の「**実行時の Azure AD 同意フレームワークのトリガー**」を参照してください。
- 承認とトークン要求のパラメーターは異なります。たとえば、Azure AD エンドポイント要求には、`scope` パラメーターはありません。その代わりに、`resource` パラメーターを使用して、承認 (管理者の同意用) またはトークンが要求されているリソース (`resource=https://graph.microsoft.com`) の URI を指定します。

次のリソースを使用して、このシナリオについてさらに詳しく調べることができます。

- さまざまな種類のアプリで Microsoft ID プラットフォームを使用する方法については、「[Microsoft ID プラットフォームのドキュメント](https://docs.microsoft.com/azure/active-directory/develop/active-directory-developers-guide)」の「**はじめに**」リンクを参照してください。 ガイドには、Microsoft ID プラットフォームのサポートされているさまざまな種類のアプリの概要トピック、クイックスタート、チュートリアル、コード サンプル、およびプロトコル ドキュメントへのリンクが含まれています。
- Microsoft ID プラットフォームのエンドポイントで使用可能な Microsoft Authentication Library (MSAL) およびサーバー ミドルウェアの詳細については、「[Microsoft Authentication Library](https://docs.microsoft.com/azure/active-directory/develop/active-directory-authentication-libraries)」を参照してください。
