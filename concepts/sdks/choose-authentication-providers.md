---
title: Microsoft Graph 認証プロバイダーを選択する
description: アプリケーションに対してシナリオ固有の認証プロバイダーを選択する方法について説明します。
localization_priority: Normal
author: MichaelMainer
ms.openlocfilehash: 8f69312b4993320e76e2fe46a2977d98c0a42c93
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/27/2019
ms.locfileid: "35275559"
---
# <a name="choose-a-microsoft-graph-authentication-provider-based-on-scenario"></a><span data-ttu-id="0e84d-103">シナリオに基づいて Microsoft Graph 認証プロバイダを選択する</span><span class="sxs-lookup"><span data-stu-id="0e84d-103">Choose a Microsoft Graph authentication provider based on scenario</span></span>

<span data-ttu-id="0e84d-104">認証プロバイダーは、Microsoft 認証ライブラリ (MSAL) を使用してトークンを取得するために必要なコードを実装します。増分の同意、期限切れのパスワード、条件付きアクセスなど、さまざまなケースの潜在的なエラーを処理します。HTTP 要求認証ヘッダーを設定します。</span><span class="sxs-lookup"><span data-stu-id="0e84d-104">Authentication providers implement the code required to acquire a token using the Microsoft Authentication Library (MSAL); handle a number of potential errors for cases like incremental consent, expired passwords, and conditional access; and then set the HTTP request authorization header.</span></span> <span data-ttu-id="0e84d-105">次の表に、さまざまな[種類のアプリケーション](https://docs.microsoft.com/en-us/azure/active-directory/develop/v2-app-types)のシナリオに一致する一連のプロバイダーを示します。</span><span class="sxs-lookup"><span data-stu-id="0e84d-105">The following table lists the set of providers that match the scenarios for different [application types](https://docs.microsoft.com/en-us/azure/active-directory/develop/v2-app-types).</span></span>

|<span data-ttu-id="0e84d-106">シナリオ</span><span class="sxs-lookup"><span data-stu-id="0e84d-106">Scenario</span></span> | <span data-ttu-id="0e84d-107">フロー/付与</span><span class="sxs-lookup"><span data-stu-id="0e84d-107">Flow/Grant</span></span> | <span data-ttu-id="0e84d-108">対象ユーザー</span><span class="sxs-lookup"><span data-stu-id="0e84d-108">Audience</span></span> | <span data-ttu-id="0e84d-109">プロバイダー</span><span class="sxs-lookup"><span data-stu-id="0e84d-109">Provider</span></span>|
|--|--|--|--|
| [<span data-ttu-id="0e84d-110">シングルページアプリ</span><span class="sxs-lookup"><span data-stu-id="0e84d-110">Single Page App</span></span>](https://docs.microsoft.com/en-us/azure/active-directory/develop/scenario-spa-acquire-token)| | | |
| | <span data-ttu-id="0e84d-111">暗黙的</span><span class="sxs-lookup"><span data-stu-id="0e84d-111">Implicit</span></span> | <span data-ttu-id="0e84d-112">委任されたコンシューマー/組織</span><span class="sxs-lookup"><span data-stu-id="0e84d-112">Delegated Consumer/Org</span></span> |[<span data-ttu-id="0e84d-113">暗黙的プロバイダー</span><span class="sxs-lookup"><span data-stu-id="0e84d-113">Implicit Provider</span></span>](#ImplicitProvider) |
| [<span data-ttu-id="0e84d-114">Web Api を呼び出す web アプリ</span><span class="sxs-lookup"><span data-stu-id="0e84d-114">Web App that calls web APIs</span></span>](https://docs.microsoft.com/en-us/azure/active-directory/develop/scenario-web-app-call-api-acquire-token) | | | |
| | <span data-ttu-id="0e84d-115">認証コード</span><span class="sxs-lookup"><span data-stu-id="0e84d-115">Authorization Code</span></span> | <span data-ttu-id="0e84d-116">委任されたコンシューマー/組織</span><span class="sxs-lookup"><span data-stu-id="0e84d-116">Delegated Consumer/Org</span></span> | [<span data-ttu-id="0e84d-117">認証コードプロバイダ</span><span class="sxs-lookup"><span data-stu-id="0e84d-117">Authorization Code Provider</span></span>](#AuthCodeProvider) |
| | <span data-ttu-id="0e84d-118">クライアント資格情報</span><span class="sxs-lookup"><span data-stu-id="0e84d-118">Client Credentials</span></span>  | <span data-ttu-id="0e84d-119">App Only</span><span class="sxs-lookup"><span data-stu-id="0e84d-119">App Only</span></span> | [<span data-ttu-id="0e84d-120">クライアント資格情報プロバイダー</span><span class="sxs-lookup"><span data-stu-id="0e84d-120">Client Credentials Provider</span></span>](#ClientCredentialsProvider) |
| [<span data-ttu-id="0e84d-121">Web api を呼び出す web API</span><span class="sxs-lookup"><span data-stu-id="0e84d-121">Web API that calls web APIs</span></span>](https://docs.microsoft.com/en-us/azure/active-directory/develop/scenario-web-api-call-api-acquire-token) | | | |
| | <span data-ttu-id="0e84d-122">代理人</span><span class="sxs-lookup"><span data-stu-id="0e84d-122">On Behalf Of</span></span> | <span data-ttu-id="0e84d-123">委任されたコンシューマー/組織</span><span class="sxs-lookup"><span data-stu-id="0e84d-123">Delegated Consumer/Org</span></span> | [<span data-ttu-id="0e84d-124">プロバイダーに代わって</span><span class="sxs-lookup"><span data-stu-id="0e84d-124">On Behalf Of Provider</span></span>](#OnBehalfOfProvider) |
| | <span data-ttu-id="0e84d-125">クライアント資格情報</span><span class="sxs-lookup"><span data-stu-id="0e84d-125">Client Credentials</span></span>  | <span data-ttu-id="0e84d-126">App Only</span><span class="sxs-lookup"><span data-stu-id="0e84d-126">App Only</span></span> | [<span data-ttu-id="0e84d-127">クライアント資格情報プロバイダー</span><span class="sxs-lookup"><span data-stu-id="0e84d-127">Client Credentials Provider</span></span>](#ClientCredentialsProvider) |
| [<span data-ttu-id="0e84d-128">Web Api を呼び出すデスクトップアプリ</span><span class="sxs-lookup"><span data-stu-id="0e84d-128">Desktop app that calls web APIs</span></span>](https://docs.microsoft.com/en-us/azure/active-directory/develop/scenario-desktop-acquire-token) | | | |
| | <span data-ttu-id="0e84d-129">Interactive</span><span class="sxs-lookup"><span data-stu-id="0e84d-129">Interactive</span></span> | <span data-ttu-id="0e84d-130">委任されたコンシューマー/組織</span><span class="sxs-lookup"><span data-stu-id="0e84d-130">Delegated Consumer/Org</span></span> | [<span data-ttu-id="0e84d-131">対話プロバイダー</span><span class="sxs-lookup"><span data-stu-id="0e84d-131">Interactive Provider</span></span>](#InteractiveProvider) |
| | <span data-ttu-id="0e84d-132">統合 Windows</span><span class="sxs-lookup"><span data-stu-id="0e84d-132">Integrated Windows</span></span> | <span data-ttu-id="0e84d-133">委任された組織</span><span class="sxs-lookup"><span data-stu-id="0e84d-133">Delegated Org</span></span> | [<span data-ttu-id="0e84d-134">統合 Windows プロバイダ</span><span class="sxs-lookup"><span data-stu-id="0e84d-134">Integrated Windows Provider</span></span>](#IntegratedWindowsProvider) |
| | <span data-ttu-id="0e84d-135">リソース所有者</span><span class="sxs-lookup"><span data-stu-id="0e84d-135">Resource Owner</span></span>  | <span data-ttu-id="0e84d-136">委任された組織</span><span class="sxs-lookup"><span data-stu-id="0e84d-136">Delegated Org</span></span> | [<span data-ttu-id="0e84d-137">Username/Password Provider</span><span class="sxs-lookup"><span data-stu-id="0e84d-137">Username / Password Provider</span></span>](#UsernamePasswordProvider) |
| | <span data-ttu-id="0e84d-138">デバイスコード</span><span class="sxs-lookup"><span data-stu-id="0e84d-138">Device Code</span></span>  | <span data-ttu-id="0e84d-139">委任された組織</span><span class="sxs-lookup"><span data-stu-id="0e84d-139">Delegated Org</span></span> | [<span data-ttu-id="0e84d-140">デバイスコードプロバイダ</span><span class="sxs-lookup"><span data-stu-id="0e84d-140">Device Code Provider</span></span>](#DeviceCodeProvider) |
| [<span data-ttu-id="0e84d-141">デーモンアプリ</span><span class="sxs-lookup"><span data-stu-id="0e84d-141">Daemon app</span></span>](https://docs.microsoft.com/en-us/azure/active-directory/develop/scenario-daemon-acquire-token) | | | |
| | <span data-ttu-id="0e84d-142">クライアント資格情報</span><span class="sxs-lookup"><span data-stu-id="0e84d-142">Client Credentials</span></span>  | <span data-ttu-id="0e84d-143">App Only</span><span class="sxs-lookup"><span data-stu-id="0e84d-143">App Only</span></span> | [<span data-ttu-id="0e84d-144">クライアント資格情報プロバイダー</span><span class="sxs-lookup"><span data-stu-id="0e84d-144">Client Credentials Provider</span></span>](#ClientCredentialsProvider) |
| [<span data-ttu-id="0e84d-145">Web Api を呼び出すモバイルアプリ</span><span class="sxs-lookup"><span data-stu-id="0e84d-145">Mobile app that calls web APIs</span></span>](https://docs.microsoft.com/en-us/azure/active-directory/develop/scenario-mobile-acquire-token) | | | |
| | <span data-ttu-id="0e84d-146">Interactive</span><span class="sxs-lookup"><span data-stu-id="0e84d-146">Interactive</span></span> | <span data-ttu-id="0e84d-147">委任されたコンシューマー/組織</span><span class="sxs-lookup"><span data-stu-id="0e84d-147">Delegated Consumer/Org</span></span> | [<span data-ttu-id="0e84d-148">対話プロバイダー</span><span class="sxs-lookup"><span data-stu-id="0e84d-148">Interactive Provider</span></span>](#InteractiveProvider) |


## <a name="a-nameauthcodeproviderauthorization-code-provider"></a><span data-ttu-id="0e84d-149"><a name="AuthCodeProvider"/>認証コードプロバイダ</span><span class="sxs-lookup"><span data-stu-id="0e84d-149"><a name="AuthCodeProvider"/>Authorization code provider</span></span>

<span data-ttu-id="0e84d-150">認証コードフローにより、ネイティブおよび web アプリはユーザーの名前でトークンを安全に取得することができます。</span><span class="sxs-lookup"><span data-stu-id="0e84d-150">The authorization code flow enables native and web apps to securely obtain tokens in the name of the user.</span></span> <span data-ttu-id="0e84d-151">詳細については、「 [Microsoft identity platform And OAuth 2.0 認証コードフロー](https://docs.microsoft.com/en-us/azure/active-directory/develop/v2-oauth2-auth-code-flow)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="0e84d-151">To learn more, see [Microsoft identity platform and OAuth 2.0 authorization code flow](https://docs.microsoft.com/en-us/azure/active-directory/develop/v2-oauth2-auth-code-flow).</span></span>

# <a name="ctabcs"></a>[<span data-ttu-id="0e84d-152">C#</span><span class="sxs-lookup"><span data-stu-id="0e84d-152">C#</span></span>](#tab/CS)

```csharp
IConfidentialClientApplication clientApplication = AuthorizationCodeProvider.CreateClientApplication(clientId, redirectUri, clientCredential);
AuthorizationCodeProvider authProvider = new AuthorizationCodeProvider(clientApplication, scopes);
```

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="0e84d-153">Javascript</span><span class="sxs-lookup"><span data-stu-id="0e84d-153">Javascript</span></span>](#tab/Javascript)

<span data-ttu-id="0e84d-154">認証コード、クライアント資格情報、および非代行の OAuth フローでは、この時点でカスタム認証プロバイダーを実装する必要があります。</span><span class="sxs-lookup"><span data-stu-id="0e84d-154">Authorization code, client credential, and on-behalf-of OAuth flows require that you implement a custom authentication provider at this time.</span></span> <span data-ttu-id="0e84d-155">詳細については、「 [Using a custom authentication provider](https://github.com/microsoftgraph/msgraph-sdk-javascript/blob/dev/docs/CustomAuthenticationProvider.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="0e84d-155">For more information, see [Using a custom authentication provider](https://github.com/microsoftgraph/msgraph-sdk-javascript/blob/dev/docs/CustomAuthenticationProvider.md).</span></span>

# <a name="javatabjava"></a>[<span data-ttu-id="0e84d-156">Java</span><span class="sxs-lookup"><span data-stu-id="0e84d-156">Java</span></span>](#tab/Java)

```java
AuthorizationCodeProvider authProvider = new AuthorizationCodeProvider(
                                                    clientId,
                                                    scopes,
                                                    authorizationCode,
                                                    redirectUri,
                                                    clientSecret);
```

# <a name="androidtabandroid"></a>[<span data-ttu-id="0e84d-157">Android</span><span class="sxs-lookup"><span data-stu-id="0e84d-157">Android</span></span>](#tab/Android)

<span data-ttu-id="0e84d-158">なし。</span><span class="sxs-lookup"><span data-stu-id="0e84d-158">Not applicable.</span></span>

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="0e84d-159">目的-C</span><span class="sxs-lookup"><span data-stu-id="0e84d-159">Objective-C</span></span>](#tab/Objective-C)

<span data-ttu-id="0e84d-160">なし。</span><span class="sxs-lookup"><span data-stu-id="0e84d-160">Not applicable.</span></span>

# <a name="phptabphp"></a>[<span data-ttu-id="0e84d-161">PHP</span><span class="sxs-lookup"><span data-stu-id="0e84d-161">PHP</span></span>](#tab/PHP)

<span data-ttu-id="0e84d-162">まだ使用できません。</span><span class="sxs-lookup"><span data-stu-id="0e84d-162">Not yet available.</span></span> <span data-ttu-id="0e84d-163">ユーザーにとって重要な場合は、 [Microsoft Graph の機能の要求](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests)をサポートするか、または開きます。</span><span class="sxs-lookup"><span data-stu-id="0e84d-163">Please support or open a [Microsoft Graph feature request](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) if this is important to you.</span></span>

# <a name="rubytabruby"></a>[<span data-ttu-id="0e84d-164">Ruby</span><span class="sxs-lookup"><span data-stu-id="0e84d-164">Ruby</span></span>](#tab/Ruby)

<span data-ttu-id="0e84d-165">まだ利用できません。</span><span class="sxs-lookup"><span data-stu-id="0e84d-165">Not available, yet.</span></span> <span data-ttu-id="0e84d-166">ユーザーにとって重要な場合は、 [Microsoft Graph の機能の要求](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests)に投票するか、開くようにしてください。</span><span class="sxs-lookup"><span data-stu-id="0e84d-166">Please vote for or open a [Microsoft Graph feature request](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) if this is important to you.</span></span>

---

##  <a name="a-nameclientcredentialsproviderclient-credentials-provider"></a><span data-ttu-id="0e84d-167"><a name="ClientCredentialsProvider"/>クライアント資格情報プロバイダー</span><span class="sxs-lookup"><span data-stu-id="0e84d-167"><a name="ClientCredentialsProvider"/>Client credentials provider</span></span>

<span data-ttu-id="0e84d-168">クライアント資格情報フローを使用すると、ユーザーによる操作なしでサービスアプリケーションを実行できます。</span><span class="sxs-lookup"><span data-stu-id="0e84d-168">The client credential flow enables service applications to run without user interaction.</span></span> <span data-ttu-id="0e84d-169">Access は、アプリケーションの id に基づいています。</span><span class="sxs-lookup"><span data-stu-id="0e84d-169">Access is based on the identity of the application.</span></span> <span data-ttu-id="0e84d-170">詳細については、「 [Microsoft identity platform」および「OAuth 2.0 クライアント資格情報フロー](https://docs.microsoft.com/en-us/azure/active-directory/develop/v2-oauth2-client-creds-grant-flow)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="0e84d-170">For more information, see [Microsoft identity platform and the OAuth 2.0 client credentials flow](https://docs.microsoft.com/en-us/azure/active-directory/develop/v2-oauth2-client-creds-grant-flow).</span></span>

# <a name="ctabcs"></a>[<span data-ttu-id="0e84d-171">C#</span><span class="sxs-lookup"><span data-stu-id="0e84d-171">C#</span></span>](#tab/CS)

```csharp
IConfidentialClientApplication clientApplication = ClientCredentialProvider.CreateClientApplication(clientId, clientCredential);
ClientCredentialProvider authProvider = new ClientCredentialProvider(clientApplication);
```

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="0e84d-172">Javascript</span><span class="sxs-lookup"><span data-stu-id="0e84d-172">Javascript</span></span>](#tab/Javascript)

<span data-ttu-id="0e84d-173">認証コード、クライアント資格情報、および非代行の OAuth フローでは、この時点でカスタム認証プロバイダーを実装する必要があります。</span><span class="sxs-lookup"><span data-stu-id="0e84d-173">Authorization code, client credential, and on-behalf-of OAuth flows require that you implement a custom authentication provider at this time.</span></span> <span data-ttu-id="0e84d-174">詳細については、「 [Using a custom authentication provider](https://github.com/microsoftgraph/msgraph-sdk-javascript/blob/dev/docs/CustomAuthenticationProvider.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="0e84d-174">For more information, see [Using a custom authentication provider](https://github.com/microsoftgraph/msgraph-sdk-javascript/blob/dev/docs/CustomAuthenticationProvider.md).</span></span>

# <a name="javatabjava"></a>[<span data-ttu-id="0e84d-175">Java</span><span class="sxs-lookup"><span data-stu-id="0e84d-175">Java</span></span>](#tab/Java)

```java
ClientCredentialProvider authProvider = new ClientCredentialProvider(
                                                    clientId,
                                                    scopes,
                                                    clientSecret,
                                                    tenant,
                                                    endpoint);
```

# <a name="androidtabandroid"></a>[<span data-ttu-id="0e84d-176">Android</span><span class="sxs-lookup"><span data-stu-id="0e84d-176">Android</span></span>](#tab/Android)

<span data-ttu-id="0e84d-177">なし。</span><span class="sxs-lookup"><span data-stu-id="0e84d-177">Not applicable.</span></span>

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="0e84d-178">目的-C</span><span class="sxs-lookup"><span data-stu-id="0e84d-178">Objective-C</span></span>](#tab/Objective-C)

<span data-ttu-id="0e84d-179">なし。</span><span class="sxs-lookup"><span data-stu-id="0e84d-179">Not applicable.</span></span>

# <a name="phptabphp"></a>[<span data-ttu-id="0e84d-180">PHP</span><span class="sxs-lookup"><span data-stu-id="0e84d-180">PHP</span></span>](#tab/PHP)

<span data-ttu-id="0e84d-181">まだ利用できません。</span><span class="sxs-lookup"><span data-stu-id="0e84d-181">Not available, yet.</span></span> <span data-ttu-id="0e84d-182">ユーザーにとって重要な場合は、 [Microsoft Graph の機能の要求](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests)をサポートするか、または開きます。</span><span class="sxs-lookup"><span data-stu-id="0e84d-182">Please support or open a [Microsoft Graph feature request](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) if this is important to you.</span></span>

# <a name="rubytabruby"></a>[<span data-ttu-id="0e84d-183">Ruby</span><span class="sxs-lookup"><span data-stu-id="0e84d-183">Ruby</span></span>](#tab/Ruby)

<span data-ttu-id="0e84d-184">まだ利用できません。</span><span class="sxs-lookup"><span data-stu-id="0e84d-184">Not available, yet.</span></span> <span data-ttu-id="0e84d-185">ユーザーにとって重要な場合は、 [Microsoft Graph の機能の要求](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests)をサポートするか、または開きます。</span><span class="sxs-lookup"><span data-stu-id="0e84d-185">Please support or open a [Microsoft Graph feature request](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) if this is important to you.</span></span>

---

##  <a name="a-nameonbehalfofprovideron-behalf-of-provider"></a><span data-ttu-id="0e84d-186"><a name="OnBehalfOfProvider"/>プロバイダーの代理</span><span class="sxs-lookup"><span data-stu-id="0e84d-186"><a name="OnBehalfOfProvider"/>On-behalf-of provider</span></span>

<span data-ttu-id="0e84d-187">アプリケーションが Microsoft Graph API を呼び出すサービスまたは web API を呼び出すときに、その代わりの流れが適用されます。</span><span class="sxs-lookup"><span data-stu-id="0e84d-187">The on-behalf-of flow is applicable when your application calls a service/web API which in turns calls the Microsoft Graph API.</span></span> <span data-ttu-id="0e84d-188">[Microsoft identity platform および OAuth 2.0 の送信フローの](https://docs.microsoft.com/en-us/azure/active-directory/develop/v2-oauth2-on-behalf-of-flow)詳細については、こちらを参照してください。</span><span class="sxs-lookup"><span data-stu-id="0e84d-188">Learn more by reading [Microsoft identity platform and OAuth 2.0 On-Behalf-Of flow](https://docs.microsoft.com/en-us/azure/active-directory/develop/v2-oauth2-on-behalf-of-flow)</span></span>

# <a name="ctabcs"></a>[<span data-ttu-id="0e84d-189">C#</span><span class="sxs-lookup"><span data-stu-id="0e84d-189">C#</span></span>](#tab/CS)

```csharp
IConfidentialClientApplication clientApplication = OnBehalfOfProvider.CreateClientApplication(clientId, redirectUri, clientCredential);
OnBehalfOfProvider authProvider = new OnBehalfOfProvider(clientApplication, scopes);
```

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="0e84d-190">Javascript</span><span class="sxs-lookup"><span data-stu-id="0e84d-190">Javascript</span></span>](#tab/Javascript)

<span data-ttu-id="0e84d-191">認証コード、クライアント資格情報、および非代行の OAuth フローでは、この時点でカスタム認証プロバイダーを実装する必要があります。</span><span class="sxs-lookup"><span data-stu-id="0e84d-191">Authorization code, client credential, and on-behalf-of OAuth flows require that you implement a custom authentication provider at this time.</span></span> <span data-ttu-id="0e84d-192">詳細については、「[カスタム認証プロバイダを使用する](https://github.com/microsoftgraph/msgraph-sdk-javascript/blob/dev/docs/CustomAuthenticationProvider.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="0e84d-192">Read [Using Custom Authentication Provider](https://github.com/microsoftgraph/msgraph-sdk-javascript/blob/dev/docs/CustomAuthenticationProvider.md) for more information.</span></span>

# <a name="javatabjava"></a>[<span data-ttu-id="0e84d-193">Java</span><span class="sxs-lookup"><span data-stu-id="0e84d-193">Java</span></span>](#tab/Java)

<span data-ttu-id="0e84d-194">まだ使用できません。</span><span class="sxs-lookup"><span data-stu-id="0e84d-194">Not yet available.</span></span> <span data-ttu-id="0e84d-195">ユーザーにとって重要な場合は、 [Microsoft Graph の機能の要求](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests)に投票するか、開くようにしてください。</span><span class="sxs-lookup"><span data-stu-id="0e84d-195">Please vote for or open a [Microsoft Graph feature request](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) if this is important to you.</span></span>

# <a name="androidtabandroid"></a>[<span data-ttu-id="0e84d-196">Android</span><span class="sxs-lookup"><span data-stu-id="0e84d-196">Android</span></span>](#tab/Android)

<span data-ttu-id="0e84d-197">なし。</span><span class="sxs-lookup"><span data-stu-id="0e84d-197">Not applicable.</span></span>

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="0e84d-198">目的-C</span><span class="sxs-lookup"><span data-stu-id="0e84d-198">Objective-C</span></span>](#tab/Objective-C)

<span data-ttu-id="0e84d-199">なし。</span><span class="sxs-lookup"><span data-stu-id="0e84d-199">Not applicable.</span></span>

# <a name="phptabphp"></a>[<span data-ttu-id="0e84d-200">PHP</span><span class="sxs-lookup"><span data-stu-id="0e84d-200">PHP</span></span>](#tab/PHP)

<span data-ttu-id="0e84d-201">まだ使用できません。</span><span class="sxs-lookup"><span data-stu-id="0e84d-201">Not yet available.</span></span> <span data-ttu-id="0e84d-202">ユーザーにとって重要な場合は、 [Microsoft Graph の機能の要求](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests)に投票するか、開くようにしてください。</span><span class="sxs-lookup"><span data-stu-id="0e84d-202">Please vote for or open a [Microsoft Graph feature request](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) if this is important to you.</span></span>

# <a name="rubytabruby"></a>[<span data-ttu-id="0e84d-203">Ruby</span><span class="sxs-lookup"><span data-stu-id="0e84d-203">Ruby</span></span>](#tab/Ruby)

<span data-ttu-id="0e84d-204">まだ使用できません。</span><span class="sxs-lookup"><span data-stu-id="0e84d-204">Not yet available.</span></span> <span data-ttu-id="0e84d-205">ユーザーにとって重要な場合は、 [Microsoft Graph の機能の要求](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests)に投票するか、開くようにしてください。</span><span class="sxs-lookup"><span data-stu-id="0e84d-205">Please vote for or open a [Microsoft Graph feature request](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) if this is important to you.</span></span>

---

## <a name="a-nameimplicitproviderimplicit-provider"></a><span data-ttu-id="0e84d-206"><a name="ImplicitProvider"/>暗黙的プロバイダー</span><span class="sxs-lookup"><span data-stu-id="0e84d-206"><a name="ImplicitProvider"/>Implicit provider</span></span>

<span data-ttu-id="0e84d-207">暗黙的な付与フローは、ブラウザーベースのアプリケーションで使用されます。</span><span class="sxs-lookup"><span data-stu-id="0e84d-207">The implicit grant flow is used in browser-based applications.</span></span> <span data-ttu-id="0e84d-208">詳細については、「 [Microsoft identity platform」および「暗黙的な許可の流れ](https://docs.microsoft.com/en-us/azure/active-directory/develop/v2-oauth2-implicit-grant-flow)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="0e84d-208">For more information, see [Microsoft identity platform and Implicit grant flow](https://docs.microsoft.com/en-us/azure/active-directory/develop/v2-oauth2-implicit-grant-flow).</span></span>

# <a name="ctabcs"></a>[<span data-ttu-id="0e84d-209">C#</span><span class="sxs-lookup"><span data-stu-id="0e84d-209">C#</span></span>](#tab/CS)

<span data-ttu-id="0e84d-210">なし。</span><span class="sxs-lookup"><span data-stu-id="0e84d-210">Not applicable.</span></span>

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="0e84d-211">Javascript</span><span class="sxs-lookup"><span data-stu-id="0e84d-211">Javascript</span></span>](#tab/Javascript)

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

# <a name="javatabjava"></a>[<span data-ttu-id="0e84d-212">Java</span><span class="sxs-lookup"><span data-stu-id="0e84d-212">Java</span></span>](#tab/Java)

<span data-ttu-id="0e84d-213">なし。</span><span class="sxs-lookup"><span data-stu-id="0e84d-213">Not applicable.</span></span>

# <a name="androidtabandroid"></a>[<span data-ttu-id="0e84d-214">Android</span><span class="sxs-lookup"><span data-stu-id="0e84d-214">Android</span></span>](#tab/Android)

<span data-ttu-id="0e84d-215">なし。</span><span class="sxs-lookup"><span data-stu-id="0e84d-215">Not applicable.</span></span>

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="0e84d-216">目的-C</span><span class="sxs-lookup"><span data-stu-id="0e84d-216">Objective-C</span></span>](#tab/Objective-C)

<span data-ttu-id="0e84d-217">なし。</span><span class="sxs-lookup"><span data-stu-id="0e84d-217">Not applicable.</span></span>

# <a name="phptabphp"></a>[<span data-ttu-id="0e84d-218">PHP</span><span class="sxs-lookup"><span data-stu-id="0e84d-218">PHP</span></span>](#tab/PHP)

<span data-ttu-id="0e84d-219">なし。</span><span class="sxs-lookup"><span data-stu-id="0e84d-219">Not applicable.</span></span>

# <a name="rubytabruby"></a>[<span data-ttu-id="0e84d-220">Ruby</span><span class="sxs-lookup"><span data-stu-id="0e84d-220">Ruby</span></span>](#tab/Ruby)

<span data-ttu-id="0e84d-221">なし。</span><span class="sxs-lookup"><span data-stu-id="0e84d-221">Not applicable.</span></span>

---

##  <a name="a-namedevicecodeproviderdevice-code-provider"></a><span data-ttu-id="0e84d-222"><a name="DeviceCodeProvider"/>デバイスコードプロバイダ</span><span class="sxs-lookup"><span data-stu-id="0e84d-222"><a name="DeviceCodeProvider"/>Device code provider</span></span>

<span data-ttu-id="0e84d-223">デバイスコードフローによって、別のデバイスを使用してデバイスにサインインできるようになります。</span><span class="sxs-lookup"><span data-stu-id="0e84d-223">The device code flow enables sign in to devices by way of another device.</span></span> <span data-ttu-id="0e84d-224">詳細については、「 [Microsoft identity platform」および「OAuth 2.0 デバイスコードフロー](https://docs.microsoft.com/en-us/azure/active-directory/develop/v2-oauth2-device-code)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="0e84d-224">For details, see [Microsoft identity platform and the OAuth 2.0 device code flow](https://docs.microsoft.com/en-us/azure/active-directory/develop/v2-oauth2-device-code).</span></span>

# <a name="ctabcs"></a>[<span data-ttu-id="0e84d-225">C#</span><span class="sxs-lookup"><span data-stu-id="0e84d-225">C#</span></span>](#tab/CS)

```csharp
IPublicClientApplication clientApplication = DeviceCodeProvider.CreateClientApplication(clientId);
DeviceCodeProvider authProvider = new DeviceCodeProvider(clientApplication, scopes);
```

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="0e84d-226">Javascript</span><span class="sxs-lookup"><span data-stu-id="0e84d-226">Javascript</span></span>](#tab/Javascript)

<span data-ttu-id="0e84d-227">まだ使用できません。</span><span class="sxs-lookup"><span data-stu-id="0e84d-227">Not yet available.</span></span> <span data-ttu-id="0e84d-228">ユーザーにとって重要な場合は、 [Microsoft Graph の機能の要求](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests)に投票するか、開くようにしてください。</span><span class="sxs-lookup"><span data-stu-id="0e84d-228">Please vote for or open a [Microsoft Graph feature request](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) if this is important to you.</span></span>

# <a name="javatabjava"></a>[<span data-ttu-id="0e84d-229">Java</span><span class="sxs-lookup"><span data-stu-id="0e84d-229">Java</span></span>](#tab/Java)

<span data-ttu-id="0e84d-230">まだ利用できません。</span><span class="sxs-lookup"><span data-stu-id="0e84d-230">Not available, yet.</span></span> <span data-ttu-id="0e84d-231">ユーザーにとって重要な場合は、 [Microsoft Graph の機能の要求](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests)をサポートするか、または開きます。</span><span class="sxs-lookup"><span data-stu-id="0e84d-231">Please support or open a [Microsoft Graph feature request](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) if this is important to you.</span></span>

# <a name="androidtabandroid"></a>[<span data-ttu-id="0e84d-232">Android</span><span class="sxs-lookup"><span data-stu-id="0e84d-232">Android</span></span>](#tab/Android)

<span data-ttu-id="0e84d-233">なし。</span><span class="sxs-lookup"><span data-stu-id="0e84d-233">Not applicable.</span></span>

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="0e84d-234">目的-C</span><span class="sxs-lookup"><span data-stu-id="0e84d-234">Objective-C</span></span>](#tab/Objective-C)

<span data-ttu-id="0e84d-235">なし。</span><span class="sxs-lookup"><span data-stu-id="0e84d-235">Not applicable.</span></span>

# <a name="phptabphp"></a>[<span data-ttu-id="0e84d-236">PHP</span><span class="sxs-lookup"><span data-stu-id="0e84d-236">PHP</span></span>](#tab/PHP)

<span data-ttu-id="0e84d-237">まだ使用できません。</span><span class="sxs-lookup"><span data-stu-id="0e84d-237">Not yet available.</span></span> <span data-ttu-id="0e84d-238">ユーザーにとって重要な場合は、 [Microsoft Graph の機能の要求](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests)に投票するか、開くようにしてください。</span><span class="sxs-lookup"><span data-stu-id="0e84d-238">Please vote for or open a [Microsoft Graph feature request](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) if this is important to you.</span></span>

# <a name="rubytabruby"></a>[<span data-ttu-id="0e84d-239">Ruby</span><span class="sxs-lookup"><span data-stu-id="0e84d-239">Ruby</span></span>](#tab/Ruby)

<span data-ttu-id="0e84d-240">まだ使用できません。</span><span class="sxs-lookup"><span data-stu-id="0e84d-240">Not yet available.</span></span> <span data-ttu-id="0e84d-241">ユーザーにとって重要な場合は、 [Microsoft Graph の機能の要求](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests)に投票するか、開くようにしてください。</span><span class="sxs-lookup"><span data-stu-id="0e84d-241">Please vote for or open a [Microsoft Graph feature request](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) if this is important to you.</span></span>

---

##  <a name="a-nameintegratedwindowsproviderintegrated-windows-provider"></a><span data-ttu-id="0e84d-242"><a name="IntegratedWindowsProvider"/>統合 Windows プロバイダ</span><span class="sxs-lookup"><span data-stu-id="0e84d-242"><a name="IntegratedWindowsProvider"/>Integrated Windows provider</span></span>

<span data-ttu-id="0e84d-243">統合 Windows フローにより、Windows コンピューターがドメインに参加している場合に、アクセストークンをサイレントに取得することができます。</span><span class="sxs-lookup"><span data-stu-id="0e84d-243">The integrated Windows flow provides a way for Windows computers to silently acquire an access token when they are domain joined.</span></span> <span data-ttu-id="0e84d-244">詳細については、「[統合 Windows 認証](https://github.com/AzureAD/microsoft-authentication-library-for-dotnet/wiki/Integrated-Windows-Authentication)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="0e84d-244">For details, see [Integrated Windows authentication](https://github.com/AzureAD/microsoft-authentication-library-for-dotnet/wiki/Integrated-Windows-Authentication).</span></span>

# <a name="ctabcs"></a>[<span data-ttu-id="0e84d-245">C#</span><span class="sxs-lookup"><span data-stu-id="0e84d-245">C#</span></span>](#tab/CS)

```csharp
IPublicClientApplication clientApplication = IntegratedWindowsAuthenticationProvider.CreateClientApplication(clientId);
IntegratedWindowsAuthenticationProvider authProvider = new IntegratedWindowsAuthenticationProvider(clientApplication, scopes);
```

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="0e84d-246">Javascript</span><span class="sxs-lookup"><span data-stu-id="0e84d-246">Javascript</span></span>](#tab/Javascript)

<span data-ttu-id="0e84d-247">なし。</span><span class="sxs-lookup"><span data-stu-id="0e84d-247">Not applicable.</span></span>

# <a name="javatabjava"></a>[<span data-ttu-id="0e84d-248">Java</span><span class="sxs-lookup"><span data-stu-id="0e84d-248">Java</span></span>](#tab/Java)

<span data-ttu-id="0e84d-249">なし。</span><span class="sxs-lookup"><span data-stu-id="0e84d-249">Not applicable.</span></span>

# <a name="androidtabandroid"></a>[<span data-ttu-id="0e84d-250">Android</span><span class="sxs-lookup"><span data-stu-id="0e84d-250">Android</span></span>](#tab/Android)

<span data-ttu-id="0e84d-251">なし。</span><span class="sxs-lookup"><span data-stu-id="0e84d-251">Not applicable.</span></span>

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="0e84d-252">目的-C</span><span class="sxs-lookup"><span data-stu-id="0e84d-252">Objective-C</span></span>](#tab/Objective-C)

<span data-ttu-id="0e84d-253">なし。</span><span class="sxs-lookup"><span data-stu-id="0e84d-253">Not applicable.</span></span>

# <a name="phptabphp"></a>[<span data-ttu-id="0e84d-254">PHP</span><span class="sxs-lookup"><span data-stu-id="0e84d-254">PHP</span></span>](#tab/PHP)

<span data-ttu-id="0e84d-255">なし。</span><span class="sxs-lookup"><span data-stu-id="0e84d-255">Not applicable.</span></span>

# <a name="rubytabruby"></a>[<span data-ttu-id="0e84d-256">Ruby</span><span class="sxs-lookup"><span data-stu-id="0e84d-256">Ruby</span></span>](#tab/Ruby)

<span data-ttu-id="0e84d-257">なし。</span><span class="sxs-lookup"><span data-stu-id="0e84d-257">Not applicable.</span></span>

---

##  <a name="a-nameinteractiveproviderinteractive-provider"></a><span data-ttu-id="0e84d-258"><a name="InteractiveProvider"/>対話プロバイダー</span><span class="sxs-lookup"><span data-stu-id="0e84d-258"><a name="InteractiveProvider"/>Interactive provider</span></span>

<span data-ttu-id="0e84d-259">対話型フローは、モバイルアプリケーション (Xamarin および UWP) およびデスクトップアプリケーションがユーザーの名前で Microsoft Graph を呼び出すために使用されます。</span><span class="sxs-lookup"><span data-stu-id="0e84d-259">The interactive flow is used by mobile applications (Xamarin and UWP) and desktops applications to call Microsoft Graph in the name of a user.</span></span> <span data-ttu-id="0e84d-260">詳細については、「[トークンを対話的に取得](https://github.com/AzureAD/microsoft-authentication-library-for-dotnet/wiki/Acquiring-tokens-interactively)する」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="0e84d-260">For details, see [Acquiring tokens interactively](https://github.com/AzureAD/microsoft-authentication-library-for-dotnet/wiki/Acquiring-tokens-interactively).</span></span>

# <a name="ctabcs"></a>[<span data-ttu-id="0e84d-261">C#</span><span class="sxs-lookup"><span data-stu-id="0e84d-261">C#</span></span>](#tab/CS)

```csharp
IPublicClientApplication clientApplication = InteractiveAuthenticationProvider.CreateClientApplication(clientId);
InteractiveAuthenticationProvider authProvider = new InteractiveAuthenticationProvider(clientApplication, scopes);
```

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="0e84d-262">Javascript</span><span class="sxs-lookup"><span data-stu-id="0e84d-262">Javascript</span></span>](#tab/Javascript)

<span data-ttu-id="0e84d-263">まだ使用できません。</span><span class="sxs-lookup"><span data-stu-id="0e84d-263">Not yet available.</span></span> <span data-ttu-id="0e84d-264">ユーザーにとって重要な場合は、 [Microsoft Graph の機能の要求](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests)に投票するか、開くようにしてください。</span><span class="sxs-lookup"><span data-stu-id="0e84d-264">Please vote for or open a [Microsoft Graph feature request](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) if this is important to you.</span></span>

# <a name="javatabjava"></a>[<span data-ttu-id="0e84d-265">Java</span><span class="sxs-lookup"><span data-stu-id="0e84d-265">Java</span></span>](#tab/Java)

<span data-ttu-id="0e84d-266">まだ使用できません。</span><span class="sxs-lookup"><span data-stu-id="0e84d-266">Not yet available.</span></span> <span data-ttu-id="0e84d-267">ユーザーにとって重要な場合は、 [Microsoft Graph の機能の要求](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests)に投票するか、開くようにしてください。</span><span class="sxs-lookup"><span data-stu-id="0e84d-267">Please vote for or open a [Microsoft Graph feature request](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) if this is important to you.</span></span>

# <a name="androidtabandroid"></a>[<span data-ttu-id="0e84d-268">Android</span><span class="sxs-lookup"><span data-stu-id="0e84d-268">Android</span></span>](#tab/Android)

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

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="0e84d-269">目的-C</span><span class="sxs-lookup"><span data-stu-id="0e84d-269">Objective-C</span></span>](#tab/Objective-C)

```objc
NSError *error = nil;
MSALPublicClientApplication *publicClientApplication = [[MSALPublicClientApplication alloc] initWithClientId:@"INSERT-CLIENT-APP-ID" 
error:&error];

MSALAuthenticationProviderOptions *authProviderOptions= [[MSALAuthenticationProviderOptions alloc] initWithScopes:<array-of-scopes-for-which-you-need-access-token>];

 MSALAuthenticationProvider *authenticationProvider = [[MSALAuthenticationProvider alloc] initWithPublicClientApplication:publicClientApplication 
 andOptions:authProviderOptions];
```

# <a name="phptabphp"></a>[<span data-ttu-id="0e84d-270">PHP</span><span class="sxs-lookup"><span data-stu-id="0e84d-270">PHP</span></span>](#tab/PHP)

<span data-ttu-id="0e84d-271">なし。</span><span class="sxs-lookup"><span data-stu-id="0e84d-271">Not applicable.</span></span>

# <a name="rubytabruby"></a>[<span data-ttu-id="0e84d-272">Ruby</span><span class="sxs-lookup"><span data-stu-id="0e84d-272">Ruby</span></span>](#tab/Ruby)

<span data-ttu-id="0e84d-273">なし。</span><span class="sxs-lookup"><span data-stu-id="0e84d-273">Not applicable.</span></span>

---

##  <a name="a-nameusernamepasswordproviderusernamepassword-provider"></a><span data-ttu-id="0e84d-274"><a name="UsernamePasswordProvider"/>Username/password provider</span><span class="sxs-lookup"><span data-stu-id="0e84d-274"><a name="UsernamePasswordProvider"/>Username/password provider</span></span>

<span data-ttu-id="0e84d-275">Username/password プロバイダーを使用すると、アプリケーションはユーザー名とパスワードを使用してユーザーにサインインできます。</span><span class="sxs-lookup"><span data-stu-id="0e84d-275">The username/password provider allows an application to sign in a user by using their username and password.</span></span> <span data-ttu-id="0e84d-276">このフローは、他の OAuth フローを使用できない場合にのみ使用してください。</span><span class="sxs-lookup"><span data-stu-id="0e84d-276">Use this flow only when you cannot use any of the other OAuth flows.</span></span> <span data-ttu-id="0e84d-277">詳細については、「 [Microsoft identity platform」および「OAuth 2.0 resource owner password credential](https://docs.microsoft.com/en-us/azure/active-directory/develop/v2-oauth-ropc) 」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="0e84d-277">For more information, see [Microsoft identity platform and the OAuth 2.0 resource owner password credential](https://docs.microsoft.com/en-us/azure/active-directory/develop/v2-oauth-ropc)</span></span>



# <a name="ctabcs"></a>[<span data-ttu-id="0e84d-278">C#</span><span class="sxs-lookup"><span data-stu-id="0e84d-278">C#</span></span>](#tab/CS)

```csharp
IPublicClientApplication clientApplication = UsernamePasswordProvider.CreateClientApplication(clientId);
UsernamePasswordProvider authProvider = new UsernamePasswordProvider(clientApplication, scopes);
```

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="0e84d-279">Javascript</span><span class="sxs-lookup"><span data-stu-id="0e84d-279">Javascript</span></span>](#tab/Javascript)

<span data-ttu-id="0e84d-280">まだ使用できません。</span><span class="sxs-lookup"><span data-stu-id="0e84d-280">Not yet available.</span></span> <span data-ttu-id="0e84d-281">ユーザーにとって重要な場合は、 [Microsoft Graph の機能の要求](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests)に投票するか、開くようにしてください。</span><span class="sxs-lookup"><span data-stu-id="0e84d-281">Please vote for or open a [Microsoft Graph feature request](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) if this is important to you.</span></span>

# <a name="javatabjava"></a>[<span data-ttu-id="0e84d-282">Java</span><span class="sxs-lookup"><span data-stu-id="0e84d-282">Java</span></span>](#tab/Java)

```java
UsernamePasswordProvider authProvider = new UsernamePasswordProvider(
                                                    clientId,
                                                    scopes,
                                                    username,
                                                    password);
```

# <a name="androidtabandroid"></a>[<span data-ttu-id="0e84d-283">Android</span><span class="sxs-lookup"><span data-stu-id="0e84d-283">Android</span></span>](#tab/Android)

<span data-ttu-id="0e84d-284">なし。</span><span class="sxs-lookup"><span data-stu-id="0e84d-284">Not applicable.</span></span>

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="0e84d-285">目的-C</span><span class="sxs-lookup"><span data-stu-id="0e84d-285">Objective-C</span></span>](#tab/Objective-C)

<span data-ttu-id="0e84d-286">なし。</span><span class="sxs-lookup"><span data-stu-id="0e84d-286">Not applicable.</span></span>

# <a name="phptabphp"></a>[<span data-ttu-id="0e84d-287">PHP</span><span class="sxs-lookup"><span data-stu-id="0e84d-287">PHP</span></span>](#tab/PHP)

<span data-ttu-id="0e84d-288">まだ使用できません。</span><span class="sxs-lookup"><span data-stu-id="0e84d-288">Not yet available.</span></span> <span data-ttu-id="0e84d-289">ユーザーにとって重要な場合は、 [Microsoft Graph の機能の要求](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests)に投票するか、開くようにしてください。</span><span class="sxs-lookup"><span data-stu-id="0e84d-289">Please vote for or open a [Microsoft Graph feature request](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) if this is important to you.</span></span>

# <a name="rubytabruby"></a>[<span data-ttu-id="0e84d-290">Ruby</span><span class="sxs-lookup"><span data-stu-id="0e84d-290">Ruby</span></span>](#tab/Ruby)

<span data-ttu-id="0e84d-291">まだ使用できません。</span><span class="sxs-lookup"><span data-stu-id="0e84d-291">Not yet available.</span></span> <span data-ttu-id="0e84d-292">ユーザーにとって重要な場合は、 [Microsoft Graph の機能の要求](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests)に投票するか、開くようにしてください。</span><span class="sxs-lookup"><span data-stu-id="0e84d-292">Please vote for or open a [Microsoft Graph feature request](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) if this is important to you.</span></span>

---

## <a name="next-steps"></a><span data-ttu-id="0e84d-293">次のステップ</span><span class="sxs-lookup"><span data-stu-id="0e84d-293">Next steps</span></span>

* <span data-ttu-id="0e84d-294">認証プロバイダーにはクライアント ID が必要です。</span><span class="sxs-lookup"><span data-stu-id="0e84d-294">Authentication providers require an client ID.</span></span> <span data-ttu-id="0e84d-295">認証プロバイダをセットアップした後に[、アプリケーションを登録](https://portal.azure.com/)する必要があります。</span><span class="sxs-lookup"><span data-stu-id="0e84d-295">You'll want to [register your application](https://portal.azure.com/) after you set up your authentication provider.</span></span>
* <span data-ttu-id="0e84d-296">必要な OAuth フローが現在サポートされていない場合は、 [Microsoft Graph の機能の要求](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests)に投票してください。</span><span class="sxs-lookup"><span data-stu-id="0e84d-296">Let us know if a required OAuth flow isn't currently supported by voting for or opening a [Microsoft Graph feature request](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests).</span></span>
