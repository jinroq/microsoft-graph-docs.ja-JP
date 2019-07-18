---
title: Microsoft Graph 認証プロバイダーを選択する
description: アプリケーションに対してシナリオ固有の認証プロバイダーを選択する方法について説明します。
localization_priority: Normal
author: MichaelMainer
ms.openlocfilehash: 7975a2049ee16d89cfc9668babde091db7dd140e
ms.sourcegitcommit: 9cee9d8229fc84dd7ef97670ff27c145e1a78408
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/18/2019
ms.locfileid: "35778300"
---
# <a name="choose-a-microsoft-graph-authentication-provider-based-on-scenario"></a>シナリオに基づいて Microsoft Graph 認証プロバイダを選択する

認証プロバイダーは、Microsoft 認証ライブラリ (MSAL) を使用してトークンを取得するために必要なコードを実装します。増分の同意、期限切れのパスワード、条件付きアクセスなど、さまざまなケースの潜在的なエラーを処理します。HTTP 要求認証ヘッダーを設定します。 次の表に、さまざまな[種類のアプリケーション](https://docs.microsoft.com/en-us/azure/active-directory/develop/v2-app-types)のシナリオに一致する一連のプロバイダーを示します。

|シナリオ | フロー/付与 | 対象ユーザー | プロバイダー|
|--|--|--|--|
| [シングルページアプリ](https://docs.microsoft.com/en-us/azure/active-directory/develop/scenario-spa-acquire-token)| | | |
| | 暗黙的 | 委任されたコンシューマー/組織 |[暗黙的プロバイダー](#ImplicitProvider) |
| [Web Api を呼び出す web アプリ](https://docs.microsoft.com/en-us/azure/active-directory/develop/scenario-web-app-call-api-acquire-token) | | | |
| | 認証コード | 委任されたコンシューマー/組織 | [認証コードプロバイダ](#AuthCodeProvider) |
| | クライアント資格情報  | App Only | [クライアント資格情報プロバイダー](#ClientCredentialsProvider) |
| [Web api を呼び出す web API](https://docs.microsoft.com/en-us/azure/active-directory/develop/scenario-web-api-call-api-acquire-token) | | | |
| | 代理人 | 委任されたコンシューマー/組織 | [プロバイダーに代わって](#OnBehalfOfProvider) |
| | クライアント資格情報  | App Only | [クライアント資格情報プロバイダー](#ClientCredentialsProvider) |
| [Web Api を呼び出すデスクトップアプリ](https://docs.microsoft.com/en-us/azure/active-directory/develop/scenario-desktop-acquire-token) | | | |
| | Interactive | 委任されたコンシューマー/組織 | [対話プロバイダー](#InteractiveProvider) |
| | 統合 Windows | 委任された組織 | [統合 Windows プロバイダ](#IntegratedWindowsProvider) |
| | リソース所有者  | 委任された組織 | [Username/Password Provider](#UsernamePasswordProvider) |
| | デバイスコード  | 委任された組織 | [デバイスコードプロバイダ](#DeviceCodeProvider) |
| [デーモンアプリ](https://docs.microsoft.com/en-us/azure/active-directory/develop/scenario-daemon-acquire-token) | | | |
| | クライアント資格情報  | App Only | [クライアント資格情報プロバイダー](#ClientCredentialsProvider) |
| [Web Api を呼び出すモバイルアプリ](https://docs.microsoft.com/en-us/azure/active-directory/develop/scenario-mobile-acquire-token) | | | |
| | Interactive | 委任されたコンシューマー/組織 | [対話プロバイダー](#InteractiveProvider) |


## <a name="a-nameauthcodeproviderauthorization-code-provider"></a><a name="AuthCodeProvider"/>認証コードプロバイダ

認証コードフローにより、ネイティブおよび web アプリはユーザーの名前でトークンを安全に取得することができます。 詳細については、「 [Microsoft identity platform And OAuth 2.0 認証コードフロー](https://docs.microsoft.com/en-us/azure/active-directory/develop/v2-oauth2-auth-code-flow)」を参照してください。

# <a name="ctabcs"></a>[C#](#tab/CS)

```csharp
IConfidentialClientApplication confidentialClientApplication = ConfidentialClientApplicationBuilder
    .Create(clientId)
    .WithRedirectUri(redirectUri)
    .WithClientSecret(clientSecret) // or .WithCertificate(certificate)
    .Build();

AuthorizationCodeProvider authProvider = new AuthorizationCodeProvider(confidentialClientApplication, scopes);  
```

# <a name="javascripttabjavascript"></a>[Javascript](#tab/Javascript)

認証コード、クライアント資格情報、および非代行の OAuth フローでは、この時点でカスタム認証プロバイダーを実装する必要があります。 詳細については、「 [Using a custom authentication provider](https://github.com/microsoftgraph/msgraph-sdk-javascript/blob/dev/docs/CustomAuthenticationProvider.md)」を参照してください。

# <a name="javatabjava"></a>[Java](#tab/Java)

```java
AuthorizationCodeProvider authProvider = new AuthorizationCodeProvider(
                                                    clientId,
                                                    scopes,
                                                    authorizationCode,
                                                    redirectUri,
                                                    clientSecret);
```

# <a name="androidtabandroid"></a>[Android](#tab/Android)

なし。

# <a name="objective-ctabobjective-c"></a>[目的-C](#tab/Objective-C)

なし。

# <a name="phptabphp"></a>[PHP](#tab/PHP)

まだ使用できません。 ユーザーにとって重要な場合は、 [Microsoft Graph の機能の要求](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests)をサポートするか、または開きます。

# <a name="rubytabruby"></a>[Ruby](#tab/Ruby)

まだ利用できません。 ユーザーにとって重要な場合は、 [Microsoft Graph の機能の要求](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests)に投票するか、開くようにしてください。

---

##  <a name="a-nameclientcredentialsproviderclient-credentials-provider"></a><a name="ClientCredentialsProvider"/>クライアント資格情報プロバイダー

クライアント資格情報フローを使用すると、ユーザーによる操作なしでサービスアプリケーションを実行できます。 Access は、アプリケーションの id に基づいています。 詳細については、「 [Microsoft identity platform」および「OAuth 2.0 クライアント資格情報フロー](https://docs.microsoft.com/en-us/azure/active-directory/develop/v2-oauth2-client-creds-grant-flow)」を参照してください。

# <a name="ctabcs"></a>[C#](#tab/CS)

```csharp
IConfidentialClientApplication confidentialClientApplication = ConfidentialClientApplicationBuilder
    .Create(clientId)
    .WithTenantId(tenantID)
    .WithClientSecret(clientSecret)
    .Build();

ClientCredentialProvider authProvider = new ClientCredentialProvider(confidentialClientApplication);
```

# <a name="javascripttabjavascript"></a>[Javascript](#tab/Javascript)

認証コード、クライアント資格情報、および非代行の OAuth フローでは、この時点でカスタム認証プロバイダーを実装する必要があります。 詳細については、「 [Using a custom authentication provider](https://github.com/microsoftgraph/msgraph-sdk-javascript/blob/dev/docs/CustomAuthenticationProvider.md)」を参照してください。

# <a name="javatabjava"></a>[Java](#tab/Java)

```java
ClientCredentialProvider authProvider = new ClientCredentialProvider(
                                                    clientId,
                                                    scopes,
                                                    clientSecret,
                                                    tenant,
                                                    endpoint);
```

# <a name="androidtabandroid"></a>[Android](#tab/Android)

なし。

# <a name="objective-ctabobjective-c"></a>[目的-C](#tab/Objective-C)

なし。

# <a name="phptabphp"></a>[PHP](#tab/PHP)

まだ利用できません。 ユーザーにとって重要な場合は、 [Microsoft Graph の機能の要求](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests)をサポートするか、または開きます。

# <a name="rubytabruby"></a>[Ruby](#tab/Ruby)

まだ利用できません。 ユーザーにとって重要な場合は、 [Microsoft Graph の機能の要求](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests)をサポートするか、または開きます。

---

##  <a name="a-nameonbehalfofprovideron-behalf-of-provider"></a><a name="OnBehalfOfProvider"/>プロバイダーの代理

アプリケーションが Microsoft Graph API を呼び出すサービスまたは web API を呼び出すときに、その代わりの流れが適用されます。 [Microsoft identity platform および OAuth 2.0 の送信フローの](https://docs.microsoft.com/en-us/azure/active-directory/develop/v2-oauth2-on-behalf-of-flow)詳細については、こちらを参照してください。

# <a name="ctabcs"></a>[C#](#tab/CS)

```csharp
IConfidentialClientApplication confidentialClientApplication = ConfidentialClientApplicationBuilder
    .Create(clientId)
    .WithRedirectUri(redirectUri)
    .WithClientSecret(clientSecret)
    .Build();

OnBehalfOfProvider authProvider = new OnBehalfOfProvider(confidentialClientApplication, scopes);
```

# <a name="javascripttabjavascript"></a>[Javascript](#tab/Javascript)

認証コード、クライアント資格情報、および非代行の OAuth フローでは、この時点でカスタム認証プロバイダーを実装する必要があります。 詳細については、「[カスタム認証プロバイダを使用する](https://github.com/microsoftgraph/msgraph-sdk-javascript/blob/dev/docs/CustomAuthenticationProvider.md)」を参照してください。

# <a name="javatabjava"></a>[Java](#tab/Java)

まだ使用できません。 ユーザーにとって重要な場合は、 [Microsoft Graph の機能の要求](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests)に投票するか、開くようにしてください。

# <a name="androidtabandroid"></a>[Android](#tab/Android)

なし。

# <a name="objective-ctabobjective-c"></a>[目的-C](#tab/Objective-C)

なし。

# <a name="phptabphp"></a>[PHP](#tab/PHP)

まだ使用できません。 ユーザーにとって重要な場合は、 [Microsoft Graph の機能の要求](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests)に投票するか、開くようにしてください。

# <a name="rubytabruby"></a>[Ruby](#tab/Ruby)

まだ使用できません。 ユーザーにとって重要な場合は、 [Microsoft Graph の機能の要求](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests)に投票するか、開くようにしてください。

---

## <a name="a-nameimplicitproviderimplicit-provider"></a><a name="ImplicitProvider"/>暗黙的プロバイダー

暗黙的な付与フローは、ブラウザーベースのアプリケーションで使用されます。 詳細については、「 [Microsoft identity platform」および「暗黙的な許可の流れ](https://docs.microsoft.com/en-us/azure/active-directory/develop/v2-oauth2-implicit-grant-flow)」を参照してください。

# <a name="ctabcs"></a>[C#](#tab/CS)

なし。

# <a name="javascripttabjavascript"></a>[Javascript](#tab/Javascript)

```javascript
const clientId = "your_client_id"; // Client Id of the registered application
const callback = (errorDesc, token, error, tokenType) => {};
// An Optional options for initializing the MSAL @see https://github.com/AzureAD/microsoft-authentication-library-for-js/wiki/MSAL-basics#configuration-options
const options = {
    redirectUri: "Your redirect URI",
};
const graphScopes = ["user.read", "mail.send"]; // An array of graph scopes

// Initialize the MSAL @see https://github.com/AzureAD/microsoft-authentication-library-for-js/wiki/MSAL-basics#initialization-of-msal
const userAgentApplication = new Msal.UserAgentApplication(clientId, undefined, callback, options);
const authProvider = new MicrosoftGraph.MSALAuthenticationProvider(userAgentApplication, graphScopes);

const options = {
    authProvider, // An instance created from previous step
};
const Client = MicrosoftGraph.Client;
const client = Client.initWithMiddleware(options);
```

# <a name="javatabjava"></a>[Java](#tab/Java)

なし。

# <a name="androidtabandroid"></a>[Android](#tab/Android)

なし。

# <a name="objective-ctabobjective-c"></a>[目的-C](#tab/Objective-C)

なし。

# <a name="phptabphp"></a>[PHP](#tab/PHP)

なし。

# <a name="rubytabruby"></a>[Ruby](#tab/Ruby)

なし。

---

##  <a name="a-namedevicecodeproviderdevice-code-provider"></a><a name="DeviceCodeProvider"/>デバイスコードプロバイダ

デバイスコードフローによって、別のデバイスを使用してデバイスにサインインできるようになります。 詳細については、「 [Microsoft identity platform」および「OAuth 2.0 デバイスコードフロー](https://docs.microsoft.com/en-us/azure/active-directory/develop/v2-oauth2-device-code)」を参照してください。

# <a name="ctabcs"></a>[C#](#tab/CS)

```csharp
IPublicClientApplication publicClientApplication = PublicClientApplicationBuilder
            .Create(clientId)
            .Build();

Func<DeviceCodeResult, Task> deviceCodeReadyCallback = async dcr => await Console.Out.WriteLineAsync(dcr.Message);

DeviceCodeProvider authProvider = new DeviceCodeProvider(publicClientApplication, scopes, deviceCodeReadyCallback);
```

# <a name="javascripttabjavascript"></a>[Javascript](#tab/Javascript)

まだ使用できません。 ユーザーにとって重要な場合は、 [Microsoft Graph の機能の要求](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests)に投票するか、開くようにしてください。

# <a name="javatabjava"></a>[Java](#tab/Java)

まだ利用できません。 ユーザーにとって重要な場合は、 [Microsoft Graph の機能の要求](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests)をサポートするか、または開きます。

# <a name="androidtabandroid"></a>[Android](#tab/Android)

なし。

# <a name="objective-ctabobjective-c"></a>[目的-C](#tab/Objective-C)

なし。

# <a name="phptabphp"></a>[PHP](#tab/PHP)

まだ使用できません。 ユーザーにとって重要な場合は、 [Microsoft Graph の機能の要求](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests)に投票するか、開くようにしてください。

# <a name="rubytabruby"></a>[Ruby](#tab/Ruby)

まだ使用できません。 ユーザーにとって重要な場合は、 [Microsoft Graph の機能の要求](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests)に投票するか、開くようにしてください。

---

##  <a name="a-nameintegratedwindowsproviderintegrated-windows-provider"></a><a name="IntegratedWindowsProvider"/>統合 Windows プロバイダ

統合 Windows フローにより、Windows コンピューターがドメインに参加している場合に、アクセストークンをサイレントに取得することができます。 詳細については、「[統合 Windows 認証](https://github.com/AzureAD/microsoft-authentication-library-for-dotnet/wiki/Integrated-Windows-Authentication)」を参照してください。

# <a name="ctabcs"></a>[C#](#tab/CS)

```csharp
IPublicClientApplication publicClientApplication = PublicClientApplicationBuilder
            .Create(clientId)
            .WithTenantId(tenantID)
            .Build();

IntegratedWindowsAuthenticationProvider authProvider = new IntegratedWindowsAuthenticationProvider(publicClientApplication, scopes);
```

# <a name="javascripttabjavascript"></a>[Javascript](#tab/Javascript)

なし。

# <a name="javatabjava"></a>[Java](#tab/Java)

なし。

# <a name="androidtabandroid"></a>[Android](#tab/Android)

なし。

# <a name="objective-ctabobjective-c"></a>[目的-C](#tab/Objective-C)

なし。

# <a name="phptabphp"></a>[PHP](#tab/PHP)

なし。

# <a name="rubytabruby"></a>[Ruby](#tab/Ruby)

なし。

---

##  <a name="a-nameinteractiveproviderinteractive-provider"></a><a name="InteractiveProvider"/>対話プロバイダー

対話型フローは、モバイルアプリケーション (Xamarin および UWP) およびデスクトップアプリケーションがユーザーの名前で Microsoft Graph を呼び出すために使用されます。 詳細については、「[トークンを対話的に取得](https://github.com/AzureAD/microsoft-authentication-library-for-dotnet/wiki/Acquiring-tokens-interactively)する」を参照してください。

# <a name="ctabcs"></a>[C#](#tab/CS)

```csharp
IPublicClientApplication publicClientApplication = PublicClientApplicationBuilder
            .Create(clientId)
            .Build();

InteractiveAuthenticationProvider authProvider = new InteractiveAuthenticationProvider(publicClientApplication, scopes);
```

# <a name="javascripttabjavascript"></a>[Javascript](#tab/Javascript)

まだ使用できません。 ユーザーにとって重要な場合は、 [Microsoft Graph の機能の要求](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests)に投票するか、開くようにしてください。

# <a name="javatabjava"></a>[Java](#tab/Java)

まだ使用できません。 ユーザーにとって重要な場合は、 [Microsoft Graph の機能の要求](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests)に投票するか、開くようにしてください。

# <a name="androidtabandroid"></a>[Android](#tab/Android)

```java
PublicClientApplication publicClientApplication = new PublicClientApplication(getApplicationContext(), "CLIENT_ID_OF_YOUR_APPLICATION");
MSALAuthenticationProvider msalAuthenticationProvider = new MSALAuthenticationProvider(
    getActivity(),
    getApplication(),
    publicClientApplication,
    scopes);

IGraphServiceClient graphClient =
  GraphServiceClient
    .builder()
    .authenticationProvider(msalAuthenticationProvider)
    .buildClient();
```

# <a name="objective-ctabobjective-c"></a>[目的-C](#tab/Objective-C)

```objc
NSError *error = nil;
MSALPublicClientApplication *publicClientApplication = [[MSALPublicClientApplication alloc] initWithClientId:@"INSERT-CLIENT-APP-ID" 
error:&error];

MSALAuthenticationProviderOptions *authProviderOptions= [[MSALAuthenticationProviderOptions alloc] initWithScopes:<array-of-scopes-for-which-you-need-access-token>];

 MSALAuthenticationProvider *authenticationProvider = [[MSALAuthenticationProvider alloc] initWithPublicClientApplication:publicClientApplication 
 andOptions:authProviderOptions];
```

# <a name="phptabphp"></a>[PHP](#tab/PHP)

なし。

# <a name="rubytabruby"></a>[Ruby](#tab/Ruby)

なし。

---

##  <a name="a-nameusernamepasswordproviderusernamepassword-provider"></a><a name="UsernamePasswordProvider"/>Username/password provider

Username/password プロバイダーを使用すると、アプリケーションはユーザー名とパスワードを使用してユーザーにサインインできます。 このフローは、他の OAuth フローを使用できない場合にのみ使用してください。 詳細については、「 [Microsoft identity platform」および「OAuth 2.0 resource owner password credential](https://docs.microsoft.com/en-us/azure/active-directory/develop/v2-oauth-ropc) 」を参照してください。



# <a name="ctabcs"></a>[C#](#tab/CS)

```csharp
IPublicClientApplication publicClientApplication = PublicClientApplicationBuilder
            .Create(clientId)
            .WithTenantId(tenantID)
            .Build();

UsernamePasswordProvider authProvider = new UsernamePasswordProvider(publicClientApplication, scopes);

GraphServiceClient graphClient = new GraphServiceClient(authProvider);

User me = await graphClient.Me.Request()
                .WithUsernamePassword(email, password)
                .GetAsync();
```

# <a name="javascripttabjavascript"></a>[Javascript](#tab/Javascript)

まだ使用できません。 ユーザーにとって重要な場合は、 [Microsoft Graph の機能の要求](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests)に投票するか、開くようにしてください。

# <a name="javatabjava"></a>[Java](#tab/Java)

```java
UsernamePasswordProvider authProvider = new UsernamePasswordProvider(
                                                    clientId,
                                                    scopes,
                                                    username,
                                                    password);
```

# <a name="androidtabandroid"></a>[Android](#tab/Android)

なし。

# <a name="objective-ctabobjective-c"></a>[目的-C](#tab/Objective-C)

なし。

# <a name="phptabphp"></a>[PHP](#tab/PHP)

まだ使用できません。 ユーザーにとって重要な場合は、 [Microsoft Graph の機能の要求](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests)に投票するか、開くようにしてください。

# <a name="rubytabruby"></a>[Ruby](#tab/Ruby)

まだ使用できません。 ユーザーにとって重要な場合は、 [Microsoft Graph の機能の要求](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests)に投票するか、開くようにしてください。

---

## <a name="next-steps"></a>次のステップ

* 認証プロバイダーにはクライアント ID が必要です。 認証プロバイダをセットアップした後に[、アプリケーションを登録](https://portal.azure.com/)する必要があります。
* 必要な OAuth フローが現在サポートされていない場合は、 [Microsoft Graph の機能の要求](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests)に投票してください。
