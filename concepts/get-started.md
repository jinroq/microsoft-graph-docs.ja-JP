# <a name="getting-started-building-microsoft-graph-apps"></a><span data-ttu-id="30fab-101">Microsoft Graph アプリの構築を開始する</span><span class="sxs-lookup"><span data-stu-id="30fab-101">Getting started building Microsoft Graph apps</span></span>

<span data-ttu-id="30fab-p101">このセクションの記事では、Microsoft Graph に接続するアプリをさまざまな言語および開発プラットフォームで構築する方法を詳しく説明します。各記事では、まず該当するプラットフォームのサンプル スターター プロジェクトを説明し、次いでユーザー認証の機能を追加する手順を説明し、そのアカウントから Microsoft Graph でメールを送信するためのサンプル要求を作成します。完成したプロジェクトは、そのプラットフォーム用の [Microsoft Graph リポジトリの Connect サンプル](https://github.com/microsoftgraph?utf8=%E2%9C%93&query=connect)とまったく同じものです。</span><span class="sxs-lookup"><span data-stu-id="30fab-p101">The articles in this section provide detailed guidance on how to build apps that connect to Microsoft Graph across a variety of languages and development platforms. Each article starts with a sample starter project for the appropriate platform, and walks you through adding functionality that authenticates the user and makes a sample request to have Microsoft Graph send an email from their account. The completed project is identical to the [Connect sample in the Microsoft Graph repo](https://github.com/microsoftgraph?utf8=%E2%9C%93&query=connect) for that platform.</span></span>

<span data-ttu-id="30fab-105">好みの認証プロバイダーと開発プラットフォームについて説明した記事を選び、Microsoft Graph への接続を開始します。</span><span class="sxs-lookup"><span data-stu-id="30fab-105">Choose the article that covers the authentication provider and development platform of your choice, and get started connecting to Microsoft Graph.</span></span>

<span data-ttu-id="30fab-106">選んだ開発プラットフォームについての記事に記載されている手順に従うことも、[クイック スタート](https://developer.microsoft.com/graph/quick-start)機能を試してみて、動作するソリューションをすばやく稼働させることもできます。</span><span class="sxs-lookup"><span data-stu-id="30fab-106">You can follow the steps in the article that covers the development platform that you choose, or, to quickly get a working solution up and running, try out the [quick start](https://developer.microsoft.com/graph/quick-start) experience.</span></span>

<span data-ttu-id="30fab-p102">完成した Connect サンプルを確認するには、GitHub の [Microsoft Graph](https://github.com/microsoftgraph) をご覧ください。次の表は、認証プロバイダーとプラットフォームごとにサンプルをリストにしたもので、REST または Microsoft Graph クライアント ライブラリのどちらを使用して Microsoft Graph に接続するかを示しています。</span><span class="sxs-lookup"><span data-stu-id="30fab-p102">To explore the finished Connect samples, see [Microsoft Graph](https://github.com/microsoftgraph) in GitHub. The following table lists the samples by authentication provider and platform, and notes whether they connect to Microsoft Graph using REST or a Microsoft Graph client library.</span></span>

<table>
  <tr>
    <th><span data-ttu-id="30fab-109">プラットフォーム</span><span class="sxs-lookup"><span data-stu-id="30fab-109">Platform</span></span></th>
    <th><span data-ttu-id="30fab-110">Azure AD エンドポイント</span><span class="sxs-lookup"><span data-stu-id="30fab-110">Azure AD endpoint</span></span></th> 
    <th><span data-ttu-id="30fab-111">Azure AD v2.0 エンドポイント</span><span class="sxs-lookup"><span data-stu-id="30fab-111">Azure AD v2.0 endpoint</span></span></th>
  </tr>
  <tr>
    <td><span data-ttu-id="30fab-112">Android</span><span class="sxs-lookup"><span data-stu-id="30fab-112">Android</span></span></td>
    <td><span data-ttu-id="30fab-113">
        <a href="https://github.com/microsoftgraph/android-java-connect-sample/tree/last_v1_auth">SDK サンプル</a>
    </span><span class="sxs-lookup"><span data-stu-id="30fab-113">
        <a href="https://github.com/microsoftgraph/android-java-connect-sample/tree/last_v1_auth">SDK sample</a>
    </span></span></td> 
        <td><span data-ttu-id="30fab-114">
                <a href="https://github.com/microsoftgraph/android-java-connect-sample">SDK サンプル</a>または ¶<a href="https://github.com/microsoftgraph/android-java-connect-rest-sample">REST サンプル</a>
    </span><span class="sxs-lookup"><span data-stu-id="30fab-114">
                <a href="https://github.com/microsoftgraph/android-java-connect-sample">SDK sample</a> or <a href="https://github.com/microsoftgraph/android-java-connect-rest-sample">REST sample</a>
    </span></span></td> 
  </tr>
  <tr>
    <td><span data-ttu-id="30fab-115">AngularJS</span><span class="sxs-lookup"><span data-stu-id="30fab-115">AngularJS</span></span></td>
    <td><span data-ttu-id="30fab-116">
        <a href="https://github.com/microsoftgraph/angular-connect-rest-sample/tree/last_v1_auth">REST サンプル</a>
    </span><span class="sxs-lookup"><span data-stu-id="30fab-116">
        <a href="https://github.com/microsoftgraph/angular-connect-rest-sample/tree/last_v1_auth">REST sample</a>
    </span></span></td> 
        <td><span data-ttu-id="30fab-117">
        <a href="https://github.com/microsoftgraph/angular-connect-sample">SDK サンプル</a>または ¶<a href="https://github.com/microsoftgraph/angular-connect-rest-sample">REST サンプル</a>
    </span><span class="sxs-lookup"><span data-stu-id="30fab-117">
        <a href="https://github.com/microsoftgraph/angular-connect-sample">SDK sample</a> or <a href="https://github.com/microsoftgraph/angular-connect-rest-sample">REST sample</a>
    </span></span></td> 
  </tr>
  <tr>
    <td><span data-ttu-id="30fab-118">ASP.NET</span><span class="sxs-lookup"><span data-stu-id="30fab-118">ASP.NET</span></span></td>
    <td><span data-ttu-id="30fab-119">
        <a href="https://github.com/microsoftgraph/aspnet-connect-rest-sample/tree/last_v1_auth">REST サンプル</a>
    </span><span class="sxs-lookup"><span data-stu-id="30fab-119">
        <a href="https://github.com/microsoftgraph/aspnet-connect-rest-sample/tree/last_v1_auth">REST sample</a>
    </span></span></td>     
    <td><span data-ttu-id="30fab-120">
        <a href="https://github.com/microsoftgraph/aspnet-connect-sample">SDK サンプル</a>または <a href="https://github.com/microsoftgraph/aspnet-connect-rest-sample">REST サンプル</a>
    </span><span class="sxs-lookup"><span data-stu-id="30fab-120">
        <a href="https://github.com/microsoftgraph/aspnet-connect-sample">SDK sample</a> or <a href="https://github.com/microsoftgraph/aspnet-connect-rest-sample">REST sample</a>
    </span></span></td> 
  </tr>
  <tr>
    <td><span data-ttu-id="30fab-121">iOS (Obj-C)</span><span class="sxs-lookup"><span data-stu-id="30fab-121">iOS (Obj-C)</span></span></td>
    <td><span data-ttu-id="30fab-122">
        <a href="https://github.com/microsoftgraph/ios-objectivec-connect-rest-sample">REST サンプル</a>
    </span><span class="sxs-lookup"><span data-stu-id="30fab-122">
        <a href="https://github.com/microsoftgraph/ios-objectivec-connect-rest-sample">REST sample</a>
    </span></span></td>     
    <td><span data-ttu-id="30fab-123">
        <a href="https://github.com/microsoftgraph/ios-objectivec-connect-sample">SDK サンプル</a>
    </span><span class="sxs-lookup"><span data-stu-id="30fab-123">
        <a href="https://github.com/microsoftgraph/ios-objectivec-connect-sample">SDK sample</a>
    </span></span></td> 
  </tr>
  <tr>
    <td><span data-ttu-id="30fab-124">iOS (Swift)</span><span class="sxs-lookup"><span data-stu-id="30fab-124">iOS (Swift)</span></span></td>
    <td><span data-ttu-id="30fab-125">
        <a href="https://github.com/microsoftgraph/ios-swift-connect-rest-sample">REST サンプル</a>
    </span><span class="sxs-lookup"><span data-stu-id="30fab-125">
        <a href="https://github.com/microsoftgraph/ios-swift-connect-rest-sample">REST sample</a>
    </span></span></td>     
    <td><span data-ttu-id="30fab-126">
        <a href="https://github.com/microsoftgraph/ios-swift-connect-sample">SDK サンプル</a>
    </span><span class="sxs-lookup"><span data-stu-id="30fab-126">
        <a href="https://github.com/microsoftgraph/ios-swift-connect-sample">SDK sample</a>
    </span></span></td> 
  </tr>
  <tr>
    <td><span data-ttu-id="30fab-127">NodeJS</span><span class="sxs-lookup"><span data-stu-id="30fab-127">NodeJS</span></span></td>
    <td><span data-ttu-id="30fab-128">
        <a href="https://github.com/microsoftgraph/nodejs-connect-rest-sample/tree/last_v1_auth">REST サンプル</a>
    </span><span class="sxs-lookup"><span data-stu-id="30fab-128">
        <a href="https://github.com/microsoftgraph/nodejs-connect-rest-sample/tree/last_v1_auth">REST sample</a>
    </span></span></td>     
    <td>    
        <span data-ttu-id="30fab-129"><a href="https://github.com/microsoftgraph/nodejs-connect-sample">SDK サンプル</a>または <a href="https://github.com/microsoftgraph/nodejs-connect-rest-sample">REST サンプル</a>
    </span><span class="sxs-lookup"><span data-stu-id="30fab-129"><a href="https://github.com/microsoftgraph/nodejs-connect-sample">SDK sample</a> or <a href="https://github.com/microsoftgraph/nodejs-connect-rest-sample">REST sample</a>
    </span></span></td> 
  </tr>
  <tr>
    <td><span data-ttu-id="30fab-130">PHP</span><span class="sxs-lookup"><span data-stu-id="30fab-130">PHP</span></span></td>
    <td><span data-ttu-id="30fab-131">
        <a href="https://github.com/microsoftgraph/php-connect-rest-sample/tree/last_v1_auth">REST サンプル</a>
    </span><span class="sxs-lookup"><span data-stu-id="30fab-131">
        <a href="https://github.com/microsoftgraph/php-connect-rest-sample/tree/last_v1_auth">REST sample</a>
    </span></span></td>     
    <td><span data-ttu-id="30fab-132">
            <a href="https://github.com/microsoftgraph/php-connect-sample">SDK サンプル</a>または ¶<a href="https://github.com/microsoftgraph/php-connect-rest-sample">REST サンプル</a>
    </span><span class="sxs-lookup"><span data-stu-id="30fab-132">
            <a href="https://github.com/microsoftgraph/php-connect-sample">SDK sample</a> or <a href="https://github.com/microsoftgraph/php-connect-rest-sample">REST sample</a>
    </span></span></td> 
  </tr>
  <tr>
    <td><span data-ttu-id="30fab-133">Python</span><span class="sxs-lookup"><span data-stu-id="30fab-133">Python</span></span></td>
    <td><span data-ttu-id="30fab-134">
        <a href="https://github.com/microsoftgraph/python3-connect-rest-sample">REST サンプル</a>
    </span><span class="sxs-lookup"><span data-stu-id="30fab-134">
        <a href="https://github.com/microsoftgraph/python3-connect-rest-sample">REST sample</a>
    </span></span></td>     
    <td>
    </td> 
  </tr>
  <tr>
    <td><span data-ttu-id="30fab-135">Ruby</span><span class="sxs-lookup"><span data-stu-id="30fab-135">Ruby</span></span></td>
    <td><span data-ttu-id="30fab-136">
        <a href="https://github.com/microsoftgraph/ruby-connect-rest-sample/tree/last_v1_auth">REST サンプル</a>
    </span><span class="sxs-lookup"><span data-stu-id="30fab-136">
        <a href="https://github.com/microsoftgraph/ruby-connect-rest-sample/tree/last_v1_auth">REST sample</a>
    </span></span></td>     
    <td><span data-ttu-id="30fab-137">
        <a href="https://github.com/microsoftgraph/ruby-connect-rest-sample">REST サンプル</a>
    </span><span class="sxs-lookup"><span data-stu-id="30fab-137">
        <a href="https://github.com/microsoftgraph/ruby-connect-rest-sample">REST sample</a>
    </span></span></td> 
  </tr>
  <tr>
    <td><span data-ttu-id="30fab-138">UWP</span><span class="sxs-lookup"><span data-stu-id="30fab-138">UWP</span></span></td>
    <td><span data-ttu-id="30fab-139">
        <a href="https://github.com/microsoftgraph/uwp-csharp-connect-rest-sample/tree/last_v1_auth">REST サンプル</a>
    </span><span class="sxs-lookup"><span data-stu-id="30fab-139">
        <a href="https://github.com/microsoftgraph/uwp-csharp-connect-rest-sample/tree/last_v1_auth">REST sample</a>
    </span></span></td>     
    <td><span data-ttu-id="30fab-140">
        <a href="https://github.com/microsoftgraph/uwp-csharp-connect-sample">SDK サンプル</a>または ¶<a href="https://github.com/microsoftgraph/uwp-csharp-connect-rest-sample">REST サンプル</a>
    </span><span class="sxs-lookup"><span data-stu-id="30fab-140">
        <a href="https://github.com/microsoftgraph/uwp-csharp-connect-sample">SDK sample</a> or <a href="https://github.com/microsoftgraph/uwp-csharp-connect-rest-sample">REST sample</a>
    </span></span></td> 
  </tr>
  <tr>
    <td><span data-ttu-id="30fab-141">Xamarin</span><span class="sxs-lookup"><span data-stu-id="30fab-141">Xamarin</span></span></td>
    <td>
    </td>     
    <td><span data-ttu-id="30fab-142">
        <a href="https://github.com/microsoftgraph/xamarin-csharp-connect-sample">SDK サンプル</a>
    </span><span class="sxs-lookup"><span data-stu-id="30fab-142">
        <a href="https://github.com/microsoftgraph/xamarin-csharp-connect-sample">SDK sample</a>
    </span></span></td> 
  </tr>
</table>

## <a name="see-also"></a><span data-ttu-id="30fab-143">関連項目</span><span class="sxs-lookup"><span data-stu-id="30fab-143">See also</span></span>
- <span data-ttu-id="30fab-144">サンプルの REST 呼び出しを [API エクスプローラー](https://developer.microsoft.com/graph/graph-explorer)で試してみてください。</span><span class="sxs-lookup"><span data-stu-id="30fab-144">Try out sample REST calls in our [API Explorer](https://developer.microsoft.com/graph/graph-explorer).</span></span>
- [<span data-ttu-id="30fab-145">Azure AD エンドポイントのドキュメント</span><span class="sxs-lookup"><span data-stu-id="30fab-145">Azure AD endpoint documentation</span></span>](https://azure.microsoft.com/documentation/services/active-directory/)
- [<span data-ttu-id="30fab-146">Azure AD v2.0 エンドポイントのドキュメント</span><span class="sxs-lookup"><span data-stu-id="30fab-146">Azure AD v2.0 endpoint documentation</span></span>](https://azure.microsoft.com/documentation/articles/?service=active-directory&term=azure+ad+v2.0)
