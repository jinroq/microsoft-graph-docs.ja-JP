---
title: Azure AD Graph .NET アプリを Microsoft Graph に移行する
description: Azure Active Directory (Azure AD) API アプリを Microsoft Graph API に移行する方法について説明します。
author: dkershaw10
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: bc48be3712b0d3b03e9799559aac4d6ae812b5d0
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/15/2019
ms.locfileid: "36422178"
---
# <a name="migrate-net-client-library-use-to-microsoft-graph"></a><span data-ttu-id="ba5d0-103">.NET クライアントライブラリを Microsoft Graph に移行する</span><span class="sxs-lookup"><span data-stu-id="ba5d0-103">Migrate .NET client library use to Microsoft Graph</span></span>

<span data-ttu-id="ba5d0-104">この記事は、「*手順 3:* アプリ[を移行するプロセス](migrate-azure-ad-graph-planning-checklist.md)の詳細を確認する」に含まれています。</span><span class="sxs-lookup"><span data-stu-id="ba5d0-104">This article is part of *step 3: review app details* of the [process to migrate apps](migrate-azure-ad-graph-planning-checklist.md).</span></span>

<span data-ttu-id="ba5d0-105">アプリで現在 Azure AD Graph クライアントライブラリを使用している場合は、 [Microsoft Graph .net クライアントライブラリ](https://github.com/microsoftgraph/msgraph-sdk-dotnet)に切り替えます。</span><span class="sxs-lookup"><span data-stu-id="ba5d0-105">If your app currently uses the Azure AD Graph client library, switch to the [Microsoft Graph .NET client library](https://github.com/microsoftgraph/msgraph-sdk-dotnet).</span></span>

><span data-ttu-id="ba5d0-106">注: Microsoft Graph .NET クライアントライブラリは、.NET Framework 4.5 および .NET Standard 1.1 でのみサポートされています。</span><span class="sxs-lookup"><span data-stu-id="ba5d0-106">NOTE: The Microsoft Graph .NET client library is only supported for .NET Framework 4.5 and .NET Standard 1.1.</span></span>  <span data-ttu-id="ba5d0-107">ただし、最新のサポート情報については、「Microsoft Graph .NET クライアントライブラリ」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="ba5d0-107">However please consult Microsoft Graph .NET client library for the latest support information.</span></span>

<span data-ttu-id="ba5d0-108">ここでは、Microsoft Graph .NET クライアントライブラリに移行するための一般的な手順について説明します。</span><span class="sxs-lookup"><span data-stu-id="ba5d0-108">Here, we'll look at some general steps to migrate over to the Microsoft Graph .NET client library:</span></span>

- <span data-ttu-id="ba5d0-109">アクセストークンを指定して Microsoft Graph クライアントを作成する方法 (ADAL または MSAL を使用して取得可能)</span><span class="sxs-lookup"><span data-stu-id="ba5d0-109">How to create a Microsoft Graph client, given an access token (that you can acquire using ADAL or MSAL)</span></span>
- <span data-ttu-id="ba5d0-110">要求を定式化する方法</span><span class="sxs-lookup"><span data-stu-id="ba5d0-110">How to formulate requests</span></span>
- <span data-ttu-id="ba5d0-111">クエリビルダーの使用方法</span><span class="sxs-lookup"><span data-stu-id="ba5d0-111">How to use query builders</span></span>
- <span data-ttu-id="ba5d0-112">コレクションとページングを処理する方法</span><span class="sxs-lookup"><span data-stu-id="ba5d0-112">How to handle collections and paging</span></span>  

## <a name="overview-of-the-migration-steps"></a><span data-ttu-id="ba5d0-113">移行手順の概要</span><span class="sxs-lookup"><span data-stu-id="ba5d0-113">Overview of the migration steps</span></span>

<span data-ttu-id="ba5d0-114">次の手順では、アプリが既に ADAL を使用して Azure AD Graph を呼び出すためのアクセストークンを取得していることを前提としています。これで、引き続き ADAL を使用することになります。</span><span class="sxs-lookup"><span data-stu-id="ba5d0-114">The following steps assume your app is already using ADAL to acquire access tokens to call Azure AD Graph, and that for now you will continue to use ADAL.</span></span> <span data-ttu-id="ba5d0-115">Msal への切り替えは、 [msal への移行](/graph/migrate-azure-ad-graph-authentication-library#migrate-to-msal)で説明されている個別の手順として実行できます。</span><span class="sxs-lookup"><span data-stu-id="ba5d0-115">Switching to MSAL can be done as a separate step described in [migrating to MSAL](/graph/migrate-azure-ad-graph-authentication-library#migrate-to-msal).</span></span>

1. <span data-ttu-id="ba5d0-116">Microsoft Graph へのアクセストークンを取得するには、 **Resourceurl**をから`https://graph.windows.net`に`https://graph.microsoft.com`更新します。</span><span class="sxs-lookup"><span data-stu-id="ba5d0-116">To acquire an access token to Microsoft Graph, update **resourceUrl** from `https://graph.windows.net` to `https://graph.microsoft.com`.</span></span>

2. <span data-ttu-id="ba5d0-117">アプリで、次のように変更して Microsoft Graph クライアントライブラリへの参照を更新します。</span><span class="sxs-lookup"><span data-stu-id="ba5d0-117">In your app, update references to the Microsoft Graph client library by changing:</span></span>

    ``` csharp
    using Microsoft.Azure.ActiveDirectory.GraphClient;
    ```

    <span data-ttu-id="ba5d0-118">宛先：</span><span class="sxs-lookup"><span data-stu-id="ba5d0-118">To:</span></span>

    ``` csharp
    using Microsoft.Graph;
    ```

3. <span data-ttu-id="ba5d0-119">パッケージマネージャーを使用して、 [Microsoft Graph NuGet パッケージ](https://www.nuget.org/packages/Microsoft.Graph/)をダウンロードして更新し、依存関係を更新します。</span><span class="sxs-lookup"><span data-stu-id="ba5d0-119">Use your package manager to download and update the [Microsoft Graph NuGet package](https://www.nuget.org/packages/Microsoft.Graph/) and update dependencies.</span></span>

4. <span data-ttu-id="ba5d0-120">を使用するのではなく`GraphServiceClient`、を作成`ActiveDirectoryClient`するようにクライアントのコンストラクターを更新します。</span><span class="sxs-lookup"><span data-stu-id="ba5d0-120">Update your client constructor to create a `GraphServiceClient`, rather than `ActiveDirectoryClient`.</span></span>  <span data-ttu-id="ba5d0-121">次のコードスニペットは、アプリが新しいトークン`AcquireTokenAsyncForUser()`を取得するためにメソッドを使用していることを前提としています。</span><span class="sxs-lookup"><span data-stu-id="ba5d0-121">The following code snippets assume your app is using the `AcquireTokenAsyncForUser()` method to acquire new tokens.</span></span> <span data-ttu-id="ba5d0-122">このメソッドの定義は、 [dotnet-graphapi のサンプル](https://github.com/Azure-Samples/active-directory-dotnet-graphapi-console/blob/archive/GraphConsoleAppV3/AuthenticationHelper.cs)の一部として検索できます。</span><span class="sxs-lookup"><span data-stu-id="ba5d0-122">You can find a definition for this method as part of the [active-directory-dotnet-graphapi-console sample](https://github.com/Azure-Samples/active-directory-dotnet-graphapi-console/blob/archive/GraphConsoleAppV3/AuthenticationHelper.cs).</span></span>

    <span data-ttu-id="ba5d0-123">変化</span><span class="sxs-lookup"><span data-stu-id="ba5d0-123">Change:</span></span>

    ``` csharp
    ActiveDirectoryClient client = new ActiveDirectoryClient(serviceRoot,
    async () => await AcquireTokenAsyncForUser());
    ```

    <span data-ttu-id="ba5d0-124">宛先：</span><span class="sxs-lookup"><span data-stu-id="ba5d0-124">To:</span></span>

    ``` csharp
    GraphServiceClient graphClient = new GraphServiceClient(serviceRoot,
       new DelegateAuthenticationProvider(async (requestMessage) => {
          var token = await AcquireTokenAsyncForUser();
          requestMessage.Headers.Authorization = new
             AuthenticationHeaderValue("bearer", token);
       }));
    ```

    <span data-ttu-id="ba5d0-125">Microsoft Graph クライアントライブラリの場合、 `serviceRoot`この値にもバージョン番号が含まれています。</span><span class="sxs-lookup"><span data-stu-id="ba5d0-125">For Microsoft Graph client library, the `serviceRoot` value also includes the version number.</span></span> <span data-ttu-id="ba5d0-126">現時点では、この`https://graph.microsoft.com/v1.0`値はです。</span><span class="sxs-lookup"><span data-stu-id="ba5d0-126">Currently, that value is `https://graph.microsoft.com/v1.0`.</span></span>

5. <span data-ttu-id="ba5d0-127">Microsoft Graph クライアント要求ビルダー構文を使用するように要求を更新するには、次のように変更します。</span><span class="sxs-lookup"><span data-stu-id="ba5d0-127">Update requests to use the Microsoft Graph client request builder syntax, by changing:</span></span>

    ``` csharp
    signedInUser = (User)await client.Me.ExecuteAsync();
    ```

    <span data-ttu-id="ba5d0-128">宛先：</span><span class="sxs-lookup"><span data-stu-id="ba5d0-128">To:</span></span>

    ``` csharp
    signedInUser = (User)await client.Me.Request().GetAsync();
    ```

    [!NOTE]
    <span data-ttu-id="ba5d0-129">Azure AD Graph クライアントライブラリでは、LINQ ベースのクエリ構文がサポートされていました。</span><span class="sxs-lookup"><span data-stu-id="ba5d0-129">The Azure AD Graph client library supported LINQ-based query syntax.</span></span> <span data-ttu-id="ba5d0-130">ただし、Microsoft Graph クライアントライブラリにはありません。</span><span class="sxs-lookup"><span data-stu-id="ba5d0-130">However, the Microsoft Graph client library does not.</span></span>  <span data-ttu-id="ba5d0-131">そのため、関連するクエリをより RESTful 式に変換する必要があります。</span><span class="sxs-lookup"><span data-stu-id="ba5d0-131">Consequently, you'll need to convert the relevant queries to a more RESTful expression.</span></span>  

    <span data-ttu-id="ba5d0-132">これを行うには、次のように変更します。</span><span class="sxs-lookup"><span data-stu-id="ba5d0-132">To do so, change:</span></span>

    ``` csharp
    var groups = await
    client.Groups.Where(g => g.DisplayName.StartsWith("a")).ExecuteAsync();
    ```

    <span data-ttu-id="ba5d0-133">宛先：</span><span class="sxs-lookup"><span data-stu-id="ba5d0-133">To:</span></span>

    ``` csharp
    var groups = await
    client.Groups.Request().Filter("startswith(displayName,'a')").GetAsync();
    ```

6. <span data-ttu-id="ba5d0-134">コードでコレクションを使用してページを作成する場合は、次の小さな調整を行います。</span><span class="sxs-lookup"><span data-stu-id="ba5d0-134">If your code pages through collections, make the following minor adjustments.</span></span> <span data-ttu-id="ba5d0-135">次の例では、グループのフェッチと比較を、一度に5個ずつ、そのメンバーまでと比較します。</span><span class="sxs-lookup"><span data-stu-id="ba5d0-135">The following example compares and contrasts fetching a group and paging through its members, 5 at a time.</span></span> <span data-ttu-id="ba5d0-136">Azure AD Graph のコードでは、グループのメンバーをフェッチするために fetcher コンストラクトが必要ですが、Microsoft Graph にはそのような要件はありません。</span><span class="sxs-lookup"><span data-stu-id="ba5d0-136">While the code for Azure AD Graph requires a fetcher construct in order to fetch a group's members, Microsoft Graph has no such requirement.</span></span> <span data-ttu-id="ba5d0-137">それ以外の場合、コードは比較的似ています。</span><span class="sxs-lookup"><span data-stu-id="ba5d0-137">Other than that, the code is relatively similar.</span></span>  <span data-ttu-id="ba5d0-138">簡潔にするために、ユーザーメンバーのみが表示されます。 try/catch および error 条件は表示されず、コードスニペットはシングルスレッドコンソールアプリ用です。</span><span class="sxs-lookup"><span data-stu-id="ba5d0-138">To be concise, only user members are displayed, try/catch and error conditions are not shown, and the code snippets are for a single-threaded console app.</span></span>

    <span data-ttu-id="ba5d0-139">例として、Azure AD Graph .NET クライアントライブラリを使用して、次のコードを変更します。</span><span class="sxs-lookup"><span data-stu-id="ba5d0-139">As an example, change the following code using the Azure AD Graph .NET client library:</span></span>

    ```csharp
    Group retrievedGroup = client.Groups.
        Where(g => g.ObjectId.Equals(id)).ExecuteAsync().Result;
    IGroupFetcher retrievedGroupFetcher = (IGroupFetcher) retrievedGroup;

    var membersPage = retrievedGroupFetcher.Members.Take(5).ExecuteAsync().Result;
    Console.WriteLine(" Members:");
    do
    {
        List<IDirectoryObject> members = membersPage.CurrentPage.ToList();
        foreach (IDirectoryObject member in members)
        {
            if (member is User)
            {
                User memberUser = (User)member;
                Console.WriteLine("        User: {0} ", memberUser.DisplayName);
            }
        }
        membersPage = membersPage.GetNextPageAsync().Result;
    } while (membersPage != null);

    ```

    <span data-ttu-id="ba5d0-140">Microsoft Graph .NET クライアントライブラリを使用して、次のコードを実行します。</span><span class="sxs-lookup"><span data-stu-id="ba5d0-140">To the following code using the Microsoft Graph .NET client library:</span></span>

    ```csharp
    var membersPage = client.Groups[id].Members.Request().Top(5).GetAsync().Result;
    Console.WriteLine(" Members:");
    do
    {
        List<DirectoryObject> members = membersPage.CurrentPage.ToList();
        foreach (DirectoryObject member in members)
        {
            if (member is User)
            {
                User memberUser = (User)member;
                Console.WriteLine("        User: {0} ", memberUser.DisplayName);
            }
        }
        if (membersPage.NextPageRequest != null)
            membersPage = membersPage.NextPageRequest.GetAsync().Result;
        else membersPage = null;
    } while (membersPage != null);

    ```

7. <span data-ttu-id="ba5d0-141">通常、名前の変更に関連するリソース、プロパティ、ナビゲーション、およびサービスアクションのエラーを構築して修正します。</span><span class="sxs-lookup"><span data-stu-id="ba5d0-141">Build and fix any resource, property, navigation, and service action errors, generally related to name changes.</span></span>

## <a name="see-also"></a><span data-ttu-id="ba5d0-142">関連項目</span><span class="sxs-lookup"><span data-stu-id="ba5d0-142">See also</span></span>

<span data-ttu-id="ba5d0-143">[C# コンソールスニペットアプリ](https://github.com/microsoftgraph/console-csharp-snippets-sample)では、Microsoft Graph クライアントライブラリと Azure AD Graph クライアントライブラリの相違点の多くが強調されています。</span><span class="sxs-lookup"><span data-stu-id="ba5d0-143">The [C# console snippets app](https://github.com/microsoftgraph/console-csharp-snippets-sample) highlights more of the differences between Microsoft Graph client library and Azure AD Graph client library.</span></span>

<span data-ttu-id="ba5d0-144">Azure AD Graph クライアントライブラリでは、.NET プラットフォームのみがサポートされています。</span><span class="sxs-lookup"><span data-stu-id="ba5d0-144">The Azure AD Graph client library supports only the .NET platform.</span></span>  <span data-ttu-id="ba5d0-145">ただし、Microsoft Graph クライアントライブラリでは、ソリューションにとってより便利な追加の[プラットフォームと言語](/graph)がサポートされています。</span><span class="sxs-lookup"><span data-stu-id="ba5d0-145">However, Microsoft Graph client library supports additional [platforms and languages](/graph) that you may find more useful for your solutions.</span></span>

## <a name="next-steps"></a><span data-ttu-id="ba5d0-146">次のステップ</span><span class="sxs-lookup"><span data-stu-id="ba5d0-146">Next Steps</span></span>

- <span data-ttu-id="ba5d0-147">Microsoft Graph に移行したアプリを[展開、テスト、および拡張](/graph/migrate-azure-ad-graph-deploy-test-extend)する方法について説明します。</span><span class="sxs-lookup"><span data-stu-id="ba5d0-147">Learn how to [deploy, test, and extend](/graph/migrate-azure-ad-graph-deploy-test-extend) apps you've migrated to Microsoft Graph.</span></span>
- <span data-ttu-id="ba5d0-148">[Microsoft Graph](/graph/overview)の概念とプラクティスについて説明します。</span><span class="sxs-lookup"><span data-stu-id="ba5d0-148">Explore [Microsoft Graph](/graph/overview) concepts and practices.</span></span>
- <span data-ttu-id="ba5d0-149">[Graph エクスプローラー](https://aka.ms/ge)を使用して、Microsoft graph を試してみてください。</span><span class="sxs-lookup"><span data-stu-id="ba5d0-149">Use [Graph Explorer](https://aka.ms/ge) to experiment with Microsoft Graph.</span></span>
