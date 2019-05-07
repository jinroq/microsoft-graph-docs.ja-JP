---
title: Azure AD Graph .NET アプリを Microsoft Graph に移行する
description: Azure Active Directory (Azure AD) API アプリを Microsoft Graph API に移行する方法について説明します。
author: dkershaw10
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: fbc7c7550cda7654f603feeafb17ff3f0eb281e1
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/06/2019
ms.locfileid: "33630259"
---
# <a name="migrate-net-client-library-use-to-microsoft-graph"></a>.NET クライアントライブラリを Microsoft Graph に移行する

この記事は、「*手順 3:* アプリ[を移行するプロセス](migrate-azure-ad-graph-planning-checklist.md)の詳細を確認する」に含まれています。

アプリで現在 Azure AD Graph クライアントライブラリを使用している場合は、 [Microsoft Graph .net クライアントライブラリ](https://github.com/microsoftgraph/msgraph-sdk-dotnet)に切り替えます。

>注: Microsoft Graph .NET クライアントライブラリは、.NET Framework 4.5 および .NET Standard 1.1 でのみサポートされています。  ただし、最新のサポート情報については、「Microsoft Graph .NET クライアントライブラリ」を参照してください。

ここでは、Microsoft Graph .NET クライアントライブラリに移行するための一般的な手順について説明します。

- アクセストークンを指定して Microsoft Graph クライアントを作成する方法 (ADAL または MSAL を使用して取得可能)
- 要求を定式化する方法
- クエリビルダーの使用方法
- コレクションとページングを処理する方法  

## <a name="overview-of-the-migration-steps"></a>移行手順の概要

次の手順では、アプリが既に ADAL を使用して Azure AD Graph を呼び出すためのアクセストークンを取得していることを前提としています。これで、引き続き ADAL を使用することになります。 Msal への切り替えは、 [msal への移行](/graph/migrate-azure-ad-graph-authentication-library#migrate-to-msal)で説明されている個別の手順として実行できます。

1. Microsoft Graph へのアクセストークンを取得するには、 **Resourceurl**をから`https://graph.windows.net`に`https://graph.microsoft.com`更新します。

2. アプリで、次のように変更して Microsoft Graph クライアントライブラリへの参照を更新します。

    ``` csharp
    using Microsoft.Azure.ActiveDirectory.GraphClient;
    ```

    宛先：

    ``` csharp
    using Microsoft.Graph;
    ```

3. パッケージマネージャーを使用して、 [Microsoft Graph NuGet パッケージ](https://www.nuget.org/packages/Microsoft.Graph/)をダウンロードして更新し、依存関係を更新します。

4. を使用するのではなく`GraphServiceClient`、を作成`ActiveDirectoryClient`するようにクライアントのコンストラクターを更新します。  次のコードスニペットは、アプリが新しいトークン`AcquireTokenAsyncForUser()`を取得するためにメソッドを使用していることを前提としています。 このメソッドの定義は、 [dotnet-graphapi のサンプル](https://github.com/Azure-Samples/active-directory-dotnet-graphapi-console/blob/archive/GraphConsoleAppV3/AuthenticationHelper.cs)の一部として検索できます。

    変化

    ``` csharp
    ActiveDirectoryClient client = new ActiveDirectoryClient(serviceRoot,
    async () =\> await AcquireTokenAsyncForUser());
    ```

    宛先：

    ``` csharp
    GraphServiceClient graphClient = new GraphServiceClient(serviceRoot,
       new DelegateAuthenticationProvider(async (requestMessage) => {
          var token = await AcquireTokenAsyncForUser();
          requestMessage.Headers.Authorization = new
             AuthenticationHeaderValue("bearer", token);
       }));
    ```

    Microsoft Graph クライアントライブラリの場合、 `serviceRoot`この値にもバージョン番号が含まれています。 現時点では、この`https://graph.microsoft.com/v1.0`値はです。

5. Microsoft Graph クライアント要求ビルダー構文を使用するように要求を更新するには、次のように変更します。

    ``` csharp
    signedInUser = (User)await client.Me.ExecuteAsync();
    ```

    宛先：

    ``` csharp
    signedInUser = (User)await client.Me.Request().GetAsync();
    ```

    [!NOTE]
    Azure AD Graph クライアントライブラリでは、LINQ ベースのクエリ構文がサポートされていました。 ただし、Microsoft Graph クライアントライブラリにはありません。  そのため、関連するクエリをより RESTful 式に変換する必要があります。  

    これを行うには、次のように変更します。

    ``` csharp
    var groups = await
    client.Groups.Where(g =\> g.DisplayName.StartsWith("a")).ExecuteAsync();
    ```

    宛先：

    ``` csharp
    var groups = await
    client.Groups.Request().Filter("startswith(displayName,'a')").GetAsync();
    ```

6. コードでコレクションを使用してページを作成する場合は、次の小さな調整を行います。 次の例では、グループのフェッチと比較を、一度に5個ずつ、そのメンバーまでと比較します。 Azure AD Graph のコードでは、グループのメンバーをフェッチするために fetcher コンストラクトが必要ですが、Microsoft Graph にはそのような要件はありません。 それ以外の場合、コードは比較的似ています。  簡潔にするために、ユーザーメンバーのみが表示されます。 try/catch および error 条件は表示されず、コードスニペットはシングルスレッドコンソールアプリ用です。

    例として、Azure AD Graph .NET クライアントライブラリを使用して、次のコードを変更します。

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

    Microsoft Graph .NET クライアントライブラリを使用して、次のコードを実行します。

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

7. 通常、名前の変更に関連するリソース、プロパティ、ナビゲーション、およびサービスアクションのエラーを構築して修正します。

## <a name="see-also"></a>関連項目

[C# コンソールスニペットアプリ](https://github.com/microsoftgraph/console-csharp-snippets-sample)では、Microsoft Graph クライアントライブラリと Azure AD Graph クライアントライブラリの相違点の多くが強調されています。

Azure AD Graph クライアントライブラリでは、.NET プラットフォームのみがサポートされています。  ただし、Microsoft Graph クライアントライブラリでは、ソリューションにとってより便利な追加の[プラットフォームと言語](/graph)がサポートされています。

## <a name="next-steps"></a>次のステップ

- Microsoft Graph に移行したアプリを[展開、テスト、および拡張](/graph/migrate-azure-ad-graph-deploy-test-extend)する方法について説明します。
- [Microsoft Graph](/graph/overview)の概念とプラクティスについて説明します。
- [Graph エクスプローラー](https://aka.ms/ge)を使用して、Microsoft graph を試してみてください。
