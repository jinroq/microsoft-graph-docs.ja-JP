---
title: Visual Studio 2017 での Microsoft Graph API を使った Office 365 サービスの呼び出し
description: Visual Studio の接続済みサービスを使い、アプリケーションから Microsoft Graph API を呼び出せるよう設定できます。この記事では、サインインしているユーザーのプロフィール写真を取得し、OneDrive へアップロードし、写真の共有リンクを記載したメールを送信する方法を説明します。
ms.openlocfilehash: 33469dec7014d81ed55c2efceb96a26c2651d239
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27092437"
---
# <a name="call-office-365-services-in-visual-studio-2017-with-the-microsoft-graph-api"></a>Visual Studio 2017 での Microsoft Graph API を使った Office 365 サービスの呼び出し

Visual Studio の接続済みサービスを使い、アプリケーションから Microsoft Graph API を呼び出せるよう設定できます。この記事では、サインインしているユーザーのプロフィール写真を取得し、OneDrive へアップロードし、写真の共有リンクを記載したメールを送信する方法を説明します。

## <a name="get-set-up"></a>設定する

Office 365 接続済みサービスを Microsoft Graph と共に使用するには、以下の手順を実行する必要があります。

- [Visual Studio 2017 プレビュー](https://www.visualstudio.com/vs/preview/)をまだダウンロードしていない場合は、ダウンロードします。Visual Studio の以前のバージョンを使用している場合は、それと合わせて Visual Studio 2017 プレビューを使用できます。

- Office 365 サブスクリプションを入手します。無料試用版を取得するには、[Office 365 開発者プログラム](https://dev.office.com/devprogram)に参加します。

## <a name="get-the-starter-project"></a>スタート プロジェクトをセットアップする

[Microsoft Graph ASP.NET 接続済みサービスサンプル](https://github.com/microsoftgraph/aspnet-connect-sample/archive/Office365connectedservice.zip)をダウンロードします。このサンプルには、Microsoft Graph で認証を行うために必要な参照が含まれています。スタート プロジェクトをダウンロードし、解凍して、Visual Studio 2017 プレビューでサンプルを開きます。

## <a name="add-the-connected-service"></a>接続済みサービスの追加

Microsoft Graph のサービスを Visual Studio プロジェクトに追加する準備が整いました。 

1. ソリューション エクスプローラーで、[**接続済みサービス**] を選択し、[接続済みサービス] タブを開きます。 

2. [**Microsoft Graph を使用して Office 365 サービスにアクセスする**] プロバイダーを選択します。ウィザードの手順に従います。次のアクセス許可を選択します (アクセス許可は後で変更することができます)。

    - **File** API のアクセス許可は**ファイルへのフルアクセス許可**を設定します。
    - **Mail** API のアクセス許可は**ユーザーとしてのメールの送信**を設定します。
    - **User** API のアクセス許可は**サインインとユーザー プロファイルの読み取り**を設定します。

## <a name="call-the-microsoft-graph-api"></a>Microsoft Graph API の呼び出し

最初のサンプルは、単純な電子メールを送信する設定です。Microsoft Graph を使ってサンプルを編集し、サインインしているユーザーの、One Drive にあるプロフィール写真へのリンクが記載されたメールを送信するようにできます。

1. Microsoft Graph を呼び出すコードがある 'Models\GraphService.cs' に移動します。

2. 以下のメソッドにある SDK への呼び出しを検索し、**コメントを解除**します。Microsoft Graph を呼び出してプロフィール写真を取得し、ファイルを One Drive にアップロードし、共有リンクを取得する方法を示します。

    ```csharp
        GetCurrentUserPhotoStream(GraphServiceClient graphClient)
    ```
    
    ```csharp
        UploadFileToOneDrive(GraphServiceClient graphClient, byte[] file)
    ```

    ```csharp
        GetSharingLink(GraphServiceClient graphClient, string Id)
    ```
 
> **ヒント:** コメントは "//Uncomment:" で始まります。
 

## <a name="run-the-sample"></a>サンプルを実行する
サンプルの構築と実行次に、右上の [**サインイン**] リンクを選択します。続いて、[**メールアドレス取得**]、[**メール送信**] を選択します。

これにより、プロフィール写真へのリンクが記載されたメールが送信されます。

>**メモ:**

>- サンプルの実行を Visual Studio から停止し、再度実行した場合は、明示的なサインアウトが必要となることがあります。
>- ユーザーが認証されていないことを示すエラーが発生する場合、[接続済みサービスの追加](#add-the-connected-service)手順を再度行います。
    

## <a name="explore-the-code"></a>コードを理解します。

これで、サービスの接続と設定を Visual Studio 2017 から行えるようになりました。最初のサンプルでは、スキャフォールディングと参照を作成できます。  

このサンプルには、次のファイルが含まれています。

- [Startup.Auth.cs](https://github.com/microsoftgraph/aspnet-connect-sample/tree/Office365connectedservice/Microsoft%20Graph%20SDK%20ASPNET%20Sample/Microsoft%20Graph%20SDK%20ASPNET%20Sample/App_Start/Startup.Auth.cs): 現在のユーザーを認証して、サンプルのトークン キャッシュを初期化します。

- Models\\[SessionTokenCache.cs](https://github.com/microsoftgraph/aspnet-connect-sample/tree/Office365connectedservice/Microsoft%20Graph%20SDK%20ASPNET%20Sample/Microsoft%20Graph%20SDK%20ASPNET%20Sample/TokenStorage/SessionTokenCache.cs):ユーザーのトークンの情報を格納します。これを独自のカスタム トークン キャッシュと置き換えることができます。詳細については、「[マルチテナント アプリケーションのアクセス トークンのキャッシュ](https://azure.microsoft.com/ja-JP/documentation/articles/guidance-multitenant-identity-token-cache/)」を参照してください。

- Models\\[SampleAuthProvider.cs](https://github.com/microsoftgraph/aspnet-connect-sample/tree/Office365connectedservice/Microsoft%20Graph%20SDK%20ASPNET%20Sample/Microsoft%20Graph%20SDK%20ASPNET%20Sample/Helpers/SampleAuthProvider.cs): ローカルの IAuthProvider インターフェイスを実装して、アクセス トークンを取得します。 

- Helpers\\[SDKHelper.cs](https://github.com/microsoftgraph/aspnet-connect-sample/tree/Office365connectedservice/Microsoft%20Graph%20SDK%20ASPNET%20Sample/Microsoft%20Graph%20SDK%20ASPNET%20Sample/Helpers/SDKHelper.cs):Microsoft Graph との対話に使用される [Microsoft Graph .NET クライアント ライブラリ](https://github.com/microsoftgraph/msgraph-sdk-dotnet)から **GraphServiceClient** を初期化します。

- Controllers\\[HomeController.cs](https://github.com/microsoftgraph/aspnet-connect-sample/tree/Office365connectedservice/Microsoft%20Graph%20SDK%20ASPNET%20Sample/Microsoft%20Graph%20SDK%20ASPNET%20Sample/Controllers/HomeController.cs):Microsoft Graph サービスを構築して呼び出しを送信し、その応答を処理するために **GraphServiceClient** を使用するメソッドが含まれています。

- Views\\Home\\[Graph.cshtml](https://github.com/microsoftgraph/aspnet-connect-sample/tree/Office365connectedservice/Microsoft%20Graph%20SDK%20ASPNET%20Sample/Microsoft%20Graph%20SDK%20ASPNET%20Sample/Views/Home/Graph.cshtml):サンプル用の UI が入っています。 


## <a name="need-help"></a>サポートが必要な場合

ヘルプが必要な場合は、[StackOverflow](https://stackoverflow.com/questions/tagged/microsoftgraph?sort=newest) に質問を投稿してください。ご質問には {microsoftgraph} のタグを付けてください。

