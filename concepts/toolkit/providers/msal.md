---
title: MSAL プロバイダ
description: MSAL のプロバイダーは MSAL を使用してユーザーにサインインし、トークンを取得して Microsoft Graph で使用します。
localization_priority: Normal
author: nmetulev
ms.openlocfilehash: b66fd9a640c6baa84767e1ab08821b80384a5464
ms.sourcegitcommit: 750c82f161a0f62bc2486995456ccd92ee5c7831
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/26/2019
ms.locfileid: "35243049"
---
# <a name="msal-provider"></a><span data-ttu-id="632fc-103">MSAL プロバイダ</span><span class="sxs-lookup"><span data-stu-id="632fc-103">MSAL provider</span></span>

<span data-ttu-id="632fc-104">MSAL プロバイダーは、 [msal .js](https://github.com/AzureAD/microsoft-authentication-library-for-js)を使用してユーザーにサインインし、Microsoft Graph で使用するトークンを取得します。</span><span class="sxs-lookup"><span data-stu-id="632fc-104">The MSAL Provider uses [MSAL.js](https://github.com/AzureAD/microsoft-authentication-library-for-js) to sign in users and acquire tokens to use with the Microsoft Graph.</span></span>

<span data-ttu-id="632fc-105">詳細については、「 [providers](../providers.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="632fc-105">To learn more, see [providers](../providers.md).</span></span>

## <a name="get-started"></a><span data-ttu-id="632fc-106">作業の開始</span><span class="sxs-lookup"><span data-stu-id="632fc-106">Get started</span></span>

<span data-ttu-id="632fc-107">MSAL プロバイダーは、HTML または JavaScript で初期化できます。</span><span class="sxs-lookup"><span data-stu-id="632fc-107">You can initialize the MSAL provider in HTML or JavaScript.</span></span>

### <a name="initialize-in-your-html-page"></a><span data-ttu-id="632fc-108">HTML ページでの初期化</span><span class="sxs-lookup"><span data-stu-id="632fc-108">Initialize in your HTML page</span></span>

<span data-ttu-id="632fc-109">新しいプロバイダーを作成する最も簡単な方法は、HTML で MSAL プロバイダーを初期化することです。</span><span class="sxs-lookup"><span data-stu-id="632fc-109">Initializing the MSAL provider in HTML is the simplest way to create a new provider.</span></span> <span data-ttu-id="632fc-110">`mgt-msal-provider`コンポーネントを使用して、**クライアント id**とその他のプロパティを設定します。</span><span class="sxs-lookup"><span data-stu-id="632fc-110">Use the `mgt-msal-provider` component to set the **client-id** and other properties.</span></span> <span data-ttu-id="632fc-111">これにより、すべて`UserAgentApplication`の認証とトークンの取得で使用される新しいインスタンスが作成されます。</span><span class="sxs-lookup"><span data-stu-id="632fc-111">This will create a new `UserAgentApplication` instance that will be used for all authentication and acquiring tokens.</span></span>

```html
<mgt-msal-provider client-id="<YOUR_CLIENT_ID>"
                   login-type="redirect/popup"
                   authority=""></mgt-msal-provider>
```

><span data-ttu-id="632fc-112">**注:**`login-type` `authority`</span><span class="sxs-lookup"><span data-stu-id="632fc-112">**Note:** `login-type` and `authority` are optional.</span></span>

### <a name="initialize-in-javascript"></a><span data-ttu-id="632fc-113">JavaScript での初期化</span><span class="sxs-lookup"><span data-stu-id="632fc-113">Initialize in JavaScript</span></span>

<span data-ttu-id="632fc-114">JavaScript でプロバイダーを初期化することで、より多くのオプションを提供できます。</span><span class="sxs-lookup"><span data-stu-id="632fc-114">You can provide more options by initializing the provider in JavaScript.</span></span>

```ts
import {Providers, MsalProvider} from '@microsoft/mgt'
import {UserAgentApplication} from "msal";

Providers.globalProvider = new MsalProvider(config: MsalConfig);
```

<span data-ttu-id="632fc-115">MsalConfig は次のとおりです。</span><span class="sxs-lookup"><span data-stu-id="632fc-115">where MsalConfig is:</span></span>

```ts
interface MsalConfig {
  clientId: string;
  scopes?: string[];
  authority?: string;
  loginType?: LoginType;
  options?: Configuration; // msal js Configuration object
}
```

<span data-ttu-id="632fc-116">を`clientId`指定する必要があります (新しい`UserAgentApplication`を作成する場合)。</span><span class="sxs-lookup"><span data-stu-id="632fc-116">You must provide a `clientId` (to create a new `UserAgentApplication`).</span></span>

<span data-ttu-id="632fc-117">詳細については、 [Msal のドキュメント](https://github.com/AzureAD/microsoft-authentication-library-for-js/wiki/MSAL-basics)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="632fc-117">To learn more, see the [MSAL documentation](https://github.com/AzureAD/microsoft-authentication-library-for-js/wiki/MSAL-basics).</span></span>

## <a name="creating-an-appclient-id"></a><span data-ttu-id="632fc-118">アプリ/クライアント ID の作成</span><span class="sxs-lookup"><span data-stu-id="632fc-118">Creating an app/client ID</span></span>

<span data-ttu-id="632fc-119">アプリを登録し、クライアント ID を取得する方法の詳細については、「[アプリのクイックスタートを登録](https://docs.microsoft.com/en-us/azure/active-directory/develop/quickstart-register-app)する」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="632fc-119">For details about how to register an app and get a client ID, see the [Register an app quick start](https://docs.microsoft.com/en-us/azure/active-directory/develop/quickstart-register-app).</span></span>

><span data-ttu-id="632fc-120">**注:** MSAL では、OAuth の暗黙的フローのみがサポートされています。</span><span class="sxs-lookup"><span data-stu-id="632fc-120">**Note:** MSAL only supports the Implicit Flow for OAuth.</span></span> <span data-ttu-id="632fc-121">Azure Portal でアプリケーションの暗黙的フローを有効にしてください (既定では有効になっていません)。</span><span class="sxs-lookup"><span data-stu-id="632fc-121">Make sure to enable Implicit Flow in your application in the Azure Portal (it is not enabled by default).</span></span> <span data-ttu-id="632fc-122">[**認証**] で、[**暗黙的な付与**] セクションを見つけて、**アクセストークン**と**ID トークン**のチェックボックスをオンにします。</span><span class="sxs-lookup"><span data-stu-id="632fc-122">Under **Authentication**, find the **Implicit grant** section and select the checkboxes for **Access tokens** and **ID tokens**.</span></span>
