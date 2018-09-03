# <a name="microsoft-teams-api-overview-preview"></a>Microsoft Teams API の概要 (プレビュー)

Microsoft Teams は、チームワークおよびインテリジェントな通信のための究極のハブです。 1 億 2 千万人を超えるユーザーが利用する Office 365 のパワーと規模に基づいて構築されている Microsoft Teams は、チャット ベースのコラボレーション、会議、通話、およびエンタープライズ ボイスのさまざまな機能を提供します。

## <a name="why-integrate-with-microsoft-teams"></a>Microsoft Teams を統合する理由

Microsoft Teams を統合することにより、独自のサービスやアプリを構築したり、何百万というエンタープライズ ユーザーに達したり、共同作業を支援したりすることが容易になります。 Microsoft Graph を使用することによって、チーム、チャネル、メッセージなどを作成し、管理することができます。

### <a name="use-microsoft-graph-in-any-kind-of-app"></a>あらゆる種類のアプリで Microsoft Graph を使用する

Microsoft Graph 上に構築された Microsoft Teams アプリは、コラボレーションの生産性を向上させ、コラボレーションをさらに推進するための新たなツールを作業グループに提供します。 Microsoft Teams を使用することにより作業グループのユーザーは、資産を共有したり、チャットで対話したり、チームの予定表でイベントの予定を管理したりできます。 Microsoft Teams API に基づくアプリを通じてチーム、チャネル、および会話の自動化機能を追加することにより、Microsoft Teams の価値をさらに高めてください。

Web サイト、サービス、およびネイティブ プラットフォーム アプリケーションは、Microsoft Teams のユーザー エクスペリエンス内では実行されませんが、Microsoft Teams の自動化シナリオを有効にする Microsoft Teams API を呼び出すために使用することができます。

**Microsoft Teams 対応のアプリの種類**

![Microsoft Teams API をタブ、ボット、Web サイト、およびサービスから呼び出す](images/TeamsAppEndpoints.png)

これらのコラボレーション ツールには、Microsoft Teams 内部で実行される Microsoft Graph 対応のタブまたはボット アプリが含まれます。 また、Web サイトまたは Web サービスからなど、Microsoft Teams アプリの外部で Microsoft Graph を呼び出すこともできます。 すでに Web サイトが Microsoft Graph 対応になっている場合、[Microsoft Teams デベロッパー プラットフォーム](https://docs.microsoft.com/en-us/microsoftteams/platform/#pivot=home&panel=home-all)を使用して、既存の Web サイト コードを使用するタブ アプリを作成することにより、そのサイトの機能を Microsoft Teams のために使用することができます。

Microsoft Teams タブまたはボット アプリがシナリオに適したものではない場合は、アプリの種類として次のいずれかを選んでください。

|アプリの種類|シナリオの説明|
|:-------|:-------------------|
|タブ|Microsoft Teams 内での拡張コンテンツを表示します。|
|コネクタ|拡張更新内容をチャネルに投稿します。|
|アクション可能なメッセージング|拡張対話機能をコネクタ カードに追加します。|
|Web サイト|Web ページに拡張コンテンツを表示します。|
|ボット|会話の中でタスクを実行するようユーザーを支援します。|
|アクティビティ フィード|フィード通知によりユーザーの参加を促します。|
|メッセージング拡張機能|ユーザーが会話の中で拡張カードに関するクエリを実行したり共有したりできるようにします。|
|サービス|Web サービスによりクライアント アプリケーションを拡張して Microsoft Graph データを使用できるようにします。|

### <a name="create-multiple-teams-and-channels"></a>複数のチームおよびチャネルを作成する

顧客が、アプリにリンクした新しい[チーム](../api-reference/beta/resources/team.md)および[チャネル](../api-reference/beta/resources/channel.md)を作成できるようにします。 Microsoft Teams API の使用により、数多くのチームの作成やそこへのユーザーとチャネルの登録の作業を容易にします。

### <a name="automate-team-lifecycles"></a>チーム ライフサイクルを自動化する

Microsoft Graph を使用することにより、業務上の新しい問題が発生した場合に新しい仮想チームを作成し、適切な人を[チームに登録](../api-reference/v1.0/api/group_post_members.md)し、チャネルによりチームを構成します。 業務上の新しい問題に関するチーム チャネル ディスカッションを開始するには、新しいチーム メンバーに対する歓迎メッセージを投稿するための新しい会話スレッドをチャネルで開始することができます。 新しいチームで業務上の問題について話し合うには、新しいイベントをチーム予定表に追加し、チームのメンバーをそのイベントに招待します。

業務上の問題が解決し、その仮想チームが不要になったら、Microsoft Teams API を使用してチームを破棄します。 仮想チームを作成する時点で最大期間がわかっている場合は、そのチームについて [Office 365 グループ有効期限ポリシー](https://support.office.com/en-us/article/office-365-group-expiration-policy-8d253fe5-0e09-4b3c-8b5e-f48def064733?ui=en-US&rs=en-US&ad=US)を設定することにより、そのポリシーに従ってチームが自動で削除されます。

## <a name="next-steps"></a>次の手順

- [Microsoft Teams API の使用](../api-reference/beta/resources/teams_api_overview.md)方法を確認する。
- [チーム](../api-reference/beta/resources/team.md)、[チャネル](../api-reference/beta/resources/channel.md)、および [グループ](../api-reference/v1.0/resources/group.md)のリソースのメソッド、プロパティ、およびリレーションシップについて詳しく調べる。
- [Graph エクスプローラー](https://developer.microsoft.com/en-us/graph/graph-explorer)で API をお試しください。
- [Microsoft Teams プログラミング モデル](https://docs.microsoft.com/en-us/microsoftteams/platform/concepts/concepts-overview)に関する詳細を読む。
- [サンプル コード](https://github.com/OfficeDev/microsoft-teams-sample-graph)を試す。
