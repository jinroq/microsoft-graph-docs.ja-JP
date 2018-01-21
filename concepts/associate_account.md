# <a name="associate-your-office-365-account-with-azure-ad-to-create-and-manage-apps"></a><span data-ttu-id="44f09-101">Office 365 アカウントを Azure AD と関連付けてアプリを作成および管理する</span><span class="sxs-lookup"><span data-stu-id="44f09-101">Associate your Office 365 account with Azure AD to create and manage apps</span></span>

<span data-ttu-id="44f09-p101">Microsoft Azure Active Directory (Azure AD) を使用してアプリケーションを認証するには、Azure AD にアプリケーションを登録する必要があります。ここに Office 365 のユーザー アカウントとアプリケーション情報が保存されています。Azure ポータルから Azure AD を管理するには、Microsoft Azure サブスクリプションが必要です。Microsoft Azure のポータルを使用して、ユーザー、ロール、アプリを管理できます。</span><span class="sxs-lookup"><span data-stu-id="44f09-p101">To authenticate your applications using Microsoft Azure Active Directory (Azure AD), you need to register them in Azure AD. This is where Office 365 user account and application information is stored. To manage Azure AD through the Azure Management Portal, you need a Microsoft Azure subscription. You can use the management portal in Microsoft Azure to manage users, roles, and apps.</span></span> 

<span data-ttu-id="44f09-106">この記事では、Office 365 アカウントを Azure AD と関連付けてアプリを作成および管理する方法を説明します。</span><span class="sxs-lookup"><span data-stu-id="44f09-106">This article shows you how to associate your Office 365 account with Azure AD to create and manage apps.</span></span>

 ><span data-ttu-id="44f09-107">**注:** この記事では、アプリの認証プロバイダーとして Azure AD を使用します。</span><span class="sxs-lookup"><span data-stu-id="44f09-107">**Note:** This article uses Azure AD as the authentication provider for your app.</span></span> <span data-ttu-id="44f09-108">Azure AD v2.0 エンドポイントを使用する場合、この手順を実行する必要はありません。</span><span class="sxs-lookup"><span data-stu-id="44f09-108">Note: This article uses Azure AD as the authentication provider for your app. If you're using the Azure AD v2.0 endpoint, you don't need to perform this step. For more information, see App authentication with Microsoft Graph.</span></span> <span data-ttu-id="44f09-109">詳細については、「[Microsoft Graph でのアプリ認証](auth_overview.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="44f09-109">For more information see [App authentication with Microsoft Graph](auth_overview.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="44f09-110">前提条件</span><span class="sxs-lookup"><span data-stu-id="44f09-110">Prerequisites</span></span>

<span data-ttu-id="44f09-111">**ビジネス向けの Office 365 アカウント**</span><span class="sxs-lookup"><span data-stu-id="44f09-111">**Office 365 for business account**</span></span>

<span data-ttu-id="44f09-112">既存のビジネス向けの Office 365 アカウントがない場合は、次の操作を実行できます。</span><span class="sxs-lookup"><span data-stu-id="44f09-112">If you don't have an existing Office 365 for business account, you can:</span></span>

- <span data-ttu-id="44f09-113">上記のいずれかの[ビジネス向けの Office 365 プラン](http://products.office.com/ja-JP/business/compare-office-365-for-business-plans)にサインアップする、または</span><span class="sxs-lookup"><span data-stu-id="44f09-113">Sign up for an [Office 365 for business plans](http://products.office.com/ja-JP/business/compare-office-365-for-business-plans) listed above, or</span></span>
- <span data-ttu-id="44f09-114">[Office 365 Developer プログラムに参加して、Office 365 の 1 年間無料のサブスクリプションを取得します](https://aka.ms/devprogramsignup)。</span><span class="sxs-lookup"><span data-stu-id="44f09-114">[Join the Office 365 Developer Program and get a free 1 year subscription to Office 365](https://aka.ms/devprogramsignup).</span></span>

<span data-ttu-id="44f09-115">**Microsoft Azure サブスクリプション**</span><span class="sxs-lookup"><span data-stu-id="44f09-115">**Microsoft Azure subscription**</span></span> 

- <span data-ttu-id="44f09-116">既存の Microsoft Azure サブスクリプションをお持ちの場合は、ビジネス向けの Office 365 サブスクリプションとそのサブスクリプションを関連付けることができます。</span><span class="sxs-lookup"><span data-stu-id="44f09-116">If you can have an existing Microsoft Azure subscription, you can associate your Office 365 for business subscription with it.</span></span> 

- <span data-ttu-id="44f09-117">それ以外の場合は、アプリを登録および管理するために、新しい Azure サブスクリプションを作成して、Office 365 アカウントに関連付ける必要があります。</span><span class="sxs-lookup"><span data-stu-id="44f09-117">Otherwise, you'll need to create a new Azure subscription and associate it with your Office 365 account in order to register and manage apps.</span></span>


<!---<a name="bk_AssociateExistingAzureSubscription"> </a>-->

## <a name="to-associate-an-existing-azure-subscription-with-your-office-365-account"></a><span data-ttu-id="44f09-118">既存の Azure サブスクリプションと Office 365 アカウントを関連付けるには</span><span class="sxs-lookup"><span data-stu-id="44f09-118">To associate an existing Azure subscription with your Office 365 account</span></span>


1. <span data-ttu-id="44f09-119">既存の Azure 資格情報 (例: user@live.com などの Microsoft ID) を使用して、[Microsoft Azure のポータル](https://portal.azure.com)にログオンします。</span><span class="sxs-lookup"><span data-stu-id="44f09-119">Log on to the  [Microsoft Azure Management portal](https://portal.azure.com) with your existing Azure credentials (for example, your Microsoft ID such as user@live.com).</span></span>
        
2. <span data-ttu-id="44f09-120">**[Active Directory]** ノードを選択し、**[ディレクトリ]** タブを選択し、画面下の **[新規]** を選択します。</span><span class="sxs-lookup"><span data-stu-id="44f09-120">Select the  **Active Directory** node, then select the **Directory** tab and, at the bottom of the screen, select **New**.</span></span> 
     
4. <span data-ttu-id="44f09-121">**[新規]** メニュー上で、**[Active Directory]**  >  **[ディレクトリ]**  >  **[カスタム作成]** を選びます。</span><span class="sxs-lookup"><span data-stu-id="44f09-121">On the **New** menu, select **Active Directory** > **Directory** > **Custom Create**.</span></span>
    
5. <span data-ttu-id="44f09-122">**[ディレクトリの追加]** の **[ディレクトリ]** ドロップダウン ボックスで、**[既存のディレクトリの使用]** を選びます。</span><span class="sxs-lookup"><span data-stu-id="44f09-122">In **Add directory**, in the **Directory** drop-down box, select  **Use existing directory**.</span></span> <span data-ttu-id="44f09-123">**[サインアウトする準備ができました]** のチェックボックスをオンにして、右下隅にあるチェック マークを選択します。</span><span class="sxs-lookup"><span data-stu-id="44f09-123">Check **I am ready to be signed out**, and then select the check mark in the lower-right corner.</span></span> 
    
    <span data-ttu-id="44f09-124">これで、Azure のポータルに戻ります。</span><span class="sxs-lookup"><span data-stu-id="44f09-124">This brings you back to the Azure Management Portal.</span></span>
        
3. <span data-ttu-id="44f09-125">Office 365 のアカウント情報を使ってログインします。</span><span class="sxs-lookup"><span data-stu-id="44f09-125">Log in with your Office 365 account information.</span></span> 
    
    <span data-ttu-id="44f09-126">ディレクトリを Azure で使用するかどうかを指定するよう、ダイアログが表示されます。</span><span class="sxs-lookup"><span data-stu-id="44f09-126">You will be prompted whether to use your directory with Azure.</span></span> 
    
    ><span data-ttu-id="44f09-127">**重要:**Office 365 アカウントと Azure AD を関連付けるには、グローバル管理者特権を持つ Office 365 ビジネス アカウントが必要です。</span><span class="sxs-lookup"><span data-stu-id="44f09-127">**Important** To associate your Office 365 account with Azure AD, you'll need  an Office 365 business account with global administrator privileges.</span></span> 
    
        
4. <span data-ttu-id="44f09-128">**[続行]**、**[今すぐサインアウトする]** の順に選択します。</span><span class="sxs-lookup"><span data-stu-id="44f09-128">Select  **continue**, and then **Sign out now**.</span></span>
        
5. <span data-ttu-id="44f09-129">ブラウザーを閉じて、もう一度[ポータル](https://manage.windowsazure.com)を開きます。</span><span class="sxs-lookup"><span data-stu-id="44f09-129">Close the browser and reopen the  [portal](https://manage.windowsazure.com).</span></span> <span data-ttu-id="44f09-130">そうしないと、アクセス拒否エラーを受け取ります。</span><span class="sxs-lookup"><span data-stu-id="44f09-130">Otherwise, you will get an access denied error.</span></span>
    
        
6. <span data-ttu-id="44f09-131">既存の Azure 資格情報 (例: user@live.com などの Microsoft ID) を使用して、もう一度ログオンします。</span><span class="sxs-lookup"><span data-stu-id="44f09-131">Log on again with your existing Azure credentials (for example, your Microsoft ID such as user@live.com).</span></span> <span data-ttu-id="44f09-132">**[Active Directory]** ノードに移動すると、**[ディレクトリ]** の一覧にお客様の Office 365 アカウントが表示されます。</span><span class="sxs-lookup"><span data-stu-id="44f09-132">Navigate to the  **Active Directory** node and, under **Directory**, you should now see your Office 365 account listed.</span></span>
    

<!--<a name="bk_AssociateNewAzureSubscription"> </a>-->

## <a name="to-create-a-new-azure-subscription-and-associate-it-with-your-office-365-account"></a><span data-ttu-id="44f09-133">新しい Azure サブスクリプションを作成して Office 365 アカウントを関連付けるには</span><span class="sxs-lookup"><span data-stu-id="44f09-133">To create a new Azure subscription and associate it with your Office 365 account</span></span>


1. <span data-ttu-id="44f09-134">Office 365 にログオンします。</span><span class="sxs-lookup"><span data-stu-id="44f09-134">Log on to Office 365.</span></span> <span data-ttu-id="44f09-135">**[ホーム]** ページから **[管理]** アイコンを選択して、Office 365 管理センターを開きます。</span><span class="sxs-lookup"><span data-stu-id="44f09-135">From the **Home** page, select the **Admin** icon to open the Office 365 admin center.</span></span>
2. <span data-ttu-id="44f09-136">ページの左側にあるメニュー ページで **[管理]** までスクロール ダウンして、**[Azure AD]** を選びます。</span><span class="sxs-lookup"><span data-stu-id="44f09-136">In the menu page along the left side of the page, scroll down to **Admin** and select **Azure AD**.</span></span>

    ><span data-ttu-id="44f09-137">**重要:**Office 365 管理センターを開いて Azure AD にアクセスするには、グローバル管理者特権を持つ Office 365 ビジネス アカウントが必要です。</span><span class="sxs-lookup"><span data-stu-id="44f09-137">**Important** To open the Office 365 admin center, and access Azure AD, you'll need  an Office 365 business account with global administrator privileges.</span></span> 
    
3. <span data-ttu-id="44f09-138">新しいサブスクリプションを作成します。</span><span class="sxs-lookup"><span data-stu-id="44f09-138">Create a new subscription.</span></span>
        
    <span data-ttu-id="44f09-p107">Office 365 の試用版を使用している場合は、Azure AD は有料サービスのお客様に制限されていることを通知するメッセージが表示されます。無料で 30 日間の試用版の Azure サブスクリプションを作成できますが、いくつかの追加の手順を実行する必要があります。</span><span class="sxs-lookup"><span data-stu-id="44f09-p107">If you're using a trial version of Office 365, you'll see a message telling you that Azure AD is limited to customers with paid services. You can still create a trial 30-day Azure subscription at no charge, but you'll need to perform a few extra steps:</span></span>
    
    1. <span data-ttu-id="44f09-141">国または地域を選択して、**[Azure サブスクリプション]** を選択します。</span><span class="sxs-lookup"><span data-stu-id="44f09-141">Select your country or region, and then choose **Azure subscription**.</span></span>
    2. <span data-ttu-id="44f09-p108">個人情報を入力します。確認のために連絡可能な電話番号を入力して、テキスト メッセージの送信または通話のいずれかを指定します。</span><span class="sxs-lookup"><span data-stu-id="44f09-p108">Enter your personal information. For verification purposes, enter a telephone number at which you can be reached, and specify whether you want to be sent a text message or called.</span></span>
    3. <span data-ttu-id="44f09-144">認証コードを受信したら、そのコードを入力して **[コードの確認]** を選びます。</span><span class="sxs-lookup"><span data-stu-id="44f09-144">When you receive your verification code, enter it and choose **Verify code**.</span></span>
    4. <span data-ttu-id="44f09-145">支払い情報を入力して、承諾のチェック ボックスをオンにし、**[サインアップ]** を選びます。</span><span class="sxs-lookup"><span data-stu-id="44f09-145">Enter payment information, check the agreement, and select **Sign up**.</span></span>
        
        <span data-ttu-id="44f09-146">クレジットカードでのお支払いは発生しません。</span><span class="sxs-lookup"><span data-stu-id="44f09-146">Your credit card will not be charged.</span></span>
        
        <span data-ttu-id="44f09-147">Azure サブスクリプションの作成中は、ブラウザーを閉じたり更新したりしないでください。</span><span class="sxs-lookup"><span data-stu-id="44f09-147">Do not close or refresh your browser while your Azure subscription is being created.</span></span>
            
4. <span data-ttu-id="44f09-148">Azure サブスクリプションが作成されたら、**[ポータル]** を選びます。</span><span class="sxs-lookup"><span data-stu-id="44f09-148">When your Azure subscription is created, choose  **Portal**.</span></span>
        
5. <span data-ttu-id="44f09-149">Azure ツアーが表示されます。</span><span class="sxs-lookup"><span data-stu-id="44f09-149">The Azure Tour appears.</span></span> <span data-ttu-id="44f09-150">ツアーを表示するか、**[X]** を選んで閉じることができます。</span><span class="sxs-lookup"><span data-stu-id="44f09-150">You can view it, or choose  **X** to close it.</span></span>
        
    <span data-ttu-id="44f09-p110">この時点で、Azure サブスクリプション内のすべての項目が表示されます。自分の Office 365 テナントの名前が付いた 1 つのディレクトリが一覧に示されます。</span><span class="sxs-lookup"><span data-stu-id="44f09-p110">You should now see all items in your Azure subscription. It lists a directory with the name of your Office 365 tenant.</span></span>
    
## <a name="see-also"></a><span data-ttu-id="44f09-153">関連項目</span><span class="sxs-lookup"><span data-stu-id="44f09-153">See also</span></span>
- [<span data-ttu-id="44f09-154">Azure AD でのアプリケーションの登録の基本</span><span class="sxs-lookup"><span data-stu-id="44f09-154">Basics of Registering an Application in Azure AD</span></span>](https://azure.microsoft.com/ja-JP/documentation/articles/active-directory-authentication-scenarios/#basics-of-registering-an-application-in-azure-ad)
- [<span data-ttu-id="44f09-155">Azure AD でアプリケーションを追加、更新、削除する</span><span class="sxs-lookup"><span data-stu-id="44f09-155">Add, update, or remove an application in Azure AD</span></span>](https://azure.microsoft.com/ja-JP/documentation/articles/active-directory-integrating-applications/)