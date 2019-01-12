---
title: 承認と Microsoft Graph セキュリティ API
description: Microsoft Graph セキュリティ API からアクセスできるセキュリティ データは機密性が高く、アクセス許可と Azure Active Directory (Azure AD) ロールによって保護されています。
author: preetikr
localization_priority: Priority
ms.prod: security
ms.openlocfilehash: e20a9abd036414eefc750fd667dbf7c1004b65bb
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27947086"
---
# <a name="authorization-and-the-microsoft-graph-security-api"></a>承認と Microsoft Graph セキュリティ API

Microsoft Graph セキュリティ API からアクセスできるセキュリティ データは機密性が高く、アクセス許可と Azure Active Directory (Azure AD) ロールによって保護されています。

Microsoft Graph セキュリティ API では 2 種類の承認がサポートされています。

- **アプリケーション レベルの承認** - ユーザーはサインインしません (例: SIEM シナリオ)。 アプリケーションに付与されたアクセス許可によって、承認が決定します。 
    >**注:** このオプションは、アプリケーションがロール ベースのアクセス制御 (RBAC) を管理しているケースにも対応します。
- **ユーザーにより委任された承認** - Azure AD テナントのメンバーであるユーザーがサインインしています。 アプリケーションに必要なアクセス許可が付与されており、ユーザーが Azure AD 制限付き管理者ロール ([セキュリティ閲覧者] または [セキュリティ管理者]) のメンバーである必要があります。

Graph エクスプローラーから Microsoft Graph セキュリティ API を呼び出す場合:

- Azure AD テナント管理者は、要求されたアクセス許可を Graph エクスプローラー アプリケーションに付与することに明示的に同意する必要があります。
- ユーザーは、Azure AD の [セキュリティ閲覧者] 制限付き管理者ロールのメンバーである必要があります ([セキュリティ閲覧者] または [セキュリティ管理者] のいずれか)。

>**注**: Graph エクスプローラーでは、アプリケーション レベルの承認がサポートされていません。

カスタム アプリケーションまたは独自のアプリケーションから Microsoft Graph セキュリティ API を呼び出す場合:

- Azure AD テナント管理者は、アプリケーションに対して明示的に承認を与える必要があります。 これは、アプリケーション レベルの承認と、ユーザーにより委任された承認の両方に必要です。
- ユーザーにより委任された承認を使用する場合、ユーザーは、Azure AD の [セキュリティ閲覧者] または [セキュリティ管理者] 制限付き管理者ロールのメンバーである必要があります。

## <a name="manage-authorization-in-security-api-client-applications"></a>セキュリティ API クライアント アプリケーションで承認を管理する

Microsoft Graph セキュリティ API から提供されるセキュリティ データは機密性が高く、適切な認証および承認メカニズムを使用して保護する必要があります。 次の表に、Microsoft Graph セキュリティ API にアクセスできるクライアント アプリケーションを登録および作成する手順を示します。

| **対象者** | **操作** |
|:---------------------|:------------------|
|アプリケーション開発者または所有者|アプリケーションをエンタープライズ アプリケーションとして登録します。|
|テナント管理者|アプリケーションにアクセス許可を付与します。|
|テナント管理者|ユーザーにロールを割り当てます。|
|アプリケーション開発者|ユーザーとしてサインインし、アプリケーションを使用して Microsoft Graph セキュリティ API にアクセスします。|

アプリケーションの登録では、アプリケーションの実行に必要なアクセス許可だけが定義されます。 これらのアクセス許可はアプリケーションに付与されません。

Azure AD テナント管理者は、アプリケーションにアクセス許可を明示的に付与する必要があります。 これはテナントごとに実行し、またアプリケーション登録ポータルでアプリケーションのアクセス許可が変更される*たびに実行する*必要があります。

たとえば、2 つの Azure AD テナント (**T1** および **T2**) と 2 つのアクセス許可 (**P1** および **P2**) があるとします。 承認プロセスを以下に示します。

- アプリケーションがアクセス許可 **P1** を必要とすることが登録されます。
- テナント **T1** のユーザーがこのアプリケーションの Azure AD トークンを取得すると、このトークンにはアクセス許可が含まれていません。
- テナント **T1** の Azure AD 管理者が、アプリケーションにアクセス許可を明示的に付与します。 テナント **T1** のユーザーがこのアプリケーションの Azure AD トークンを取得すると、このトークンにはアクセス許可 **P1** が含まれています。
- テナント **T2** のユーザーがアプリケーションの Azure AD トークンを取得すると、このトークンにはアクセス許可が含まれていません。これは、テナント **T2** の管理者がアプリケーションにアクセス許可をまだ付与していないためです。 アクセス許可は*テナントごと*および*アプリケーションごと*に付与する必要があります。
- アプリケーションの登録が変更され、アクセス許可 **P1** と **P2** が必要になりました。
- テナント **T1** のユーザーがこのアプリケーションの Azure AD トークンを取得すると、このトークンにはアクセス許可 **P1** だけが含まれています。 アプリケーションに付与されたアクセス許可は、付与された内容のスナップショットとして記録されます。アプリケーションの登録 (アクセス許可) を変更しても、アクセス許可は*自動的には変更されません*。
- テナント **T2** の管理者がアクセス許可 **P1** と **P2** をアプリケーションに付与します。 次にテナント **T2** のユーザーがこのアプリケーションの Azure AD トークンを取得すると、このトークンにはアクセス許可 **P1** と **P2** が含まれています。

>**注**: テナント **T1** のアプリケーションとテナント **T2** のアプリケーションの Azure AD トークンに含まれているアクセス許可はそれぞれ異なります。これは、それぞれのテナント管理者がアプリケーションに対して異なるアクセス許可を付与しているためです。

- アプリケーションをテナント **T1** で再び実行できるようにするには、テナント **T1** の管理者が、アクセス許可 **P1** と **P2** をアプリケーションに明示的に付与する必要があります。

## <a name="register-an-application-in-the-azure-ad-v20-endpoint"></a>Azure AD v2.0 エンドポイントでアプリケーションを登録する

Azure AD v2.0 エンドポイントでアプリケーションを登録するには、次の情報が必要です。

- **アプリケーション名** - アプリケーション名として使用される文字列。
- **リダイレクト URL** - Azure AD からの承認応答の送信先 URL。 最初に、テスト クライアント Web アプリケーション ホーム ページを使用できます。
- **必要なアクセス許可** - アプリケーションが Microsoft Graph を呼び出すことができるようにするために必要なアクセス許可。

アプリケーションを登録するには、次の操作を行います。

1. https://apps.dev.microsoft.com/ に移動し、サインインします。
    >**注**: テナント管理者である必要はありません。**[マイ アプリケーション]** リストにリダイレクトされます。
2. 新しいアプリケーションを作成するため、**[アプリの追加]** を選択し、**[アプリケーション名]** にアプリケーションを入力します、
3. 新しいアプリケーションの登録ページで **[プラットフォームの追加]** > **[Web]** を選択します。 **[リダイレクト URL]** フィールドにリダイレクト URL を入力します。
4. **[Microsoft Graph のアクセス許可]** セクションの **[委任されたアクセス許可]** で、**[追加]** を選択します。 ダイアログ ボックスで、必要なアクセス許可を選択します。 アクセス許可のリストについては、「[セキュリティのアクセス許可](permissions-reference.md#security-permissions)」を参照してください。

    >Microsoft Graph セキュリティ API では、GET クエリに SecurityEvents.Read.All スコープ、PATCH/POST クエリに SecurityEvents.ReadWrite.All スコープが必要です。

5. **[保存]** を選択します。

以下の情報を保存します。

- アプリケーション ID
- リダイレクト URL
- 必要なアクセス許可のリスト

詳細については、「[アプリを Azure AD v2.0 エンドポイントに登録する](auth-register-app-v2.md)」を参照してください。

## <a name="grant-permissions-to-an-application"></a>アプリケーションにアクセス許可を付与する

アプリケーションの登録では、アプリケーションに必要なアクセス許可が定義されますが、アプリケーションにこれらのアクセス許可は付与されません。 Azure AD テナント管理者は、管理者の同意エンドポイントを呼び出して、これらのアクセス許可を明示的に付与する必要があります。 詳細については、「[管理者の同意エンドポイントを使用する](https://docs.microsoft.com/ja-JP/azure/active-directory/develop/active-directory-v2-scopes#using-the-admin-consent-endpoint)」を参照してください。

アプリケーションにアクセス許可を付与するには、以下の情報が必要です。

- **アプリケーション ID** - アプリケーション登録ポータルのアプリケーション ID。
- **リダイレクト URL** - アプリケーション登録ポータルで認証応答のために設定した文字列。

アクセス許可を付与するには、次の操作を行います。

- テキスト エディターで、以下の URL 文字列を作成します。

    `https://login.microsoftonline.com/common/adminconsent?client_id=<Application Id>&state=12345&redirect_uri=<Redirect URL>`

- Web ブラウザーでこの URL に移動し、テナント管理者としてサインインします。 ダイアログ ボックスに、アプリケーション登録ポータルで指定した、アプリケーションに必要なアクセス許可のリストが表示されます。 **[OK]** を選択し、アプリケーションにこれらのアクセス許可を付与します。

> **注:** この手順では、アクセス許可がユーザーではなくアプリケーションに付与されます。 つまり、このアプリケーションを使用する Azure AD テナントに属するすべてのユーザー (管理者以外のユーザーを含む) に、これらのアクセス許可が付与されます。

## <a name="assign-azure-ad-roles-to-users"></a>Azure AD のロールをユーザーに割り当てる

アプリケーションにアクセス許可が付与されると、そのアプリケーションにアクセスできるすべてのユーザー (Azure AD テナントのメンバー) に、付与されたアクセス許可が与えられます。 機密性の高いセキュリティ データの保護を強化するため、Microsoft Graph セキュリティ API では、ユーザーに Azure AD の **[セキュリティ閲覧者]** ロールが割り当てられている必要があります。 詳細については、「[Azure Active Directory での管理者ロールの割り当て](https://docs.microsoft.com/ja-JP/azure/active-directory/active-directory-assign-admin-roles-azure-portal)」と「[Azure Active Directory でユーザーを管理者ロールに割り当てる](https://docs.microsoft.com/ja-JP/azure/active-directory/active-directory-users-assign-role-azure-portal)」を参照してください。

>**注:** この手順を実行するには、テナント管理者でなければなりません。

ユーザーにロールを割り当てるには、次の操作を行います。

- [Azure Portal](https://portal.azure.com) (https://portal.azure.com) にサインインします。
- メニューで **[Azure Active Directory]** > **[ユーザー]** を選択します。
- ユーザーの名前を選択します。
- **[管理]** > **[ディレクトリ ロール]** を選択します。
- **[制限付き管理者]** を選択し、**[セキュリティ閲覧者]** チェック ボックスをオンにします。
- **[保存]** を選択します。

## <a name="create-an-authentication-code"></a>認証コードを作成する

認証コードを作成するには、以下の情報が必要です。

- **アプリケーション ID** - アプリケーション登録ポータルのアプリケーション ID。
- **リダイレクト URL** - Azure AD からの承認応答の送信先 URL。 最初に、https://localhost またはテスト クライアント Web アプリケーション ホーム ページを使用できます。
- **アプリケーション キー** (オプション) - アプリケーションのキー。 これは、アプリケーション専用認証コードを使用するアプリケーションを開発する場合に適用されます (つまりユーザーにより委任される認証はサポートされません)。

次の表に、認証コードの作成に使用できるリソースを示します。

|**アプリケーションの種類**|**認証ライブラリ**|
|------------------------|----------------------------|
|[デスクトップ アプリケーション - iOS](https://docs.microsoft.com/ja-JP/azure/active-directory/develop/guidedsetups/active-directory-ios)|[MSAL.framework: iOS 用 Microsoft Authentication Library プレビュー](https://github.com/AzureAD/microsoft-authentication-library-for-objc)|
|[デスクトップ アプリケーション - Android](https://docs.microsoft.com/ja-JP/azure/active-directory/develop/guidedsetups/active-directory-android)|[Microsoft Authentication Library (MSAL)](https://javadoc.io/doc/com.microsoft.identity.client/msal)|
|[デスクトップ アプリケーション - .Net](https://docs.microsoft.com/ja-JP/azure/active-directory/develop/guidedsetups/active-directory-windesktop)|[Microsoft Authentication Library (MSAL)](https://www.nuget.org/packages/Microsoft.Identity.Client)|
|[Web アプリケーション - JavaScript SPA](https://docs.microsoft.com/ja-JP/azure/active-directory/develop/guidedsetups/active-directory-javascriptspa)|[JavaScript 用 Microsoft Authentication Library プレビュー](https://github.com/AzureAD/microsoft-authentication-library-for-js)|
|[Web アプリケーション - .NET Web Server](https://docs.microsoft.com/ja-JP/azure/active-directory/develop/guidedsetups/active-directory-aspnetwebapp)|OpenIdConnection、Cookies、SystemWeb|
|[Web アプリケーション - NodeJS Web アプリケーション](https://docs.microsoft.com/ja-JP/azure/active-directory/develop/active-directory-v2-devquickstarts-node-web)||

既存のライブラリを使用しないアプリケーションの場合は、「[ユーザーの代わりにアクセスを取得](auth-v2-user.md)」を参照してください。

1. Azure AD からコードを取得します。 呼び出すクエリには、アプリケーション ID、リダイレクト URI、および**必要なアクセス許可**のパラメーターが指定されています。
2. コードを使用してアクセス トークンを取得します。

OpenId Connect ライブラリを使用する場合は、「[Azure AD および OpenID Connect を使用して認証する](https://docs.microsoft.com/ja-JP/azure/architecture/multitenant-identity/authenticate)」を参照し、`app.UseOpenIdConnectAuthentication()` を呼び出してください。

>**注:** ユーザーにより委任された認証トークンを要求する場合、ライブラリのパラメーターは **Requested Scopes** です。 このパラメーターには、登録アプリケーションに必要なスコープではなく、User.Read を使用してください。 **Requested Scopes** パラメーターは、返される認証トークンに含まれるアクセス許可には影響しません。 これらのアクセス許可は、テナント管理者がアプリケーションに付与したアクセス許可によって決定します。

たとえば .NET MSAL ライブラリを使用している場合には、次のように呼び出します。

`var accessToken = (await client.AcquireTokenAsync(scopes)).AccessToken;`

>**注:** この例では、最小限の特権を持つアクセス許可 (User.Read など) を使用する必要があります。 ただし、返されるアクセス トークンには、テナント管理者が現在のユーザー テナントに付与したアクセス許可 (User.Read.All、User.ReadWrite.All など) が含まれることがあります。

Azure AD により、認証情報とアプリケーションに必要なアクセス許可が含まれているトークン (文字列) が返されます。 以下の例に示すように、このトークンをベアラー トークンとして HTTP ヘッダーに割り当てます。

`request.Headers.Authorization = new AuthenticationHeaderValue("bearer", accessToken);`

Microsoft Graph により、このトークンに含まれている情報が検証され、アクセスが付与または拒否されます。

返されるトークンに含まれている要求を確認するには、NuGet library System.IdentityModel.Tokens.Jwt を使用します。

`JwtSecurityTokenHandler tokenHandler = new JwtSecurityTokenHandler();`</br>
`var securityToken = tokenHandler.ReadToken(accessToken) as JwtSecurityToken;`

Microsoft Graph からの応答には、client-request-id というヘッダーが含まれています。これは GUID です。 アクセスが拒否される場合は、[Microsoft 技術コミュニティ](https://techcommunity.microsoft.com/t5/Microsoft-Graph-Security-API/ct-p/SecurityGraphAPI)でサポートを要請する際にこの GUID を指定してください。これにより、この認証エラーの原因の調査を支援できます。
