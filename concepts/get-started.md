# <a name="getting-started-building-microsoft-graph-apps"></a>Microsoft Graph アプリの構築を開始する

このセクションの記事では、Microsoft Graph に接続するアプリをさまざまな言語および開発プラットフォームで構築する方法を詳しく説明します。各記事では、まず該当するプラットフォームのサンプル スターター プロジェクトを説明し、次いでユーザー認証の機能を追加する手順を説明し、そのアカウントから Microsoft Graph でメールを送信するためのサンプル要求を作成します。完成したプロジェクトは、そのプラットフォーム用の [Microsoft Graph リポジトリの Connect サンプル](https://github.com/microsoftgraph?utf8=%E2%9C%93&query=connect)とまったく同じものです。

好みの認証プロバイダーと開発プラットフォームについて説明した記事を選び、Microsoft Graph への接続を開始します。 詳細については、「[v2.0 エンドポイントの相違点](https://docs.microsoft.com/en-us/azure/active-directory/develop/active-directory-v2-compare)」を参照してください。

選んだ開発プラットフォームについての記事に記載されている手順に従うことも、[クイック スタート](https://developer.microsoft.com/graph/quick-start)機能を試してみて、動作するソリューションをすばやく稼働させることもできます。

完成した Connect サンプルを確認するには、GitHub の「[Microsoft Graph](https://github.com/microsoftgraph)」を参照してください。 次の表は、認証プロバイダーとプラットフォームごとにサンプルをリストにしたもので、REST または Microsoft Graph クライアント ライブラリのどちらを使用して Microsoft Graph に接続するかを示しています。


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

- [サンプルの REST 呼び出しを Graph エクスプローラーでお試しください](https://developer.microsoft.com/en-us/graph/graph-explorer)
- [Azure AD エンドポイントのドキュメント](https://docs.microsoft.com/en-us/azure/active-directory/develop/active-directory-developers-guide)
- [Azure AD v2.0 エンドポイントのドキュメント](https://docs.microsoft.com/en-us/azure/active-directory/develop/active-directory-appmodel-v2-overview)
