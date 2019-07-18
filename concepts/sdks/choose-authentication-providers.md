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
# <a name="choose-a-microsoft-graph-authentication-provider-based-on-scenario"></a><span data-ttu-id="3883e-103">シナリオに基づいて Microsoft Graph 認証プロバイダを選択する</span><span class="sxs-lookup"><span data-stu-id="3883e-103">Choose a Microsoft Graph authentication provider based on scenario</span></span>

<span data-ttu-id="3883e-104">認証プロバイダーは、Microsoft 認証ライブラリ (MSAL) を使用してトークンを取得するために必要なコードを実装します。増分の同意、期限切れのパスワード、条件付きアクセスなど、さまざまなケースの潜在的なエラーを処理します。HTTP 要求認証ヘッダーを設定します。</span><span class="sxs-lookup"><span data-stu-id="3883e-104">Authentication providers implement the code required to acquire a token using the Microsoft Authentication Library (MSAL); handle a number of potential errors for cases like incremental consent, expired passwords, and conditional access; and then set the HTTP request authorization header.</span></span> <span data-ttu-id="3883e-105">次の表に、さまざまな[種類のアプリケーション](https://docs.microsoft.com/en-us/azure/active-directory/develop/v2-app-types)のシナリオに一致する一連のプロバイダーを示します。</span><span class="sxs-lookup"><span data-stu-id="3883e-105">The following table lists the set of providers that match the scenarios for different [application types](https://docs.microsoft.com/en-us/azure/active-directory/develop/v2-app-types).</span></span>

|<span data-ttu-id="3883e-106">シナリオ</span><span class="sxs-lookup"><span data-stu-id="3883e-106">Scenario</span></span> | <span data-ttu-id="3883e-107">フロー/付与</span><span class="sxs-lookup"><span data-stu-id="3883e-107">Flow/Grant</span></span> | <span data-ttu-id="3883e-108">対象ユーザー</span><span class="sxs-lookup"><span data-stu-id="3883e-108">Audience</span></span> | <span data-ttu-id="3883e-109">プロバイダー</span><span class="sxs-lookup"><span data-stu-id="3883e-109">Provider</span></span>|
|--|--|--|--|
| [<span data-ttu-id="3883e-110">シングルページアプリ</span><span class="sxs-lookup"><span data-stu-id="3883e-110">Single Page App</span></span>](https://docs.microsoft.com/en-us/azure/active-directory/develop/scenario-spa-acquire-token)| | | |
| | <span data-ttu-id="3883e-111">暗黙的</span><span class="sxs-lookup"><span data-stu-id="3883e-111">Implicit</span></span> | <span data-ttu-id="3883e-112">委任されたコンシューマー/組織</span><span class="sxs-lookup"><span data-stu-id="3883e-112">Delegated Consumer/Org</span></span> |[<span data-ttu-id="3883e-113">暗黙的プロバイダー</span><span class="sxs-lookup"><span data-stu-id="3883e-113">Implicit Provider</span></span>](#ImplicitProvider) |
| [<span data-ttu-id="3883e-114">Web Api を呼び出す web アプリ</span><span class="sxs-lookup"><span data-stu-id="3883e-114">Web App that calls web APIs</span></span>](https://docs.microsoft.com/en-us/azure/active-directory/develop/scenario-web-app-call-api-acquire-token) | | | |
| | <span data-ttu-id="3883e-115">認証コード</span><span class="sxs-lookup"><span data-stu-id="3883e-115">Authorization Code</span></span> | <span data-ttu-id="3883e-116">委任されたコンシューマー/組織</span><span class="sxs-lookup"><span data-stu-id="3883e-116">Delegated Consumer/Org</span></span> | [<span data-ttu-id="3883e-117">認証コードプロバイダ</span><span class="sxs-lookup"><span data-stu-id="3883e-117">Authorization Code Provider</span></span>](#AuthCodeProvider) |
| | <span data-ttu-id="3883e-118">クライアント資格情報</span><span class="sxs-lookup"><span data-stu-id="3883e-118">Client Credentials</span></span>  | <span data-ttu-id="3883e-119">App Only</span><span class="sxs-lookup"><span data-stu-id="3883e-119">App Only</span></span> | [<span data-ttu-id="3883e-120">クライアント資格情報プロバイダー</span><span class="sxs-lookup"><span data-stu-id="3883e-120">Client Credentials Provider</span></span>](#ClientCredentialsProvider) |
| [<span data-ttu-id="3883e-121">Web api を呼び出す web API</span><span class="sxs-lookup"><span data-stu-id="3883e-121">Web API that calls web APIs</span></span>](https://docs.microsoft.com/en-us/azure/active-directory/develop/scenario-web-api-call-api-acquire-token) | | | |
| | <span data-ttu-id="3883e-122">代理人</span><span class="sxs-lookup"><span data-stu-id="3883e-122">On Behalf Of</span></span> | <span data-ttu-id="3883e-123">委任されたコンシューマー/組織</span><span class="sxs-lookup"><span data-stu-id="3883e-123">Delegated Consumer/Org</span></span> | [<span data-ttu-id="3883e-124">プロバイダーに代わって</span><span class="sxs-lookup"><span data-stu-id="3883e-124">On Behalf Of Provider</span></span>](#OnBehalfOfProvider) |
| | <span data-ttu-id="3883e-125">クライアント資格情報</span><span class="sxs-lookup"><span data-stu-id="3883e-125">Client Credentials</span></span>  | <span data-ttu-id="3883e-126">App Only</span><span class="sxs-lookup"><span data-stu-id="3883e-126">App Only</span></span> | [<span data-ttu-id="3883e-127">クライアント資格情報プロバイダー</span><span class="sxs-lookup"><span data-stu-id="3883e-127">Client Credentials Provider</span></span>](#ClientCredentialsProvider) |
| [<span data-ttu-id="3883e-128">Web Api を呼び出すデスクトップアプリ</span><span class="sxs-lookup"><span data-stu-id="3883e-128">Desktop app that calls web APIs</span></span>](https://docs.microsoft.com/en-us/azure/active-directory/develop/scenario-desktop-acquire-token) | | | |
| | <span data-ttu-id="3883e-129">Interactive</span><span class="sxs-lookup"><span data-stu-id="3883e-129">Interactive</span></span> | <span data-ttu-id="3883e-130">委任されたコンシューマー/組織</span><span class="sxs-lookup"><span data-stu-id="3883e-130">Delegated Consumer/Org</span></span> | [<span data-ttu-id="3883e-131">対話プロバイダー</span><span class="sxs-lookup"><span data-stu-id="3883e-131">Interactive Provider</span></span>](#InteractiveProvider) |
| | <span data-ttu-id="3883e-132">統合 Windows</span><span class="sxs-lookup"><span data-stu-id="3883e-132">Integrated Windows</span></span> | <span data-ttu-id="3883e-133">委任された組織</span><span class="sxs-lookup"><span data-stu-id="3883e-133">Delegated Org</span></span> | [<span data-ttu-id="3883e-134">統合 Windows プロバイダ</span><span class="sxs-lookup"><span data-stu-id="3883e-134">Integrated Windows Provider</span></span>](#IntegratedWindowsProvider) |
| | <span data-ttu-id="3883e-135">リソース所有者</span><span class="sxs-lookup"><span data-stu-id="3883e-135">Resource Owner</span></span>  | <span data-ttu-id="3883e-136">委任された組織</span><span class="sxs-lookup"><span data-stu-id="3883e-136">Delegated Org</span></span> | [<span data-ttu-id="3883e-137">Username/Password Provider</span><span class="sxs-lookup"><span data-stu-id="3883e-137">Username / Password Provider</span></span>](#UsernamePasswordProvider) |
| | <span data-ttu-id="3883e-138">デバイスコード</span><span class="sxs-lookup"><span data-stu-id="3883e-138">Device Code</span></span>  | <span data-ttu-id="3883e-139">委任された組織</span><span class="sxs-lookup"><span data-stu-id="3883e-139">Delegated Org</span></span> | [<span data-ttu-id="3883e-140">デバイスコードプロバイダ</span><span class="sxs-lookup"><span data-stu-id="3883e-140">Device Code Provider</span></span>](#DeviceCodeProvider) |
| [<span data-ttu-id="3883e-141">デーモンアプリ</span><span class="sxs-lookup"><span data-stu-id="3883e-141">Daemon app</span></span>](https://docs.microsoft.com/en-us/azure/active-directory/develop/scenario-daemon-acquire-token) | | | |
| | <span data-ttu-id="3883e-142">クライアント資格情報</span><span class="sxs-lookup"><span data-stu-id="3883e-142">Client Credentials</span></span>  | <span data-ttu-id="3883e-143">App Only</span><span class="sxs-lookup"><span data-stu-id="3883e-143">App Only</span></span> | [<span data-ttu-id="3883e-144">クライアント資格情報プロバイダー</span><span class="sxs-lookup"><span data-stu-id="3883e-144">Client Credentials Provider</span></span>](#ClientCredentialsProvider) |
| [<span data-ttu-id="3883e-145">Web Api を呼び出すモバイルアプリ</span><span class="sxs-lookup"><span data-stu-id="3883e-145">Mobile app that calls web APIs</span></span>](https://docs.microsoft.com/en-us/azure/active-directory/develop/scenario-mobile-acquire-token) | | | |
| | <span data-ttu-id="3883e-146">Interactive</span><span class="sxs-lookup"><span data-stu-id="3883e-146">Interactive</span></span> | <span data-ttu-id="3883e-147">委任されたコンシューマー/組織</span><span class="sxs-lookup"><span data-stu-id="3883e-147">Delegated Consumer/Org</span></span> | [<span data-ttu-id="3883e-148">対話プロバイダー</span><span class="sxs-lookup"><span data-stu-id="3883e-148">Interactive Provider</span></span>](#InteractiveProvider) |


## <a name="a-nameauthcodeproviderauthorization-code-provider"></a><span data-ttu-id="3883e-149"><a name="AuthCodeProvider"/>認証コードプロバイダ</span><span class="sxs-lookup"><span data-stu-id="3883e-149"><a name="AuthCodeProvider"/>Authorization code provider</span></span>

<span data-ttu-id="3883e-150">認証コードフローにより、ネイティブおよび web アプリはユーザーの名前でトークンを安全に取得することができます。</span><span class="sxs-lookup"><span data-stu-id="3883e-150">The authorization code flow enables native and web apps to securely obtain tokens in the name of the user.</span></span> <span data-ttu-id="3883e-151">詳細については、「 [Microsoft identity platform And OAuth 2.0 認証コードフロー](https://docs.microsoft.com/en-us/azure/active-directory/develop/v2-oauth2-auth-code-flow)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="3883e-151">To learn more, see [Microsoft identity platform and OAuth 2.0 authorization code flow](https://docs.microsoft.com/en-us/azure/active-directory/develop/v2-oauth2-auth-code-flow).</span></span>

# <a name="ctabcs"></a>[<span data-ttu-id="3883e-152">C#</span><span class="sxs-lookup"><span data-stu-id="3883e-152">C#</span></span>](#tab/CS)

```csharp
IConfidentialClientApplication confidentialClientApplication = ConfidentialClientApplicationBuilder
    .Create(clientId)
    .WithRedirectUri(redirectUri)
    .WithClientSecret(clientSecret) // or .WithCertificate(certificate)
    .Build();

AuthorizationCodeProvider authProvider = new AuthorizationCodeProvider(confidentialClientApplication, scopes);  
```

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="3883e-153">Javascript</span><span class="sxs-lookup"><span data-stu-id="3883e-153">Javascript</span></span>](#tab/Javascript)

<span data-ttu-id="3883e-154">認証コード、クライアント資格情報、および非代行の OAuth フローでは、この時点でカスタム認証プロバイダーを実装する必要があります。</span><span class="sxs-lookup"><span data-stu-id="3883e-154">Authorization code, client credential, and on-behalf-of OAuth flows require that you implement a custom authentication provider at this time.</span></span> <span data-ttu-id="3883e-155">詳細については、「 [Using a custom authentication provider](https://github.com/microsoftgraph/msgraph-sdk-javascript/blob/dev/docs/CustomAuthenticationProvider.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="3883e-155">For more information, see [Using a custom authentication provider](https://github.com/microsoftgraph/msgraph-sdk-javascript/blob/dev/docs/CustomAuthenticationProvider.md).</span></span>

# <a name="javatabjava"></a>[<span data-ttu-id="3883e-156">Java</span><span class="sxs-lookup"><span data-stu-id="3883e-156">Java</span></span>](#tab/Java)

```java
AuthorizationCodeProvider authProvider = new AuthorizationCodeProvider(
                                                    clientId,
                                                    scopes,
                                                    authorizationCode,
                                                    redirectUri,
                                                    clientSecret);
```

# <a name="androidtabandroid"></a>[<span data-ttu-id="3883e-157">Android</span><span class="sxs-lookup"><span data-stu-id="3883e-157">Android</span></span>](#tab/Android)

<span data-ttu-id="3883e-158">なし。</span><span class="sxs-lookup"><span data-stu-id="3883e-158">Not applicable.</span></span>

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="3883e-159">目的-C</span><span class="sxs-lookup"><span data-stu-id="3883e-159">Objective-C</span></span>](#tab/Objective-C)

<span data-ttu-id="3883e-160">なし。</span><span class="sxs-lookup"><span data-stu-id="3883e-160">Not applicable.</span></span>

# <a name="phptabphp"></a>[<span data-ttu-id="3883e-161">PHP</span><span class="sxs-lookup"><span data-stu-id="3883e-161">PHP</span></span>](#tab/PHP)

<span data-ttu-id="3883e-162">まだ使用できません。</span><span class="sxs-lookup"><span data-stu-id="3883e-162">Not yet available.</span></span> <span data-ttu-id="3883e-163">ユーザーにとって重要な場合は、 [Microsoft Graph の機能の要求](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests)をサポートするか、または開きます。</span><span class="sxs-lookup"><span data-stu-id="3883e-163">Please support or open a [Microsoft Graph feature request](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) if this is important to you.</span></span>

# <a name="rubytabruby"></a>[<span data-ttu-id="3883e-164">Ruby</span><span class="sxs-lookup"><span data-stu-id="3883e-164">Ruby</span></span>](#tab/Ruby)

<span data-ttu-id="3883e-165">まだ利用できません。</span><span class="sxs-lookup"><span data-stu-id="3883e-165">Not available, yet.</span></span> <span data-ttu-id="3883e-166">ユーザーにとって重要な場合は、 [Microsoft Graph の機能の要求](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests)に投票するか、開くようにしてください。</span><span class="sxs-lookup"><span data-stu-id="3883e-166">Please vote for or open a [Microsoft Graph feature request](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) if this is important to you.</span></span>

---

##  <a name="a-nameclientcredentialsproviderclient-credentials-provider"></a><span data-ttu-id="3883e-167"><a name="ClientCredentialsProvider"/>クライアント資格情報プロバイダー</span><span class="sxs-lookup"><span data-stu-id="3883e-167"><a name="ClientCredentialsProvider"/>Client credentials provider</span></span>

<span data-ttu-id="3883e-168">クライアント資格情報フローを使用すると、ユーザーによる操作なしでサービスアプリケーションを実行できます。</span><span class="sxs-lookup"><span data-stu-id="3883e-168">The client credential flow enables service applications to run without user interaction.</span></span> <span data-ttu-id="3883e-169">Access は、アプリケーションの id に基づいています。</span><span class="sxs-lookup"><span data-stu-id="3883e-169">Access is based on the identity of the application.</span></span> <span data-ttu-id="3883e-170">詳細については、「 [Microsoft identity platform」および「OAuth 2.0 クライアント資格情報フロー](https://docs.microsoft.com/en-us/azure/active-directory/develop/v2-oauth2-client-creds-grant-flow)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="3883e-170">For more information, see [Microsoft identity platform and the OAuth 2.0 client credentials flow](https://docs.microsoft.com/en-us/azure/active-directory/develop/v2-oauth2-client-creds-grant-flow).</span></span>

# <a name="ctabcs"></a>[<span data-ttu-id="3883e-171">C#</span><span class="sxs-lookup"><span data-stu-id="3883e-171">C#</span></span>](#tab/CS)

```csharp
IConfidentialClientApplication confidentialClientApplication = ConfidentialClientApplicationBuilder
    .Create(clientId)
    .WithTenantId(tenantID)
    .WithClientSecret(clientSecret)
    .Build();

ClientCredentialProvider authProvider = new ClientCredentialProvider(confidentialClientApplication);
```

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="3883e-172">Javascript</span><span class="sxs-lookup"><span data-stu-id="3883e-172">Javascript</span></span>](#tab/Javascript)

<span data-ttu-id="3883e-173">認証コード、クライアント資格情報、および非代行の OAuth フローでは、この時点でカスタム認証プロバイダーを実装する必要があります。</span><span class="sxs-lookup"><span data-stu-id="3883e-173">Authorization code, client credential, and on-behalf-of OAuth flows require that you implement a custom authentication provider at this time.</span></span> <span data-ttu-id="3883e-174">詳細については、「 [Using a custom authentication provider](https://github.com/microsoftgraph/msgraph-sdk-javascript/blob/dev/docs/CustomAuthenticationProvider.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="3883e-174">For more information, see [Using a custom authentication provider](https://github.com/microsoftgraph/msgraph-sdk-javascript/blob/dev/docs/CustomAuthenticationProvider.md).</span></span>

# <a name="javatabjava"></a>[<span data-ttu-id="3883e-175">Java</span><span class="sxs-lookup"><span data-stu-id="3883e-175">Java</span></span>](#tab/Java)

```java
ClientCredentialProvider authProvider = new ClientCredentialProvider(
                                                    clientId,
                                                    scopes,
                                                    clientSecret,
                                                    tenant,
                                                    endpoint);
```

# <a name="androidtabandroid"></a>[<span data-ttu-id="3883e-176">Android</span><span class="sxs-lookup"><span data-stu-id="3883e-176">Android</span></span>](#tab/Android)

<span data-ttu-id="3883e-177">なし。</span><span class="sxs-lookup"><span data-stu-id="3883e-177">Not applicable.</span></span>

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="3883e-178">目的-C</span><span class="sxs-lookup"><span data-stu-id="3883e-178">Objective-C</span></span>](#tab/Objective-C)

<span data-ttu-id="3883e-179">なし。</span><span class="sxs-lookup"><span data-stu-id="3883e-179">Not applicable.</span></span>

# <a name="phptabphp"></a>[<span data-ttu-id="3883e-180">PHP</span><span class="sxs-lookup"><span data-stu-id="3883e-180">PHP</span></span>](#tab/PHP)

<span data-ttu-id="3883e-181">まだ利用できません。</span><span class="sxs-lookup"><span data-stu-id="3883e-181">Not available, yet.</span></span> <span data-ttu-id="3883e-182">ユーザーにとって重要な場合は、 [Microsoft Graph の機能の要求](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests)をサポートするか、または開きます。</span><span class="sxs-lookup"><span data-stu-id="3883e-182">Please support or open a [Microsoft Graph feature request](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) if this is important to you.</span></span>

# <a name="rubytabruby"></a>[<span data-ttu-id="3883e-183">Ruby</span><span class="sxs-lookup"><span data-stu-id="3883e-183">Ruby</span></span>](#tab/Ruby)

<span data-ttu-id="3883e-184">まだ利用できません。</span><span class="sxs-lookup"><span data-stu-id="3883e-184">Not available, yet.</span></span> <span data-ttu-id="3883e-185">ユーザーにとって重要な場合は、 [Microsoft Graph の機能の要求](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests)をサポートするか、または開きます。</span><span class="sxs-lookup"><span data-stu-id="3883e-185">Please support or open a [Microsoft Graph feature request](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) if this is important to you.</span></span>

---

##  <a name="a-nameonbehalfofprovideron-behalf-of-provider"></a><span data-ttu-id="3883e-186"><a name="OnBehalfOfProvider"/>プロバイダーの代理</span><span class="sxs-lookup"><span data-stu-id="3883e-186"><a name="OnBehalfOfProvider"/>On-behalf-of provider</span></span>

<span data-ttu-id="3883e-187">アプリケーションが Microsoft Graph API を呼び出すサービスまたは web API を呼び出すときに、その代わりの流れが適用されます。</span><span class="sxs-lookup"><span data-stu-id="3883e-187">The on-behalf-of flow is applicable when your application calls a service/web API which in turns calls the Microsoft Graph API.</span></span> <span data-ttu-id="3883e-188">[Microsoft identity platform および OAuth 2.0 の送信フローの](https://docs.microsoft.com/en-us/azure/active-directory/develop/v2-oauth2-on-behalf-of-flow)詳細については、こちらを参照してください。</span><span class="sxs-lookup"><span data-stu-id="3883e-188">Learn more by reading [Microsoft identity platform and OAuth 2.0 On-Behalf-Of flow](https://docs.microsoft.com/en-us/azure/active-directory/develop/v2-oauth2-on-behalf-of-flow)</span></span>

# <a name="ctabcs"></a>[<span data-ttu-id="3883e-189">C#</span><span class="sxs-lookup"><span data-stu-id="3883e-189">C#</span></span>](#tab/CS)

```csharp
IConfidentialClientApplication confidentialClientApplication = ConfidentialClientApplicationBuilder
    .Create(clientId)
    .WithRedirectUri(redirectUri)
    .WithClientSecret(clientSecret)
    .Build();

OnBehalfOfProvider authProvider = new OnBehalfOfProvider(confidentialClientApplication, scopes);
```

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="3883e-190">Javascript</span><span class="sxs-lookup"><span data-stu-id="3883e-190">Javascript</span></span>](#tab/Javascript)

<span data-ttu-id="3883e-191">認証コード、クライアント資格情報、および非代行の OAuth フローでは、この時点でカスタム認証プロバイダーを実装する必要があります。</span><span class="sxs-lookup"><span data-stu-id="3883e-191">Authorization code, client credential, and on-behalf-of OAuth flows require that you implement a custom authentication provider at this time.</span></span> <span data-ttu-id="3883e-192">詳細については、「[カスタム認証プロバイダを使用する](https://github.com/microsoftgraph/msgraph-sdk-javascript/blob/dev/docs/CustomAuthenticationProvider.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="3883e-192">Read [Using Custom Authentication Provider](https://github.com/microsoftgraph/msgraph-sdk-javascript/blob/dev/docs/CustomAuthenticationProvider.md) for more information.</span></span>

# <a name="javatabjava"></a>[<span data-ttu-id="3883e-193">Java</span><span class="sxs-lookup"><span data-stu-id="3883e-193">Java</span></span>](#tab/Java)

<span data-ttu-id="3883e-194">まだ使用できません。</span><span class="sxs-lookup"><span data-stu-id="3883e-194">Not yet available.</span></span> <span data-ttu-id="3883e-195">ユーザーにとって重要な場合は、 [Microsoft Graph の機能の要求](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests)に投票するか、開くようにしてください。</span><span class="sxs-lookup"><span data-stu-id="3883e-195">Please vote for or open a [Microsoft Graph feature request](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) if this is important to you.</span></span>

# <a name="androidtabandroid"></a>[<span data-ttu-id="3883e-196">Android</span><span class="sxs-lookup"><span data-stu-id="3883e-196">Android</span></span>](#tab/Android)

<span data-ttu-id="3883e-197">なし。</span><span class="sxs-lookup"><span data-stu-id="3883e-197">Not applicable.</span></span>

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="3883e-198">目的-C</span><span class="sxs-lookup"><span data-stu-id="3883e-198">Objective-C</span></span>](#tab/Objective-C)

<span data-ttu-id="3883e-199">なし。</span><span class="sxs-lookup"><span data-stu-id="3883e-199">Not applicable.</span></span>

# <a name="phptabphp"></a>[<span data-ttu-id="3883e-200">PHP</span><span class="sxs-lookup"><span data-stu-id="3883e-200">PHP</span></span>](#tab/PHP)

<span data-ttu-id="3883e-201">まだ使用できません。</span><span class="sxs-lookup"><span data-stu-id="3883e-201">Not yet available.</span></span> <span data-ttu-id="3883e-202">ユーザーにとって重要な場合は、 [Microsoft Graph の機能の要求](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests)に投票するか、開くようにしてください。</span><span class="sxs-lookup"><span data-stu-id="3883e-202">Please vote for or open a [Microsoft Graph feature request](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) if this is important to you.</span></span>

# <a name="rubytabruby"></a>[<span data-ttu-id="3883e-203">Ruby</span><span class="sxs-lookup"><span data-stu-id="3883e-203">Ruby</span></span>](#tab/Ruby)

<span data-ttu-id="3883e-204">まだ使用できません。</span><span class="sxs-lookup"><span data-stu-id="3883e-204">Not yet available.</span></span> <span data-ttu-id="3883e-205">ユーザーにとって重要な場合は、 [Microsoft Graph の機能の要求](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests)に投票するか、開くようにしてください。</span><span class="sxs-lookup"><span data-stu-id="3883e-205">Please vote for or open a [Microsoft Graph feature request](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) if this is important to you.</span></span>

---

## <a name="a-nameimplicitproviderimplicit-provider"></a><span data-ttu-id="3883e-206"><a name="ImplicitProvider"/>暗黙的プロバイダー</span><span class="sxs-lookup"><span data-stu-id="3883e-206"><a name="ImplicitProvider"/>Implicit provider</span></span>

<span data-ttu-id="3883e-207">暗黙的な付与フローは、ブラウザーベースのアプリケーションで使用されます。</span><span class="sxs-lookup"><span data-stu-id="3883e-207">The implicit grant flow is used in browser-based applications.</span></span> <span data-ttu-id="3883e-208">詳細については、「 [Microsoft identity platform」および「暗黙的な許可の流れ](https://docs.microsoft.com/en-us/azure/active-directory/develop/v2-oauth2-implicit-grant-flow)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="3883e-208">For more information, see [Microsoft identity platform and Implicit grant flow](https://docs.microsoft.com/en-us/azure/active-directory/develop/v2-oauth2-implicit-grant-flow).</span></span>

# <a name="ctabcs"></a>[<span data-ttu-id="3883e-209">C#</span><span class="sxs-lookup"><span data-stu-id="3883e-209">C#</span></span>](#tab/CS)

<span data-ttu-id="3883e-210">なし。</span><span class="sxs-lookup"><span data-stu-id="3883e-210">Not applicable.</span></span>

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="3883e-211">Javascript</span><span class="sxs-lookup"><span data-stu-id="3883e-211">Javascript</span></span>](#tab/Javascript)

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

# <a name="javatabjava"></a>[<span data-ttu-id="3883e-212">Java</span><span class="sxs-lookup"><span data-stu-id="3883e-212">Java</span></span>](#tab/Java)

<span data-ttu-id="3883e-213">なし。</span><span class="sxs-lookup"><span data-stu-id="3883e-213">Not applicable.</span></span>

# <a name="androidtabandroid"></a>[<span data-ttu-id="3883e-214">Android</span><span class="sxs-lookup"><span data-stu-id="3883e-214">Android</span></span>](#tab/Android)

<span data-ttu-id="3883e-215">なし。</span><span class="sxs-lookup"><span data-stu-id="3883e-215">Not applicable.</span></span>

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="3883e-216">目的-C</span><span class="sxs-lookup"><span data-stu-id="3883e-216">Objective-C</span></span>](#tab/Objective-C)

<span data-ttu-id="3883e-217">なし。</span><span class="sxs-lookup"><span data-stu-id="3883e-217">Not applicable.</span></span>

# <a name="phptabphp"></a>[<span data-ttu-id="3883e-218">PHP</span><span class="sxs-lookup"><span data-stu-id="3883e-218">PHP</span></span>](#tab/PHP)

<span data-ttu-id="3883e-219">なし。</span><span class="sxs-lookup"><span data-stu-id="3883e-219">Not applicable.</span></span>

# <a name="rubytabruby"></a>[<span data-ttu-id="3883e-220">Ruby</span><span class="sxs-lookup"><span data-stu-id="3883e-220">Ruby</span></span>](#tab/Ruby)

<span data-ttu-id="3883e-221">なし。</span><span class="sxs-lookup"><span data-stu-id="3883e-221">Not applicable.</span></span>

---

##  <a name="a-namedevicecodeproviderdevice-code-provider"></a><span data-ttu-id="3883e-222"><a name="DeviceCodeProvider"/>デバイスコードプロバイダ</span><span class="sxs-lookup"><span data-stu-id="3883e-222"><a name="DeviceCodeProvider"/>Device code provider</span></span>

<span data-ttu-id="3883e-223">デバイスコードフローによって、別のデバイスを使用してデバイスにサインインできるようになります。</span><span class="sxs-lookup"><span data-stu-id="3883e-223">The device code flow enables sign in to devices by way of another device.</span></span> <span data-ttu-id="3883e-224">詳細については、「 [Microsoft identity platform」および「OAuth 2.0 デバイスコードフロー](https://docs.microsoft.com/en-us/azure/active-directory/develop/v2-oauth2-device-code)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="3883e-224">For details, see [Microsoft identity platform and the OAuth 2.0 device code flow](https://docs.microsoft.com/en-us/azure/active-directory/develop/v2-oauth2-device-code).</span></span>

# <a name="ctabcs"></a>[<span data-ttu-id="3883e-225">C#</span><span class="sxs-lookup"><span data-stu-id="3883e-225">C#</span></span>](#tab/CS)

```csharp
IPublicClientApplication publicClientApplication = PublicClientApplicationBuilder
            .Create(clientId)
            .Build();

Func<DeviceCodeResult, Task> deviceCodeReadyCallback = async dcr => await Console.Out.WriteLineAsync(dcr.Message);

DeviceCodeProvider authProvider = new DeviceCodeProvider(publicClientApplication, scopes, deviceCodeReadyCallback);
```

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="3883e-226">Javascript</span><span class="sxs-lookup"><span data-stu-id="3883e-226">Javascript</span></span>](#tab/Javascript)

<span data-ttu-id="3883e-227">まだ使用できません。</span><span class="sxs-lookup"><span data-stu-id="3883e-227">Not yet available.</span></span> <span data-ttu-id="3883e-228">ユーザーにとって重要な場合は、 [Microsoft Graph の機能の要求](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests)に投票するか、開くようにしてください。</span><span class="sxs-lookup"><span data-stu-id="3883e-228">Please vote for or open a [Microsoft Graph feature request](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) if this is important to you.</span></span>

# <a name="javatabjava"></a>[<span data-ttu-id="3883e-229">Java</span><span class="sxs-lookup"><span data-stu-id="3883e-229">Java</span></span>](#tab/Java)

<span data-ttu-id="3883e-230">まだ利用できません。</span><span class="sxs-lookup"><span data-stu-id="3883e-230">Not available, yet.</span></span> <span data-ttu-id="3883e-231">ユーザーにとって重要な場合は、 [Microsoft Graph の機能の要求](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests)をサポートするか、または開きます。</span><span class="sxs-lookup"><span data-stu-id="3883e-231">Please support or open a [Microsoft Graph feature request](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) if this is important to you.</span></span>

# <a name="androidtabandroid"></a>[<span data-ttu-id="3883e-232">Android</span><span class="sxs-lookup"><span data-stu-id="3883e-232">Android</span></span>](#tab/Android)

<span data-ttu-id="3883e-233">なし。</span><span class="sxs-lookup"><span data-stu-id="3883e-233">Not applicable.</span></span>

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="3883e-234">目的-C</span><span class="sxs-lookup"><span data-stu-id="3883e-234">Objective-C</span></span>](#tab/Objective-C)

<span data-ttu-id="3883e-235">なし。</span><span class="sxs-lookup"><span data-stu-id="3883e-235">Not applicable.</span></span>

# <a name="phptabphp"></a>[<span data-ttu-id="3883e-236">PHP</span><span class="sxs-lookup"><span data-stu-id="3883e-236">PHP</span></span>](#tab/PHP)

<span data-ttu-id="3883e-237">まだ使用できません。</span><span class="sxs-lookup"><span data-stu-id="3883e-237">Not yet available.</span></span> <span data-ttu-id="3883e-238">ユーザーにとって重要な場合は、 [Microsoft Graph の機能の要求](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests)に投票するか、開くようにしてください。</span><span class="sxs-lookup"><span data-stu-id="3883e-238">Please vote for or open a [Microsoft Graph feature request](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) if this is important to you.</span></span>

# <a name="rubytabruby"></a>[<span data-ttu-id="3883e-239">Ruby</span><span class="sxs-lookup"><span data-stu-id="3883e-239">Ruby</span></span>](#tab/Ruby)

<span data-ttu-id="3883e-240">まだ使用できません。</span><span class="sxs-lookup"><span data-stu-id="3883e-240">Not yet available.</span></span> <span data-ttu-id="3883e-241">ユーザーにとって重要な場合は、 [Microsoft Graph の機能の要求](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests)に投票するか、開くようにしてください。</span><span class="sxs-lookup"><span data-stu-id="3883e-241">Please vote for or open a [Microsoft Graph feature request](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) if this is important to you.</span></span>

---

##  <a name="a-nameintegratedwindowsproviderintegrated-windows-provider"></a><span data-ttu-id="3883e-242"><a name="IntegratedWindowsProvider"/>統合 Windows プロバイダ</span><span class="sxs-lookup"><span data-stu-id="3883e-242"><a name="IntegratedWindowsProvider"/>Integrated Windows provider</span></span>

<span data-ttu-id="3883e-243">統合 Windows フローにより、Windows コンピューターがドメインに参加している場合に、アクセストークンをサイレントに取得することができます。</span><span class="sxs-lookup"><span data-stu-id="3883e-243">The integrated Windows flow provides a way for Windows computers to silently acquire an access token when they are domain joined.</span></span> <span data-ttu-id="3883e-244">詳細については、「[統合 Windows 認証](https://github.com/AzureAD/microsoft-authentication-library-for-dotnet/wiki/Integrated-Windows-Authentication)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="3883e-244">For details, see [Integrated Windows authentication](https://github.com/AzureAD/microsoft-authentication-library-for-dotnet/wiki/Integrated-Windows-Authentication).</span></span>

# <a name="ctabcs"></a>[<span data-ttu-id="3883e-245">C#</span><span class="sxs-lookup"><span data-stu-id="3883e-245">C#</span></span>](#tab/CS)

```csharp
IPublicClientApplication publicClientApplication = PublicClientApplicationBuilder
            .Create(clientId)
            .WithTenantId(tenantID)
            .Build();

IntegratedWindowsAuthenticationProvider authProvider = new IntegratedWindowsAuthenticationProvider(publicClientApplication, scopes);
```

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="3883e-246">Javascript</span><span class="sxs-lookup"><span data-stu-id="3883e-246">Javascript</span></span>](#tab/Javascript)

<span data-ttu-id="3883e-247">なし。</span><span class="sxs-lookup"><span data-stu-id="3883e-247">Not applicable.</span></span>

# <a name="javatabjava"></a>[<span data-ttu-id="3883e-248">Java</span><span class="sxs-lookup"><span data-stu-id="3883e-248">Java</span></span>](#tab/Java)

<span data-ttu-id="3883e-249">なし。</span><span class="sxs-lookup"><span data-stu-id="3883e-249">Not applicable.</span></span>

# <a name="androidtabandroid"></a>[<span data-ttu-id="3883e-250">Android</span><span class="sxs-lookup"><span data-stu-id="3883e-250">Android</span></span>](#tab/Android)

<span data-ttu-id="3883e-251">なし。</span><span class="sxs-lookup"><span data-stu-id="3883e-251">Not applicable.</span></span>

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="3883e-252">目的-C</span><span class="sxs-lookup"><span data-stu-id="3883e-252">Objective-C</span></span>](#tab/Objective-C)

<span data-ttu-id="3883e-253">なし。</span><span class="sxs-lookup"><span data-stu-id="3883e-253">Not applicable.</span></span>

# <a name="phptabphp"></a>[<span data-ttu-id="3883e-254">PHP</span><span class="sxs-lookup"><span data-stu-id="3883e-254">PHP</span></span>](#tab/PHP)

<span data-ttu-id="3883e-255">なし。</span><span class="sxs-lookup"><span data-stu-id="3883e-255">Not applicable.</span></span>

# <a name="rubytabruby"></a>[<span data-ttu-id="3883e-256">Ruby</span><span class="sxs-lookup"><span data-stu-id="3883e-256">Ruby</span></span>](#tab/Ruby)

<span data-ttu-id="3883e-257">なし。</span><span class="sxs-lookup"><span data-stu-id="3883e-257">Not applicable.</span></span>

---

##  <a name="a-nameinteractiveproviderinteractive-provider"></a><span data-ttu-id="3883e-258"><a name="InteractiveProvider"/>対話プロバイダー</span><span class="sxs-lookup"><span data-stu-id="3883e-258"><a name="InteractiveProvider"/>Interactive provider</span></span>

<span data-ttu-id="3883e-259">対話型フローは、モバイルアプリケーション (Xamarin および UWP) およびデスクトップアプリケーションがユーザーの名前で Microsoft Graph を呼び出すために使用されます。</span><span class="sxs-lookup"><span data-stu-id="3883e-259">The interactive flow is used by mobile applications (Xamarin and UWP) and desktops applications to call Microsoft Graph in the name of a user.</span></span> <span data-ttu-id="3883e-260">詳細については、「[トークンを対話的に取得](https://github.com/AzureAD/microsoft-authentication-library-for-dotnet/wiki/Acquiring-tokens-interactively)する」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="3883e-260">For details, see [Acquiring tokens interactively](https://github.com/AzureAD/microsoft-authentication-library-for-dotnet/wiki/Acquiring-tokens-interactively).</span></span>

# <a name="ctabcs"></a>[<span data-ttu-id="3883e-261">C#</span><span class="sxs-lookup"><span data-stu-id="3883e-261">C#</span></span>](#tab/CS)

```csharp
IPublicClientApplication publicClientApplication = PublicClientApplicationBuilder
            .Create(clientId)
            .Build();

InteractiveAuthenticationProvider authProvider = new InteractiveAuthenticationProvider(publicClientApplication, scopes);
```

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="3883e-262">Javascript</span><span class="sxs-lookup"><span data-stu-id="3883e-262">Javascript</span></span>](#tab/Javascript)

<span data-ttu-id="3883e-263">まだ使用できません。</span><span class="sxs-lookup"><span data-stu-id="3883e-263">Not yet available.</span></span> <span data-ttu-id="3883e-264">ユーザーにとって重要な場合は、 [Microsoft Graph の機能の要求](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests)に投票するか、開くようにしてください。</span><span class="sxs-lookup"><span data-stu-id="3883e-264">Please vote for or open a [Microsoft Graph feature request](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) if this is important to you.</span></span>

# <a name="javatabjava"></a>[<span data-ttu-id="3883e-265">Java</span><span class="sxs-lookup"><span data-stu-id="3883e-265">Java</span></span>](#tab/Java)

<span data-ttu-id="3883e-266">まだ使用できません。</span><span class="sxs-lookup"><span data-stu-id="3883e-266">Not yet available.</span></span> <span data-ttu-id="3883e-267">ユーザーにとって重要な場合は、 [Microsoft Graph の機能の要求](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests)に投票するか、開くようにしてください。</span><span class="sxs-lookup"><span data-stu-id="3883e-267">Please vote for or open a [Microsoft Graph feature request](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) if this is important to you.</span></span>

# <a name="androidtabandroid"></a>[<span data-ttu-id="3883e-268">Android</span><span class="sxs-lookup"><span data-stu-id="3883e-268">Android</span></span>](#tab/Android)

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

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="3883e-269">目的-C</span><span class="sxs-lookup"><span data-stu-id="3883e-269">Objective-C</span></span>](#tab/Objective-C)

```objc
NSError *error = nil;
MSALPublicClientApplication *publicClientApplication = [[MSALPublicClientApplication alloc] initWithClientId:@"INSERT-CLIENT-APP-ID" 
error:&error];

MSALAuthenticationProviderOptions *authProviderOptions= [[MSALAuthenticationProviderOptions alloc] initWithScopes:<array-of-scopes-for-which-you-need-access-token>];

 MSALAuthenticationProvider *authenticationProvider = [[MSALAuthenticationProvider alloc] initWithPublicClientApplication:publicClientApplication 
 andOptions:authProviderOptions];
```

# <a name="phptabphp"></a>[<span data-ttu-id="3883e-270">PHP</span><span class="sxs-lookup"><span data-stu-id="3883e-270">PHP</span></span>](#tab/PHP)

<span data-ttu-id="3883e-271">なし。</span><span class="sxs-lookup"><span data-stu-id="3883e-271">Not applicable.</span></span>

# <a name="rubytabruby"></a>[<span data-ttu-id="3883e-272">Ruby</span><span class="sxs-lookup"><span data-stu-id="3883e-272">Ruby</span></span>](#tab/Ruby)

<span data-ttu-id="3883e-273">なし。</span><span class="sxs-lookup"><span data-stu-id="3883e-273">Not applicable.</span></span>

---

##  <a name="a-nameusernamepasswordproviderusernamepassword-provider"></a><span data-ttu-id="3883e-274"><a name="UsernamePasswordProvider"/>Username/password provider</span><span class="sxs-lookup"><span data-stu-id="3883e-274"><a name="UsernamePasswordProvider"/>Username/password provider</span></span>

<span data-ttu-id="3883e-275">Username/password プロバイダーを使用すると、アプリケーションはユーザー名とパスワードを使用してユーザーにサインインできます。</span><span class="sxs-lookup"><span data-stu-id="3883e-275">The username/password provider allows an application to sign in a user by using their username and password.</span></span> <span data-ttu-id="3883e-276">このフローは、他の OAuth フローを使用できない場合にのみ使用してください。</span><span class="sxs-lookup"><span data-stu-id="3883e-276">Use this flow only when you cannot use any of the other OAuth flows.</span></span> <span data-ttu-id="3883e-277">詳細については、「 [Microsoft identity platform」および「OAuth 2.0 resource owner password credential](https://docs.microsoft.com/en-us/azure/active-directory/develop/v2-oauth-ropc) 」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="3883e-277">For more information, see [Microsoft identity platform and the OAuth 2.0 resource owner password credential](https://docs.microsoft.com/en-us/azure/active-directory/develop/v2-oauth-ropc)</span></span>



# <a name="ctabcs"></a>[<span data-ttu-id="3883e-278">C#</span><span class="sxs-lookup"><span data-stu-id="3883e-278">C#</span></span>](#tab/CS)

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

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="3883e-279">Javascript</span><span class="sxs-lookup"><span data-stu-id="3883e-279">Javascript</span></span>](#tab/Javascript)

<span data-ttu-id="3883e-280">まだ使用できません。</span><span class="sxs-lookup"><span data-stu-id="3883e-280">Not yet available.</span></span> <span data-ttu-id="3883e-281">ユーザーにとって重要な場合は、 [Microsoft Graph の機能の要求](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests)に投票するか、開くようにしてください。</span><span class="sxs-lookup"><span data-stu-id="3883e-281">Please vote for or open a [Microsoft Graph feature request](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) if this is important to you.</span></span>

# <a name="javatabjava"></a>[<span data-ttu-id="3883e-282">Java</span><span class="sxs-lookup"><span data-stu-id="3883e-282">Java</span></span>](#tab/Java)

```java
UsernamePasswordProvider authProvider = new UsernamePasswordProvider(
                                                    clientId,
                                                    scopes,
                                                    username,
                                                    password);
```

# <a name="androidtabandroid"></a>[<span data-ttu-id="3883e-283">Android</span><span class="sxs-lookup"><span data-stu-id="3883e-283">Android</span></span>](#tab/Android)

<span data-ttu-id="3883e-284">なし。</span><span class="sxs-lookup"><span data-stu-id="3883e-284">Not applicable.</span></span>

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="3883e-285">目的-C</span><span class="sxs-lookup"><span data-stu-id="3883e-285">Objective-C</span></span>](#tab/Objective-C)

<span data-ttu-id="3883e-286">なし。</span><span class="sxs-lookup"><span data-stu-id="3883e-286">Not applicable.</span></span>

# <a name="phptabphp"></a>[<span data-ttu-id="3883e-287">PHP</span><span class="sxs-lookup"><span data-stu-id="3883e-287">PHP</span></span>](#tab/PHP)

<span data-ttu-id="3883e-288">まだ使用できません。</span><span class="sxs-lookup"><span data-stu-id="3883e-288">Not yet available.</span></span> <span data-ttu-id="3883e-289">ユーザーにとって重要な場合は、 [Microsoft Graph の機能の要求](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests)に投票するか、開くようにしてください。</span><span class="sxs-lookup"><span data-stu-id="3883e-289">Please vote for or open a [Microsoft Graph feature request](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) if this is important to you.</span></span>

# <a name="rubytabruby"></a>[<span data-ttu-id="3883e-290">Ruby</span><span class="sxs-lookup"><span data-stu-id="3883e-290">Ruby</span></span>](#tab/Ruby)

<span data-ttu-id="3883e-291">まだ使用できません。</span><span class="sxs-lookup"><span data-stu-id="3883e-291">Not yet available.</span></span> <span data-ttu-id="3883e-292">ユーザーにとって重要な場合は、 [Microsoft Graph の機能の要求](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests)に投票するか、開くようにしてください。</span><span class="sxs-lookup"><span data-stu-id="3883e-292">Please vote for or open a [Microsoft Graph feature request](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) if this is important to you.</span></span>

---

## <a name="next-steps"></a><span data-ttu-id="3883e-293">次のステップ</span><span class="sxs-lookup"><span data-stu-id="3883e-293">Next steps</span></span>

* <span data-ttu-id="3883e-294">認証プロバイダーにはクライアント ID が必要です。</span><span class="sxs-lookup"><span data-stu-id="3883e-294">Authentication providers require an client ID.</span></span> <span data-ttu-id="3883e-295">認証プロバイダをセットアップした後に[、アプリケーションを登録](https://portal.azure.com/)する必要があります。</span><span class="sxs-lookup"><span data-stu-id="3883e-295">You'll want to [register your application](https://portal.azure.com/) after you set up your authentication provider.</span></span>
* <span data-ttu-id="3883e-296">必要な OAuth フローが現在サポートされていない場合は、 [Microsoft Graph の機能の要求](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests)に投票してください。</span><span class="sxs-lookup"><span data-stu-id="3883e-296">Let us know if a required OAuth flow isn't currently supported by voting for or opening a [Microsoft Graph feature request](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests).</span></span>
