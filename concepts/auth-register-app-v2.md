---
title: アプリを Azure AD v2.0 エンドポイントに登録する
description: アプリは、Azure AD に登録する必要があります。 アプリを登録すると、トークンの取得のための Azure AD での認証でアプリケーションが使用する一意のアプリケーション ID と他の値が確定します。
author: jackson-woods
localization_priority: Priority
ms.prod: microsoft-identity-platform
ms.openlocfilehash: d62fb12c094307fcd09f3e4600046b818ec4bbaa
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32521909"
---
# <a name="register-your-app-with-the-azure-ad-v20-endpoint"></a><span data-ttu-id="697e5-104">アプリを Azure AD v2.0 エンドポイントに登録する</span><span class="sxs-lookup"><span data-stu-id="697e5-104">Register your app with the Azure AD v2.0 endpoint</span></span>

<span data-ttu-id="697e5-p102">アプリは、Azure AD に登録する必要があります。アプリを登録すると、トークンの取得のための Azure AD での認証でアプリケーションが使用する一意のアプリケーション ID と他の値が確定します。Azure AD v2.0 エンドポイントの場合は、[Microsoft アプリ登録ポータル](https://apps.dev.microsoft.com)でアプリを登録します。アプリを登録するには、Microsoft アカウントのほか、職場または学校のアカウントを使用できます。開発するアプリケーションの種類によっては、アプリケーションの認証と承認の設定で 1 つまたは複数のプロパティをコピーする必要があります。</span><span class="sxs-lookup"><span data-stu-id="697e5-p102">Your app must be registered with Azure AD. Registering your app establishes a unique application ID and other values that your app uses to authenticate with Azure AD and get tokens. For the Azure AD v2.0 endpoint, you register your app with the [Microsoft App Registration Portal](https://apps.dev.microsoft.com). You can use either a Microsoft account or a work or school account to register your app. Depending on the type of app you are developing, you will need to copy one or more properties during registration to use when you configure authentication and authorization for your app.</span></span> 


> <span data-ttu-id="697e5-p103">**注:** この記事では、主にアプリケーションの Azure AD v2.0 のエンドポイントへの登録ついて説明します。Azure AD のエンドポイントへのアプリケーションの登録に関する詳細は「[Azure AD エンドポイントについて考慮すべき事項](#azure-ad-endpoint-considerations)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="697e5-p103">**Note:** This article primarily covers registering apps with the Azure AD v2.0 endpoint. For information about registering your app with the Azure AD endpoint, see [Azure AD endpoint considerations](#azure-ad-endpoint-considerations) below.</span></span>
> 
> <span data-ttu-id="697e5-112">あらかじめ Microsoft Azure ポータルに登録済みのアプリはアプリ登録ポータルには表示されないため、ご注意ください。</span><span class="sxs-lookup"><span data-stu-id="697e5-112">Also, be aware that if you've previously registered apps in the Microsoft Azure portal, those apps will not be listed in the App Registration Portal.</span></span> <span data-ttu-id="697e5-113">それらのアプリは Azure ポータルで管理します。</span><span class="sxs-lookup"><span data-stu-id="697e5-113">Manage those apps in the Azure portal.</span></span> 


<span data-ttu-id="697e5-p105">次のスクリーンショットは、パスワードと暗黙的フローを使用して構成された Web アプリの登録の例を示しています。![パスワードと暗黙的許可による Web アプリの登録。](./images/v2-web-registration.png)</span><span class="sxs-lookup"><span data-stu-id="697e5-p105">The following screenshot shows an example web app registration that has been configured with a password and implicit flow. ![Web app registration with password and implicit grant.](./images/v2-web-registration.png)</span></span>

<span data-ttu-id="697e5-116">アプリを登録するには、以下の手順に従います。アプリの承認を設定するときには、指定された値をコピーして使用してください。</span><span class="sxs-lookup"><span data-stu-id="697e5-116">To register your app, follow these steps; be sure to copy the indicated values to use when configuring authorization for your app:</span></span>

1. <span data-ttu-id="697e5-117">[Microsoft アプリ登録ポータル](https://apps.dev.microsoft.com/)にサインインします。</span><span class="sxs-lookup"><span data-stu-id="697e5-117">Sign into the [Microsoft App Registration Portal](https://apps.dev.microsoft.com/).</span></span>
   
    <span data-ttu-id="697e5-118">Microsoft アカウントのほか、職場または学校のアカウントを使用してサインインできます。</span><span class="sxs-lookup"><span data-stu-id="697e5-118">You can sign in with either a Microsoft account or a work or school account.</span></span> 

2. <span data-ttu-id="697e5-119">**[アプリの追加]** を選択します。</span><span class="sxs-lookup"><span data-stu-id="697e5-119">Choose **Add an app**.</span></span>
    > <span data-ttu-id="697e5-120">注:職場または学校のアカウントを使用してサインインした場合は、署名する場合は、**統合アプリケーション**の **[アプリの追加]** ボタンを選択します。</span><span class="sxs-lookup"><span data-stu-id="697e5-120">Note: If you signed in with a work or school account, select the **Add an app** button for **Converged applications**.</span></span> 

3. <span data-ttu-id="697e5-121">アプリの名前を入力して、**[アプリケーションの作成]** を選択します。</span><span class="sxs-lookup"><span data-stu-id="697e5-121">Enter a name for the app and choose **Create application**.</span></span>

    <span data-ttu-id="697e5-122">登録ページが表示され、アプリのプロパティが一覧表示されます。</span><span class="sxs-lookup"><span data-stu-id="697e5-122">The registration page displays, listing the properties of your app.</span></span>

4. <span data-ttu-id="697e5-p106">アプリケーション ID をコピーします。これは、アプリの一意識別子です。</span><span class="sxs-lookup"><span data-stu-id="697e5-p106">Copy the application ID. This is the unique identifier for your app.</span></span>

    <span data-ttu-id="697e5-125">アプリを構成するには、アプリケーション ID を使用します。</span><span class="sxs-lookup"><span data-stu-id="697e5-125">You'll use the application ID to configure the app.</span></span>

5. <span data-ttu-id="697e5-126">**[プラットフォーム]** で、**[プラットフォームの追加]** を選び、アプリに適したプラットフォームを選びます。</span><span class="sxs-lookup"><span data-stu-id="697e5-126">Under **Platforms**, choose **Add Platform**, and select the appropriate platform for your app:</span></span>
    
    <span data-ttu-id="697e5-127">**ネイティブまたはモバイル アプリケーションでは**</span><span class="sxs-lookup"><span data-stu-id="697e5-127">**For native or mobile apps**:</span></span>

    1. <span data-ttu-id="697e5-128">**[ネイティブ アプリケーション]** を選択します。</span><span class="sxs-lookup"><span data-stu-id="697e5-128">Select **Native Application**.</span></span>

    2. <span data-ttu-id="697e5-p107">**[組み込みリダイレクト URI]** の値をコピーします。このアプリを構成するため、後でこの値が必要になります。</span><span class="sxs-lookup"><span data-stu-id="697e5-p107">Copy the **Built-in redirect URI** value. You'll need this to configure your app.</span></span>

        <span data-ttu-id="697e5-131">リダイレクト URI は、アプリケーションに提供される一意の URI であり、その URI に送信されたメッセージはそのアプリケーションだけに送信されます。</span><span class="sxs-lookup"><span data-stu-id="697e5-131">The redirect URI is a unique URI provided for your application to ensure that messages sent to that URI are only sent to that application.</span></span> 

    <span data-ttu-id="697e5-132">**Web アプリの場合**:</span><span class="sxs-lookup"><span data-stu-id="697e5-132">**For web apps**:</span></span>

    1. <span data-ttu-id="697e5-133">**[Web]** を選びます。</span><span class="sxs-lookup"><span data-stu-id="697e5-133">Select **Web**.</span></span>

    2. <span data-ttu-id="697e5-134">使用している認証フローの種類によっては、**[暗黙的フローを許可する]** チェック ボックスが選択されていることを確認する必要があります。</span><span class="sxs-lookup"><span data-stu-id="697e5-134">Depending on the type of authentication flow you're using, you may have to make sure the **Allow Implicit Flow** check box is selected.</span></span> 
        
        <span data-ttu-id="697e5-p108">**[暗黙的フローを許可する]** オプションにより、OpenID Connect ハイブリッド フローと暗黙的フローが有効になります。ハイブリッド フローにより、アプリはサインイン情報 (ID トークン) と成果物 (この場合は認証コード) の両方を受け取れるようになり、アプリはアクセス トークンを取得するときにこれらを使用できます。ハイブリッド フローは、OWIN OpenID Connect ミドルウェアが使用する既定のフローです。シングル ページ アプリ (SPA) では、アプリは暗黙的フローにより、サインイン情報とアクセス トークンを受け取ることができます。</span><span class="sxs-lookup"><span data-stu-id="697e5-p108">The **Allow Implicit Flow** option enables the OpenID Connect hybrid and implicit flows. The hybrid flow enables the app to receive both sign-in info (the id token) and artifacts (in this case, an authorization code) that the app uses to obtain an access token. The hybrid flow is the default flow used by the OWIN OpenID Connect middleware. For single page apps (SPA), the implicit flow enables the app to receive sign-in info and the access token.</span></span> 

    3. <span data-ttu-id="697e5-139">リダイレクト URL を指定します。</span><span class="sxs-lookup"><span data-stu-id="697e5-139">Specify a Redirect URL.</span></span>
        
        <span data-ttu-id="697e5-140">リダイレクト URL は、Azure AD v2.0 エンドポイントが認証要求処理を完了した際に呼び出す、アプリ内の場所です。</span><span class="sxs-lookup"><span data-stu-id="697e5-140">The redirect URL is the location in your app that the Azure AD v2.0 endpoint calls when it has processed the authentication request.</span></span>

    4. <span data-ttu-id="697e5-p109">**[アプリケーション シークレット]** で、**[新しいパスワードを生成する]** を選びます。**[新しいパスワードが生成されました]** ダイアログ ボックスからアプリケーション シークレットをコピーします。</span><span class="sxs-lookup"><span data-stu-id="697e5-p109">Under **Application Secrets**, choose **Generate New Password**. Copy the app secret from the **New password generated** dialog box.</span></span>
        > <span data-ttu-id="697e5-p110">**重要**:**[新しいパスワードが生成されました]** ダイアログを閉じる前に、アプリケーションの機密情報をコピーする必要があります。ダイアログ ボックスを閉じた後は、機密情報は取得できません。</span><span class="sxs-lookup"><span data-stu-id="697e5-p110">**Important** You must copy the app secret before you close the **New password generated** dialog. After you close the dialog, you cannot retrieve the secret.</span></span> 
            
6. <span data-ttu-id="697e5-145">**[保存]** を選択します。</span><span class="sxs-lookup"><span data-stu-id="697e5-145">Choose **Save**.</span></span>


<span data-ttu-id="697e5-p111">以下の表に、さまざまな種類のアプリケーションの設定とコピーに必要となるプロパティを示します。_割り当て済み_とは、Azure AD で割り当てられた値を使用する必要があることを示します。</span><span class="sxs-lookup"><span data-stu-id="697e5-p111">The following table shows the properties that you need to configure and copy for different kinds of apps. _Assigned_ means that you should use the value assigned by Azure AD.</span></span>


| <span data-ttu-id="697e5-148">アプリの種類</span><span class="sxs-lookup"><span data-stu-id="697e5-148">App type</span></span> | <span data-ttu-id="697e5-149">プラットフォーム</span><span class="sxs-lookup"><span data-stu-id="697e5-149">Platform</span></span> | <span data-ttu-id="697e5-150">アプリケーション ID</span><span class="sxs-lookup"><span data-stu-id="697e5-150">Application ID</span></span> | <span data-ttu-id="697e5-151">アプリケーション シークレット</span><span class="sxs-lookup"><span data-stu-id="697e5-151">Application Secret</span></span> | <span data-ttu-id="697e5-152">リダイレクト URI/URL</span><span class="sxs-lookup"><span data-stu-id="697e5-152">Redirect URI/URL</span></span> | <span data-ttu-id="697e5-153">暗黙的フロー</span><span class="sxs-lookup"><span data-stu-id="697e5-153">Implicit Flow</span></span> 
| --- | --- | --- | --- | --- | --- |
| <span data-ttu-id="697e5-154">ネイティブ/モバイル</span><span class="sxs-lookup"><span data-stu-id="697e5-154">Native/Mobile</span></span> | <span data-ttu-id="697e5-155">ネイティブ</span><span class="sxs-lookup"><span data-stu-id="697e5-155">Native</span></span> | <span data-ttu-id="697e5-156">割り当て済み</span><span class="sxs-lookup"><span data-stu-id="697e5-156">Assigned</span></span>  | <span data-ttu-id="697e5-157">いいえ</span><span class="sxs-lookup"><span data-stu-id="697e5-157">No</span></span> | <span data-ttu-id="697e5-158">割り当て済み</span><span class="sxs-lookup"><span data-stu-id="697e5-158">Assigned</span></span> | <span data-ttu-id="697e5-159">いいえ</span><span class="sxs-lookup"><span data-stu-id="697e5-159">No</span></span> |
| <span data-ttu-id="697e5-160">Web App</span><span class="sxs-lookup"><span data-stu-id="697e5-160">Web App</span></span> | <span data-ttu-id="697e5-161">Web</span><span class="sxs-lookup"><span data-stu-id="697e5-161">Web</span></span> | <span data-ttu-id="697e5-162">割り当て済み</span><span class="sxs-lookup"><span data-stu-id="697e5-162">Assigned</span></span> | <span data-ttu-id="697e5-163">はい</span><span class="sxs-lookup"><span data-stu-id="697e5-163">Yes</span></span> | <span data-ttu-id="697e5-164">はい</span><span class="sxs-lookup"><span data-stu-id="697e5-164">Yes</span></span> | <span data-ttu-id="697e5-165">省略可能</span><span class="sxs-lookup"><span data-stu-id="697e5-165">Optional</span></span> <br/><span data-ttu-id="697e5-166">既定で、Open ID Connect ミドルウェアでハイブリッド フローを使用する (はい)</span><span class="sxs-lookup"><span data-stu-id="697e5-166">Open ID Connect middleware uses hybrid flow by default (Yes)</span></span> | 
| <span data-ttu-id="697e5-167">シングル ページ アプリ (SPA)</span><span class="sxs-lookup"><span data-stu-id="697e5-167">Single Page App (SPA)</span></span> | <span data-ttu-id="697e5-168">Web</span><span class="sxs-lookup"><span data-stu-id="697e5-168">Web</span></span> | <span data-ttu-id="697e5-169">割り当て済み</span><span class="sxs-lookup"><span data-stu-id="697e5-169">Assigned</span></span> | <span data-ttu-id="697e5-170">はい</span><span class="sxs-lookup"><span data-stu-id="697e5-170">Yes</span></span> | <span data-ttu-id="697e5-171">はい</span><span class="sxs-lookup"><span data-stu-id="697e5-171">Yes</span></span> | <span data-ttu-id="697e5-172">はい</span><span class="sxs-lookup"><span data-stu-id="697e5-172">Yes</span></span> <br/> <span data-ttu-id="697e5-173">SPA で Open ID Connect 暗黙的フローを使用する</span><span class="sxs-lookup"><span data-stu-id="697e5-173">SPAs use Open ID Connect implicit Flow</span></span> |
| <span data-ttu-id="697e5-174">サービス/デーモン</span><span class="sxs-lookup"><span data-stu-id="697e5-174">Service/Daemon</span></span> | <span data-ttu-id="697e5-175">Web</span><span class="sxs-lookup"><span data-stu-id="697e5-175">Web</span></span> | <span data-ttu-id="697e5-176">割り当て済み</span><span class="sxs-lookup"><span data-stu-id="697e5-176">Assigned</span></span> | <span data-ttu-id="697e5-177">はい</span><span class="sxs-lookup"><span data-stu-id="697e5-177">Yes</span></span> | <span data-ttu-id="697e5-178">はい</span><span class="sxs-lookup"><span data-stu-id="697e5-178">Yes</span></span> | <span data-ttu-id="697e5-179">いいえ</span><span class="sxs-lookup"><span data-stu-id="697e5-179">No</span></span> |

<span data-ttu-id="697e5-180">管理者の同意エクスペリエンスを提供するアプリケーションでは、応答を送信するために Azure AD のリダイレクト URL がもう一つ必要となることがあります。</span><span class="sxs-lookup"><span data-stu-id="697e5-180">Apps that provide an administrator consent experience may need an additional Redirect URL for Azure AD to return the response to.</span></span>

<span data-ttu-id="697e5-181">アプリケーション登録ポータルとアプリケーション設定のプロパティに関する詳細は「[アプリの登録リファレンス](https://docs.microsoft.com/ja-JP/azure/active-directory/develop/active-directory-v2-registration-portal)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="697e5-181">For more detail about the App Registration Portal and the properties you can configure for your App, see [App registration reference](https://docs.microsoft.com/ja-JP/azure/active-directory/develop/active-directory-v2-registration-portal).</span></span>  

## <a name="azure-ad-endpoint-considerations"></a><span data-ttu-id="697e5-182">Azure AD エンドポイントに関して考慮すべき事項</span><span class="sxs-lookup"><span data-stu-id="697e5-182">Azure AD endpoint considerations</span></span>

<span data-ttu-id="697e5-p112">[Azure ポータル](https://aka.ms/aadapplist)は Azure AD エンドポイントのアプリを登録するために使用します。v 2.0 エンドポイントの場合と同様、アプリケーション ID、アプリケーションの機密情報、リダイレクト URI と URL などを設定します。ただし、これには注意すべき重要な違いがいくつかあります。</span><span class="sxs-lookup"><span data-stu-id="697e5-p112">You use the [Azure portal](https://aka.ms/aadapplist) to register your app for the Azure AD endpoint. You configure the same basic properties like Application ID, Application Secret, and Redirect URI/URL, as you would for the v2.0 endpoint; however, there are some important differences to be aware of:</span></span> 

- <span data-ttu-id="697e5-185">アプリケーションの登録には、職場または学校のアカウントのみを使用できます。</span><span class="sxs-lookup"><span data-stu-id="697e5-185">You can only use a work or school account to register an app.</span></span>
- <span data-ttu-id="697e5-186">アプリケーションには、プラットフォームごとのアプリケーション ID が必要です。</span><span class="sxs-lookup"><span data-stu-id="697e5-186">Your app will require a different Application ID for each platform.</span></span>
- <span data-ttu-id="697e5-187">アプリケーションがマルチ テナント アプリケーションの場合は、ポータルでマルチ テナントとなるよう明示的に設定する必要があります。</span><span class="sxs-lookup"><span data-stu-id="697e5-187">If your app is a multi-tenant app, you must explicitly configure it to be multi-tenant at the portal.</span></span>
- <span data-ttu-id="697e5-188">アプリケーションがポータルで必要とするすべてのアクセス許可 (Microsoft Graph アクセス許可を含む) を事前に設定しておく必要があります。</span><span class="sxs-lookup"><span data-stu-id="697e5-188">You must pre-configure all the permissions (including Microsoft Graph permissions) that your app needs at the portal.</span></span> 

<span data-ttu-id="697e5-189">Azure ポータルを使用してアプリケーションを追加する方法の詳細については「[アプリを Azure Active Directory v2.0 エンドポイントに登録する](https://docs.microsoft.com/ja-JP/azure/active-directory/develop/quickstart-v2-register-an-app)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="697e5-189">For guidance on using the Azure portal to add an app, see [Register an app with the Azure Active Directory v2.0 endpoint](https://docs.microsoft.com/ja-JP/azure/active-directory/develop/quickstart-v2-register-an-app).</span></span>
