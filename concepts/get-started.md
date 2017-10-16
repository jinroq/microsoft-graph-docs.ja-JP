# <a name="getting-started-building-microsoft-graph-apps"></a><span data-ttu-id="c2ba6-101">Microsoft Graph アプリの構築を開始する</span><span class="sxs-lookup"><span data-stu-id="c2ba6-101">Getting started building Microsoft Graph apps</span></span>

<span data-ttu-id="c2ba6-p101">このセクションの記事では、Microsoft Graph に接続するアプリをさまざまな言語および開発プラットフォームで構築する方法を詳しく説明します。各記事では、まず該当するプラットフォームのサンプル スターター プロジェクトを説明し、次いでユーザー認証の機能を追加する手順を説明し、そのアカウントから Microsoft Graph でメールを送信するためのサンプル要求を作成します。完成したプロジェクトは、そのプラットフォーム用の [Microsoft Graph リポジトリの Connect サンプル](https://github.com/microsoftgraph?utf8=%E2%9C%93&query=connect)とまったく同じものです。</span><span class="sxs-lookup"><span data-stu-id="c2ba6-p101">The articles in this section provide detailed guidance on how to build apps that connect to Microsoft Graph across a variety of languages and development platforms. Each article starts with a sample starter project for the appropriate platform, and walks you through adding functionality that authenticates the user and makes a sample request to have Microsoft Graph send an email from their account. The completed project is identical to the [Connect sample in the Microsoft Graph repo](https://github.com/microsoftgraph?utf8=%E2%9C%93&query=connect) for that platform.</span></span>

<span data-ttu-id="c2ba6-105">好みの認証プロバイダーと開発プラットフォームについて説明した記事を選び、Microsoft Graph への接続を開始します。</span><span class="sxs-lookup"><span data-stu-id="c2ba6-105">Choose the article that covers the authentication provider and development platform of your choice, and get started connecting to Microsoft Graph.</span></span> <span data-ttu-id="c2ba6-106">詳細については、「[v2.0 エンドポイントの相違点](https://docs.microsoft.com/en-us/azure/active-directory/develop/active-directory-v2-compare)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="c2ba6-106">For more information, see [What's different about the v2.0 endpoint?](https://docs.microsoft.com/en-us/azure/active-directory/develop/active-directory-v2-compare)</span></span>

<span data-ttu-id="c2ba6-107">選んだ開発プラットフォームについての記事に記載されている手順に従うことも、[クイック スタート](https://developer.microsoft.com/graph/quick-start)機能を試してみて、動作するソリューションをすばやく稼働させることもできます。</span><span class="sxs-lookup"><span data-stu-id="c2ba6-107">You can follow the steps in the article that covers the development platform that you choose, or, to quickly get a working solution up and running, try out the [quick start](https://developer.microsoft.com/graph/quick-start) experience.</span></span>

<span data-ttu-id="c2ba6-p103">完成した Connect サンプルを確認するには、GitHub の [Microsoft Graph](https://github.com/microsoftgraph) をご覧ください。次の表は、認証プロバイダーとプラットフォームごとにサンプルをリストにしたもので、REST または Microsoft Graph クライアント ライブラリのどちらを使用して Microsoft Graph に接続するかを示しています。</span><span class="sxs-lookup"><span data-stu-id="c2ba6-p103">To explore the finished Connect samples, see [Microsoft Graph](https://github.com/microsoftgraph) in GitHub. The following table lists the samples by authentication provider and platform, and notes whether they connect to Microsoft Graph using REST or a Microsoft Graph client library.</span></span>

<table>
  <tr>
    <th><span data-ttu-id="c2ba6-110">プラットフォーム</span><span class="sxs-lookup"><span data-stu-id="c2ba6-110">Platform</span></span></th>
    <th><span data-ttu-id="c2ba6-111">Azure AD エンドポイント</span><span class="sxs-lookup"><span data-stu-id="c2ba6-111">Azure AD endpoint</span></span></th> 
    <th><span data-ttu-id="c2ba6-112">Azure AD v2.0 エンドポイント</span><span class="sxs-lookup"><span data-stu-id="c2ba6-112">Azure AD v2.0 endpoint</span></span></th>
  </tr>
  <tr>
    <td><span data-ttu-id="c2ba6-113">Android</span><span class="sxs-lookup"><span data-stu-id="c2ba6-113">Android</span></span></td>
    <td><span data-ttu-id="c2ba6-114">
        <a href="https://github.com/microsoftgraph/android-java-connect-sample/tree/last_v1_auth">SDK サンプル</a>
    </span><span class="sxs-lookup"><span data-stu-id="c2ba6-114">
        <a href="https://github.com/microsoftgraph/android-java-connect-sample/tree/last_v1_auth">SDK sample</a>
    </span></span></td> 
        <td><span data-ttu-id="c2ba6-115">
                <a href="https://github.com/microsoftgraph/android-java-connect-sample">SDK サンプル</a>または ¶<a href="https://github.com/microsoftgraph/android-java-connect-rest-sample">REST サンプル</a>
    </span><span class="sxs-lookup"><span data-stu-id="c2ba6-115">
                <a href="https://github.com/microsoftgraph/android-java-connect-sample">SDK sample</a> or <a href="https://github.com/microsoftgraph/android-java-connect-rest-sample">REST sample</a>
    </span></span></td> 
  </tr>
  <tr>
    <td><span data-ttu-id="c2ba6-116">AngularJS</span><span class="sxs-lookup"><span data-stu-id="c2ba6-116">AngularJS</span></span></td>
    <td><span data-ttu-id="c2ba6-117">
        <a href="https://github.com/microsoftgraph/angular-connect-rest-sample/tree/last_v1_auth">REST サンプル</a>
    </span><span class="sxs-lookup"><span data-stu-id="c2ba6-117">
        <a href="https://github.com/microsoftgraph/angular-connect-rest-sample/tree/last_v1_auth">REST sample</a>
    </span></span></td> 
        <td><span data-ttu-id="c2ba6-118">
        <a href="https://github.com/microsoftgraph/angular-connect-sample">SDK サンプル</a>または ¶<a href="https://github.com/microsoftgraph/angular-connect-rest-sample">REST サンプル</a>
    </span><span class="sxs-lookup"><span data-stu-id="c2ba6-118">
        <a href="https://github.com/microsoftgraph/angular-connect-sample">SDK sample</a> or <a href="https://github.com/microsoftgraph/angular-connect-rest-sample">REST sample</a>
    </span></span></td> 
  </tr>
  <tr>
    <td><span data-ttu-id="c2ba6-119">ASP.NET</span><span class="sxs-lookup"><span data-stu-id="c2ba6-119">ASP.NET</span></span></td>
    <td><span data-ttu-id="c2ba6-120">
        <a href="https://github.com/microsoftgraph/aspnet-connect-rest-sample/tree/last_v1_auth">REST サンプル</a>
    </span><span class="sxs-lookup"><span data-stu-id="c2ba6-120">
        <a href="https://github.com/microsoftgraph/aspnet-connect-rest-sample/tree/last_v1_auth">REST sample</a>
    </span></span></td>     
    <td><span data-ttu-id="c2ba6-121">
        <a href="https://github.com/microsoftgraph/aspnet-connect-sample">SDK サンプル</a>または <a href="https://github.com/microsoftgraph/aspnet-connect-rest-sample">REST サンプル</a>
    </span><span class="sxs-lookup"><span data-stu-id="c2ba6-121">
        <a href="https://github.com/microsoftgraph/aspnet-connect-sample">SDK sample</a> or <a href="https://github.com/microsoftgraph/aspnet-connect-rest-sample">REST sample</a>
    </span></span></td> 
  </tr>
  <tr>
    <td><span data-ttu-id="c2ba6-122">iOS (Obj-C)</span><span class="sxs-lookup"><span data-stu-id="c2ba6-122">iOS (Obj-C)</span></span></td>
    <td><span data-ttu-id="c2ba6-123">
        <a href="https://github.com/microsoftgraph/ios-objectivec-connect-rest-sample">REST サンプル</a>
    </span><span class="sxs-lookup"><span data-stu-id="c2ba6-123">
        <a href="https://github.com/microsoftgraph/ios-objectivec-connect-rest-sample">REST sample</a>
    </span></span></td>     
    <td><span data-ttu-id="c2ba6-124">
        <a href="https://github.com/microsoftgraph/ios-objectivec-connect-sample">SDK サンプル</a>
    </span><span class="sxs-lookup"><span data-stu-id="c2ba6-124">
        <a href="https://github.com/microsoftgraph/ios-objectivec-connect-sample">SDK sample</a>
    </span></span></td> 
  </tr>
  <tr>
    <td><span data-ttu-id="c2ba6-125">iOS (Swift)</span><span class="sxs-lookup"><span data-stu-id="c2ba6-125">iOS (Swift)</span></span></td>
    <td><span data-ttu-id="c2ba6-126">
        <a href="https://github.com/microsoftgraph/ios-swift-connect-rest-sample">REST サンプル</a>
    </span><span class="sxs-lookup"><span data-stu-id="c2ba6-126">
        <a href="https://github.com/microsoftgraph/ios-swift-connect-rest-sample">REST sample</a>
    </span></span></td>     
    <td><span data-ttu-id="c2ba6-127">
        <a href="https://github.com/microsoftgraph/ios-swift-connect-sample">SDK サンプル</a>
    </span><span class="sxs-lookup"><span data-stu-id="c2ba6-127">
        <a href="https://github.com/microsoftgraph/ios-swift-connect-sample">SDK sample</a>
    </span></span></td> 
  </tr>
  <tr>
    <td><span data-ttu-id="c2ba6-128">NodeJS</span><span class="sxs-lookup"><span data-stu-id="c2ba6-128">NodeJS</span></span></td>
    <td><span data-ttu-id="c2ba6-129">
        <a href="https://github.com/microsoftgraph/nodejs-connect-rest-sample/tree/last_v1_auth">REST サンプル</a>
    </span><span class="sxs-lookup"><span data-stu-id="c2ba6-129">
        <a href="https://github.com/microsoftgraph/nodejs-connect-rest-sample/tree/last_v1_auth">REST sample</a>
    </span></span></td>     
    <td>    
        <span data-ttu-id="c2ba6-130"><a href="https://github.com/microsoftgraph/nodejs-connect-sample">SDK サンプル</a>または <a href="https://github.com/microsoftgraph/nodejs-connect-rest-sample">REST サンプル</a>
    </span><span class="sxs-lookup"><span data-stu-id="c2ba6-130"><a href="https://github.com/microsoftgraph/nodejs-connect-sample">SDK sample</a> or <a href="https://github.com/microsoftgraph/nodejs-connect-rest-sample">REST sample</a>
    </span></span></td> 
  </tr>
  <tr>
    <td><span data-ttu-id="c2ba6-131">PHP</span><span class="sxs-lookup"><span data-stu-id="c2ba6-131">PHP</span></span></td>
    <td><span data-ttu-id="c2ba6-132">
        <a href="https://github.com/microsoftgraph/php-connect-rest-sample/tree/last_v1_auth">REST サンプル</a>
    </span><span class="sxs-lookup"><span data-stu-id="c2ba6-132">
        <a href="https://github.com/microsoftgraph/php-connect-rest-sample/tree/last_v1_auth">REST sample</a>
    </span></span></td>     
    <td><span data-ttu-id="c2ba6-133">
            <a href="https://github.com/microsoftgraph/php-connect-sample">SDK サンプル</a>または ¶<a href="https://github.com/microsoftgraph/php-connect-rest-sample">REST サンプル</a>
    </span><span class="sxs-lookup"><span data-stu-id="c2ba6-133">
            <a href="https://github.com/microsoftgraph/php-connect-sample">SDK sample</a> or <a href="https://github.com/microsoftgraph/php-connect-rest-sample">REST sample</a>
    </span></span></td> 
  </tr>
  <tr>
    <td><span data-ttu-id="c2ba6-134">Python</span><span class="sxs-lookup"><span data-stu-id="c2ba6-134">Python</span></span></td>
    <td><span data-ttu-id="c2ba6-135">
        <a href="https://github.com/microsoftgraph/python3-connect-rest-sample">REST サンプル</a>
    </span><span class="sxs-lookup"><span data-stu-id="c2ba6-135">
        <a href="https://github.com/microsoftgraph/python3-connect-rest-sample">REST sample</a>
    </span></span></td>     
    <td>
    </td> 
  </tr>
  <tr>
    <td><span data-ttu-id="c2ba6-136">Ruby</span><span class="sxs-lookup"><span data-stu-id="c2ba6-136">Ruby</span></span></td>
    <td><span data-ttu-id="c2ba6-137">
        <a href="https://github.com/microsoftgraph/ruby-connect-rest-sample/tree/last_v1_auth">REST サンプル</a>
    </span><span class="sxs-lookup"><span data-stu-id="c2ba6-137">
        <a href="https://github.com/microsoftgraph/ruby-connect-rest-sample/tree/last_v1_auth">REST sample</a>
    </span></span></td>     
    <td><span data-ttu-id="c2ba6-138">
        <a href="https://github.com/microsoftgraph/ruby-connect-rest-sample">REST サンプル</a>
    </span><span class="sxs-lookup"><span data-stu-id="c2ba6-138">
        <a href="https://github.com/microsoftgraph/ruby-connect-rest-sample">REST sample</a>
    </span></span></td> 
  </tr>
  <tr>
    <td><span data-ttu-id="c2ba6-139">UWP</span><span class="sxs-lookup"><span data-stu-id="c2ba6-139">UWP</span></span></td>
    <td><span data-ttu-id="c2ba6-140">
        <a href="https://github.com/microsoftgraph/uwp-csharp-connect-rest-sample/tree/last_v1_auth">REST サンプル</a>
    </span><span class="sxs-lookup"><span data-stu-id="c2ba6-140">
        <a href="https://github.com/microsoftgraph/uwp-csharp-connect-rest-sample/tree/last_v1_auth">REST sample</a>
    </span></span></td>     
    <td><span data-ttu-id="c2ba6-141">
        <a href="https://github.com/microsoftgraph/uwp-csharp-connect-sample">SDK サンプル</a>または ¶<a href="https://github.com/microsoftgraph/uwp-csharp-connect-rest-sample">REST サンプル</a>
    </span><span class="sxs-lookup"><span data-stu-id="c2ba6-141">
        <a href="https://github.com/microsoftgraph/uwp-csharp-connect-sample">SDK sample</a> or <a href="https://github.com/microsoftgraph/uwp-csharp-connect-rest-sample">REST sample</a>
    </span></span></td> 
  </tr>
  <tr>
    <td><span data-ttu-id="c2ba6-142">Xamarin</span><span class="sxs-lookup"><span data-stu-id="c2ba6-142">Xamarin</span></span></td>
    <td>
    </td>     
    <td><span data-ttu-id="c2ba6-143">
        <a href="https://github.com/microsoftgraph/xamarin-csharp-connect-sample">SDK サンプル</a>
    </span><span class="sxs-lookup"><span data-stu-id="c2ba6-143">
        <a href="https://github.com/microsoftgraph/xamarin-csharp-connect-sample">SDK sample</a>
    </span></span></td> 
  </tr>
</table>

## <a name="see-also"></a><span data-ttu-id="c2ba6-144">関連項目</span><span class="sxs-lookup"><span data-stu-id="c2ba6-144">See also</span></span>

- <span data-ttu-id="c2ba6-145">サンプルの REST 呼び出しを [Graph エクスプローラー](https://developer.microsoft.com/en-us/graph/graph-explorer)で試してみてください。</span><span class="sxs-lookup"><span data-stu-id="c2ba6-145">Try out sample REST calls in our [API Explorer](https://developer.microsoft.com/en-us/graph/graph-explorer).</span></span>
- [<span data-ttu-id="c2ba6-146">Azure AD エンドポイントのドキュメント</span><span class="sxs-lookup"><span data-stu-id="c2ba6-146">Azure AD endpoint documentation</span></span>](https://docs.microsoft.com/en-us/azure/active-directory/develop/active-directory-developers-guide)
- [<span data-ttu-id="c2ba6-147">Azure AD v2.0 エンドポイントのドキュメント</span><span class="sxs-lookup"><span data-stu-id="c2ba6-147">Azure AD v2.0 endpoint documentation</span></span>](https://docs.microsoft.com/en-us/azure/active-directory/develop/active-directory-appmodel-v2-overview)
