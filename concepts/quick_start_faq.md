# <a name="microsoft-graph-quick-start-faq"></a>Microsoft Graph のクイック スタートのよくあるご質問

この FAQ は、[Microsoft Graph Quick Starts](https://developer.microsoft.com/en-us/graph/quick-start) に関連する質問に回答します。

## <a name="what-do-the-quick-starts-do"></a>クイック スタートでは何を行うでのすか。

クイック スタートのサンプルでは、Microsoft Graph の機能にアクセスする方法を示します。 

Office 365 の REST API を使用する場合は、呼び出したいサービスに対して認証を行う必要があります。 Microsoft Graph では、認証を統合し、単一のエントリ ポイントによってすべての API にアクセスできるようにすることで、この複雑さが解消されています。 一度認証を受けさえすれば、複数のアプリケーションとサービスに及ぶ情報にアクセスできるようになりました。 

Microsoft Graph のクイック スタートでは、1 回の認証で 3 つのサービスにアクセスします。Microsoft アカウント、OneDrive、Outlook です。 各クイック スタートでは、Microsoft アカウントのユーザー プロファイル情報にアクセスし、データを OneDrive (写真) へ書き込み、Outlook を使用して電子メールを (その写真へのリンクを含めて) 生成します。 

クイック スタートには、次の 4 つのステップがあります。
- プラットフォームを選択する、 
- アプリ ID (別名: クライアント ID) を取得する、
- サンプルをビルドする、
- サインインして電子メールでプロフィール写真を送信する、という 4 つのステップがあります。

クイック スタートを完了すると、すぐに実行できるアプリがあります。


## <a name="general-quick-start-sample-questions"></a>クイック スタートのサンプルに関する一般的な質問
このセクションでは、クイック スタートのサンプルの編成と内容に関する質問に回答します。

### <a name="why-does-my-quick-start-contain-a-readme-file"></a>クイック スタートに readme ファイルが含まれているのはなぜですか。

各クイック スタートでは、新しいアプリケーションを登録し、GitHub リポジトリの内容が含まれた zip ファイルを作成します。 さらに、リポジトリ内のサンプル アプリケーションを構成しなくてもよいように、リポジトリ内のファイルを更新します。 これらのリポジトリは、GitHub の [MicrosoftGraph 組織](https://github.com/microsoftgraph?utf8=%E2%9C%93&q=connect)にあります。

各クイック スタートに関連付けられているリポジトリを自由に参照して、そこで問題をファイリングし、Readme にある手順に従ってご自身のアプリケーションを登録してください。 リポジトリにアクセスするには、各クイック スタートのステップ 2 の下にあるリンクの「**サンプル コードのみを入手する**」を参照してください。

### <a name="which-microsoft-graph-features-do-the-quick-start-samples-use"></a>クイック スタートのサンプルで使用するのは、Microsoft Graph のどの機能ですか。

クイック スタート サンプルは継続的に更新されています。 更新プログラムを入手するには、該当するサンプルのリポジトリを確認してください。 機能を追加すると、サンプルの readme ファイルが新しい情報で更新されます。 次の表に各サンプルの現在の機能を示します。
 +<!-- Replace the check mark images with an actual character that can be read by a screen reader. Or you could add alt text to each instance of the image. -->

|サンプル|認証|プロフィール画像の取得|OneDrive への画像のアップロード|電子メールでの共有リンク|電子メールへの画像の添付|電子メールの送信|
|-----:|-----:|-----:|------:|------:|------:|-----:|
|[Android 用の接続](https://github.com/microsoftgraph/android-java-connect-sample)|![](./images/Check.PNG)|![](./images/Check.PNG)|![](./images/Check.PNG)|![](./images/Check.PNG)|![](./images/Check.PNG)|![](./images/Check.PNG)|
|[Angular 2 用の接続](https://github.com/microsoftgraph/angular-connect-sample)|![](./images/Check.PNG)| | | | |![](./images/Check.PNG)|
|[Angular 2 用の接続 REST](https://github.com/microsoftgraph/angular2-connect-rest-sample)|![](./images/Check.PNG)| | | | |![](./images/Check.PNG)|
|[ASP.NET 用の接続](https://github.com/microsoftgraph/aspnet-connect-sample)|![](./images/Check.PNG)|![](./images/Check.PNG)|![](./images/Check.PNG)|![](./images/Check.PNG)|![](./images/Check.PNG)|![](./images/Check.PNG)|
|[iOS 用の接続 - Swift](https://github.com/microsoftgraph/ios-swift-connect-sample)|![](./images/Check.PNG)|![](./images/Check.PNG)|![](./images/Check.PNG)|![](./images/Check.PNG)|![](./images/Check.PNG)|![](./images/Check.PNG)|
|[iOS 用の接続 REST - Objective C](https://github.com/microsoftgraph/ios-objectivec-connect-rest-sample)|![](./images/Check.PNG)| | | | |![](./images/Check.PNG)|[](./images/Check.PNG)|
|[Node.js 用の接続 REST](https://github.com/microsoftgraph/nodejs-connect-rest-sample)|![](./images/Check.PNG)|![](./images/Check.PNG)|![](./images/Check.PNG)|![](./images/Check.PNG)| |![](./images/Check.PNG)|
|[php 用の接続 REST](https://github.com/microsoftgraph/php-connect-rest-sample)|![](./images/Check.PNG)| | | | |![](./images/Check.PNG)|
|[php 用の接続](https://github.com/microsoftgraph/php-connect-sample)|![](./images/Check.PNG)| | | | |![](./images/Check.PNG)|
|[Ruby 用の接続 REST](https://github.com/microsoftgraph/ruby-connect-rest-sample)|![](./images/Check.PNG)| | | | |![](./images/Check.PNG)|
|[UWP 用の接続](https://github.com/microsoftgraph/uwp-csharp-connect-sample) |![](./images/Check.PNG)|![](./images/Check.PNG)|![](./images/Check.PNG)|![](./images/Check.PNG)|![](./images/Check.PNG)|![](./images/Check.PNG)|
|[Xamarin 用の接続](https://github.com/microsoftgraph/uwp-csharp-connect-sample)|![](./images/Check.PNG)|![](./images/Check.PNG)|![](./images/Check.PNG)|![](./images/Check.PNG)|![](./images/Check.PNG)|![](./images/Check.PNG)|

## <a name="authentication-and-authorization"></a>認証と承認
このセクションでは、認証と承認の問題に関連する質問に回答します。 

### <a name="why-dont-any-of-the-quick-start-samples-show-advanced-authentication-use-cases"></a>どのクイック スタートのサンプルも、高度な認証のユース ケースを示していないのはなぜですか。

クイック スタートのサンプルでは、認証と Microsoft Graph API 呼び出しの概要を示しています。 認証と Microsoft Graph API 呼び出しを実稼働アプリケーションに追加する場合、セキュリティや条件付きアクセスの問題に関わる高度な認証シナリオを設計する方法を認識している必要があります。

使用する認証ライブラリに対する高度な認証シナリオの詳細を、以下の認証ライブラリの発行元のページにアクセスして確認できます。

- [Android と iOS 用の OAuth2Client](https://github.com/nxtbgthng/OAuth2Client)
- [Node 用の Passport](http://passportjs.org/)
- [PHP 用の Illuminate Auth](https://github.com/illuminate/auth)
- [Python 3 用の Flask](https://pypi.python.org/pypi/Flask-OAuth2-Provider/0.2.1)
- [Ruby 用の OmniAuth](https://github.com/omniauth/omniauth)
- [.NET 用の Microsoft Authentication Library (MSAL)](https://github.com/AzureAD/microsoft-authentication-library-for-dotnet)
- [Android 用の Microsoft Authentication Library](https://github.com/AzureAD/microsoft-authentication-library-for-android)
- [JavaScript 用の Microsoft Authentication Library](https://github.com/AzureAD/microsoft-authentication-library-for-js)

## <a name="microsoft-graph-api"></a>Microsoft Graph API
このセクションでは、Microsoft Graph API を使用するアプリケーションのコーディングに関する質問に回答します。

### <a name="i-didnt-get-an-email-and-i-dont-see-any-errors-or-exceptions-why-didnt-this-work"></a>電子メールを受信できません。エラーも例外も表示されていません。 なぜ正しく動作しないのですか。

電子メールを送信するサンプルが表示されるものの、受信トレイに表示されない場合は、迷惑メール フォルダーを確認してください。 テスト テナントからメッセージを送信する場合、メッセージにスパムのフラグが付く場合があります。

### <a name="why-doesnt-the-email-sent-by-the-sample-have-my-profile-picture"></a>サンプルによって送信された電子メールに自分のプロフィール画像が添付されないのはなぜですか。

これは通常、プロフィールがユーザーのプロフィール画像を使って設定されていないためです。 Microsoft アカウントを使用してサインインした場合、プロフィール画像がある場合でも、その画像は電子メールに表示されません。 Microsoft Graph API では、Microsoft アカウントからのユーザーのプロフィール画像を現在サポートしていません。 クイック スタートのサンプルのほとんどは、プロファイル画像を取得し、それを OneDrive アカウントのルート ディレクトリにアップロードします。 Microsoft アカウント (live.com、hotmail.com) でサインインしている場合、Microsoft Graph は現時点ではプロファイル画像をフェッチできないため、考えを示す吹き出しの画像に戻されます。

Node iOS Objective C のサンプルでは、ユーザーのプロフィール画像が電子メール メッセージに添付されません。 

## <a name="aspnet"></a>ASP.NET
このセクションでは、ASP.NET クイック スタートのサンプルのコーディング、ビルド、または実行に関連する質問に回答します。

### <a name="why-wont-my-aspnet-project-build"></a>ASP.NET プロジェクトがビルドされないのはなぜですか。
.NET ライブラリを使用するサンプルが Visual Studio でのビルドに失敗した場合、1 つまたは複数のプロジェクトで、Windows の 260 文字のパス長の制限に引っかかることがあります。 ソリューションをルート ディレクトリまたはそれに近い場所に移動してみてください。 

## <a name="universal-windows-platform-uwp"></a>ユニバーサル Windows プラットフォーム (UWP)
このセクションでは、UWP クイック スタートのサンプルのコーディング、ビルド、または実行に関連する質問に回答します。

### <a name="why-wont-my-uwp-project-build"></a>UWP プロジェクトがビルドされないのはなぜですか。
.NET ライブラリを使用するサンプルが Visual Studio でのビルドに失敗した場合、1 つまたは複数のプロジェクトで、Windows の 260 文字のパス長の制限に引っかかることがあります。 ソリューションをルート ディレクトリまたはそれに近い場所に移動してみてください。 

## <a name="xamarin"></a>Xamarin
このセクションでは、Xamarin クイック スタートのサンプルのコーディング、ビルド、または実行に関連する質問に回答します。

### <a name="why-wont-my-xamarin-project-build"></a>Xamarin プロジェクトがビルドされないのはなぜですか。

.NET ライブラリを使用するサンプルが Visual Studio でのビルドに失敗した場合、1 つまたは複数のプロジェクトで、Windows の 260 文字のパス長の制限に引っかかることがあります。 特に、Xamarin ソリューションの場合、Xamarin ソリューション内の Android プロジェクトがこの影響を受けやすくなります。 ソリューションをルート ディレクトリまたはそれに近い場所に移動してみてください。 

## <a name="web-stack-samples"></a>Web スタックのサンプル
このセクションでは、Web テクノロジを使ってビルドされたクイック スタートのサンプルのコーディング、ビルド、または実行に関連する質問に回答します。

### <a name="how-do-i-know-if-my-local-computer-supports-a-local-web-server"></a>ローカル コンピューターでローカル Web サーバーをサポートしているかどうかはどうすればわかりますか。
Web テクノロジに基づくクイック スタートのサンプルでは、ローカル Web サーバーの起動とホストに必要なロジックが用意されています。 たとえば、PHP 5.4.0 以上のランタイムに基づく PHP のサンプルには、開発のために使用する[組み込みの Web サーバー](http://php.net/manual/en/features.commandline.webserver.php)が含まれています。 これは、実稼働環境での使用が想定されていません。 

Node.js のサンプルをダウンロードした場合は、この「[Node.js ファースト ステップ ガイド](https://nodejs.org/en/docs/guides/getting-started-guide/)」を確認して、Node Web サーバーの起動について学習してください。 

ASP.NET のサンプルの場合、Visual Studio 2015 以降のバージョンには、このサンプルを実行すると自動的に起動される開発用 Web サーバーが含まれています。 この Web サーバーを使用するためのサンプル プロジェクトを構成する必要はありません。 

Ruby 用接続のサンプルの [Readme](https://github.com/microsoftgraph/ruby-connect-rest-sample/blob/master/README.md) には、Ruby のローカル Web サーバーを起動するために必要な手順が記載されています。 

### <a name="if-a-web-platform-quick-start-provides-rest-and-sdk-samples-can-i-run-them-both-at-the-same-time"></a>Web プラットフォームのクイック スタートで REST および SDK のサンプルが提供されている場合、それらを同時に実行できますか。

はい、同時に両方のサンプルを実行できます。 ただし、既定のポートでいずれかが実行されていないことを確認してください。 つまり、Web サーバーのテストを開始するとき、サンプルの少なくとも 1 つのバージョンに対してポート番号を指定する必要があります。

### <a name="why-do-some-quick-starts-include-an-app-secret-and-others-dont"></a>一部のクイック スタートにアプリ シークレットが含まれ、他のクイック スタートにはそれが含まれないのはなぜですか。

Microsoft Graph API のセキュリティで保護された呼び出しを行う必要があるサーバー側の Web アプリケーションには、アプリ シークレットが必要です。 このため、ASP.NET MVC、Node.js、PHP、および Ruby のクイック スタートではアプリ シークレットが提供されます。

### <a name="why-doesnt-the-angular-quick-start-give-me-an-app-secret-when-all-the-other-web-platform-quick-starts-do"></a>他のすべての Web プラットフォームのクイック スタートではアプリ シークレットが提供されるのに、Angular クイック スタートでは提供されないのはなぜですか。

アプリ シークレットを必要とするのは、サーバー側の Web アプリケーションのみです。

### <a name="i-get-an-error-when-i-try-to-sign-in-and-authorize-the-sample-app-what-steps-can-i-take-to-fix-this"></a>サインインして、サンプル アプリを承認しようとするとエラーが発生します。 この問題を解決するにはどのような手順を実行したらよいですか。 

最初に、InPrivate または Incognito ウィンドウでサンプル アプリを実行します。 特に、複数の Microsoft アカウントでサインインした場合、Web ブラウザーのキャッシュ設定が原因で承認の手順が失敗することがあります。 これが機能しない場合は、[スタック オーバーフロー](https://stackoverflow.com/questions/tagged/microsoft-graph)でフォローアップしてください。 必ず Microsoft Graph を使用して質問にタグを付け、エラー情報を質問にコピーしてください。

## <a name="didnt-find-what-you-need"></a>必要な情報が見つかりませんか。

1 つまたは複数のクイック スタートで生じた疑問や問題が、この「よくあるご質問」に記載されていない場合は、[スタック オーバーフロー](https://stackoverflow.com/questions/tagged/microsoft-graph)でお知らせください。 ご質問には "microsoft-graph" のタグを付けてください。

クイック スタートに付属のコード サンプルに関連した問題については、GitHub サンプル リポジトリで問題をファイリングすることもできます。 リポジトリを検索するには、各クイック スタートのステップ 2 の下にあるリンクの「**サンプル コードのみを入手する**」をクリックします。
