# <a name="use-the-microsoft-graph-api-to-work-with-project-rome"></a>Microsoft Graph API を使用して Project Rome を操作するには

[Project Rome](https://developer.microsoft.com/en-us/windows/project-rome) は、クロス デバイスのエクスペリエンス プラットフォームを構築するために Microsoft が構想したものです。 Project Rome により、ユーザーがクライアントのデバイスでサインインするために使用するのと同じ Microsoft アカウントを使用してサインインする場合に、ローカル クライアントまたはサービス上のアプリが、リモート ホスト上のアプリおよびサービスと対話をすることが可能になります。 これにより、デバイスではなくユーザー タスクを中心に構築されたクロス デバイスおよびクロス プラットフォームのエクスペリエンスをプログラムすることができます。

重要なコンポーネントはこれらのエクスペリエンス、つまりアクティビティを可能にするために、Microsoft Graph を使用して公開されます。

## <a name="activities"></a>アクティビティ

Microsoft Graph のアクティビティにより、デバイスやプラットフォームをまたがったアプリとのユーザー エンゲージメントを推進することができます。 アクティビティはユーザー エンゲージメントの構成単位で、3 つのコンポーネントで構成されています：

- ディープ リンク
- 視覚表示
- [http://schema.org/](http://schema.org/) で共有されたボキャブラリを使用した、アクティビティを記述するコンテンツのメタデータ

アプリケーションによってセッションが作成されると、履歴項目がアクティビティに追加され、ユーザー エンゲージメントの期間が反映されます。 ユーザーがアクティビティに再エンゲージするたびに、新しい履歴項目がアクティビティに追加され、ユーザー エンゲージメントが蓄積されます。

アプリケーションがユーザー アクティビティのオブジェクトを公開する場合、オブジェクトは Windows の新しい UI サーフィスのいくつかに表示されます。例：Cortana の通知とタイムライン アクティビティのオブジェクトで、豊富なメタデータ（アクティビティを適切なコンテンツに表示するためのもの）と豊富なビジュアル（[Adaptive Card](http://adaptivecards.io/) のマークアップを使用）を指定することができます。

次の Microsoft Graph API を使用して、アクティビティを作成して読み出すことができます。

- [アクティビティを作成または置換する](../api/projectrome_put_activity.md)
- [アクティビティを取得する](../api/projectrome_get_activities.md)
- [最近のアクティビティを取得する](../api/projectrome_get_recent_activities.md)
- [アクティビティを削除する](../api/projectrome_delete_activity.md)
- [履歴項目を作成または置換する](../api/projectrome_put_historyitem.md)
- [履歴項目を削除する](../api/projectrome_delete_historyitem.md)