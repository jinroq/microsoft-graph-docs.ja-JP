---
title: Microsoft Teams プロバイダ
description: Microsoft Teams タブの内部にある Teams プロバイダーを使用して、認証と Microsoft Graph のすべてのコンポーネントへのアクセスを容易にします。
localization_priority: Normal
author: nmetulev
ms.openlocfilehash: 348980225f04adfac4ded6f79a72654fbeec81e7
ms.sourcegitcommit: 750c82f161a0f62bc2486995456ccd92ee5c7831
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/26/2019
ms.locfileid: "35243045"
---
# <a name="microsoft-teams-provider"></a><span data-ttu-id="63bd5-103">Microsoft Teams プロバイダ</span><span class="sxs-lookup"><span data-stu-id="63bd5-103">Microsoft Teams provider</span></span>

<span data-ttu-id="63bd5-104">Microsoft Teams タブの内部にある Teams プロバイダーを使用して、認証と Microsoft Graph のすべてのコンポーネントへのアクセスを容易にします。</span><span class="sxs-lookup"><span data-stu-id="63bd5-104">Use the Teams provider inside your Microsoft Teams tab to facilitate authentication and Microsoft Graph access to all components.</span></span>

<span data-ttu-id="63bd5-105">詳細については、「 [providers](../providers.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="63bd5-105">To learn more, see [providers](../providers.md).</span></span>

## <a name="get-started"></a><span data-ttu-id="63bd5-106">作業の開始</span><span class="sxs-lookup"><span data-stu-id="63bd5-106">Get started</span></span>

<span data-ttu-id="63bd5-107">Teams プロバイダーを使用する前に、ページで[Microsoft TEAMS SDK](https://docs.microsoft.com/en-us/javascript/api/overview/msteams-client?view=msteams-client-js-latest#using-the-sdk)を参照していることを確認する必要があります。</span><span class="sxs-lookup"><span data-stu-id="63bd5-107">Before using the Teams provider, you will need to make sure you have referenced the [Microsoft Teams SDK](https://docs.microsoft.com/en-us/javascript/api/overview/msteams-client?view=msteams-client-js-latest#using-the-sdk) in your page.</span></span>

<span data-ttu-id="63bd5-108">次の例では、HTML (CDN 経由) でプロバイダーを使用します。</span><span class="sxs-lookup"><span data-stu-id="63bd5-108">The following example uses the provider in HTML (via CDN).</span></span>

```html
<!-- Microsoft Teams sdk must be referenced before the toolkit -->
<script src="https://unpkg.com/@microsoft/teams-js/dist/MicrosoftTeams.min.js" crossorigin="anonymous"></script>
<script src="https://unpkg.com/@microsoft/mgt/dist/bundle/mgt-loader.js"></script>

<mgt-teams-provider
  client-id="<YOUR_CLIENT_ID>"
  auth-popup-url="https://<YOUR-DOMAIN>.com/AUTH-PATH"
></mgt-teams-provider>
```

<span data-ttu-id="63bd5-109">次の例では、(NPM を介して) JS モジュールでプロバイダーを使用しています。</span><span class="sxs-lookup"><span data-stu-id="63bd5-109">The following example uses the provider in JS modules (via NPM).</span></span>

<span data-ttu-id="63bd5-110">ツールキットと Microsoft Teams SDK の両方がインストールされていることを確認してください。</span><span class="sxs-lookup"><span data-stu-id="63bd5-110">Make sure to install both the toolkit and the Microsoft Teams SDK.</span></span>

```bash
npm install @microsoft/mgt @microsoft/teams-js
```

<span data-ttu-id="63bd5-111">次に、プロバイダーをインポートして使用します。</span><span class="sxs-lookup"><span data-stu-id="63bd5-111">Next, import and use the provider.</span></span>

```ts
import '@microsoft/teams-js';
import {Providers, TeamsProvider} from '@microsoft/mgt'; 
Providers.globalProvider = new TeamsProvider(config);
```

<span data-ttu-id="63bd5-112">where `config`は</span><span class="sxs-lookup"><span data-stu-id="63bd5-112">where `config` is</span></span>

```ts
export interface TeamsConfig {
  clientId: string;
  authPopupUrl: string;
  scopes?: string[];
  msalOptions?: Configuration;
}
```

<span data-ttu-id="63bd5-113">完全な例については、「 [Microsoft Teams タブのサンプル](https://github.com/microsoftgraph/microsoft-graph-toolkit/tree/master/samples/teams-tab)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="63bd5-113">For a complete example, see [Microsoft Teams tab sample](https://github.com/microsoftgraph/microsoft-graph-toolkit/tree/master/samples/teams-tab).</span></span>

## <a name="configure-your-teams-app"></a><span data-ttu-id="63bd5-114">Teams アプリを構成する</span><span class="sxs-lookup"><span data-stu-id="63bd5-114">Configure your Teams app</span></span>

<span data-ttu-id="63bd5-115">Teams アプリの使用を開始するだけの場合は、「 [Microsoft teams アプリにタブを追加する](https://docs.microsoft.com/en-us/microsoftteams/platform/concepts/tabs/tabs-overview)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="63bd5-115">If you're just getting started with Teams apps, see [Add tabs to Microsoft Teams apps](https://docs.microsoft.com/en-us/microsoftteams/platform/concepts/tabs/tabs-overview).</span></span> <span data-ttu-id="63bd5-116">アプリ[Studio](https://docs.microsoft.com/en-us/microsoftteams/platform/get-started/get-started-app-studio)を使用して、アプリマニフェストをすばやく開発することもできます。</span><span class="sxs-lookup"><span data-stu-id="63bd5-116">You can also use [App Studio](https://docs.microsoft.com/en-us/microsoftteams/platform/get-started/get-started-app-studio) to quickly develop your app manifest.</span></span>

<span data-ttu-id="63bd5-117">タブを使用してアプリをインストールした後、コンポーネントを使用する準備ができたら、アプリが Microsoft Graph にアクセスするための適切なアクセス許可を持っていることを確認する必要があります。</span><span class="sxs-lookup"><span data-stu-id="63bd5-117">After you install your app with a tab, and you're ready to use the components, you need to make sure that your app has the right permissions to access Microsoft Graph.</span></span> <span data-ttu-id="63bd5-118">必要なアクセス許可を使用してアプリを構成するには、次のようにします。</span><span class="sxs-lookup"><span data-stu-id="63bd5-118">To configure your app with the necessary permissions:</span></span>

1. [<span data-ttu-id="63bd5-119">ドメイン名を取得する</span><span class="sxs-lookup"><span data-stu-id="63bd5-119">Retrieve your domain name</span></span>](https://docs.microsoft.com/en-us/azure/active-directory/identity-protection/graph-get-started#retrieve-your-domain-name)
2. [<span data-ttu-id="63bd5-120">新しいアプリの登録を作成する</span><span class="sxs-lookup"><span data-stu-id="63bd5-120">Create a new app registration</span></span>](https://docs.microsoft.com/en-us/azure/active-directory/identity-protection/graph-get-started#create-a-new-app-registration)
3. [<span data-ttu-id="63bd5-121">アプリケーションのアクセス許可を付与する</span><span class="sxs-lookup"><span data-stu-id="63bd5-121">Grant your application permission</span></span>](https://docs.microsoft.com/en-us/azure/active-directory/identity-protection/graph-get-started#grant-your-application-permission-to-use-the-api)

<span data-ttu-id="63bd5-122">[ **API へのアクセスの追加] ページ**に適切な権限を追加することが重要です。</span><span class="sxs-lookup"><span data-stu-id="63bd5-122">It's important to add the right permission on the **Add API access page**.</span></span> <span data-ttu-id="63bd5-123">必要なコンポーネントに応じて、管理者がアクセス許可を追加して承認する必要があります。</span><span class="sxs-lookup"><span data-stu-id="63bd5-123">You will need an administrator to add and approve the permissions, depending on which component you need.</span></span>

><span data-ttu-id="63bd5-124">**ヒント:** 追加するアクセス許可がわからない場合は、各コンポーネントのドキュメントを参照してください。</span><span class="sxs-lookup"><span data-stu-id="63bd5-124">**Tip:** If you're not sure what permissions to add, see the documentation for each component.</span></span>

### <a name="enable-implicit-grant-flow"></a><span data-ttu-id="63bd5-125">暗黙的な許可フローを有効にする</span><span class="sxs-lookup"><span data-stu-id="63bd5-125">Enable implicit grant Flow</span></span>

<span data-ttu-id="63bd5-126">暗黙的な許可フローを有効にしてください。これは、クライアント側からトークンを要求する web アプリの要件です。</span><span class="sxs-lookup"><span data-stu-id="63bd5-126">Make sure to enable implicit grant flow; this is a requirement for web apps that request tokens from the client side.</span></span> <span data-ttu-id="63bd5-127">Azure Portal では、アプリの登録を管理するときに、マニフェストを`oauth2AllowImplicitFlow`編集`true`してに変更します。</span><span class="sxs-lookup"><span data-stu-id="63bd5-127">In the Azure Portal, when managing your app registration, edit the manifest and change `oauth2AllowImplicitFlow` to `true`.</span></span>

### <a name="create-the-popup-page"></a><span data-ttu-id="63bd5-128">ポップアップページを作成する</span><span class="sxs-lookup"><span data-stu-id="63bd5-128">Create the popup page</span></span>

<span data-ttu-id="63bd5-129">Teams の資格情報を使用してサインインするには、Teams アプリがポップアップで開く URL を指定する必要があります。これは、認証フローに従います。</span><span class="sxs-lookup"><span data-stu-id="63bd5-129">In order to sign in with your Teams credentials, you need to provide a URL that the Teams app will open in a popup, which will follow the authentication flow.</span></span> <span data-ttu-id="63bd5-130">この URL は、ドメイン内に存在する必要があり、 `TeamsProvider.handleAuth();`メソッドを呼び出す必要があります。</span><span class="sxs-lookup"><span data-stu-id="63bd5-130">This URL needs to be in your domain, and it needs to call the `TeamsProvider.handleAuth();` method.</span></span> <span data-ttu-id="63bd5-131">このページで実行する必要があるのは、これだけです。</span><span class="sxs-lookup"><span data-stu-id="63bd5-131">That's the only thing that this page needs to do.</span></span> <span data-ttu-id="63bd5-132">次に例を示します。</span><span class="sxs-lookup"><span data-stu-id="63bd5-132">For example:</span></span>

```html
<script src="https://unpkg.com/@microsoft/teams-js/dist/MicrosoftTeams.min.js" crossorigin="anonymous"></script>
<script src="https://unpkg.com/@microsoft/mgt/dist/bundle/mgt-loader.js">

<script>        
  mgt.TeamsProvider.handleAuth();
</script>
```

### <a name="configure-redirect-uris"></a><span data-ttu-id="63bd5-133">リダイレクト Uri を構成する</span><span class="sxs-lookup"><span data-stu-id="63bd5-133">Configure redirect URIs</span></span>

<span data-ttu-id="63bd5-134">このページを web サイトに公開した後、 `auth-popup-url/authPopupUrl`プロパティで URL を使用する必要があります。</span><span class="sxs-lookup"><span data-stu-id="63bd5-134">After you publish this page on your website, you need to use the URL in the `auth-popup-url/authPopupUrl` property.</span></span> <span data-ttu-id="63bd5-135">この URL は、Azure AD ポータルのアプリ構成で有効なリダイレクト URI として構成する必要もあります。</span><span class="sxs-lookup"><span data-stu-id="63bd5-135">This URL also needs to be configured as a valid redirect URI in your app configuration in the Azure AD portal.</span></span>
