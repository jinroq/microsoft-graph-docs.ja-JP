# <a name="microsoft-graph-quick-start-faq"></a>Microsoft Graph のクイック スタートのよくあるご質問

この「よくあるご質問」では、[Microsoft Graph のクイック スタート](https://developer.microsoft.com/en-us/graph/quick-start)のいずれかを実行する際に発生する可能性がある質問や問題について扱います。

## <a name="what-do-the-quick-starts-do"></a>クイック スタートでは何ができますか。

選択したプラットフォームに関係なく、各クイック スタートでは次の処理が行われます。

- [アプリケーション登録ポータル](https://apps.dev.microsoft.com)で新規アプリケーションを登録します。 このため、**アプリケーション ID を取得**する際に Microsoft アカウントでサインインする必要があります。 アプリケーションでアプリ シークレットが必要な場合、クイック スタートで作成されます。 
- GitHub リポジトリに格納されているサンプル コードのコピーをダウンロードします。 これらのリポジトリは、GitHub の [MicrosoftGraph 組織](https://github.com/microsoftgraph?utf8=%E2%9C%93&q=connect)にあります。
- 新しいアプリ ID と、必要に応じてアプリ シークレットを GitHub リポジトリに格納されているサンプル コード内の構成ファイルに挿入します。 HTTP 要求内の機密情報が送信されることを避けるため、新しいアプリケーションを作成した後にアプリ シークレットをコピーし、サンプルのコピーをダウンロードする前にそれをクイック スタートのフォームにコピーしてください。
- 完全に構成されたサンプルをダウンロードするようにダイアログが表示されます。 サンプル コードをダウンロードして解凍すると、稼働するはずのクライアントまたは Web のアプリケーションが出現します。これは、指定された前提条件 (IDE、Web フレームワークなど) が開発環境にインストールされていることを前提としています。


## <a name="why-wont-my--aspnet-uwp-or-xamarin-project-build"></a>ASP.NET、UWP、または Xamarin プロジェクトがビルドされないのはなぜですか。

.NET ライブラリを使用するサンプルが Visual Studio でのビルドに失敗した場合、1 つまたは複数のプロジェクトで、Windows の 260 文字のパス長の制限に引っかかることがあります。 特に、Xamarin ソリューションの場合、Xamarin ソリューション内の Android プロジェクトがこの影響を受けやすくなります。 ソリューションをルート ディレクトリまたはそれに近い場所に移動してみてください。 

## <a name="if-a-web-platform-quick-start-provides-rest-and-sdk-samples-can-i-run-them-both-at-the-same-time"></a>Web プラットフォームのクイック スタートで REST および SDK のサンプルが提供されている場合、それらを同時に実行できますか。

はい、同時に両方のサンプルを実行できます。 ただし、既定のポートでいずれかが実行されていないことを確認してください。 つまり、Web サーバーのテストを開始するとき、サンプルの少なくとも 1 つのバージョンに対してポート番号を指定する必要があります。

## <a name="i-didnt-get-an-email-and-i-see-no-errors-or-exceptions-why-didnt-this-work"></a>電子メールを受信できません。エラーまたは例外は表示されていません。 なぜ正しく動作しないのですか。

電子メールを送信するサンプルが表示されるものの、受信トレイに表示されない場合は、迷惑メール フォルダーを確認してください。 テスト テナントからメッセージを送信する場合、メッセージにスパムのフラグが付く場合があります。

## <a name="i-get-an-error-when-i-try-to-sign-in-and-authorize-the-sample-app-what-steps-can-i-take-to-fix-this"></a>サインインして、サンプル アプリを承認しようとするとエラーが発生します。 この問題を解決するにはどのような手順を実行したらよいですか。 

最初に、InPrivate または Incognito ウィンドウでサンプル アプリを実行します。 特に、複数の Microsoft アカウントでサインインした場合、Web ブラウザーのキャッシュ設定が原因で承認の手順が失敗することがあります。 これが機能しない場合は、[スタック オーバーフロー](https://stackoverflow.com/questions/tagged/microsoft-graph)でフォローアップしてください。 Microsoft graph を使用して質問にタグを付け、エラー情報を質問にコピーしてください。

## <a name="why-do-some-quick-starts-include-an-app-secret-and-others-dont"></a>一部のクイック スタートにアプリ シークレットが含まれ、他のクイック スタートにはそれが含まれないのはなぜですか。

Microsoft Graph API のセキュリティで保護された呼び出しを行う必要があるサーバー側の Web アプリケーションには、アプリ シークレットが必要です。 このため、ASP.NET MVC、Node.js、PHP、および Ruby のクイック スタートではアプリ シークレットが提供されます。

## <a name="why-doesnt-the-angular-quick-start-give-me-an-app-secret-when-all-the-other-web-platform-quick-starts-do"></a>他のすべての Web プラットフォームのクイック スタートではアプリ シークレットが提供されるのに、Angular クイック スタートでは提供されないのはなぜですか。

アプリ シークレットを必要とするのは、サーバー側の Web アプリケーションのみです。

## <a name="why-does-my-quick-start-contain-a-readme-file"></a>クイック スタートに Readme ファイルが含まれているのはなぜですか。

各クイック スタートは、新しいアプリケーションを登録し、GitHub リポジトリの内容が含まれた zip ファイルを作成します。 さらに、リポジトリ内のサンプル アプリケーションを構成しなくてもよいように、リポジトリ内のファイルを更新します。 これらのリポジトリは、GitHub の [MicrosoftGraph 組織](https://github.com/microsoftgraph?utf8=%E2%9C%93&q=connect)にあります。

各クイック スタートに関連付けられているリポジトリを自由に参照して、そこで問題をファイリングし、Readme にある指示に従って自身のアプリケーションを登録してください。 関連付けられているリポジトリにアクセスするには、各クイック スタートのステップ 2 の下にある「**サンプル コードのみを入手する**」リンクに従ってください。

## <a name="why-did-the-sample-give-me-an-image-containing-a-thought-bubble"></a>サンプルの画像に考えを示す吹き出しが含まれているのはなぜですか。

クイック スタートで提供されるサンプルのほとんどは、プロファイル画像を取得し、それを OneDrive アカウントのルート ディレクトリにアップロードします。 Microsoft アカウント (live.com、hotmail.com) でサインインしている場合、Microsoft Graph は現時点ではプロファイル画像をフェッチできないため、考えを示す吹き出しの画像に戻されます。 アカウントにプロファイル画像が存在しない場合、サンプルもこの画像を使用します。

## <a name="why-do-you-provide-a-manage-your-apphttpsappsdevmicrosoftcom-link-after-i-get-an-app-id"></a>アプリ ID を取得した後に**[アプリの管理](https://apps.dev.microsoft.com)** リンクが表示されるのはなぜですか。

このリンクが表示されるのは、アプリ ID の手順で[アプリケーション登録ポータル](https://apps.dev.microsoft.com)に新規アプリケーションを登録するためです。 このリンクを使用して、このアプリケーションの設定を表示したり、アプリケーションを削除したり、サンプルを実行した後にアプリケーションの設定を更新したりすることもできます。 

## <a name="didnt-find-what-you-need"></a>必要な情報が見つかりませんか。

お尋ねになりたい質問や、1 つまたは複数のクイック スタートで発生した問題が、この「よくあるご質問」に記載されていない場合は、[スタック オーバーフロー](https://stackoverflow.com/questions/tagged/microsoft-graph)でお知らせください。 

クイック スタートに付属のコード サンプルに関連した問題については、GitHub サンプル リポジトリで問題をファイリングすることもできます。 リポジトリを検索するには、各クイック スタートのステップ 2 の下にある「**サンプル コードのみを入手する**」リンクにアクセスします。
