# <a name="use-the-microsoft-graph-api"></a>Microsoft Graph API を使用する

Microsoft Graph は、Microsoft Cloud サービス リソースへのアクセスを可能にする RESTful Web API です。 [アプリを登録](auth_register_app_v2.md) して、[サービス](auth_v2_service.md) または [ユーザーの認証トークンを取得する](auth_v2_user.md) と、Microsoft Graph API に対して要求を行うことができます。

> **重要:**条件付きアクセス ポリシーの Microsoft Graph への適用方法は変更されています。 条件付きアクセス ポリシーが構成されるシナリオを処理するよう、アプリケーションを更新する必要があります。 詳細およびガイダンスについては、「[Azure Active Directory の条件付きアクセスについての開発者ガイド]((https://docs.microsoft.com/azure/active-directory/develop/active-directory-conditional-access-developer))」を参照してください。

ユーザーや電子メール メッセージなど、リソースの読み取りや書き込みを行うには、次のような要求を構築します。

```http
https://graph.microsoft.com/{version}/{resource}?query-parameters
```

要求のコンポーネントには以下が含まれます。

* [HTTP メソッド](#http-methods) - Microsoft Graph への要求で使用する HTTP メソッド。
* [`{version}`](#version) - アプリケーションが使用している Microsoft Graph API のバージョン。
* [`{resource}`](#resource) - ユーザーが参照している Microsoft Graph のリソース。
* [クエリ パラメーター](#query-parameters-optional) - 要求または応答を変更するパラメーターのオプションのセット。

要求を行うと、次を含む応答が返されます。 

* 状態コード - 成功または失敗を示す HTTP 状態コード。 HTTP エラー コードの詳細については、「[エラー](errors.md)」を参照してください。
* 応答メッセージ - 要求したデータ、または操作の結果。応答メッセージは、いくつかの操作で空になる場合があります。
* **[次へ]** リンク - 要求が大量のデータを返す場合は、**[次ヘ]** を選択して、ページを進める必要があります。 詳細については、「[ページング](paging.md)」を参照してください。

## <a name="http-methods"></a>HTTP メソッド

Microsoft Graph は、要求で HTTP メソッドを使用し、要求が何を行っているかを特定します。API は次のメソッドをサポートしています。


|**メソッド** |**説明**                             |
| :----- | :------------------------------------------- |
| GET    | リソースからデータを読み取ります。                   |
| POST   | 新しいリソースを作成、または処理を実行します。 |
| PATCH  | リソースを新しい値で更新します。           |
| PUT    | リソースを新しいものと置換します。           |
| DELETE | リソースを削除します。                           |

* メソッド **GET** と **DELETE** では、要求本文は必要ありません。
* **POST**、**PATCH**、および **PUT** メソッドは、通常 JSON 形式で指定されている要求本文を必要とし、それには、リソースのプロパティの値などの追加の情報が含まれます。

## <a name="version"></a>バージョン

Microsoft Graph は、現在 `v1.0` と `beta` の 2 つのバージョンをサポートしています。

* `v1.0` には、一般公開されている API が含まれます。 すべての運用アプリで、v1.0 バージョンを使用します。
* `beta` には、現在プレビュー段階の API が含まれます。 ベータ版 API に重大な変更を導入する可能性があるため、開発中のアプリのテストにのみ、ベータ版を使用することをお勧めします。運用アプリでは、ベータ版 API を使用しないでください。

ベータ版 API のフィードバックを常に募集しています。 フィードバックの提供または機能のご要望は、「[UserVoice]((https://officespdev.uservoice.com/))」ページを参照してください。

API のバージョンに関する詳細については、「[バージョン管理とサポート](versioning_and_support.md)」を参照してください。

## <a name="resource"></a>リソース

ユーザーの URL には、要求で操作するリソースが含まれます。たとえば、`me`、`users`、`groups`、`drives`、`sites` などです。 最上位のリソースそれぞれにも、**リレーションシップ**が含まれます。`me/messages` または `me/drive` のように、追加のリソースにアクセスするのに使用できます。 **メソッド**を使用して、リソースを操作することもできます。たとえば、電子メールを送信するには `me/sendMail` を使用します。

リソースのリレーションシップおよびメソッドを移動する方法に関する詳細については、「[グラフをスキャンする](traverse_the_graph.md)」を参照してください。 

各リソースにアクセスするために異なるアクセス許可が必要になる可能性があります。リソースの作成または更新には、リソースの読み取りよりも高いレベルのアクセス許可が必要になります。必要なアクセス許可に関する詳細については、メソッドの参照トピックを参照してください。 

アクセス許可に関する詳細については、「[アクセス許可の参照](permissions_reference.md)」を参照してください。

## <a name="query-parameters-optional"></a>クエリ パラメーター (オプション)

Microsoft Graph アプリで応答をカスタマイズするには、オプションのクエリ パラメーターを使用できます。クエリ パラメーターを使用して、既定の応答よりも多い、または少ないプロパティを含めたり、カスタム クエリに一致するアイテムの応答をフィルター処理したり、メソッドの追加のパラメーターを提供したりします。

たとえば、次のフィルター パラメーターを追加すると、メッセージが `jon@contoso.com` の `emailAddress` プロパティを持つものだけに返されるよう制限されます。

```http
https://graph.microsoft.com/v1.0/me/messages?filter=emailAddress eq 'jon@contoso.com'
```

クエリ パラメーターに関する詳細については、「[応答をカスタマイズする](query_parameters.md)」を参照してください。

## <a name="next-steps"></a>次の手順

Microsoft Graph を使用して、起動および実行する準備ができました。 詳細について知るには、[Graph エクスプローラー]((https://developer.microsoft.com/ja-JP/graph/graph-explorer))に移動して、いくつかの要求や[クイック スタート]((https://developer.microsoft.com/ja-JP/graph/quick-start))を試したり、「[SDK とコード サンプル]((https://developer.microsoft.com/ja-JP/graph/code-samples-and-sdks))」のいずれかを使用して開始したりします。
