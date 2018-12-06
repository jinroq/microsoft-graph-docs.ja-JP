---
title: Visual Studio 2017 での Microsoft Graph API を使った Office 365 サービスの呼び出し
description: Visual Studio の接続済みサービスを使い、アプリケーションから Microsoft Graph API を呼び出せるよう設定できます。この記事では、サインインしているユーザーのプロフィール写真を取得し、OneDrive へアップロードし、写真の共有リンクを記載したメールを送信する方法を説明します。
ms.openlocfilehash: 33469dec7014d81ed55c2efceb96a26c2651d239
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27092437"
---
# <a name="call-office-365-services-in-visual-studio-2017-with-the-microsoft-graph-api"></a><span data-ttu-id="f27af-104">Visual Studio 2017 での Microsoft Graph API を使った Office 365 サービスの呼び出し</span><span class="sxs-lookup"><span data-stu-id="f27af-104">Call Office 365 services in Visual Studio 2017 with the Microsoft Graph API</span></span>

<span data-ttu-id="f27af-p102">Visual Studio の接続済みサービスを使い、アプリケーションから Microsoft Graph API を呼び出せるよう設定できます。この記事では、サインインしているユーザーのプロフィール写真を取得し、OneDrive へアップロードし、写真の共有リンクを記載したメールを送信する方法を説明します。</span><span class="sxs-lookup"><span data-stu-id="f27af-p102">You can use the Connected Services in Visual Studio to configure your app to call the Microsoft Graph API. This article describes how to get a signed in user's profile photo, upload it to OneDrive, and send an email with a sharing link to the photo.</span></span>

## <a name="get-set-up"></a><span data-ttu-id="f27af-107">設定する</span><span class="sxs-lookup"><span data-stu-id="f27af-107">Get set up</span></span>

<span data-ttu-id="f27af-108">Office 365 接続済みサービスを Microsoft Graph と共に使用するには、次に従います。</span><span class="sxs-lookup"><span data-stu-id="f27af-108">To use the Office 365 Connected Services with Microsoft Graph, you'll need to do the following:</span></span>

- <span data-ttu-id="f27af-p103">[Visual Studio 2017 プレビュー](https://www.visualstudio.com/vs/preview/)をまだダウンロードしていない場合は、ダウンロードします。Visual Studio の以前のバージョンを使用している場合は、それと合わせて Visual Studio 2017 プレビューを使用できます。</span><span class="sxs-lookup"><span data-stu-id="f27af-p103">Download the [Visual Studio 2017 Preview](https://www.visualstudio.com/vs/preview/), if you haven't already. If you're using an earlier version of Visual Studio, you can use Visual Studio 2017 Preview side by side with your current version.</span></span>

- <span data-ttu-id="f27af-p104">Office 365 サブスクリプションを入手します。無料試用版を取得するには、[Office 365 開発者プログラム](https://dev.office.com/devprogram)に参加します。</span><span class="sxs-lookup"><span data-stu-id="f27af-p104">Get an Office 365 subscription. To get a free trial, join the [Office 365 Developer program](https://dev.office.com/devprogram).</span></span>

## <a name="get-the-starter-project"></a><span data-ttu-id="f27af-113">スタート プロジェクトをセットアップする</span><span class="sxs-lookup"><span data-stu-id="f27af-113">Get the starter project</span></span>

<span data-ttu-id="f27af-p105">[Microsoft Graph ASP.NET 接続済みサービスサンプル](https://github.com/microsoftgraph/aspnet-connect-sample/archive/Office365connectedservice.zip)をダウンロードします。このサンプルには、Microsoft Graph で認証を行うために必要な参照が含まれています。スタート プロジェクトをダウンロードし、解凍して、Visual Studio 2017 プレビューでサンプルを開きます。</span><span class="sxs-lookup"><span data-stu-id="f27af-p105">Download the [Microsoft Graph ASP.NET Connected Services Sample](https://github.com/microsoftgraph/aspnet-connect-sample/archive/Office365connectedservice.zip). This sample includes the references that you need to authenticate against Microsoft Graph. After you download the starter project, unzip, and open the sample in Visual Studio 2017 Preview.</span></span>

## <a name="add-the-connected-service"></a><span data-ttu-id="f27af-117">接続済みサービスの追加</span><span class="sxs-lookup"><span data-stu-id="f27af-117">Add the Connected Service</span></span>

<span data-ttu-id="f27af-118">Microsoft Graph のサービスを Visual Studio プロジェクトに追加する準備が整いました。</span><span class="sxs-lookup"><span data-stu-id="f27af-118">You're now ready to add the Microsoft Graph service to your Visual Studio project.</span></span> 

1. <span data-ttu-id="f27af-119">ソリューション エクスプローラーで、[**接続済みサービス**] を選択し、[接続済みサービス] タブを開きます。</span><span class="sxs-lookup"><span data-stu-id="f27af-119">In Solution Explorer, choose **Connected Services** to open the Connected Services tab.</span></span> 

2. <span data-ttu-id="f27af-p106">**Microsoft Graph で Office 365 サービスをアクセス** プロバイダーを選択します。ウィザードに従います。以下のアクセス許可を選択します (アクセス許可は後から変更できます)。</span><span class="sxs-lookup"><span data-stu-id="f27af-p106">Choose the **Access Office 365 Services with Microsoft Graph** provider. Follow the wizard. Select the following permissions (you can change the permisssions later):</span></span>

    - <span data-ttu-id="f27af-123">**File** API のアクセス許可は**ファイルへのフルアクセス許可**を設定します。</span><span class="sxs-lookup"><span data-stu-id="f27af-123">For the **File** APIs, set permissions to **Have full access to your files**.</span></span>
    - <span data-ttu-id="f27af-124">**Mail** API のアクセス許可は**ユーザーとしてのメールの送信**を設定します。</span><span class="sxs-lookup"><span data-stu-id="f27af-124">For the **Mail** APIs, set permissions to **Send mail as you**.</span></span>
    - <span data-ttu-id="f27af-125">**User** API のアクセス許可は**サインインとユーザー プロファイルの読み取り**を設定します。</span><span class="sxs-lookup"><span data-stu-id="f27af-125">For the **User** APIs, set permissions to **Sign you in and read your profile**.</span></span>

## <a name="call-the-microsoft-graph-api"></a><span data-ttu-id="f27af-126">Microsoft Graph API の呼び出し</span><span class="sxs-lookup"><span data-stu-id="f27af-126">Call the Microsoft Graph API</span></span>

<span data-ttu-id="f27af-p107">最初のサンプルは、単純な電子メールを送信する設定です。Microsoft Graph を使ってサンプルを編集し、サインインしているユーザーの、One Drive にあるプロフィール写真へのリンクが記載されたメールを送信するようにできます。</span><span class="sxs-lookup"><span data-stu-id="f27af-p107">The starter sample is configured to send a simple email. You can use Microsoft Graph to update the sample to send an email with a link to the signed-in user's profile photo in OneDrive.</span></span>

1. <span data-ttu-id="f27af-129">Microsoft Graph を呼び出すコードがある 'Models\GraphService.cs' に移動します。</span><span class="sxs-lookup"><span data-stu-id="f27af-129">Go to 'Models\GraphService.cs', which hosts the code to call Microsoft Graph.</span></span>

2. <span data-ttu-id="f27af-p108">以下のメソッドにある SDK への呼び出しを検索し、**コメントを解除**します。Microsoft Graph を呼び出してプロフィール写真を取得し、ファイルを One Drive にアップロードし、共有リンクを取得する方法を示します。</span><span class="sxs-lookup"><span data-stu-id="f27af-p108">Find and **Uncomment** calls to the SDK in the following methods. This shows how to call Microsoft Graph to get a profile photo, upload a file to OneDrive, and get a sharing link.</span></span>

    ```csharp
        GetCurrentUserPhotoStream(GraphServiceClient graphClient)
    ```
    
    ```csharp
        UploadFileToOneDrive(GraphServiceClient graphClient, byte[] file)
    ```

    ```csharp
        GetSharingLink(GraphServiceClient graphClient, string Id)
    ```
 
> <span data-ttu-id="f27af-132">**ヒント:** コメントは「//Uncomment:」で始まります。</span><span class="sxs-lookup"><span data-stu-id="f27af-132">**Tip:** Each comment starts with '//Uncomment:'</span></span>
 

## <a name="run-the-sample"></a><span data-ttu-id="f27af-133">サンプルを実行する</span><span class="sxs-lookup"><span data-stu-id="f27af-133">Run the sample</span></span>
<span data-ttu-id="f27af-p109">サンプルの構築と実行次に、右上の [**サインイン**] リンクを選択します。続いて、[**メールアドレス取得**]、[**メール送信**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="f27af-p109">Build and run the sample. Next, choose the **Sign-in** link on the top right, and then choose **Get email address** followed by **Send email**.</span></span>

<span data-ttu-id="f27af-136">これにより、プロフィール写真へのリンクが記載されたメールが送信されます。</span><span class="sxs-lookup"><span data-stu-id="f27af-136">This will send an email that includes a link to your profile photo.</span></span>

><span data-ttu-id="f27af-137">**メモ:**</span><span class="sxs-lookup"><span data-stu-id="f27af-137">**Notes:**</span></span>

>- <span data-ttu-id="f27af-138">サンプルの実行を Visual Studio から停止し、再度実行した場合は、明示的なサインアウトが必要となることがあります。</span><span class="sxs-lookup"><span data-stu-id="f27af-138">If you stop and rerun the sample from Visual Studio, you might need to explicitly sign out for the sample to work.</span></span>
>- <span data-ttu-id="f27af-139">ユーザーが認証されていないことを示すエラーが発生する場合、[接続済みサービスの追加](#add-the-connected-service)手順を再度行います。</span><span class="sxs-lookup"><span data-stu-id="f27af-139">If you get an exception that indicates that the User is not authenticated, you might need to repeat the [Add the Connected Service](#add-the-connected-service) step.</span></span>
    

## <a name="explore-the-code"></a><span data-ttu-id="f27af-140">コードを理解します。</span><span class="sxs-lookup"><span data-stu-id="f27af-140">Explore the code</span></span>

<span data-ttu-id="f27af-p110">これで、サービスの接続と設定を Visual Studio 2017 から行えるようになりました。最初のサンプルでは、スキャフォールディングと参照を作成できます。</span><span class="sxs-lookup"><span data-stu-id="f27af-p110">You can now use Visual Studio 2017 to connect to and configure your services. The starter sample creates the scaffolding and references for you.</span></span>  

<span data-ttu-id="f27af-143">このサンプルには、次のファイルが含まれています。</span><span class="sxs-lookup"><span data-stu-id="f27af-143">The starter sample includes the following files:</span></span>

- <span data-ttu-id="f27af-144">[Startup.Auth.cs](https://github.com/microsoftgraph/aspnet-connect-sample/tree/Office365connectedservice/Microsoft%20Graph%20SDK%20ASPNET%20Sample/Microsoft%20Graph%20SDK%20ASPNET%20Sample/App_Start/Startup.Auth.cs):現在のユーザーを認証して、サンプルのトークン キャッシュを初期化します。</span><span class="sxs-lookup"><span data-stu-id="f27af-144">[Startup.Auth.cs](https://github.com/microsoftgraph/aspnet-connect-sample/tree/Office365connectedservice/Microsoft%20Graph%20SDK%20ASPNET%20Sample/Microsoft%20Graph%20SDK%20ASPNET%20Sample/App_Start/Startup.Auth.cs) - Authenticates the current user and initializes the sample's token cache.</span></span>

- <span data-ttu-id="f27af-p111">Models\\[SessionTokenCache.cs](https://github.com/microsoftgraph/aspnet-connect-sample/tree/Office365connectedservice/Microsoft%20Graph%20SDK%20ASPNET%20Sample/Microsoft%20Graph%20SDK%20ASPNET%20Sample/TokenStorage/SessionTokenCache.cs):ユーザーのトークンの情報を格納します。これを独自のカスタム トークン キャッシュと置き換えることができます。詳細については、「[マルチテナント アプリケーションのアクセス トークンのキャッシュ](https://azure.microsoft.com/en-us/documentation/articles/guidance-multitenant-identity-token-cache/)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="f27af-p111">Models\\[SessionTokenCache.cs](https://github.com/microsoftgraph/aspnet-connect-sample/tree/Office365connectedservice/Microsoft%20Graph%20SDK%20ASPNET%20Sample/Microsoft%20Graph%20SDK%20ASPNET%20Sample/TokenStorage/SessionTokenCache.cs) - Stores the user's token information. You can replace this with your own custom token cache. For more information, see [Caching access tokens in a multitenant application](https://azure.microsoft.com/en-us/documentation/articles/guidance-multitenant-identity-token-cache/).</span></span>

- <span data-ttu-id="f27af-148">Models\\[SampleAuthProvider.cs](https://github.com/microsoftgraph/aspnet-connect-sample/tree/Office365connectedservice/Microsoft%20Graph%20SDK%20ASPNET%20Sample/Microsoft%20Graph%20SDK%20ASPNET%20Sample/Helpers/SampleAuthProvider.cs):ローカルの IAuthProvider インターフェイスを実装して、アクセス トークンを取得します。</span><span class="sxs-lookup"><span data-stu-id="f27af-148">Models\\[SampleAuthProvider.cs](https://github.com/microsoftgraph/aspnet-connect-sample/tree/Office365connectedservice/Microsoft%20Graph%20SDK%20ASPNET%20Sample/Microsoft%20Graph%20SDK%20ASPNET%20Sample/Helpers/SampleAuthProvider.cs) - Implements the local IAuthProvider interface, and gets an access token.</span></span> 

- <span data-ttu-id="f27af-149">Helpers\\[SDKHelper.cs](https://github.com/microsoftgraph/aspnet-connect-sample/tree/Office365connectedservice/Microsoft%20Graph%20SDK%20ASPNET%20Sample/Microsoft%20Graph%20SDK%20ASPNET%20Sample/Helpers/SDKHelper.cs):Microsoft Graph との対話に使用される [Microsoft Graph .NET クライアント ライブラリ](https://github.com/microsoftgraph/msgraph-sdk-dotnet)から **GraphServiceClient** を初期化します。</span><span class="sxs-lookup"><span data-stu-id="f27af-149">Helpers\\[SDKHelper.cs](https://github.com/microsoftgraph/aspnet-connect-sample/tree/Office365connectedservice/Microsoft%20Graph%20SDK%20ASPNET%20Sample/Microsoft%20Graph%20SDK%20ASPNET%20Sample/Helpers/SDKHelper.cs) - Initializes the **GraphServiceClient** from the [Microsoft Graph .NET Client Library](https://github.com/microsoftgraph/msgraph-sdk-dotnet) that is used to interact with the Microsoft Graph.</span></span>

- <span data-ttu-id="f27af-150">Controllers\\[HomeController.cs](https://github.com/microsoftgraph/aspnet-connect-sample/tree/Office365connectedservice/Microsoft%20Graph%20SDK%20ASPNET%20Sample/Microsoft%20Graph%20SDK%20ASPNET%20Sample/Controllers/HomeController.cs):Microsoft Graph サービスを構築して呼び出しを送信し、その応答を処理するために **GraphServiceClient** を使用するメソッドが含まれています。</span><span class="sxs-lookup"><span data-stu-id="f27af-150">Controllers\\[HomeController.cs](https://github.com/microsoftgraph/aspnet-connect-sample/tree/Office365connectedservice/Microsoft%20Graph%20SDK%20ASPNET%20Sample/Microsoft%20Graph%20SDK%20ASPNET%20Sample/Controllers/HomeController.cs) - Contains methods that use the **GraphServiceClient** to build and send calls to the Microsoft Graph service and to process the response.</span></span>

- <span data-ttu-id="f27af-151">Views\\Home\\[Graph.cshtml](https://github.com/microsoftgraph/aspnet-connect-sample/tree/Office365connectedservice/Microsoft%20Graph%20SDK%20ASPNET%20Sample/Microsoft%20Graph%20SDK%20ASPNET%20Sample/Views/Home/Graph.cshtml):サンプル用の UI が入っています。</span><span class="sxs-lookup"><span data-stu-id="f27af-151">Views\\Home\\[Graph.cshtml](https://github.com/microsoftgraph/aspnet-connect-sample/tree/Office365connectedservice/Microsoft%20Graph%20SDK%20ASPNET%20Sample/Microsoft%20Graph%20SDK%20ASPNET%20Sample/Views/Home/Graph.cshtml) - Contains the UI for the sample.</span></span> 


## <a name="need-help"></a><span data-ttu-id="f27af-152">サポートが必要な場合</span><span class="sxs-lookup"><span data-stu-id="f27af-152">Need help?</span></span>

<span data-ttu-id="f27af-p112">ヘルプが必要な場合は、[StackOverflow](https://stackoverflow.com/questions/tagged/microsoftgraph?sort=newest) に質問を投稿してください。ご質問には {microsoftgraph} のタグを付けてください。</span><span class="sxs-lookup"><span data-stu-id="f27af-p112">If you need help, post your questions on [StackOverflow](https://stackoverflow.com/questions/tagged/microsoftgraph?sort=newest). Tag your post with {microsoftgraph}.</span></span>

