---
title: クラウド ソリューション プロバイダーのアプリケーションからの Microsoft Graph の呼び出し
description: このトピックは、パートナーが管理する顧客のアプリケーションへのアクセスを Microsoft Graph を介し、認証コードの許可のフローまたはサービス間クライアント資格情報フローにより許容する方法を説明します。
ms.openlocfilehash: a14c610090a1232c72ec2fde4469dd1cd1d6f694
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27092450"
---
# <a name="call-microsoft-graph-from-a-cloud-solution-provider-application"></a><span data-ttu-id="5b749-103">クラウド ソリューション プロバイダーのアプリケーションからの Microsoft Graph の呼び出し</span><span class="sxs-lookup"><span data-stu-id="5b749-103">Call Microsoft Graph from a Cloud Solution Provider application</span></span>

> <span data-ttu-id="5b749-p101">**注:** このトピックは Microsoft クラウド ソリューション プロバイダー (CSP) アプリケーション開発者**のみ**に適用されます。[Microsoft クラウド ソリューション プロバイダー (CSP)](https://partner.microsoft.com/ja-JP/cloud-solution-provider) プログラムは、マイクロソフトパートナーが Microsoft Online サービスを再販し、管理することを可能とします。</span><span class="sxs-lookup"><span data-stu-id="5b749-p101">**Note:** This topic applies **only** to Microsoft Cloud Solution Provider (CSP) application developers. The [Microsoft Cloud Solution Provider (CSP)](https://partner.microsoft.com/ja-JP/cloud-solution-provider) program enables Microsoft’s partners to resell and manage Microsoft Online services to customers.</span></span>

<span data-ttu-id="5b749-106">このトピックは、パートナーが管理する顧客のアプリケーションへのアクセスを Microsoft Graph を介し、[認証コードの許可のフロー](https://docs.microsoft.com/ja-JP/azure/active-directory/develop/active-directory-protocols-oauth-code)または[サービス間クライアント資格情報フロー](https://docs.microsoft.com/ja-JP/azure/active-directory/develop/active-directory-protocols-oauth-service-to-service)により許容する方法を説明します。</span><span class="sxs-lookup"><span data-stu-id="5b749-106">This topic describes how to enable application access to partner-managed customer data via Microsoft Graph using either the [authorization code grant flow](https://docs.microsoft.com/ja-JP/azure/active-directory/develop/active-directory-protocols-oauth-code) or the [service to service client credentials flow](https://docs.microsoft.com/ja-JP/azure/active-directory/develop/active-directory-protocols-oauth-service-to-service).</span></span>

<span data-ttu-id="5b749-107">**重要:** CSP アプリケーションからの Microsoft Graph の呼び出しは、ディレクトリ リソース (**user**、**group**、**device**、**organization** など) と [Intune](/graph/api/resources/intune-graph-overview?view=graph-rest-beta) リソースでのみサポートされています。</span><span class="sxs-lookup"><span data-stu-id="5b749-107">**Important:** Calling Microsoft Graph from a CSP application is only supported for directory resources (such as **user**, **group**,**device**, **organization**) and [Intune](/graph/api/resources/intune-graph-overview?view=graph-rest-beta) resources.</span></span>

## <a name="what-is-a-partner-managed-application"></a><span data-ttu-id="5b749-108">パートナー管理アプリケーションとは</span><span class="sxs-lookup"><span data-stu-id="5b749-108">What is a partner-managed application</span></span>

<span data-ttu-id="5b749-p102">CSP プログラムは、マイクロソフトパートナーが Microsoft Online サービス (Office 365、Microsoft Azure、CRM Online など) を再販し、管理することを可能とします。顧客サービスの管理は、特に任命されたパートナー ユーザー (エージェントといいます) にその顧客の環境をアクセスし、設定する権限を与える Delegated Admin 権限により行います。</span><span class="sxs-lookup"><span data-stu-id="5b749-p102">The CSP program enables Microsoft’s partners to resell and manage Microsoft Online Services (such as Office 365, Microsoft Azure, and CRM Online) to customers. Management of customer services is done through Delegated Admin Privileges, which enables designated partner users (known as agents) to access and configure their customers’ environments.</span></span>

<span data-ttu-id="5b749-p103">さらに、パートナー開発者は顧客の Microsoft サービスを管理する**パートナー管理アプリケーション**を作成できます。すべての顧客は自動的にパートナー管理アプリケーションを事前承認するため、パートナー管理アプリケーションは*事前承認*アプリケーションとも呼ばれます。つまり、顧客テナントのユーザーがパートナー管理アプリケーションを使用するには、同意のプロンプトは不要です。パートナー管理アプリケーションは Delegated Admin 権限を継承するため、パートナーエージェントもパートナー管理アプリケーションを介して顧客にアクセスする権限を持ちます。</span><span class="sxs-lookup"><span data-stu-id="5b749-p103">Additionally, as a partner developer, you can build a **partner-managed app** to manage your customers' Microsoft services. Partner-managed apps are often called *pre-consented* apps because all your customers are automatically pre-consented for your partner-managed apps. This means when a user from one of your customer tenants uses one of your partner-managed apps, the user can use it without being prompted to give consent. Partner-managed apps also inherit Delegated Admin Privileges, so your partner agents can also get privileged access to your customers through your partner-managed application.</span></span>

## <a name="how-to-set-up-a-partner-managed-application"></a><span data-ttu-id="5b749-115">パートナー管理アプリケーションのセットアップ方法</span><span class="sxs-lookup"><span data-stu-id="5b749-115">How to set-up a partner-managed application</span></span>

<span data-ttu-id="5b749-116">顧客のデータをアクセスする特権が付与された場合、アプリケーションは*パートナー管理*と表示されます。</span><span class="sxs-lookup"><span data-stu-id="5b749-116">An application is viewed as *partner-managed* when it is granted elevated permissions to access your customers' data.</span></span>

> <span data-ttu-id="5b749-117">**注:** パートナー管理アプリケーションはパートナーテナントに*のみ*設定でき、顧客テナントのリソースを管理するため、パートナー管理アプリケーションは**マルチ テナント アプリケーション**として**設定しなければなりません**。</span><span class="sxs-lookup"><span data-stu-id="5b749-117">**Note:** Partner-managed apps can *only* be configured on Partner tenants, and in order to manage customer tenant resources, partner-managed apps **must** be configured as **multi-tenant applications**.</span></span>

### <a name="register-and-configure-a-multi-tenant-app"></a><span data-ttu-id="5b749-118">マルチ テナント アプリケーションの登録と構成</span><span class="sxs-lookup"><span data-stu-id="5b749-118">Register and configure a multi-tenant app</span></span>

<span data-ttu-id="5b749-119">ここで必要な最初の手順は、他のマルチテナントのアプリケーションの登録と設定の手順とほぼ同じです。</span><span class="sxs-lookup"><span data-stu-id="5b749-119">The initial steps required here follow most of the same steps used to register and configure a multi-tenant application:</span></span>

1. <span data-ttu-id="5b749-p104">[Azure ポータル](https://portal.azure.com)を使い、パートナー テナントに[アプリケーションを登録します](https://docs.microsoft.com/ja-JP/azure/active-directory/active-directory-app-registration)。パートナー管理アプリケーションとして機能するよう、アプリケーションを [multi-tenant app](https://docs.microsoft.com/ja-JP/azure/active-directory/develop/active-directory-devhowto-multi-tenant-overview#update-registration-to-be-multi-tenant) として設定します。また、アプリが複数の地域で配布、販売される場合は、<a href="#region">ここ</a>で示すようにそれぞれの地域で登録する必要があります。</span><span class="sxs-lookup"><span data-stu-id="5b749-p104">[Register your application](https://docs.microsoft.com/ja-JP/azure/active-directory/active-directory-app-registration) in your Partner tenant using the [Azure Portal](https://portal.azure.com). To function as a partner-managed app, an application must be configured as a [multi-tenant app](https://docs.microsoft.com/ja-JP/azure/active-directory/develop/active-directory-devhowto-multi-tenant-overview#update-registration-to-be-multi-tenant). Additionally, if your app is deployed and sold in multiple geographic regions you will need to register your app in each of those regions as described <a href="#region">here</a>.</span></span>
2. <span data-ttu-id="5b749-123">再度 Azure ポータルから、最小限の特権のアプローチにより*必要となる権限*でマルチテナントのアプリケーションを設定します。</span><span class="sxs-lookup"><span data-stu-id="5b749-123">Configure your multi-tenant app, again through the Azure Portal, with the *required permissions* it needs using a least privileged approach.</span></span>

### <a name="pre-consent-your-app-for-all-your-customers"></a><span data-ttu-id="5b749-124">アプリをすべての顧客について事前同意します。</span><span class="sxs-lookup"><span data-stu-id="5b749-124">Pre-consent your app for all your customers</span></span>

<span data-ttu-id="5b749-p105">最後に、パートナー管理アプリケーションに設定した権限をすべての顧客に付与します。そのためには、Azure AD powershell V2 を使用して、アプリを示す **servicePrincipal** をパートナー テナントの *Adminagents* グループに追加します。Azure AD PowerShell V2 は、[ここ](https://www.powershellgallery.com/packages/AzureAD)からダウンロードし、インストールできます。*Adminagents* グループと **servicePrincipal** を検索し、これをグループに追加するには以下の手順に従います。</span><span class="sxs-lookup"><span data-stu-id="5b749-p105">Finally grant your partner-managed app those configured permissions for all your customers. You can do this by adding the **servicePrincipal** that represents the app to the *Adminagents* group in your Partner tenant, using Azure AD powershell V2. You can download and install Azure AD PowerShell V2 from [here](https://www.powershellgallery.com/packages/AzureAD).  Follow these steps to find the *Adminagents* group, the **servicePrincipal** and add it to the group.</span></span>

1. <span data-ttu-id="5b749-129">PowerShell セッションを開き、サインイン ウィンドウに、管理者資格情報を入力してパートナーのテナントに接続します。</span><span class="sxs-lookup"><span data-stu-id="5b749-129">Open a PowerShell session and connect to your partner tenant by entering your admin credentials into the sign-in window.</span></span>

    ```PowerShell
    Connect-AzureAd
    ```

2. <span data-ttu-id="5b749-130">*Adminagents* を表すグループを探します。</span><span class="sxs-lookup"><span data-stu-id="5b749-130">Find the group that represents the *Adminagents*.</span></span>

    ```PowerShell
    $group = Get-AzureADGroup -Filter "displayName eq 'Adminagents'"
    ```

3. <span data-ttu-id="5b749-131">使用しているアプリケーションと同じ *appId* を持つサービス プリンシパルを検索します。</span><span class="sxs-lookup"><span data-stu-id="5b749-131">Find the service principal that has the same *appId* as your app.</span></span>

    ```PowerShell
    $sp = Get-AzureADServicePrincipal -Filter "appId eq '{yourAppsAppId}'"
    ```

4. <span data-ttu-id="5b749-132">最後に、サービス プリンシパルを *Adminagents* グループに追加します。</span><span class="sxs-lookup"><span data-stu-id="5b749-132">Finally, add the service principal to the *Adminagents* group.</span></span>

    ```PowerShell
    Add-AzureADGroupMember -ObjectId $group.ObjectId -RefObjectId $sp.ObjectId
    ```

## <a name="token-acquisition-flows"></a><span data-ttu-id="5b749-133">トークン取得のフロー</span><span class="sxs-lookup"><span data-stu-id="5b749-133">Token acquisition flows</span></span>

<span data-ttu-id="5b749-134">パートナー管理アプリケーションのトークン取得フロー、つまり[認証コード付与のフロー](https://docs.microsoft.com/ja-JP/azure/active-directory/develop/active-directory-protocols-oauth-code)と[サービス間クライアント資格情報のフロー](https://docs.microsoft.com/ja-JP/azure/active-directory/develop/active-directory-protocols-oauth-service-to-service)は、普通のマルチテナントのアプリケーションと同じです。</span><span class="sxs-lookup"><span data-stu-id="5b749-134">Token acquisition flows for partner-managed apps - [authorization code grant flow](https://docs.microsoft.com/ja-JP/azure/active-directory/develop/active-directory-protocols-oauth-code) and [service-to-service client credentials flow](https://docs.microsoft.com/ja-JP/azure/active-directory/develop/active-directory-protocols-oauth-service-to-service) - are the same as regular multi-tenant apps.</span></span>

<span data-ttu-id="5b749-p106">すべての顧客テナントへの事前承認済みアクセス以外に、パートナー管理アプリケーションにはもうひとつの機能があります。それは、エージェントがアプリケーションを使って顧客テナントのデータへアクセスできるようにする機能です (delegated admin 権限を使って)。概念的には次のように動作します。</span><span class="sxs-lookup"><span data-stu-id="5b749-p106">Apart from pre-consented access to all your customer tenants, partner-managed apps have one additional capability. It allows for your agents to use your app to access your customers' tenant data (using delegated admin privileges). Conceptually it works like this:</span></span>

1. <span data-ttu-id="5b749-138">エージェントは、パートナー テナントが発行したエージェント自身のユーザー資格情報を使ってアプリケーションにサインインします。</span><span class="sxs-lookup"><span data-stu-id="5b749-138">Your agent signs in to your app with their user credentials issued from your partner tenant.</span></span>
2. <span data-ttu-id="5b749-139">アプリケーションは目的となるパートナー管理顧客テナントへのアクセス トークンを要求します。</span><span class="sxs-lookup"><span data-stu-id="5b749-139">Your app requests an access token for the intended partner-managed customer tenant.</span></span>
3. <span data-ttu-id="5b749-140">アプリはアクセス トークンを使用して、Microsoft Graph を呼び出します。</span><span class="sxs-lookup"><span data-stu-id="5b749-140">Your app uses the access token to call Microsoft Graph.</span></span>

<span data-ttu-id="5b749-p107">これは、標準的な[認証コード付与のフロー](https://docs.microsoft.com/ja-JP/azure/active-directory/develop/active-directory-protocols-oauth-code)ですが、エージェントがパートナーのアカウントを使用してサインインする必要がある点が異なります。わかりやすくするため、パートナーテナントを *partner.com* (エージェントのホーム テナント) とし、顧客を *customer.com* とします。</span><span class="sxs-lookup"><span data-stu-id="5b749-p107">This is a standard [authorization code grant flow](https://docs.microsoft.com/ja-JP/azure/active-directory/develop/active-directory-protocols-oauth-code), except that your agents must sign-in using their partner accounts. To see how this would look, imagine your partner tenant is *partner.com* (which is the home tenant for your agents) and one of your customers is *customer.com*:</span></span>

1. <span data-ttu-id="5b749-p108">[認証コードを取得する](https://docs.microsoft.com/ja-JP/azure/active-directory/develop/active-directory-protocols-oauth-code#request-an-authorization-code)アプリケーションは ```/authorize``` エンドポイントに要求を送信します。ターゲット テナントとして**顧客テナント** (この例では ```customer.com```) を指定しなくてはなりません。エージェントは、引き続き自分の ```username@partner.com``` アカウントでサインインします。</span><span class="sxs-lookup"><span data-stu-id="5b749-p108">[Acquire an authorization code:](https://docs.microsoft.com/ja-JP/azure/active-directory/develop/active-directory-protocols-oauth-code#request-an-authorization-code) Your app makes a request to the ```/authorize``` endpoint and must use a **customer tenant**, in our example ```customer.com```, for the target tenant. Your agents would still sign-in with their ```username@partner.com``` account.</span></span>

    ```http
    GET https://login.microsoftonline.com/customer.com/oauth2/authorize
    ```

2. <span data-ttu-id="5b749-145">[承認コードを使用してアクセス トークンを取得する](https://docs.microsoft.com/ja-JP/azure/active-directory/develop/active-directory-protocols-oauth-code#use-the-authorization-code-to-request-an-access-token)アプリケーションは、```token``` エンドポイントに要求を送る際、ターゲット テナントを**顧客テナント** (この例では ```customer.com```) とする必要があります。</span><span class="sxs-lookup"><span data-stu-id="5b749-145">[Aquire an access token using the authorization code:](https://docs.microsoft.com/ja-JP/azure/active-directory/develop/active-directory-protocols-oauth-code#use-the-authorization-code-to-request-an-access-token) Your app must use a **customer tenant** as the target tenant, in our example ```customer.com```, when making the request to the ```token``` endpoint:</span></span>

    ```http
    POST https://login.microsoftonline.com/customer.com/oauth2/token
    ```

3. <span data-ttu-id="5b749-146">トークンへのアクセスができたら、HTTP 認証ヘッダーにトークンを入れて Microsoft Graph を呼び出します。</span><span class="sxs-lookup"><span data-stu-id="5b749-146">Now you have an access token, call Microsoft Graph, putting the access token in the HTTP authorization header:</span></span>

    ```http
    GET https://graph.microsoft.com/beta/users
    Authorization: Bearer <token>
    ```

## <a name="register-your-app-in-the-regions-you-support"></a><span data-ttu-id="5b749-147">サポートする地域でのアプリケーションの登録</span><span class="sxs-lookup"><span data-stu-id="5b749-147">Register your app in the regions you support</span></span>
<a name="region"></a>

<span data-ttu-id="5b749-p109">今のところ、CSP 顧客契約は 1 つの地域に限定されています。パートナー管理アプリケーションには、いくつかの制限があります。つまり、販売を展開する地域ごとにテナントを用意する必要があります。たとえば、パートナー管理アプリケーションを米国のテナントに登録し、顧客は EU に在住している場合は、パートナー管理アプリケーションは機能しません。同一地域の顧客を管理するには、各地域パートナーのテナントは、各自の一連のパートナー管理アプリケーションを維持する必要があります。これにより、アプリケーションに顧客のサインイン名を取得し、地域専用のどのパートナー管理アプリケーションを使用するか決定するための (サインイン前の) ロジックを追加する必要が生じることがあります。</span><span class="sxs-lookup"><span data-stu-id="5b749-p109">CSP customer engagement is currently limited to a single region. Partner-managed applications carry the same limitation. This means you must have a separate tenant for each region you sell in. For example, if your partner-managed app is registered in a tenant in the US but your customer is in the EU – the partner-managed app will not work.  Each of your regional partner tenants must maintain their own set of partner-managed apps to manage customers within the same region. This might require additional logic in your app (prior to sign-in) to get your customers' sign-in username to decide which region-specific partner-managed app identity to use, to serve the user.</span></span>

## <a name="calling-microsoft-graph-immediately-after-customer-creation"></a><span data-ttu-id="5b749-154">顧客作成後すぐに Microsoft Graph を呼び出す</span><span class="sxs-lookup"><span data-stu-id="5b749-154">Calling Microsoft Graph immediately after customer creation</span></span>

<span data-ttu-id="5b749-p110">[Partner Center API](https://partnercenter.microsoft.com/ja-JP/partner/developer) を使用して新しい顧客を作成すると、新しい顧客テナントも作成されます。さらに、パートナーの関連付けが行われ、この新しい顧客テナントとレコードのパートナーとしての関連付けが行われます。このパートナー関係が新しい顧客テナントに反映されるには最長 3 分かかることがあります。作成後すぐにアプリケーションが直接に Microsoft Graph を呼び出すと、アクセス拒否エラーを受け取ることがあります。既存の顧客が招待を受け付けると、これと同じ遅延が発生することがあります。このため、事前承認は顧客テナントに存在しているパートナー関係に依存します。</span><span class="sxs-lookup"><span data-stu-id="5b749-p110">When you create a new customer using the [Partner Center API](https://partnercenter.microsoft.com/ja-JP/partner/developer), a new customer tenant gets created. Additionally, a partner relationship also gets created, which makes you the partner of record for this new customer tenant. This partner relationship can take up to 3 minutes to propagate to the new customer tenant. If your app calls Microsoft Graph straight after creation, your app will likely receive an access denied error. A similar delay may be experienced when an existing customer accepts your invitation. This is because pre-consent relies on the partner relationship being present in the customer tenant.</span></span>

<span data-ttu-id="5b749-p111">この問題を回避するには、顧客の作成後、パートナーアプリケーションは (Microsoft Graph 呼び出しのための) トークン取得のために Azure AD を呼び出す前に **3 分間**待機することを推奨します。ほとんどの場合がこれで解決します。3 分待機しても認証エラーが発生する場合は、さらに 60 秒間待機してからもう一度お試しください。</span><span class="sxs-lookup"><span data-stu-id="5b749-p111">To avoid this problem, we recommend that your partner app should should wait **three minutes** after customer creation before calling Azure AD to acquire a token (to call Microsoft Graph). This should cover most cases. However, if after waiting three minutes you still recieve an authorization error, please wait an additional 60 seconds and try again.</span></span>

> <span data-ttu-id="5b749-p112">**注:** 再試行のためには、Microsoft Graph を呼び出す前に Azure  AD から新しいアクセス トークンを取得する必要があります。既存のアクセストークンを使用して Microsoft Graph を呼び出すことはできません。アクセス トークンは 1 時間のみ有効で、事前承認の要求が含まれないためです。</span><span class="sxs-lookup"><span data-stu-id="5b749-p112">**Note:** On the retry, you must acquire a new access token from Azure AD, before calling Microsoft Graph.  Calling Microsoft Graph with the access token you already have will not work, because the access token is good for an hour and won’t contain the pre-consented permission claims.</span></span>
