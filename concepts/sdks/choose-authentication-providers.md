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
# <a name="choose-a-microsoft-graph-authentication-provider-based-on-oauth-flow"></a><span data-ttu-id="6738d-103">OAuth フローに基づいて Microsoft Graph 認証プロバイダを選択する</span><span class="sxs-lookup"><span data-stu-id="6738d-103">Choose a Microsoft Graph authentication provider based on OAuth flow</span></span>

<span data-ttu-id="6738d-104">認証プロバイダーは、認証クライアントライブラリに必要なパラメーターを抽象化することで、アクセストークンの取得を簡素化します。</span><span class="sxs-lookup"><span data-stu-id="6738d-104">Authentication providers simplify getting an access token by abstracting the parameters required by the authentication client libraries.</span></span> <span data-ttu-id="6738d-105">Microsoft Graph 認証プロバイダーは、各プラットフォームのアダプターを提供することにより、Microsoft Authentication Library (MSAL) の使用を簡素化します。</span><span class="sxs-lookup"><span data-stu-id="6738d-105">The Microsoft Graph authentication providers simplify the use of the Microsoft Authentication Library (MSAL) by providing adapters for each platform.</span></span> <span data-ttu-id="6738d-106">これらのアダプターは、アプリケーションのトークンの取得を処理します。</span><span class="sxs-lookup"><span data-stu-id="6738d-106">These adapters handle token acquisition for your application.</span></span> <span data-ttu-id="6738d-107">Microsoft Graph 認証プロバイダーは、OAuth 付与フローにマップされます。</span><span class="sxs-lookup"><span data-stu-id="6738d-107">The Microsoft Graph authentication providers map to an OAuth grant flow.</span></span> <span data-ttu-id="6738d-108">アプリケーションに対して適切な認証プロバイダーを選択するために、アプリケーションに対してどの OAuth 付与フローを使用するかを把握する必要があります。</span><span class="sxs-lookup"><span data-stu-id="6738d-108">You'll need to know which OAuth grant flow to use for your application in order to select the appropriate authentication provider for your application.</span></span>

## <a name="authorization-code-oauth-flow"></a><span data-ttu-id="6738d-109">認証コード OAuth フロー</span><span class="sxs-lookup"><span data-stu-id="6738d-109">Authorization code OAuth flow</span></span>

<span data-ttu-id="6738d-110">認証コードフローにより、ネイティブおよび web アプリはユーザーの名前でトークンを安全に取得することができます。</span><span class="sxs-lookup"><span data-stu-id="6738d-110">The authorization code flow enables native and web apps to securely obtain tokens in the name of the user.</span></span> <span data-ttu-id="6738d-111">詳細については、「 [Microsoft identity platform And OAuth 2.0 認証コードフロー](https://docs.microsoft.com/en-us/azure/active-directory/develop/v2-oauth2-auth-code-flow)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="6738d-111">To learn more, see [Microsoft identity platform and OAuth 2.0 authorization code flow](https://docs.microsoft.com/en-us/azure/active-directory/develop/v2-oauth2-auth-code-flow).</span></span>

# <a name="ctabcs"></a>[<span data-ttu-id="6738d-112">Visual</span><span class="sxs-lookup"><span data-stu-id="6738d-112">C#</span></span>](#tab/CS)

```csharp
IConfidentialClientApplication clientApplication = AuthorizationCodeProvider.CreateClientApplication(clientId, redirectUri, clientCredential);
AuthorizationCodeProvider authProvider = new AuthorizationCodeProvider(clientApplication, scopes);
```

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="6738d-113">Java</span><span class="sxs-lookup"><span data-stu-id="6738d-113">Javascript</span></span>](#tab/Javascript)

<span data-ttu-id="6738d-114">認証コード、クライアント資格情報、および非代行の OAuth フローでは、この時点でカスタム認証プロバイダーを実装する必要があります。</span><span class="sxs-lookup"><span data-stu-id="6738d-114">Authorization code, client credential, and on-behalf-of OAuth flows require that you implement a custom authentication provider at this time.</span></span> <span data-ttu-id="6738d-115">詳細については、「 [Using a custom authentication provider](https://github.com/microsoftgraph/msgraph-sdk-javascript/blob/dev/docs/CustomAuthenticationProvider.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="6738d-115">For more information, see [Using a custom authentication provider](https://github.com/microsoftgraph/msgraph-sdk-javascript/blob/dev/docs/CustomAuthenticationProvider.md).</span></span>

# <a name="javatabjava"></a>[<span data-ttu-id="6738d-116">Java</span><span class="sxs-lookup"><span data-stu-id="6738d-116">Java</span></span>](#tab/Java)

```java
AuthorizationCodeProvider authProvider = new AuthorizationCodeProvider(
                                                    clientId,
                                                    scopes,
                                                    authorizationCode,
                                                    redirectUri,
                                                    clientSecret);
```

# <a name="androidtabandroid"></a>[<span data-ttu-id="6738d-117">Android</span><span class="sxs-lookup"><span data-stu-id="6738d-117">Android</span></span>](#tab/Android)

<span data-ttu-id="6738d-118">なし。</span><span class="sxs-lookup"><span data-stu-id="6738d-118">Not applicable.</span></span>

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="6738d-119">目的-C</span><span class="sxs-lookup"><span data-stu-id="6738d-119">Objective-C</span></span>](#tab/Objective-C)

<span data-ttu-id="6738d-120">なし。</span><span class="sxs-lookup"><span data-stu-id="6738d-120">Not applicable.</span></span>

# <a name="phptabphp"></a>[<span data-ttu-id="6738d-121">PHP</span><span class="sxs-lookup"><span data-stu-id="6738d-121">PHP</span></span>](#tab/PHP)

<span data-ttu-id="6738d-122">まだ使用できません。</span><span class="sxs-lookup"><span data-stu-id="6738d-122">Not yet available.</span></span> <span data-ttu-id="6738d-123">ユーザーにとって重要な場合は、 [Microsoft Graph の機能の要求](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests)をサポートするか、または開きます。</span><span class="sxs-lookup"><span data-stu-id="6738d-123">Please support or open a [Microsoft Graph feature request](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) if this is important to you.</span></span>

# <a name="rubytabruby"></a>[<span data-ttu-id="6738d-124">Ruby</span><span class="sxs-lookup"><span data-stu-id="6738d-124">Ruby</span></span>](#tab/Ruby)

<span data-ttu-id="6738d-125">まだ利用できません。</span><span class="sxs-lookup"><span data-stu-id="6738d-125">Not available, yet.</span></span> <span data-ttu-id="6738d-126">ユーザーにとって重要な場合は、 [Microsoft Graph の機能の要求](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests)に投票するか、開くようにしてください。</span><span class="sxs-lookup"><span data-stu-id="6738d-126">Please vote for or open a [Microsoft Graph feature request](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) if this is important to you.</span></span>

---

## <a name="client-credential-oauth-flow"></a><span data-ttu-id="6738d-127">クライアント資格情報 OAuth フロー</span><span class="sxs-lookup"><span data-stu-id="6738d-127">Client credential OAuth flow</span></span>

<span data-ttu-id="6738d-128">クライアント資格情報フローを使用すると、ユーザーによる操作なしでサービスアプリケーションを実行できます。</span><span class="sxs-lookup"><span data-stu-id="6738d-128">The client credential flow enables service applications to run without user interaction.</span></span> <span data-ttu-id="6738d-129">Access は、アプリケーションの id に基づいています。</span><span class="sxs-lookup"><span data-stu-id="6738d-129">Access is based on the identity of the application.</span></span> <span data-ttu-id="6738d-130">詳細については、「 [Microsoft identity platform」および「OAuth 2.0 クライアント資格情報フロー](https://docs.microsoft.com/en-us/azure/active-directory/develop/v2-oauth2-client-creds-grant-flow)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="6738d-130">For more information, see [Microsoft identity platform and the OAuth 2.0 client credentials flow](https://docs.microsoft.com/en-us/azure/active-directory/develop/v2-oauth2-client-creds-grant-flow).</span></span>

# <a name="ctabcs"></a>[<span data-ttu-id="6738d-131">Visual</span><span class="sxs-lookup"><span data-stu-id="6738d-131">C#</span></span>](#tab/CS)

```csharp
IConfidentialClientApplication clientApplication = ClientCredentialProvider.CreateClientApplication(clientId, clientCredential);
ClientCredentialProvider authProvider = new ClientCredentialProvider(clientApplication);
```

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="6738d-132">Java</span><span class="sxs-lookup"><span data-stu-id="6738d-132">Javascript</span></span>](#tab/Javascript)

<span data-ttu-id="6738d-133">認証コード、クライアント資格情報、および非代行の OAuth フローでは、この時点でカスタム認証プロバイダーを実装する必要があります。</span><span class="sxs-lookup"><span data-stu-id="6738d-133">Authorization code, client credential, and on-behalf-of OAuth flows require that you implement a custom authentication provider at this time.</span></span> <span data-ttu-id="6738d-134">詳細については、「 [Using a custom authentication provider](https://github.com/microsoftgraph/msgraph-sdk-javascript/blob/dev/docs/CustomAuthenticationProvider.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="6738d-134">For more information, see [Using a custom authentication provider](https://github.com/microsoftgraph/msgraph-sdk-javascript/blob/dev/docs/CustomAuthenticationProvider.md).</span></span>

# <a name="javatabjava"></a>[<span data-ttu-id="6738d-135">Java</span><span class="sxs-lookup"><span data-stu-id="6738d-135">Java</span></span>](#tab/Java)

```java
ClientCredentialProvider authProvider = new ClientCredentialProvider(
                                                    clientId,
                                                    scopes,
                                                    clientSecret,
                                                    tenant,
                                                    endpoint);
```

# <a name="androidtabandroid"></a>[<span data-ttu-id="6738d-136">Android</span><span class="sxs-lookup"><span data-stu-id="6738d-136">Android</span></span>](#tab/Android)

<span data-ttu-id="6738d-137">なし。</span><span class="sxs-lookup"><span data-stu-id="6738d-137">Not applicable.</span></span>

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="6738d-138">目的-C</span><span class="sxs-lookup"><span data-stu-id="6738d-138">Objective-C</span></span>](#tab/Objective-C)

<span data-ttu-id="6738d-139">なし。</span><span class="sxs-lookup"><span data-stu-id="6738d-139">Not applicable.</span></span>

# <a name="phptabphp"></a>[<span data-ttu-id="6738d-140">PHP</span><span class="sxs-lookup"><span data-stu-id="6738d-140">PHP</span></span>](#tab/PHP)

<span data-ttu-id="6738d-141">まだ利用できません。</span><span class="sxs-lookup"><span data-stu-id="6738d-141">Not available, yet.</span></span> <span data-ttu-id="6738d-142">ユーザーにとって重要な場合は、 [Microsoft Graph の機能の要求](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests)をサポートするか、または開きます。</span><span class="sxs-lookup"><span data-stu-id="6738d-142">Please support or open a [Microsoft Graph feature request](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) if this is important to you.</span></span>

# <a name="rubytabruby"></a>[<span data-ttu-id="6738d-143">Ruby</span><span class="sxs-lookup"><span data-stu-id="6738d-143">Ruby</span></span>](#tab/Ruby)

<span data-ttu-id="6738d-144">まだ利用できません。</span><span class="sxs-lookup"><span data-stu-id="6738d-144">Not available, yet.</span></span> <span data-ttu-id="6738d-145">ユーザーにとって重要な場合は、 [Microsoft Graph の機能の要求](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests)をサポートするか、または開きます。</span><span class="sxs-lookup"><span data-stu-id="6738d-145">Please support or open a [Microsoft Graph feature request](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) if this is important to you.</span></span>

---

## <a name="on-behalf-of-oauth-flow"></a><span data-ttu-id="6738d-146">非代行の OAuth フロー</span><span class="sxs-lookup"><span data-stu-id="6738d-146">On-behalf-of OAuth flow</span></span>

<span data-ttu-id="6738d-147">アプリケーションが Microsoft Graph API を呼び出すサービスまたは web API を呼び出すときに、その代わりの流れが適用されます。</span><span class="sxs-lookup"><span data-stu-id="6738d-147">The on-behalf-of flow is applicable when your application calls a service/web API which in turns calls the Microsoft Graph API.</span></span> <span data-ttu-id="6738d-148">[Microsoft identity platform および OAuth 2.0 の送信フローの](https://docs.microsoft.com/en-us/azure/active-directory/develop/v2-oauth2-on-behalf-of-flow)詳細については、こちらを参照してください。</span><span class="sxs-lookup"><span data-stu-id="6738d-148">Learn more by reading [Microsoft identity platform and OAuth 2.0 On-Behalf-Of flow](https://docs.microsoft.com/en-us/azure/active-directory/develop/v2-oauth2-on-behalf-of-flow)</span></span>

# <a name="ctabcs"></a>[<span data-ttu-id="6738d-149">Visual</span><span class="sxs-lookup"><span data-stu-id="6738d-149">C#</span></span>](#tab/CS)

```csharp
IConfidentialClientApplication clientApplication = OnBehalfOfProvider.CreateClientApplication(clientId, redirectUri, clientCredential);
OnBehalfOfProvider authProvider = new OnBehalfOfProvider(clientApplication, scopes);
```

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="6738d-150">Java</span><span class="sxs-lookup"><span data-stu-id="6738d-150">Javascript</span></span>](#tab/Javascript)

<span data-ttu-id="6738d-151">認証コード、クライアント資格情報、および非代行の OAuth フローでは、この時点でカスタム認証プロバイダーを実装する必要があります。</span><span class="sxs-lookup"><span data-stu-id="6738d-151">Authorization code, client credential, and on-behalf-of OAuth flows require that you implement a custom authentication provider at this time.</span></span> <span data-ttu-id="6738d-152">詳細については、「[カスタム認証プロバイダを使用する](https://github.com/microsoftgraph/msgraph-sdk-javascript/blob/dev/docs/CustomAuthenticationProvider.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="6738d-152">Read [Using Custom Authentication Provider](https://github.com/microsoftgraph/msgraph-sdk-javascript/blob/dev/docs/CustomAuthenticationProvider.md) for more information.</span></span>

# <a name="javatabjava"></a>[<span data-ttu-id="6738d-153">Java</span><span class="sxs-lookup"><span data-stu-id="6738d-153">Java</span></span>](#tab/Java)

<span data-ttu-id="6738d-154">まだ使用できません。</span><span class="sxs-lookup"><span data-stu-id="6738d-154">Not yet available.</span></span> <span data-ttu-id="6738d-155">ユーザーにとって重要な場合は、 [Microsoft Graph の機能の要求](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests)に投票するか、開くようにしてください。</span><span class="sxs-lookup"><span data-stu-id="6738d-155">Please vote for or open a [Microsoft Graph feature request](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) if this is important to you.</span></span>

# <a name="androidtabandroid"></a>[<span data-ttu-id="6738d-156">Android</span><span class="sxs-lookup"><span data-stu-id="6738d-156">Android</span></span>](#tab/Android)

<span data-ttu-id="6738d-157">なし。</span><span class="sxs-lookup"><span data-stu-id="6738d-157">Not applicable.</span></span>

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="6738d-158">目的-C</span><span class="sxs-lookup"><span data-stu-id="6738d-158">Objective-C</span></span>](#tab/Objective-C)

<span data-ttu-id="6738d-159">なし。</span><span class="sxs-lookup"><span data-stu-id="6738d-159">Not applicable.</span></span>

# <a name="phptabphp"></a>[<span data-ttu-id="6738d-160">PHP</span><span class="sxs-lookup"><span data-stu-id="6738d-160">PHP</span></span>](#tab/PHP)

<span data-ttu-id="6738d-161">まだ使用できません。</span><span class="sxs-lookup"><span data-stu-id="6738d-161">Not yet available.</span></span> <span data-ttu-id="6738d-162">ユーザーにとって重要な場合は、 [Microsoft Graph の機能の要求](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests)に投票するか、開くようにしてください。</span><span class="sxs-lookup"><span data-stu-id="6738d-162">Please vote for or open a [Microsoft Graph feature request](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) if this is important to you.</span></span>

# <a name="rubytabruby"></a>[<span data-ttu-id="6738d-163">Ruby</span><span class="sxs-lookup"><span data-stu-id="6738d-163">Ruby</span></span>](#tab/Ruby)

<span data-ttu-id="6738d-164">まだ使用できません。</span><span class="sxs-lookup"><span data-stu-id="6738d-164">Not yet available.</span></span> <span data-ttu-id="6738d-165">ユーザーにとって重要な場合は、 [Microsoft Graph の機能の要求](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests)に投票するか、開くようにしてください。</span><span class="sxs-lookup"><span data-stu-id="6738d-165">Please vote for or open a [Microsoft Graph feature request](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) if this is important to you.</span></span>

---

## <a name="implicit-grant-oauth-flow"></a><span data-ttu-id="6738d-166">暗黙的付与 OAuth フロー</span><span class="sxs-lookup"><span data-stu-id="6738d-166">Implicit grant OAuth flow</span></span>

<span data-ttu-id="6738d-167">暗黙的な付与フローは、ブラウザーベースのアプリケーションで使用されます。</span><span class="sxs-lookup"><span data-stu-id="6738d-167">The implicit grant flow is used in browser-based applications.</span></span> <span data-ttu-id="6738d-168">詳細については、「 [Microsoft identity platform」および「暗黙的な許可の流れ](https://docs.microsoft.com/en-us/azure/active-directory/develop/v2-oauth2-implicit-grant-flow)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="6738d-168">For more information, see [Microsoft identity platform and Implicit grant flow](https://docs.microsoft.com/en-us/azure/active-directory/develop/v2-oauth2-implicit-grant-flow).</span></span>

# <a name="ctabcs"></a>[<span data-ttu-id="6738d-169">Visual</span><span class="sxs-lookup"><span data-stu-id="6738d-169">C#</span></span>](#tab/CS)

<span data-ttu-id="6738d-170">なし。</span><span class="sxs-lookup"><span data-stu-id="6738d-170">Not applicable.</span></span>

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="6738d-171">Java</span><span class="sxs-lookup"><span data-stu-id="6738d-171">Javascript</span></span>](#tab/Javascript)

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

# <a name="javatabjava"></a>[<span data-ttu-id="6738d-172">Java</span><span class="sxs-lookup"><span data-stu-id="6738d-172">Java</span></span>](#tab/Java)

<span data-ttu-id="6738d-173">なし。</span><span class="sxs-lookup"><span data-stu-id="6738d-173">Not applicable.</span></span>

# <a name="androidtabandroid"></a>[<span data-ttu-id="6738d-174">Android</span><span class="sxs-lookup"><span data-stu-id="6738d-174">Android</span></span>](#tab/Android)

<span data-ttu-id="6738d-175">なし。</span><span class="sxs-lookup"><span data-stu-id="6738d-175">Not applicable.</span></span>

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="6738d-176">目的-C</span><span class="sxs-lookup"><span data-stu-id="6738d-176">Objective-C</span></span>](#tab/Objective-C)

<span data-ttu-id="6738d-177">なし。</span><span class="sxs-lookup"><span data-stu-id="6738d-177">Not applicable.</span></span>

# <a name="phptabphp"></a>[<span data-ttu-id="6738d-178">PHP</span><span class="sxs-lookup"><span data-stu-id="6738d-178">PHP</span></span>](#tab/PHP)

<span data-ttu-id="6738d-179">なし。</span><span class="sxs-lookup"><span data-stu-id="6738d-179">Not applicable.</span></span>

# <a name="rubytabruby"></a>[<span data-ttu-id="6738d-180">Ruby</span><span class="sxs-lookup"><span data-stu-id="6738d-180">Ruby</span></span>](#tab/Ruby)

<span data-ttu-id="6738d-181">なし。</span><span class="sxs-lookup"><span data-stu-id="6738d-181">Not applicable.</span></span>

---

## <a name="device-code-oauth-flow"></a><span data-ttu-id="6738d-182">デバイスコード OAuth フロー</span><span class="sxs-lookup"><span data-stu-id="6738d-182">Device code OAuth flow</span></span>

<span data-ttu-id="6738d-183">デバイスコードフローによって、別のデバイスを使用してデバイスにサインインできるようになります。</span><span class="sxs-lookup"><span data-stu-id="6738d-183">The device code flow enables sign in to devices by way of another device.</span></span> <span data-ttu-id="6738d-184">詳細については、「 [Microsoft identity platform」および「OAuth 2.0 デバイスコードフロー](https://docs.microsoft.com/en-us/azure/active-directory/develop/v2-oauth2-device-code)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="6738d-184">For details, see [Microsoft identity platform and the OAuth 2.0 device code flow](https://docs.microsoft.com/en-us/azure/active-directory/develop/v2-oauth2-device-code).</span></span>

# <a name="ctabcs"></a>[<span data-ttu-id="6738d-185">Visual</span><span class="sxs-lookup"><span data-stu-id="6738d-185">C#</span></span>](#tab/CS)

```csharp
IPublicClientApplication clientApplication = DeviceCodeProvider.CreateClientApplication(clientId);
DeviceCodeProvider authProvider = new DeviceCodeProvider(clientApplication, scopes);
```

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="6738d-186">Java</span><span class="sxs-lookup"><span data-stu-id="6738d-186">Javascript</span></span>](#tab/Javascript)

<span data-ttu-id="6738d-187">まだ使用できません。</span><span class="sxs-lookup"><span data-stu-id="6738d-187">Not yet available.</span></span> <span data-ttu-id="6738d-188">ユーザーにとって重要な場合は、 [Microsoft Graph の機能の要求](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests)に投票するか、開くようにしてください。</span><span class="sxs-lookup"><span data-stu-id="6738d-188">Please vote for or open a [Microsoft Graph feature request](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) if this is important to you.</span></span>

# <a name="javatabjava"></a>[<span data-ttu-id="6738d-189">Java</span><span class="sxs-lookup"><span data-stu-id="6738d-189">Java</span></span>](#tab/Java)

<span data-ttu-id="6738d-190">まだ利用できません。</span><span class="sxs-lookup"><span data-stu-id="6738d-190">Not available, yet.</span></span> <span data-ttu-id="6738d-191">ユーザーにとって重要な場合は、 [Microsoft Graph の機能の要求](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests)をサポートするか、または開きます。</span><span class="sxs-lookup"><span data-stu-id="6738d-191">Please support or open a [Microsoft Graph feature request](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) if this is important to you.</span></span>

# <a name="androidtabandroid"></a>[<span data-ttu-id="6738d-192">Android</span><span class="sxs-lookup"><span data-stu-id="6738d-192">Android</span></span>](#tab/Android)

<span data-ttu-id="6738d-193">なし。</span><span class="sxs-lookup"><span data-stu-id="6738d-193">Not applicable.</span></span>

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="6738d-194">目的-C</span><span class="sxs-lookup"><span data-stu-id="6738d-194">Objective-C</span></span>](#tab/Objective-C)

<span data-ttu-id="6738d-195">なし。</span><span class="sxs-lookup"><span data-stu-id="6738d-195">Not applicable.</span></span>

# <a name="phptabphp"></a>[<span data-ttu-id="6738d-196">PHP</span><span class="sxs-lookup"><span data-stu-id="6738d-196">PHP</span></span>](#tab/PHP)

<span data-ttu-id="6738d-197">まだ使用できません。</span><span class="sxs-lookup"><span data-stu-id="6738d-197">Not yet available.</span></span> <span data-ttu-id="6738d-198">ユーザーにとって重要な場合は、 [Microsoft Graph の機能の要求](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests)に投票するか、開くようにしてください。</span><span class="sxs-lookup"><span data-stu-id="6738d-198">Please vote for or open a [Microsoft Graph feature request](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) if this is important to you.</span></span>

# <a name="rubytabruby"></a>[<span data-ttu-id="6738d-199">Ruby</span><span class="sxs-lookup"><span data-stu-id="6738d-199">Ruby</span></span>](#tab/Ruby)

<span data-ttu-id="6738d-200">まだ使用できません。</span><span class="sxs-lookup"><span data-stu-id="6738d-200">Not yet available.</span></span> <span data-ttu-id="6738d-201">ユーザーにとって重要な場合は、 [Microsoft Graph の機能の要求](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests)に投票するか、開くようにしてください。</span><span class="sxs-lookup"><span data-stu-id="6738d-201">Please vote for or open a [Microsoft Graph feature request](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) if this is important to you.</span></span>

---

## <a name="integrated-windows-flow"></a><span data-ttu-id="6738d-202">統合 Windows フロー</span><span class="sxs-lookup"><span data-stu-id="6738d-202">Integrated Windows flow</span></span>

<span data-ttu-id="6738d-203">統合 Windows フローにより、Windows コンピューターがドメインに参加している場合に、アクセストークンをサイレントに取得することができます。</span><span class="sxs-lookup"><span data-stu-id="6738d-203">The integrated Windows flow provides a way for Windows computers to silently acquire an access token when they are domain joined.</span></span> <span data-ttu-id="6738d-204">詳細については、「[統合 Windows 認証](https://github.com/AzureAD/microsoft-authentication-library-for-dotnet/wiki/Integrated-Windows-Authentication)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="6738d-204">For details, see [Integrated Windows authentication](https://github.com/AzureAD/microsoft-authentication-library-for-dotnet/wiki/Integrated-Windows-Authentication).</span></span>

# <a name="ctabcs"></a>[<span data-ttu-id="6738d-205">Visual</span><span class="sxs-lookup"><span data-stu-id="6738d-205">C#</span></span>](#tab/CS)

```csharp
IPublicClientApplication clientApplication = IntegratedWindowsAuthenticationProvider.CreateClientApplication(clientId);
IntegratedWindowsAuthenticationProvider authProvider = new IntegratedWindowsAuthenticationProvider(clientApplication, scopes);
```

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="6738d-206">Java</span><span class="sxs-lookup"><span data-stu-id="6738d-206">Javascript</span></span>](#tab/Javascript)

<span data-ttu-id="6738d-207">なし。</span><span class="sxs-lookup"><span data-stu-id="6738d-207">Not applicable.</span></span>

# <a name="javatabjava"></a>[<span data-ttu-id="6738d-208">Java</span><span class="sxs-lookup"><span data-stu-id="6738d-208">Java</span></span>](#tab/Java)

<span data-ttu-id="6738d-209">なし。</span><span class="sxs-lookup"><span data-stu-id="6738d-209">Not applicable.</span></span>

# <a name="androidtabandroid"></a>[<span data-ttu-id="6738d-210">Android</span><span class="sxs-lookup"><span data-stu-id="6738d-210">Android</span></span>](#tab/Android)

<span data-ttu-id="6738d-211">なし。</span><span class="sxs-lookup"><span data-stu-id="6738d-211">Not applicable.</span></span>

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="6738d-212">目的-C</span><span class="sxs-lookup"><span data-stu-id="6738d-212">Objective-C</span></span>](#tab/Objective-C)

<span data-ttu-id="6738d-213">なし。</span><span class="sxs-lookup"><span data-stu-id="6738d-213">Not applicable.</span></span>

# <a name="phptabphp"></a>[<span data-ttu-id="6738d-214">PHP</span><span class="sxs-lookup"><span data-stu-id="6738d-214">PHP</span></span>](#tab/PHP)

<span data-ttu-id="6738d-215">なし。</span><span class="sxs-lookup"><span data-stu-id="6738d-215">Not applicable.</span></span>

# <a name="rubytabruby"></a>[<span data-ttu-id="6738d-216">Ruby</span><span class="sxs-lookup"><span data-stu-id="6738d-216">Ruby</span></span>](#tab/Ruby)

<span data-ttu-id="6738d-217">なし。</span><span class="sxs-lookup"><span data-stu-id="6738d-217">Not applicable.</span></span>

---

## <a name="interactive-flow"></a><span data-ttu-id="6738d-218">対話型フロー</span><span class="sxs-lookup"><span data-stu-id="6738d-218">Interactive flow</span></span>

<span data-ttu-id="6738d-219">対話型フローは、モバイルアプリケーション (Xamarin および UWP) およびデスクトップアプリケーションがユーザーの名前で Microsoft Graph を呼び出すために使用されます。</span><span class="sxs-lookup"><span data-stu-id="6738d-219">The interactive flow is used by mobile applications (Xamarin and UWP) and desktops applications to call Microsoft Graph in the name of a user.</span></span> <span data-ttu-id="6738d-220">詳細については、「[トークンを対話的に取得](https://github.com/AzureAD/microsoft-authentication-library-for-dotnet/wiki/Acquiring-tokens-interactively)する」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="6738d-220">For details, see [Acquiring tokens interactively](https://github.com/AzureAD/microsoft-authentication-library-for-dotnet/wiki/Acquiring-tokens-interactively).</span></span>

# <a name="ctabcs"></a>[<span data-ttu-id="6738d-221">Visual</span><span class="sxs-lookup"><span data-stu-id="6738d-221">C#</span></span>](#tab/CS)

```csharp
IPublicClientApplication clientApplication = InteractiveAuthenticationProvider.CreateClientApplication(clientId);
InteractiveAuthenticationProvider authProvider = new InteractiveAuthenticationProvider(clientApplication, scopes);
```

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="6738d-222">Java</span><span class="sxs-lookup"><span data-stu-id="6738d-222">Javascript</span></span>](#tab/Javascript)

<span data-ttu-id="6738d-223">まだ使用できません。</span><span class="sxs-lookup"><span data-stu-id="6738d-223">Not yet available.</span></span> <span data-ttu-id="6738d-224">ユーザーにとって重要な場合は、 [Microsoft Graph の機能の要求](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests)に投票するか、開くようにしてください。</span><span class="sxs-lookup"><span data-stu-id="6738d-224">Please vote for or open a [Microsoft Graph feature request](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) if this is important to you.</span></span>

# <a name="javatabjava"></a>[<span data-ttu-id="6738d-225">Java</span><span class="sxs-lookup"><span data-stu-id="6738d-225">Java</span></span>](#tab/Java)

<span data-ttu-id="6738d-226">まだ使用できません。</span><span class="sxs-lookup"><span data-stu-id="6738d-226">Not yet available.</span></span> <span data-ttu-id="6738d-227">ユーザーにとって重要な場合は、 [Microsoft Graph の機能の要求](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests)に投票するか、開くようにしてください。</span><span class="sxs-lookup"><span data-stu-id="6738d-227">Please vote for or open a [Microsoft Graph feature request](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) if this is important to you.</span></span>

# <a name="androidtabandroid"></a>[<span data-ttu-id="6738d-228">Android</span><span class="sxs-lookup"><span data-stu-id="6738d-228">Android</span></span>](#tab/Android)

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

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="6738d-229">目的-C</span><span class="sxs-lookup"><span data-stu-id="6738d-229">Objective-C</span></span>](#tab/Objective-C)

```objc
NSError *error = nil;
MSALPublicClientApplication *publicClientApplication = [[MSALPublicClientApplication alloc] initWithClientId:@"INSERT-CLIENT-APP-ID" 
error:&error];

MSALAuthenticationProviderOptions *authProviderOptions= [[MSALAuthenticationProviderOptions alloc] initWithScopes:<array-of-scopes-for-which-you-need-access-token>];

 MSALAuthenticationProvider *authenticationProvider = [[MSALAuthenticationProvider alloc] initWithPublicClientApplication:publicClientApplication 
 andOptions:authProviderOptions];
```

# <a name="phptabphp"></a>[<span data-ttu-id="6738d-230">PHP</span><span class="sxs-lookup"><span data-stu-id="6738d-230">PHP</span></span>](#tab/PHP)

<span data-ttu-id="6738d-231">なし。</span><span class="sxs-lookup"><span data-stu-id="6738d-231">Not applicable.</span></span>

# <a name="rubytabruby"></a>[<span data-ttu-id="6738d-232">Ruby</span><span class="sxs-lookup"><span data-stu-id="6738d-232">Ruby</span></span>](#tab/Ruby)

<span data-ttu-id="6738d-233">なし。</span><span class="sxs-lookup"><span data-stu-id="6738d-233">Not applicable.</span></span>

---

## <a name="resource-owner-password-credential-grant-oauth-flow"></a><span data-ttu-id="6738d-234">リソース所有者のパスワード資格情報に OAuth フローを付与する</span><span class="sxs-lookup"><span data-stu-id="6738d-234">Resource owner password credential grant OAuth flow</span></span>

<span data-ttu-id="6738d-235">リソース所有者のパスワード資格情報のフローによって、アプリケーションはユーザー名とパスワードを使用してユーザーにサインインすることができます。</span><span class="sxs-lookup"><span data-stu-id="6738d-235">The resource owner password credential flow allows an application to sign in a user by using their username and password.</span></span> <span data-ttu-id="6738d-236">このフローは、他の OAuth フローを使用できない場合にのみ使用してください。</span><span class="sxs-lookup"><span data-stu-id="6738d-236">Use this flow only when you cannot use any of the other OAuth flows.</span></span> <span data-ttu-id="6738d-237">詳細については、「 [Microsoft identity platform」および「OAuth 2.0 resource owner password credential](https://docs.microsoft.com/en-us/azure/active-directory/develop/v2-oauth-ropc) 」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="6738d-237">For more information, see [Microsoft identity platform and the OAuth 2.0 resource owner password credential](https://docs.microsoft.com/en-us/azure/active-directory/develop/v2-oauth-ropc)</span></span>



# <a name="ctabcs"></a>[<span data-ttu-id="6738d-238">Visual</span><span class="sxs-lookup"><span data-stu-id="6738d-238">C#</span></span>](#tab/CS)

```csharp
IPublicClientApplication clientApplication = UsernamePasswordProvider.CreateClientApplication(clientId);
UsernamePasswordProvider authProvider = new UsernamePasswordProvider(clientApplication, scopes);
```

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="6738d-239">Java</span><span class="sxs-lookup"><span data-stu-id="6738d-239">Javascript</span></span>](#tab/Javascript)

<span data-ttu-id="6738d-240">まだ使用できません。</span><span class="sxs-lookup"><span data-stu-id="6738d-240">Not yet available.</span></span> <span data-ttu-id="6738d-241">ユーザーにとって重要な場合は、 [Microsoft Graph の機能の要求](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests)に投票するか、開くようにしてください。</span><span class="sxs-lookup"><span data-stu-id="6738d-241">Please vote for or open a [Microsoft Graph feature request](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) if this is important to you.</span></span>

# <a name="javatabjava"></a>[<span data-ttu-id="6738d-242">Java</span><span class="sxs-lookup"><span data-stu-id="6738d-242">Java</span></span>](#tab/Java)

```java
UsernamePasswordProvider authProvider = new UsernamePasswordProvider(
                                                    clientId,
                                                    scopes,
                                                    username,
                                                    password);
```

# <a name="androidtabandroid"></a>[<span data-ttu-id="6738d-243">Android</span><span class="sxs-lookup"><span data-stu-id="6738d-243">Android</span></span>](#tab/Android)

<span data-ttu-id="6738d-244">なし。</span><span class="sxs-lookup"><span data-stu-id="6738d-244">Not applicable.</span></span>

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="6738d-245">目的-C</span><span class="sxs-lookup"><span data-stu-id="6738d-245">Objective-C</span></span>](#tab/Objective-C)

<span data-ttu-id="6738d-246">なし。</span><span class="sxs-lookup"><span data-stu-id="6738d-246">Not applicable.</span></span>

# <a name="phptabphp"></a>[<span data-ttu-id="6738d-247">PHP</span><span class="sxs-lookup"><span data-stu-id="6738d-247">PHP</span></span>](#tab/PHP)

<span data-ttu-id="6738d-248">まだ使用できません。</span><span class="sxs-lookup"><span data-stu-id="6738d-248">Not yet available.</span></span> <span data-ttu-id="6738d-249">ユーザーにとって重要な場合は、 [Microsoft Graph の機能の要求](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests)に投票するか、開くようにしてください。</span><span class="sxs-lookup"><span data-stu-id="6738d-249">Please vote for or open a [Microsoft Graph feature request](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) if this is important to you.</span></span>

# <a name="rubytabruby"></a>[<span data-ttu-id="6738d-250">Ruby</span><span class="sxs-lookup"><span data-stu-id="6738d-250">Ruby</span></span>](#tab/Ruby)

<span data-ttu-id="6738d-251">まだ使用できません。</span><span class="sxs-lookup"><span data-stu-id="6738d-251">Not yet available.</span></span> <span data-ttu-id="6738d-252">ユーザーにとって重要な場合は、 [Microsoft Graph の機能の要求](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests)に投票するか、開くようにしてください。</span><span class="sxs-lookup"><span data-stu-id="6738d-252">Please vote for or open a [Microsoft Graph feature request](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests) if this is important to you.</span></span>

---

## <a name="next-steps"></a><span data-ttu-id="6738d-253">次の手順</span><span class="sxs-lookup"><span data-stu-id="6738d-253">Next steps</span></span>

* <span data-ttu-id="6738d-254">認証プロバイダーにはクライアント ID が必要です。</span><span class="sxs-lookup"><span data-stu-id="6738d-254">Authentication providers require an client ID.</span></span> <span data-ttu-id="6738d-255">認証プロバイダをセットアップした後に[、アプリケーションを登録](https://portal.azure.com/)する必要があります。</span><span class="sxs-lookup"><span data-stu-id="6738d-255">You'll want to [register your application](https://portal.azure.com/) after you set up your authentication provider.</span></span>
* <span data-ttu-id="6738d-256">必要な OAuth フローが現在サポートされていない場合は、 [Microsoft Graph の機能の要求](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests)に投票してください。</span><span class="sxs-lookup"><span data-stu-id="6738d-256">Let us know if a required OAuth flow isn't currently supported by voting for or opening a [Microsoft Graph feature request](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests).</span></span>