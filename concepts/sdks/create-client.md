---
title: Microsoft Graph クライアントを作成する
description: Microsoft Graph への呼び出しを行うために使用するクライアントを作成する方法について説明します。 認証を設定し、独立 cloud を選択する方法について説明します。
localization_priority: Normal
author: MichaelMainer
ms.openlocfilehash: 3d120f626f3623545366a105aaf9c072c8501e1b
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/06/2019
ms.locfileid: "33630189"
---
# <a name="create-a-microsoft-graph-client"></a>Microsoft Graph クライアントを作成する

Microsoft Graph クライアントは、Microsoft Graph を呼び出すことが簡単になるように設計されています。 アプリケーションの有効期間中は、単一のクライアントインスタンスを使用できます。 Microsoft Graph クライアントパッケージをプロジェクトに追加してインストールする方法については、「 [SDK をインストール](sdk-installation.md)する」を参照してください。

次のコード例は、サポートされている言語で認証プロバイダを使用して Microsoft Graph クライアントのインスタンスを作成する方法を示しています。 認証プロバイダーは、アプリケーションのアクセストークンの取得を処理します。 言語とプラットフォームごとに、さまざまな認証プロバイダを使用できます。 さまざまなアプリケーションプロバイダーが、さまざまなクライアントシナリオをサポートしています。 シナリオに適したプロバイダーとオプションの詳細については、「[認証プロバイダーを選択](choose-authentication-providers.md)する」を参照してください。

# <a name="ctabcs"></a>[Visual](#tab/CS)

```csharp
var app = DeviceCodeProvider.CreateClientApplication("INSERT-CLIENT-APP-ID");
var authProvider = new DeviceCodeProvider(app);
var client = new GraphServiceClient(authProvider);
```

# <a name="javascripttabjavascript"></a>[Java](#tab/Javascript)

```javascript
const clientId = "INSERT-CLIENT-APP-ID"; // Client Id of the registered application
const callback = (errorDesc, token, error, tokenType) => {};
// An Optional options for initializing the MSAL @see https://github.com/AzureAD/microsoft-authentication-library-for-js/wiki/MSAL-basics#configuration-options
const options = {
    redirectUri: "Your redirect URI",
};
const graphScopes = ["user.read", "mail.send"]; // An array of graph scopes

// Initialize the MSAL @see https://github.com/AzureAD/microsoft-authentication-library-for-js/wiki/MSAL-basics#initialization-of-msal
const userAgentApplication = new UserAgentApplication(clientId, undefined, callback, options);
const authProvider = new MSALAuthenticationProvider(userAgentApplication, scopes);
```

# <a name="javatabjava"></a>[Java](#tab/Java)

```java
ClientCredentialProvider authProvider = new ClientCredentialProvider(CLIENT_ID, SCOPES, CLIENT_SECRET, TENANT_GUID, NATIONAL_CLOUD);

IGraphServiceClient graphClient = GraphServiceClient
                .builder()
                .authenticationProvider(authProvider)
                .buildClient();
```

# <a name="androidtabandroid"></a>[Android](#tab/Android)

```java
PublicClientApplication publicClientApplication = new PublicClientApplication(getApplicationContext(), "INSERT-CLIENT-APP-ID");

MSALAuthenticationProvider msalAuthenticationProvider = new MSALAuthenticationProvider(
    getActivity(),
    getApplication(),
    publicClientApplication,
    scopes);

IGraphServiceClient graphClient = GraphServiceClient
                .builder()
                .authenticationProvider(authProvider)
                .buildClient();
```

# <a name="objective-ctabobjective-c"></a>[目的-C](#tab/Objective-C)

```objc
// Create the authenticationProvider.
NSError *error = nil;
MSALPublicClientApplication *publicClientApplication = [[MSALPublicClientApplication alloc] initWithClientId:@"INSERT-CLIENT-APP-ID" 
error:&error];
MSALAuthenticationProviderOptions *authProviderOptions= [[MSALAuthenticationProviderOptions alloc] initWithScopes:<array-of-scopes-for-which-you-need-access-token>];
 MSALAuthenticationProvider *authenticationProvider = [[MSALAuthenticationProvider alloc] initWithPublicClientApplication:publicClientApplication 
 andOptions:authProviderOptions];

// Create the client with the authenticationProvider and create a request to the /me resource.
MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/me"]]];

// Create the task to send the request and handle the response.
MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest
    completionHandler:^(NSData *data, NSURLResponse *response, NSError *error) {

    //Do something

    }];

[meDataTask execute];
```

# <a name="phptabphp"></a>[PHP](#tab/PHP)

```php
// PHP client currently doesn't have an authentication provider. You will need to handle
// getting an access token. The following example demonstrates the client credential
// OAuth flow and assumes that an administrator has consented to the application.
$guzzle = new \GuzzleHttp\Client();
$url = 'https://login.microsoftonline.com/' . $tenantId . '/oauth2/token?api-version=1.0';
$token = json_decode($guzzle->post($url, [
    'form_params' => [
        'client_id' => $clientId,
        'client_secret' => $clientSecret,
        'resource' => 'https://graph.microsoft.com/',
        'grant_type' => 'client_credentials',
    ],
])->getBody()->getContents());
$accessToken = $token->access_token;

// Create a new Graph client.
$graph = new Graph();
$graph->setAccessToken($accessToken);

// Make a call to /me Graph resource.
$user = $graph->createRequest("GET", "/me")
                ->setReturnType(Model\User::class)
                ->execute();
```
---
