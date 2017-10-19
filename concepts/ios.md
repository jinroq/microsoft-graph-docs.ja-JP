# <a name="ios-samples-for-the-microsoft-graph-api"></a>Microsoft Graph API の iOS サンプル
この記事では、Office 365 またはコンシューマ Outlook ユーザーなどの管理されたサービス アカウント (MSA) に対してユーザーを認証する 2 つの iOS サンプルについて説明します。 どちらのサンプルも、Outlook サービスを通じて電子メールを送信しますが、一方のサンプルはユーザーのプロファイル写真を取得して、それを電子メールの本文で送信して機能を拡張しています。

## <a name="ios-objective-c-connect-rest-sample"></a>iOS Objective C Connect REST サンプル
このサンプルでは、標準の iOS HTTPS ライブラリを使用して Microsoft Graph に REST 呼び出しを行います。 Microsoft 認証ライブラリ (MSAL) を使用してユーザーを認証します。 MSAL ライブラリでは、アプリが Office 365 または MSA アカウントからユーザーを認証できます。 ただし、オンプレミスの Azure Active Directory インスタンスからのユーザーは認証できません。

このサンプルでは、電子メールを送信できますが、認証されたユーザーの写真を取得したり、それを電子メールに埋め込んだりすることはできません。

- [Objectve C iOS アプリで Microsoft Graph を使ってみる](ios_objectivec.md)

## <a name="ios-swift-sonnect-sample"></a>iOS Swift Sonnect のサンプル
このサンプルでは、Objective C 向けの Microsoft Graph クライアント ライブラリを使用して Microsoft Graph エンドポイントにアクセスします。 ユーザー認証はサードパーティの [NXOAuth2Client](https://github.com/nxtbgthng/OAuth2Client) ライブラリで処理されます。 このライブラリでは、アプリがオンプレミスの Azure Active Directory インスタンスからのユーザーを認証しますが、MSA ユーザーは認証しません。

サンプルでは、Graph を介してどのようにユーザーの Azure プロファイルにアクセスするかを示しています。 ユーザーのプロファイル写真を取得する方法、その写真をユーザーの OneDrive ストレージにアップロードする方法、およびその写真を Outlook 電子メール メッセージの本文に埋め込む方法についても説明します。

- [iOS アプリで Microsoft Graph を使ってみる](ios_swift.md)