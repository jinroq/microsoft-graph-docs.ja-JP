---
title: Microsoft Graph API で Postman を使用する
description: Microsoft Graph Postman のコレクションを使用して、Microsoft Graph API をすぐに開始できます。
author: ''
localization_priority: Priority
ms.openlocfilehash: 2140dec07328b75f7b1729cd3e7cf7c86e65f738
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36038186"
---
# <a name="use-postman-with-the-microsoft-graph-api"></a>Microsoft Graph API で Postman を使用する

Microsoft Graph Postman のコレクションを使用して、Microsoft Graph API をすぐに開始できます。

![Postman の画像](https://github.com/microsoftgraph/microsoftgraph-postman-collections/blob/master/images/postman.png?raw=true)

この記事では、Postman と Microsoft Graph の使用方法について説明します。 
  [Graph Explorer](https://developer.microsoft.com/ja-JP/graph/graph-explorer) を使用して、web ブラウザーで直接 Microsoft Graph API を検索することもできます。

## <a name="accessing-the-collection"></a>コレクションへのアクセス
Postman のコレクションにアクセスするには、2 つの方法があります。使用する方法、付与する方法です。 最初にコンピューターで [Postman](https://www.getpostman.com/) を実行している必要があります。

### <a name="consume-the-collection"></a>コレクションを使用する
Microsoft Graph API の使用を開始するには、コレクションを使用するのが最も簡単な方法です。 [Postman 共有リンク](https://www.getpostman.com/collections/d89a737b5f0c0825898a) によって Postman が起動します。

共有コレクションを使用する利点は、追加の作業をすることなく、新しい要求が自動的に表示されることです。

コレクションを取得したら、環境変数をセットアップする必要があります。

1. **[ファイル | インポート ...]** を選択します。
2. **[URL からインポートする]** を選択します。
3. 次の URL をコピーして貼り付け、**[インポート]** を選択します。
 
    ```
    https://raw.githubusercontent.com/microsoftgraph/microsoftgraph-postman-collections/master/Microsoft%20Graph%20v1.0.postman_environment.json
    ```

右上のドロップダウンに目のアイコンで **Microsoft Graph 環境** が表示されます。 次に、[環境の設定](#using-the-collection)をする必要があります。

### <a name="contribute-to-the-collection"></a>コレクションに付与する
独自の要求を付与する場合は、[Microsoft Graph Postman コレクション](https://github.com/microsoftgraph/microsoftgraph-postman-collections)の github リポジトリにフォークする必要があります。 

詳細については、次のビデオをご覧ください。

> [!VIDEO https://www.youtube-nocookie.com/embed/4tg-OBdv_8o]

Postman コレクションをインポートするには:

1. [Postman](https://www.getpostman.com/) をダウンロードして登録します。
2. **[ファイル | インポート ...]** を選択します。
3. **[URL からインポートする]** を選択します。
4. 次の 2 つの URL を貼り付けて **[インポート]** を選択します。

    ```
      https://raw.githubusercontent.com/microsoftgraph/microsoftgraph-postman-collections/master/Microsoft%20Graph%20v1.0.postman_collection.json
      
    ```
    ```
      https://raw.githubusercontent.com/microsoftgraph/microsoftgraph-postman-collections/master/Microsoft%20Graph%20v1.0.postman_environment.json

    ```

**[コレクション]** ウィンドウに **Microsoft Graph v1.0** コレクションが表示されます。

## <a name="using-the-collection"></a>コレクションの使用
Postman に **Microsoft Graph v1.0** コレクションと **Microsoftr Graph 環境** を取得したら、次の手順を実行します。

### <a name="set-up-application-api-calls"></a>アプリケーション API の呼び出しを設定する

1. 右上隅の **[環境なし]** ドロップダウンを選択します。
2. **[Microsoft Graph 環境]** を選択します。
3. 右の **目**のアイコンを選択し、**[編集]** を選択します。
4. **カレント** (非**初期**) 変数で Microsoft ID アプリケーションを入力します: **ClientID**、**ClientSecret**、**TenantID**。 
 アプリケーションの作成方法、およびアプリのみのフローの管理方法の詳細については、[Postman を使用して Microsoft Graph を呼び出す](https://developer.microsoft.com/en-us/graph/blogs/30daysmsgraph-day-13-postman-to-make-microsoft-graph-calls/) ブログの投稿を参照してください。

5. **[更新]** を選択します。 **[環境の管理]** ダイアログボックスを閉じます。 **MicrosoftGraph v1.0 | アプリケーション** コレクションの左側の、**[アプリ専用アクセス トークンの取得]** を選択します。 右側の **[送信]** を選びます。
6. **アプリケーション | ユーザー** フォルダーを展開し、**[ユーザーの取得]** を選択します。 次に **[送信]** を選択します。

Microsoft Graph v 1.0 コレクションを使用する準備ができました。。

>**Note:** コレクション内の他の API を実行する場合は、アプリケーションに必要なアクセス許可に同意する必要があります。

### <a name="set-up-on-behalf-of-api-calls"></a>代理として API 呼び出しを設定する
代理として API 呼び出しを設定するには、環境設定で、**ユーザー名** と **ユーザー パスワード** を設定し、**ユーザーの代理 | ユーザーのアクセス トークンを取得 ** を使用します。 

>**重要:** この情報は Postman に直接格納されるため、実稼働ユーザーアカウントを使用することはお勧めしません。 また、この方法を使用して、運用環境でアクセス トークンを取得することもお勧めしません。 テスト目的にのみ使用ください。

ユーザー名とパスワードを Postman cloud アカウントに同期する環境変数に格納しない場合は、**[新しいアクセス トークンの取得]** 機能を使用して、Postman を終了せずにトークンを取得できます。

1. **ユーザーの代理 | Postman を使用してアクセス トークンを取得する ** を選択します。
2. **[承認]** タブを選択します。
3. **[アクセス トークンを取得する]** ボタン選択します。
4. 実際のテナントとアプリケーションの値を、次のボックスに入力します。 ここでは環境変数を使用できません。実際の値を使用する必要があります。 Portal.azure.com のアプリケーションブレードで **EndPoints** を選ぶと、値を見つけることができます。

    - コールバック URL: https://app.getpostman.com/oauth2/callback
    - 認証 URL: https://login.microsoftonline.com/**TENANTID**/oauth2/v2.0/authorize
    - アクセス トークン URL: https://login.microsoftonline.com/**TENANTID**/oauth2/v2.0/token
    - クライアント ID: **CLIENTID**
    - クライアントシークレット: **CLIENTSECRET**
    - スコープ: https://graph.microsoft.com/.default
    - 状態: **RANDOMSTRING**
 
5. **トークンを要求する**を選択する。 サインインと同意の許可を求める UI プロンプトが表示されます。
6. アクセス トークンをコピーし、環境変数を開いて、 **UserAccessToken** フィールドに貼り付けます。

すべての依頼が機能するようになりました。
