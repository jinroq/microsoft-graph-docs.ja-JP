# <a name="use-microsoft-graph-to-integrate-with-onenote"></a>Microsoft Graph を使用して OneNote に統合する

アプリを OneNote に統合することで、世界中の数百万人のユーザーに到達する複数のプラットフォーム間で、強化されたエクスペリエンスを作成できます。 Microsoft Graph を使用して OneNote のノートブック、セクション、ページにアクセスし、ユーザーによるアイデアや情報の計画や整理を支援するソリューションを作成することができます。

## <a name="why-create-onenote-apps"></a>OneNote アプリを作成する理由

Microsoft Graph を使用して、ノート、リスト、画像、ファイルなどを OneNote ノートブックで作成して管理できます。

### <a name="collect-and-organize-notes-and-ideas"></a>メモやアイデアを収集して整理する  
コンテンツを追加したり、アレンジしたりできるキャンバスとして OneNote を使用します。 Microsoft Graph を使用すると、学生がメモを取って調査すること、家族が計画とアイデアを共有すること、買い物客が画像を共有することを可能にするアプリを簡単に作成できます。 アプリでは、みんなが必要とする情報を集め、OneNote に送り、それらを整理することができます。

### <a name="capture-information-in-many-formats"></a>さまざまな形式で情報をキャプチャする
HTML、埋め込み画像 (ローカルやパブリック URL にある)、ビデオ、オーディオ、メール メッセージ、その他の一般的なファイル タイプをキャプチャします。 OneNote では、Web ページや PDF ファイルをスナップショットとして表示することもできます。 Microsoft Graph は、OneNote ページ レイアウト用に標準 HTML および CSS のセットをサポートします。そのため、表、インライン イメージ、基本書式を使用して思いどおりの外観を実現できます。 

### <a name="use-the-onenote-ecosystem-to-enhance-your-core-scenarios"></a>OneNote エコシステムを使用して、コア シナリオを強化する
その他の強力な OneNote の機能を利用できます。 この Microsoft Graph の OneNote API では、イメージに対する OCR の実行、フルテキスト検索のサポート、クライアントの自動同期、イメージの処理、名刺キャプチャ、オンライン製品一覧やレシピ一覧の抽出などを実行できます。 メモや軽量メディアのクラウドでのデジタル メモリ ストアとして、またはドメイン固有データのデータ フィードとして OneNote を使用します。 

### <a name="reach-millions-of-onenote-users-on-all-major-platforms"></a>すべての主要プラットフォームの数百万人に上る OneNote ユーザーに到達する
OneNote を使用すると、アプリの使用量が増加します。 OneNote は新しい Windows デバイスにプレインストールされており、ほとんどのプラットフォームでオンライン、および Office 365 の一部として利用可能です。 機能の豊富な OneNote 環境を利用するアプリを公開すると、広範なクロスプラットフォーム市場の潜在的な可能性にアクセスできるようになります。

<!-- Might be good to show a few examples of Microsoft Graph API calls here, similar to what we have in the featured scenarios topic: https://developer.microsoft.com/en-us/graph/docs/concepts/featured_scenarios. You could have an H2 section called "What can I do with OneNote APIs in Microsoft Graph?"-->

## <a name="what-can-i-do-with-onenote-apis-in-microsoft-graph"></a>Microsoft Graph の OneNote API で実行できること

OneNote のリソースの操作で最もよく使用される要求の一部を次に示します。

|操作|URL|
|:--------|:--|
|自分のノートブックを取得する|[https://graph.microsoft.com/v1.0/me/onenote/notebooks](https://developer.microsoft.com/ja-JP/graph/graph-explorer?request=me/onenote/notebooks&version=1.0)|
|自分のセクションを取得する|[https://graph.microsoft.com/v1.0/me/onenote/sections](https://developer.microsoft.com/ja-JP/graph/graph-explorer?request=me/onenote/sections&version=1.0)|
|自分のページを取得する|[https://graph.microsoft.com/v1.0/me/onenote/pages](https://developer.microsoft.com/ja-JP/graph/graph-explorer?request=me/onenote/pages&version=1.0)|

## <a name="explore-the-onenote-apis"></a>OneNote API を使ってみる
[Microsoft Graph Explorer](https://developer.microsoft.com/ja-JP/graph/graph-explorer) を使用して、自分の OneNote ノートブックで OneNote API を試してみます。

Graph Explorer から OneNote API 呼び出しを行うには、左側の列にある **[その他のサンプルを表示]** を選択します。 メニューを使用して、OneNote を **[オン]** に切り替えます。 また、適切なアクセス許可を有効にする必要があります。 左側のメニューのアカウント名の下で、**[アクセス許可の修正]** を選択します。 OneNote のアクセス許可の詳細については、「[メモのアクセス許可](permissions_reference.md#notes-permissions)」を参照してください。

Microsoft Graph の OneNote API を使い始めるには、[OneNote 参照コンテンツ](../api-reference/v1.0/resources/onenote.md)に関する記事をご覧ください。

## <a name="see-also"></a>関連項目

* [ブランドのガイドライン](https://msdn.microsoft.com/ja-JP/office/office365/howto/onenote-branding)
* [OneNote コンテンツと構造を取得する](https://msdn.microsoft.com/ja-JP/office/office365/howto/onenote-get-content)
* [画像、ビデオ、ファイルを追加する](https://msdn.microsoft.com/ja-JP/office/office365/howto/onenote-images-files)
* [絶対配置要素を作成する](https://msdn.microsoft.com/ja-JP/office/office365/howto/onenote-abs-pos)
* [データを抽出する](https://msdn.microsoft.com/ja-JP/office/office365/howto/onenote-extract-data)
* [ノート シールを使用する](https://msdn.microsoft.com/ja-JP/office/office365/howto/onenote-note-tags)

