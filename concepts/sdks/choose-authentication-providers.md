---
title: Microsoft Graph 認証プロバイダーを選択する
description: アプリケーションに対してシナリオ固有の認証プロバイダーを選択する方法について説明します。
localization_priority: Normal
author: MichaelMainer
ms.openlocfilehash: 5061b38249f31a6eea959ecec94899337bf57326
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/06/2019
ms.locfileid: "33630196"
---
# <a name="choose-a-microsoft-graph-authentication-provider-based-on-oauth-flow"></a>OAuth フローに基づいて Microsoft Graph 認証プロバイダを選択する

認証プロバイダーは、認証クライアントライブラリに必要なパラメーターを抽象化することで、アクセストークンの取得を簡素化します。 Microsoft Graph 認証プロバイダーは、各プラットフォームのアダプターを提供することにより、Microsoft Authentication Library (MSAL) の使用を簡素化します。 これらのアダプターは、アプリケーションのトークンの取得を処理します。 Microsoft Graph 認証プロバイダーは、OAuth 付与フローにマップされます。 アプリケーションに対して適切な認証プロバイダーを選択するために、アプリケーションに対してどの OAuth 付与フローを使用するかを把握する必要があります。

## <a name="authorization-code-oauth-flow"></a>認証コード OAuth フロー

認証コードフローにより、ネイティブおよび web アプリはユーザーの名前でトークンを安全に取得することができます。 詳細については、「 [Microsoft identity platform And OAuth 2.0 認証コードフロー](https://docs.microsoft.com/en-us/azure/active-directory/develop/v2-oauth2-auth-code-flow)」を参照してください。

# <a name="ctabcs"></a>[Visual](#tab/CS)

```csharp
IConfidentialClientApplication clientApplication = AuthorizationCodeProvider.CreateClientApplication(clientId, redirectUri, clientCredential);
AuthorizationCodeProvider authProvider = new AuthorizationCodeProvider(clientApplication, scopes);
```

# <a name="javascripttabjavascript"></a>[Java](#tab/Javascript)

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

## <a name="client-credential-oauth-flow"></a>クライアント資格情報 OAuth フロー

クライアント資格情報フローを使用すると、ユーザーによる操作なしでサービスアプリケーションを実行できます。 Access は、アプリケーションの id に基づいています。 詳細については、「 [Microsoft identity platform」および「OAuth 2.0 クライアント資格情報フロー](https://docs.microsoft.com/en-us/azure/active-directory/develop/v2-oauth2-client-creds-grant-flow)」を参照してください。

# <a name="ctabcs"></a>[Visual](#tab/CS)

```csharp
IConfidentialClientApplication clientApplication = ClientCredentialProvider.CreateClientApplication(clientId, clientCredential);
ClientCredentialProvider authProvider = new ClientCredentialProvider(clientApplication);
```

# <a name="javascripttabjavascript"></a>[Java](#tab/Javascript)

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

## <a name="on-behalf-of-oauth-flow"></a>非代行の OAuth フロー

アプリケーションが Microsoft Graph API を呼び出すサービスまたは web API を呼び出すときに、その代わりの流れが適用されます。 [Microsoft identity platform および OAuth 2.0 の送信フローの](https://docs.microsoft.com/en-us/azure/active-directory/develop/v2-oauth2-on-behalf-of-flow)詳細については、こちらを参照してください。

# <a name="ctabcs"></a>[Visual](#tab/CS)

```csharp
IConfidentialClientApplication clientApplication = OnBehalfOfProvider.CreateClientApplication(clientId, redirectUri, clientCredential);
OnBehalfOfProvider authProvider = new OnBehalfOfProvider(clientApplication, scopes);
```

# <a name="javascripttabjavascript"></a>[Java](#tab/Javascript)

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

## <a name="implicit-grant-oauth-flow"></a>暗黙的付与 OAuth フロー

暗黙的な付与フローは、ブラウザーベースのアプリケーションで使用されます。 詳細については、「 [Microsoft identity platform」および「暗黙的な許可の流れ](https://docs.microsoft.com/en-us/azure/active-directory/develop/v2-oauth2-implicit-grant-flow)」を参照してください。

# <a name="ctabcs"></a>[Visual](#tab/CS)

なし。

# <a name="javascripttabjavascript"></a>[Java](#tab/Javascript)

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

## <a name="device-code-oauth-flow"></a>デバイスコード OAuth フロー

デバイスコードフローによって、別のデバイスを使用してデバイスにサインインできるようになります。 詳細については、「 [Microsoft identity platform」および「OAuth 2.0 デバイスコードフロー](https://docs.microsoft.com/en-us/azure/active-directory/develop/v2-oauth2-device-code)」を参照してください。

# <a name="ctabcs"></a>[Visual](#tab/CS)

```csharp
IPublicClientApplication clientApplication = DeviceCodeProvider.CreateClientApplication(clientId);
DeviceCodeProvider authProvider = new DeviceCodeProvider(clientApplication, scopes);
```

# <a name="javascripttabjavascript"></a>[Java](#tab/Javascript)

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

## <a name="integrated-windows-flow"></a>統合 Windows フロー

統合 Windows フローにより、Windows コンピューターがドメインに参加している場合に、アクセストークンをサイレントに取得することができます。 詳細については、「[統合 Windows 認証](https://github.com/AzureAD/microsoft-authentication-library-for-dotnet/wiki/Integrated-Windows-Authentication)」を参照してください。

# <a name="ctabcs"></a>[Visual](#tab/CS)

```csharp
IPublicClientApplication clientApplication = IntegratedWindowsAuthenticationProvider.CreateClientApplication(clientId);
IntegratedWindowsAuthenticationProvider authProvider = new IntegratedWindowsAuthenticationProvider(clientApplication, scopes);
```

# <a name="javascripttabjavascript"></a>[Java](#tab/Javascript)

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

## <a name="interactive-flow"></a>対話型フロー

対話型フローは、モバイルアプリケーション (Xamarin および UWP) およびデスクトップアプリケーションがユーザーの名前で Microsoft Graph を呼び出すために使用されます。 詳細については、「[トークンを対話的に取得](https://github.com/AzureAD/microsoft-authentication-library-for-dotnet/wiki/Acquiring-tokens-interactively)する」を参照してください。

# <a name="ctabcs"></a>[Visual](#tab/CS)

```csharp
IPublicClientApplication clientApplication = InteractiveAuthenticationProvider.CreateClientApplication(clientId);
InteractiveAuthenticationProvider authProvider = new InteractiveAuthenticationProvider(clientApplication, scopes);
```

# <a name="javascripttabjavascript"></a>[Java](#tab/Javascript)

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

## <a name="resource-owner-password-credential-grant-oauth-flow"></a>リソース所有者のパスワード資格情報に OAuth フローを付与する

リソース所有者のパスワード資格情報のフローによって、アプリケーションはユーザー名とパスワードを使用してユーザーにサインインすることができます。 このフローは、他の OAuth フローを使用できない場合にのみ使用してください。 詳細については、「 [Microsoft identity platform」および「OAuth 2.0 resource owner password credential](https://docs.microsoft.com/en-us/azure/active-directory/develop/v2-oauth-ropc) 」を参照してください。



# <a name="ctabcs"></a>[Visual](#tab/CS)

```csharp
IPublicClientApplication clientApplication = UsernamePasswordProvider.CreateClientApplication(clientId);
UsernamePasswordProvider authProvider = new UsernamePasswordProvider(clientApplication, scopes);
```

# <a name="javascripttabjavascript"></a>[Java](#tab/Javascript)

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

## <a name="next-steps"></a>次の手順

* 認証プロバイダーにはクライアント ID が必要です。 認証プロバイダをセットアップした後に[、アプリケーションを登録](https://portal.azure.com/)する必要があります。
* 必要な OAuth フローが現在サポートされていない場合は、 [Microsoft Graph の機能の要求](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests)に投票してください。