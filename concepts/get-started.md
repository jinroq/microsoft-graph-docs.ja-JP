# <a name="getting-started-building-microsoft-graph-apps"></a>Microsoft Graph アプリの構築を開始する

このセクションの記事では、Microsoft Graph に接続するアプリをさまざまな言語および開発プラットフォームで構築する方法を詳しく説明します。 各記事で、スタート プロジェクトをはじめ、Microsoft Graph への接続の基本ステップをたどりながら解説します。

 1. アプリケーションを登録する
 2. アプリケーションで、ユーザーを認証し、アクセス トークンを取得する
 3. アプリケーションから Microsoft Graph を呼び出す
 4. アプリケーションを実行する

ソリューションを起動し、より素早く実行したい場合は、[クイック スタート](https://developer.microsoft.com/graph/quick-start)をお試しください。

完成した各プロジェクトは、そのプラットフォーム用の [Microsoft Graph リポジトリの Connect サンプル](https://github.com/microsoftgraph?utf8=%E2%9C%93&query=connect)とまったく同じものです。

さらにコードをご覧になりますか?

GitHub の [Microsoft Graph サンプル](https://github.com/microsoftgraph) をすべて調べることができます。 次の表は、このセクションで取り上げているサンプルの追加バージョンの一覧です。 両方の ADAL エンドポイント (v1.0 と v2.0) でユーザーを認証し、未加工の REST 呼び出しまたは Microsoft Graph クライアント ライブラリ (SDK) を使って Microsoft Graph に接続する方法を示します。

(好みの認証プロバイダーと開発プラットフォームについて説明した記事を選び、Microsoft Graph への接続を開始します。 詳細については、「[v2.0 エンドポイントの相違点](https://docs.microsoft.com/ja-JP/azure/active-directory/develop/active-directory-v2-compare)」を参照してください。)


|プラットフォーム |Azure AD エンドポイント |Azure AD v2.0 エンドポイント |
|:--- |:--- |:---|
|Android |<a href="https://github.com/microsoftgraph/android-java-connect-sample/tree/last_v1_auth">SDK サンプル</a> |<a href="https://github.com/microsoftgraph/android-java-connect-sample">SDK サンプル</a> または <a href="https://github.com/microsoftgraph/android-java-connect-rest-sample">REST サンプル</a> |
|AngularJS |<a href="https://github.com/microsoftgraph/angular-connect-rest-sample/tree/last_v1_auth">REST サンプル</a> |<a href="https://github.com/microsoftgraph/angular-connect-sample">SDK サンプル</a> または <a href="https://github.com/microsoftgraph/angular-connect-rest-sample">REST サンプル</a> |
|ASP.NET |<a href="https://github.com/microsoftgraph/aspnet-connect-rest-sample/tree/last_v1_auth">REST サンプル</a> |<a href="https://github.com/microsoftgraph/aspnet-connect-sample">SDK サンプル</a> または <a href="https://github.com/microsoftgraph/aspnet-connect-rest-sample">REST サンプル</a> |
|iOS (Obj-C) |<a href="https://github.com/microsoftgraph/ios-objectivec-connect-rest-sample">REST サンプル</a> |<a href="https://github.com/microsoftgraph/ios-objectivec-connect-sample">SDK サンプル</a> |
|iOS (Swift) |<a href="https://github.com/microsoftgraph/ios-swift-connect-rest-sample">REST サンプル</a> |<a href="https://github.com/microsoftgraph/ios-swift-connect-sample">SDK サンプル</a> |
|NodeJS |<a href="https://github.com/microsoftgraph/nodejs-connect-rest-sample/tree/last_v1_auth">REST サンプル</a> |<a href="https://github.com/microsoftgraph/nodejs-connect-sample">SDK サンプル</a> または <a href="https://github.com/microsoftgraph/nodejs-connect-rest-sample">REST サンプル</a> |
|PHP |<a href="https://github.com/microsoftgraph/php-connect-rest-sample/tree/last_v1_auth">REST サンプル</a> |<a href="https://github.com/microsoftgraph/php-connect-sample">SDK サンプル</a> または <a href="https://github.com/microsoftgraph/php-connect-rest-sample">REST サンプル</a> |
|Python |<a href="https://github.com/microsoftgraph/python-sample-auth/blob/master/sample_adal.py">REST サンプル</a> |<a href="https://aka.ms/graph-python-samples">REST サンプル</a>
|Ruby |<a href="https://github.com/microsoftgraph/ruby-connect-rest-sample/tree/last_v1_auth">REST サンプル</a> |<a href="https://github.com/microsoftgraph/ruby-connect-rest-sample">REST サンプル</a> |
|UWP |<a href="https://github.com/microsoftgraph/uwp-csharp-connect-rest-sample/tree/last_v1_auth">REST サンプル</a> |<a href="https://github.com/microsoftgraph/uwp-csharp-connect-sample">SDK サンプル</a> または <a href="https://github.com/microsoftgraph/uwp-csharp-connect-rest-sample">REST サンプル</a> |
|Xamarin | |<a href="https://github.com/microsoftgraph/xamarin-csharp-connect-sample">SDK サンプル</a> |

<br/>

## <a name="see-also"></a>関連項目

- [サンプルの REST 呼び出しを Graph エクスプローラーでお試しください](https://developer.microsoft.com/ja-JP/graph/graph-explorer)
- [Azure AD エンドポイントのドキュメント](https://docs.microsoft.com/ja-JP/azure/active-directory/develop/active-directory-developers-guide)
- [Azure AD v2.0 エンドポイントのドキュメント](https://docs.microsoft.com/ja-JP/azure/active-directory/develop/active-directory-appmodel-v2-overview)
