---
title: アプリを Azure AD v2.0 エンドポイントに登録する
description: 'アプリは、Azure AD に登録する必要があります。アプリを登録すると、トークンの取得のための Azure AD での認証でアプリケーションが使用する一意のアプリケーション ID と他の値が確定します。Azure AD v2.0 エンドポイントの場合は、Microsoft アプリ登録ポータルでアプリを登録します。アプリを登録するには、Microsoft アカウントのほか、職場または学校のアカウントを使用できます。開発するアプリケーションの種類によっては、アプリケーションの認証と承認の設定で 1 つまたは複数のプロパティをコピーする必要があります。 '
author: jackson-woods
localization_priority: Priority
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 87bff46dcb18585ba0814a5848f3cd67deb855d1
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27930559"
---
# <a name="register-your-app-with-the-azure-ad-v20-endpoint"></a><span data-ttu-id="8953d-107">アプリを Azure AD v2.0 エンドポイントに登録する</span><span class="sxs-lookup"><span data-stu-id="8953d-107">Register your app with the Azure AD v2.0 endpoint</span></span>

<span data-ttu-id="8953d-p102">アプリは、Azure AD に登録する必要があります。アプリを登録すると、トークンの取得のための Azure AD での認証でアプリケーションが使用する一意のアプリケーション ID と他の値が確定します。Azure AD v2.0 エンドポイントの場合は、[Microsoft アプリ登録ポータル](https://apps.dev.microsoft.com)でアプリを登録します。アプリを登録するには、Microsoft アカウントのほか、職場または学校のアカウントを使用できます。開発するアプリケーションの種類によっては、アプリケーションの認証と承認の設定で 1 つまたは複数のプロパティをコピーする必要があります。</span><span class="sxs-lookup"><span data-stu-id="8953d-p102">Your app must be registered with Azure AD. Registering your app establishes a unique application ID and other values that your app uses to authenticate with Azure AD and get tokens. For the Azure AD v2.0 endpoint, you register your app with the [Microsoft App Registration Portal](https://apps.dev.microsoft.com). You can use either a Microsoft account or a work or school account to register your app. Depending on the type of app you are developing, you will need to copy one or more properties during registration to use when you configure authentication and authorization for your app.</span></span> 


> <span data-ttu-id="8953d-p103">**注:** この記事では、主にアプリケーションの Azure AD v2.0 のエンドポイントへの登録ついて説明します。Azure AD のエンドポイントへのアプリケーションの登録に関する詳細は「[Azure AD エンドポイントについて考慮すべき事項](#azure-ad-endpoint-considerations)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="8953d-p103">**Note:** This article primarily covers registering apps with the Azure AD v2.0 endpoint. For information about registering your app with the Azure AD endpoint, see [Azure AD endpoint considerations](#azure-ad-endpoint-considerations) below.</span></span>
> 
> <span data-ttu-id="8953d-115">あらかじめ Microsoft Azure ポータルに登録済みのアプリはアプリ登録ポータルには表示されないため、ご注意ください。</span><span class="sxs-lookup"><span data-stu-id="8953d-115">Also, be aware that if you've previously registered apps in the Microsoft Azure portal, those apps will not be listed in the App Registration Portal.</span></span> <span data-ttu-id="8953d-116">それらのアプリは Azure ポータルで管理します。</span><span class="sxs-lookup"><span data-stu-id="8953d-116">Manage those apps in the Azure portal.</span></span> 


<span data-ttu-id="8953d-p105">次のスクリーンショットは、パスワードと暗黙的フローを使用して構成された Web アプリの登録の例を示しています。![パスワードと暗黙的許可による Web アプリの登録。](./images/v2-web-registration.png)</span><span class="sxs-lookup"><span data-stu-id="8953d-p105">The following screenshot shows an example web app registration that has been configured with a password and implicit flow. ![Web app registration with password and implicit grant.](./images/v2-web-registration.png)</span></span>

<span data-ttu-id="8953d-119">アプリを登録するには、以下の手順に従います。アプリの承認を設定するときには、指定された値をコピーして使用してください。</span><span class="sxs-lookup"><span data-stu-id="8953d-119">To register your app, follow these steps; be sure to copy the indicated values to use when configuring authorization for your app:</span></span>

1. <span data-ttu-id="8953d-120">[Microsoft アプリ登録ポータル](https://apps.dev.microsoft.com/)にサインインします。</span><span class="sxs-lookup"><span data-stu-id="8953d-120">Sign into the [Microsoft App Registration Portal](https://apps.dev.microsoft.com/).</span></span>
   
    <span data-ttu-id="8953d-121">Microsoft アカウントのほか、職場または学校のアカウントを使用してサインインできます。</span><span class="sxs-lookup"><span data-stu-id="8953d-121">You can sign in with either a Microsoft account or a work or school account.</span></span> 

2. <span data-ttu-id="8953d-122">**[アプリの追加]** を選択します。</span><span class="sxs-lookup"><span data-stu-id="8953d-122">Choose **Add an app**.</span></span>
    > <span data-ttu-id="8953d-123">注:職場または学校のアカウントを使用してサインインした場合は、署名する場合は、**統合アプリケーション**の **[アプリの追加]** ボタンを選択します。</span><span class="sxs-lookup"><span data-stu-id="8953d-123">Note: If you signed in with a work or school account, select the **Add an app** button for **Converged applications**.</span></span> 

3. <span data-ttu-id="8953d-124">アプリの名前を入力して、**[アプリケーションの作成]** を選択します。</span><span class="sxs-lookup"><span data-stu-id="8953d-124">Enter a name for the app and choose **Create application**.</span></span>

    <span data-ttu-id="8953d-125">登録ページが表示され、アプリのプロパティが一覧表示されます。</span><span class="sxs-lookup"><span data-stu-id="8953d-125">The registration page displays, listing the properties of your app.</span></span>

4. <span data-ttu-id="8953d-p106">アプリケーション ID をコピーします。これは、アプリの一意識別子です。</span><span class="sxs-lookup"><span data-stu-id="8953d-p106">Copy the application ID. This is the unique identifier for your app.</span></span>

    <span data-ttu-id="8953d-128">アプリを構成するには、アプリケーション ID を使用します。</span><span class="sxs-lookup"><span data-stu-id="8953d-128">You'll use the application ID to configure the app.</span></span>

5. <span data-ttu-id="8953d-129">**[プラットフォーム]** で、**[プラットフォームの追加]** を選び、アプリに適したプラットフォームを選びます。</span><span class="sxs-lookup"><span data-stu-id="8953d-129">Under **Platforms**, choose **Add Platform**, and select the appropriate platform for your app:</span></span>
    
    <span data-ttu-id="8953d-130">**ネイティブまたはモバイル アプリケーションでは**</span><span class="sxs-lookup"><span data-stu-id="8953d-130">**For native or mobile apps**:</span></span>

    1. <span data-ttu-id="8953d-131">**[ネイティブ アプリケーション]** を選択します。</span><span class="sxs-lookup"><span data-stu-id="8953d-131">Select **Native Application**.</span></span>

    2. <span data-ttu-id="8953d-p107">**[組み込みリダイレクト URI]** の値をコピーします。このアプリを構成するため、後でこの値が必要になります。</span><span class="sxs-lookup"><span data-stu-id="8953d-p107">Copy the **Built-in redirect URI** value. You'll need this to configure your app.</span></span>

        <span data-ttu-id="8953d-134">リダイレクト URI は、アプリケーションに提供される一意の URI であり、その URI に送信されたメッセージはそのアプリケーションだけに送信されます。</span><span class="sxs-lookup"><span data-stu-id="8953d-134">The redirect URI is a unique URI provided for your application to ensure that messages sent to that URI are only sent to that application.</span></span> 

    <span data-ttu-id="8953d-135">**Web アプリの場合**:</span><span class="sxs-lookup"><span data-stu-id="8953d-135">**For web apps**:</span></span>

    1. <span data-ttu-id="8953d-136">**[Web]** を選びます。</span><span class="sxs-lookup"><span data-stu-id="8953d-136">Select **Web**.</span></span>

    2. <span data-ttu-id="8953d-137">使用している認証フローの種類によっては、**[暗黙的フローを許可する]** チェック ボックスが選択されていることを確認する必要があります。</span><span class="sxs-lookup"><span data-stu-id="8953d-137">Depending on the type of authentication flow you're using, you may have to make sure the **Allow Implicit Flow** check box is selected.</span></span> 
        
        <span data-ttu-id="8953d-p108">**[暗黙的フローを許可する]** オプションにより、OpenID Connect ハイブリッド フローと暗黙的フローが有効になります。ハイブリッド フローにより、アプリはサインイン情報 (ID トークン) と成果物 (この場合は認証コード) の両方を受け取れるようになり、アプリはアクセス トークンを取得するときにこれらを使用できます。ハイブリッド フローは、OWIN OpenID Connect ミドルウェアが使用する既定のフローです。シングル ページ アプリ (SPA) では、アプリは暗黙的フローにより、サインイン情報とアクセス トークンを受け取ることができます。</span><span class="sxs-lookup"><span data-stu-id="8953d-p108">The **Allow Implicit Flow** option enables the OpenID Connect hybrid and implicit flows. The hybrid flow enables the app to receive both sign-in info (the id token) and artifacts (in this case, an authorization code) that the app uses to obtain an access token. The hybrid flow is the default flow used by the OWIN OpenID Connect middleware. For single page apps (SPA), the implicit flow enables the app to receive sign-in info and the access token.</span></span> 

    3. <span data-ttu-id="8953d-142">リダイレクト URL を指定します。</span><span class="sxs-lookup"><span data-stu-id="8953d-142">Specify a Redirect URL.</span></span>
        
        <span data-ttu-id="8953d-143">リダイレクト URL は、Azure AD v2.0 エンドポイントが認証要求処理を完了した際に呼び出す、アプリ内の場所です。</span><span class="sxs-lookup"><span data-stu-id="8953d-143">The redirect URL is the location in your app that the Azure AD v2.0 endpoint calls when it has processed the authentication request.</span></span>

    4. <span data-ttu-id="8953d-p109">**[アプリケーション シークレット]** で、**[新しいパスワードを生成する]** を選びます。**[新しいパスワードが生成されました]** ダイアログ ボックスからアプリケーション シークレットをコピーします。</span><span class="sxs-lookup"><span data-stu-id="8953d-p109">Under **Application Secrets**, choose **Generate New Password**. Copy the app secret from the **New password generated** dialog box.</span></span>
        > <span data-ttu-id="8953d-p110">**重要**:**[新しいパスワードが生成されました]** ダイアログを閉じる前に、アプリケーションの機密情報をコピーする必要があります。ダイアログ ボックスを閉じた後は、機密情報は取得できません。</span><span class="sxs-lookup"><span data-stu-id="8953d-p110">**Important** You must copy the app secret before you close the **New password generated** dialog. After you close the dialog, you cannot retrieve the secret.</span></span> 
            
6. <span data-ttu-id="8953d-148">**[保存]** を選択します。</span><span class="sxs-lookup"><span data-stu-id="8953d-148">Choose **Save**.</span></span>


<span data-ttu-id="8953d-p111">以下の表に、さまざまな種類のアプリケーションの設定とコピーに必要となるプロパティを示します。_割り当て済み_とは、Azure AD で割り当てられた値を使用する必要があることを示します。</span><span class="sxs-lookup"><span data-stu-id="8953d-p111">The following table shows the properties that you need to configure and copy for different kinds of apps. _Assigned_ means that you should use the value assigned by Azure AD.</span></span>


| <span data-ttu-id="8953d-151">アプリの種類</span><span class="sxs-lookup"><span data-stu-id="8953d-151">App type</span></span> | <span data-ttu-id="8953d-152">プラットフォーム</span><span class="sxs-lookup"><span data-stu-id="8953d-152">Platform</span></span> | <span data-ttu-id="8953d-153">アプリケーション ID</span><span class="sxs-lookup"><span data-stu-id="8953d-153">Application ID</span></span> | <span data-ttu-id="8953d-154">アプリケーション シークレット</span><span class="sxs-lookup"><span data-stu-id="8953d-154">Application Secret</span></span> | <span data-ttu-id="8953d-155">リダイレクト URI/URL</span><span class="sxs-lookup"><span data-stu-id="8953d-155">Redirect URI/URL</span></span> | <span data-ttu-id="8953d-156">暗黙的フロー</span><span class="sxs-lookup"><span data-stu-id="8953d-156">Implicit Flow</span></span> 
| --- | --- | --- | --- | --- | --- |
| <span data-ttu-id="8953d-157">ネイティブ/モバイル</span><span class="sxs-lookup"><span data-stu-id="8953d-157">Native/Mobile</span></span> | <span data-ttu-id="8953d-158">ネイティブ</span><span class="sxs-lookup"><span data-stu-id="8953d-158">Native</span></span> | <span data-ttu-id="8953d-159">割り当て済み</span><span class="sxs-lookup"><span data-stu-id="8953d-159">Assigned</span></span>  | <span data-ttu-id="8953d-160">いいえ</span><span class="sxs-lookup"><span data-stu-id="8953d-160">No</span></span> | <span data-ttu-id="8953d-161">割り当て済み</span><span class="sxs-lookup"><span data-stu-id="8953d-161">Assigned</span></span> | <span data-ttu-id="8953d-162">いいえ</span><span class="sxs-lookup"><span data-stu-id="8953d-162">No</span></span> |
| <span data-ttu-id="8953d-163">Web App</span><span class="sxs-lookup"><span data-stu-id="8953d-163">Web App</span></span> | <span data-ttu-id="8953d-164">Web</span><span class="sxs-lookup"><span data-stu-id="8953d-164">Web</span></span> | <span data-ttu-id="8953d-165">割り当て済み</span><span class="sxs-lookup"><span data-stu-id="8953d-165">Assigned</span></span> | <span data-ttu-id="8953d-166">はい</span><span class="sxs-lookup"><span data-stu-id="8953d-166">Yes</span></span> | <span data-ttu-id="8953d-167">はい</span><span class="sxs-lookup"><span data-stu-id="8953d-167">Yes</span></span> | <span data-ttu-id="8953d-168">省略可能</span><span class="sxs-lookup"><span data-stu-id="8953d-168">Optional</span></span> <br/><span data-ttu-id="8953d-169">既定で、Open ID Connect ミドルウェアでハイブリッド フローを使用する (はい)</span><span class="sxs-lookup"><span data-stu-id="8953d-169">Open ID Connect middleware uses hybrid flow by default (Yes)</span></span> | 
| <span data-ttu-id="8953d-170">シングル ページ アプリ (SPA)</span><span class="sxs-lookup"><span data-stu-id="8953d-170">Single Page App (SPA)</span></span> | <span data-ttu-id="8953d-171">Web</span><span class="sxs-lookup"><span data-stu-id="8953d-171">Web</span></span> | <span data-ttu-id="8953d-172">割り当て済み</span><span class="sxs-lookup"><span data-stu-id="8953d-172">Assigned</span></span> | <span data-ttu-id="8953d-173">はい</span><span class="sxs-lookup"><span data-stu-id="8953d-173">Yes</span></span> | <span data-ttu-id="8953d-174">はい</span><span class="sxs-lookup"><span data-stu-id="8953d-174">Yes</span></span> | <span data-ttu-id="8953d-175">はい</span><span class="sxs-lookup"><span data-stu-id="8953d-175">Yes</span></span> <br/> <span data-ttu-id="8953d-176">SPA で Open ID Connect 暗黙的フローを使用する</span><span class="sxs-lookup"><span data-stu-id="8953d-176">SPAs use Open ID Connect implicit Flow</span></span> |
| <span data-ttu-id="8953d-177">サービス/デーモン</span><span class="sxs-lookup"><span data-stu-id="8953d-177">Service/Daemon</span></span> | <span data-ttu-id="8953d-178">Web</span><span class="sxs-lookup"><span data-stu-id="8953d-178">Web</span></span> | <span data-ttu-id="8953d-179">割り当て済み</span><span class="sxs-lookup"><span data-stu-id="8953d-179">Assigned</span></span> | <span data-ttu-id="8953d-180">はい</span><span class="sxs-lookup"><span data-stu-id="8953d-180">Yes</span></span> | <span data-ttu-id="8953d-181">はい</span><span class="sxs-lookup"><span data-stu-id="8953d-181">Yes</span></span> | <span data-ttu-id="8953d-182">いいえ</span><span class="sxs-lookup"><span data-stu-id="8953d-182">No</span></span> |

<span data-ttu-id="8953d-183">管理者の同意エクスペリエンスを提供するアプリケーションでは、応答を送信するために Azure AD のリダイレクト URL がもう一つ必要となることがあります。</span><span class="sxs-lookup"><span data-stu-id="8953d-183">Apps that provide an administrator consent experience may need an additional Redirect URL for Azure AD to return the response to.</span></span>

<span data-ttu-id="8953d-184">アプリケーション登録ポータルとアプリケーション設定のプロパティに関する詳細は「[アプリの登録リファレンス](https://docs.microsoft.com/ja-JP/azure/active-directory/develop/active-directory-v2-registration-portal)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="8953d-184">For more detail about the App Registration Portal and the properties you can configure for your App, see [App registration reference](https://docs.microsoft.com/ja-JP/azure/active-directory/develop/active-directory-v2-registration-portal).</span></span>  

## <a name="azure-ad-endpoint-considerations"></a><span data-ttu-id="8953d-185">Azure AD エンドポイントに関して考慮すべき事項</span><span class="sxs-lookup"><span data-stu-id="8953d-185">Azure AD endpoint considerations</span></span>

<span data-ttu-id="8953d-p112">[Azure ポータル](https://aka.ms/aadapplist)は Azure AD エンドポイントのアプリを登録するために使用します。v 2.0 エンドポイントの場合と同様、アプリケーション ID、アプリケーションの機密情報、リダイレクト URI と URL などを設定します。ただし、これには注意すべき重要な違いがいくつかあります。</span><span class="sxs-lookup"><span data-stu-id="8953d-p112">You use the [Azure portal](https://aka.ms/aadapplist) to register your app for the Azure AD endpoint. You configure the same basic properties like Application ID, Application Secret, and Redirect URI/URL, as you would for the v2.0 endpoint; however, there are some important differences to be aware of:</span></span> 

- <span data-ttu-id="8953d-188">アプリケーションの登録には、職場または学校のアカウントのみを使用できます。</span><span class="sxs-lookup"><span data-stu-id="8953d-188">You can only use a work or school account to register an app.</span></span>
- <span data-ttu-id="8953d-189">アプリケーションには、プラットフォームごとのアプリケーション ID が必要です。</span><span class="sxs-lookup"><span data-stu-id="8953d-189">Your app will require a different Application ID for each platform.</span></span>
- <span data-ttu-id="8953d-190">アプリケーションがマルチ テナント アプリケーションの場合は、ポータルでマルチ テナントとなるよう明示的に設定する必要があります。</span><span class="sxs-lookup"><span data-stu-id="8953d-190">If your app is a multi-tenant app, you must explicitly configure it to be multi-tenant at the portal.</span></span>
- <span data-ttu-id="8953d-191">アプリケーションがポータルで必要とするすべてのアクセス許可 (Microsoft Graph アクセス許可を含む) を事前に設定しておく必要があります。</span><span class="sxs-lookup"><span data-stu-id="8953d-191">You must pre-configure all the permissions (including Microsoft Graph permissions) that your app needs at the portal.</span></span> 

<span data-ttu-id="8953d-192">Azure ポータルを使用してアプリケーションを追加する方法の詳細については「[アプリケーションと Azure Active Directory の統合:アプリケーションの追加](https://docs.microsoft.com/azure/active-directory/develop/active-directory-integrating-applications#adding-an-application)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="8953d-192">For guidance on using the Azure portal to add an app, see [Integrating applications with Azure Active Directory: Adding an application](https://docs.microsoft.com/azure/active-directory/develop/active-directory-integrating-applications#adding-an-application).</span></span>
