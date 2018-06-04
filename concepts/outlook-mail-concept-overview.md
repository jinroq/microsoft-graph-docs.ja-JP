# <a name="outlook-mail-api-overview"></a>Outlook メール API の概要

Outlook は、Office 365 のメッセージング通信ハブです。 これにより、連絡先の管理、会議のスケジュール管理、組織内のユーザーに関する情報の検索、オンライン会話の開始、ファイルの共有、およびグループでの共同作業をすることができます。

## <a name="why-integrate-with-outlook-mail"></a>Outlook メールと統合する理由

### <a name="integrate-with-rich-features-and-reach-hundreds-of-millions-of-customers"></a>豊富な機能を統合して何億というユーザーに達する

Outlook を統合するなら、多くのユーザーの好む豊かなエクスペリエンスを取り入れることになります。それは、メール、[連絡先](outlook-contacts-concept-overview.md)、[予定表](outlook-calendar-concept-overview.md)のための直感的で一貫したエクスペリエンスであり、モバイル、Web、およびデスクトップのどのデバイス上でも利用可能です。

[Microsoft Graph](overview.md) を使用することにより、アプリを 1 回だけ作成することにより Outlook と統合することができ、Outlook をメール クライアントとして選んでいる何億人という消費者、何千万という組織ユーザーに達することができます。 メール シナリオを中心としたアプリを作成したり、Outlook および 非 Outlook の他のリレーションシップ、リソース、およびインテリジェンスの宝庫に接続したり、Microsoft クラウドによってサポートされるシナリオを実現したりすることができます。

### <a name="automate-message-organization-and-processing"></a>メッセージの整理と処理を自動化する

多くのユーザーは、Outlook で情報を整理するのを好んでいます。 Microsoft Graph により、それらの機能をアプリ開発者が利用することができ、情報の発見作業を最適化し、効率や生産性を向上させるユーザー ワークフローを構築することができます: 

- ユーザーは、さまざまな方法でメッセージを整理できます。メッセージを全部受信トレイに入れたまま検索する人もいれば、複数のフォルダーにメッセージを分類保存する人もいます。 フラットな整理方法とフォルダー ベースの整理方法の両方をサポートする Outlook の柔軟で直感的なアプローチがユーザーに好まれています。 アプリでは、特定のフォルダー内のメッセージまたはユーザーのメールボックス全体のメッセージに対して[フィルター処理、検索、またはソート](query_parameters.md)を便利に実行することができます。

- Outlook では、名前と色によってカテゴリが区別されます。 カテゴリを利用することによりユーザーは、メッセージにタグを付けて、整理や情報発見の作業をさらに便利なものにすることができます。 アプリでは、[ユーザーのカテゴリ マスター リストにアクセスしたり定義したり](../api-reference/v1.0/api/outlookuser_post_mastercategories.md)できます。 さらにそのリストは、Outlook のメッセージ、またイベント、連絡先、タスク、およびグループ投稿を通じて共有され、アプリ開発者にとってクリエイティブなシナリオの可能性をもたらします。 たとえば、オンライン研修業者であれば、電子メール、コース イベント、およびフォローアップ課題を、ユーザーが登録しているコースごとに色分けすることができます。

- さらに、アプリのユーザーは、メッセージ (あるいは、イベントまたはタスク) の重要度を変更したり、メッセージにフォローアップ用のフラグを付けたりすることができます。 (現時点で Microsoft Graph のフラグの機能は[プレビュー段階](versioning_and_support.md#beta-version)です。)

- ルール API を利用すれば、メッセージの整理がさらに上のレベルになります。 アプリでは、[受信トレイ ルール](../api-reference/v1.0/resources/messagerule.md)をセットアップすることにより、受信メッセージを迅速に処理し、メールが乱雑な状態になるのを軽減できます。 たとえば、アプリにより、メッセージの件名に特定のキーワードが含まれている場合にメッセージを別のフォルダーに移動したり、後でそれに対応する作業を容易にするためにカテゴリや重要度を割り当てたりすることができます。

### <a name="write-smarter-apps-that-leverage-intelligence"></a>インテリジェンスを活用した高度なアプリを作成する 

Microsoft Graph を利用することにより、アプリ ユーザーに対してコンテキスト データを提案することができます:

- [優先受信トレイ](../api-reference/v1.0/resources/manage_focused_inbox.md)および [@ メンション (プレビュー)](../api-reference/beta/api/message_get.md#request-2) を統合し、アプリ ユーザーが気になっているものを最初に読み、返信できるようにする。 

- メッセージ作成中に[メール ヒント (プレビュー)](../api-reference/beta/resources/mailtips.md) をチェックして、受信者に関する有用な情報を得る (受信者が自動返信を送信中なのか、あるいはメールボックスがいっぱいなのかなど)。 メール ヒントは、アプリに対して特定の条件を警告することにより、フォローアップのアクションの効率を上げることができます。 

- [連絡先 API](people_example.md) の利用により、アプリの中で連絡先を選択するなど、対話式のコントロールが提供されます。 連絡先 API では、ユーザーの通信および共同作業のパターン、そしてビジネス上の付き合いに基づいて、ユーザーに最も関係の深い連絡先を提案することができます。 

- アプリ ユーザーに対して、メッセージ作成中に添付ファイルに関連して、気の利いたファイル選択機能を提供したり、最近利用したファイルを提案したりする。 [Insights](../api-reference/beta/resources/insights.md) では、高度な分析機能を使用することにより、ユーザーの周辺で頻繁に使用されるファイル、最近ユーザーが表示または編集したファイル、あるいはそのユーザーと共有したファイルについての提案がなされます。


### <a name="store-app-data-in-a-resource-or-resource-instance"></a>アプリ データをリソースまたはリソース インスタンスに保存する

アプリでは、データを外部データ ストアに保存するために、データの管理とアクセスのためのオーバーヘッドが発生することが少なくありません。 アプリで Microsoft Graph を使用すれば、単に[カスタム データを個々のリソース インスタンスに保存](extensibility_overview.md#open-extensions)するか、あるいは該当する場合には、スキーマを拡張し、カスタム プロパティを追加して、Microsoft Graph リソースの中に型指定されたデータを保存することができます。 そのような[スキーマ拡張](extensibility_overview.md#schema-extensions)を、検出可能また共有可能なものにすることができます。 


## <a name="next-steps"></a>次の手順

- [Graph Explorer](https://developer.microsoft.com/graph/graph-explorer/?request=me%2Fmessages&version=v1.0) で Outlook メール サンプル クエリを選択して試行する。 左側の列の **[サンプルをさらに表示]** を選択します。 メニューを使用して **Outlook メール** をオンにします。
- 以下について調べます。

  - [メッセージの作成と送信](outlook-create-send-messages.md)
  - [メッセージの整理方法](outlook-organize-messages.md)
  - [メッセージ フォルダーを共有する](outlook-share-messages-folders.md)方法

- Microsoft Graph v1.0 での[メール API の使用](../api-reference/v1.0/resources/mail_api_overview.md) とその[用途](../api-reference/v1.0/resources/mail_api_overview.md#common-use-cases)について調べる。


