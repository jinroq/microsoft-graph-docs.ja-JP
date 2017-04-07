# <a name="contribute-to-microsoft-graph-documentation"></a>Microsoft Graph ドキュメントへの投稿

Microsoft Graph ドキュメントにご関心をお寄せいただき、ありがとうございます。

* [投稿する方法](#ways-to-contribute)
* [プル要求が承諾される前](#before-we-can-accept-your-pull-request)
* [GitHub、Git、およびこのリポジトリを使用する](#use-github-git-and-this-repository)
* [Markdown を使用してトピックを書式設定する方法](#how-to-use-markdown-to-format-your-topic)
* [標準の Markdown](#standard-markdown)
* [その他のリソース](#more-resources)

## <a name="ways-to-contribute"></a>投稿する方法

[Microsoft Graph ドキュメント](http://graph.microsoft.io)には、次の方法で投稿できます。

* [公開されている Microsoft Graph 開発者向けドキュメント リポジトリ](https://github.com/microsoftgraph/microsoft-graph-docs)から記事を投稿する
    * /beta 分岐か、/v1.0 分岐、またはその両方に個別のプル要求を送信します。この手順は、バージョンの分岐が、常に最後の変更が反映された最新の状態であるようにするために必要です。 
    * また、/master 分岐に別のプル要求を送信します。これは、Microsoft Graph Web サイトのドキュメント サイトが常に最新の変更で更新されるようにするための手順です。 
* [GitHub の [問題]](https://github.com/microsoftgraph/microsoft-graph-docs/issues) を使用してドキュメントの不具合を報告する
* 「[Office Developer Platform UserVoice](http://officespdev.uservoice.com)」サイトにドキュメント要求を追加します。

##<a name="before-we-can-accept-your-pull-request"></a>プル要求が承諾される前

###<a name="minor-corrections"></a>細かな修正

このリポジトリのドキュメントとコード例に対して提出した細かな修正や説明には、投稿者のライセンス同意書 (CLA) は必要ありません。提出は、プル要求の形式で行われます。プル要求は 10 営業日以内に確認するよう最善を尽くします。


###<a name="larger-submissions"></a>大規模な提出

次のグループのいずれかに該当する場合は、ドキュメントとコード例への新規または重要な変更を提出する際に、署名した投稿者のライセンス同意書 (CLA) をプル要求が承諾される前に送信する必要があります。

* Microsoft Open Technologies グループのメンバー
* Microsoft の従業員でない投稿者

コミュニティ メンバーは、**このプロジェクトへの大規模な提出を行う前に投稿者のライセンス同意書 (CLA) に署名する必要があります**。ただし、ドキュメントの完了と提出を行う必要があるのは 1 度のみです。ドキュメントを慎重に確認してください。雇用主によるドキュメントへの署名が必要になる場合もあります。

投稿者のライセンス同意書 (CLA) への署名により、メイン リポジトリにコミットする権限が付与されるわけではありませんが、Office Developer および Office Developer Content Publishing チームが投稿の確認と検討を行えるようになります。また、必要に応じて自身の名義が入ります。

投稿者のライセンス同意書 (CLA) は、[こちら](https://github.com/microsoftgraph/microsoft-graph-docs/raw/master/Contribution%20License%20Agreement.pdf)でダウンロードできます。フォームに記入して、電子メールで [officedev@microsoft.com](mailto:officedev@microsoft.com) に送信してください。

CLA を受領、処理したのち、10 営業日以内にプル要求を確認するよう最善を尽くします。

## <a name="use-github-git-and-this-repository"></a>GitHub、Git、およびこのリポジトリを使用する

**注:**このセクションの情報のほとんどは、「[GitHub ヘルプ] []」の記事で見つけることができます。Git と GitHub のことをよく知っている場合は、「**コンテンツを投稿して編集する**」のセクションまでスキップして、このリポジトリのコード / コンテンツ フローの詳細を参照してください。

### <a name="setting-up-your-fork-of-the-repository"></a>リポジトリのフォークのセットアップ

1.    このプロジェクトに投稿できるように、GitHub のアカウントをセットアップします。まだ行っていない場合は、今すぐ [GitHub ホーム] []にアクセスしてセットアップします。
2.    Git でマシンをセットアップします。[[Git セットアップ チュートリアル]] [Set Up Git] の指示に従います。
3.    このリポジトリの独自のフォークを作成します。これを行うには、ページの上部にある **[フォーク]** ボタンをクリックします。
4.    フォークをローカル コンピューターにコピーします。これを行うには、GitBash に移動して開きます。コマンド プロンプトで、次のように入力します。

        git clone https://github.com/{your user name}/microsoft-graph-docs.git

    次に、以下のコマンドを入力してルート リポジトリへの参照を作成します。

        cd microsoft-graph-docs   git remote add upstream https://github.com/microsoftgraph/microsoft-graph-docs.git   git fetch upstream

おめでとうございます。リポジトリをセットアップできました。今後、同じ手順をもう一度繰り返す必要はありません。

### <a name="contribute-and-edit-content"></a>コンテンツを投稿して編集する

投稿プロセスをできるだけシームレスにするため、以下の手順に従ってください。

1. 新しい分岐を作成します。
2. 新しい内容を追加するか、既存の内容を編集します。
3. メイン リポジトリにプル リクエストを提出します。
4. 分岐を削除します。

ワークフローを効率化してマージによる競合の可能性を減らすため、各分岐を単一の概念/記事に限定してください。新しい分岐には、次の種類の投稿が適しています。

* 新しい記事 (および関連する画像)
* 記事のスペル チェックと文法の編集
* 大規模な記事セット全体への単一の書式設定変更の適用 (たとえば、新しい著作権フッターの適用)。

#### <a name="create-a-new-branch"></a>新しい分岐を作成する

1.    GitBash を開きます。
2.    プロンプトで `git pull upstream master:<new branch name>` を入力します。これにより、最新の *microsoftgraph* マスター分岐からコピーされた新しい分岐がローカルに作成されます。**注:**内部投稿者の場合は、コマンドの `master` を、対象にしている発行日の分岐に置き換えます。
3.    プロンプトで `git push origin <new branch name>` を入力します。これにより、新しい分岐に関するアラートが GitHub に送信されます。これで、GitHub 上のリポジトリのフォーク内に新しい分岐が表示されるはずです。
4.    `git checkout <new branch name>` を入力して、新しい分岐に切り替えます。

#### <a name="add-new-content-or-edit-existing-content"></a>新しい内容を追加するか既存の内容を編集する

エクスプローラーを使用して、ローカル コンピューター上のリポジトリに移動します。リポジトリ ファイルは、`C:\Users\<yourusername>\microsoft-graph-docs` にあります。

ファイルを編集するには、好みのエディターで開いて変更します。新しいファイルを作成するには、好みのエディターを使用して、リポジトリのローカル コピー内の適切な場所に新しいファイルを保存します。作業中は、必ず頻繁に作業内容を保存してください。

`C:\Users\<yourusername>\microsoft-graph-docs` 内のファイルは、ローカル リポジトリ内で作成した新しい分岐の作業コピーです。このフォルダーで行った変更は、変更をコミットするまでローカル リポジトリに影響しません。ローカル リポジトリに変更をコミットするには、GitBash で次のコマンドを入力します。

    git add .
    git commit -v -a -m "<Describe the changes made in this commit>"

`add` コマンドにより、変更はリポジトリへのコミットの準備としてステージング領域に追加されます。`add` コマンドの後のピリオドは、サブフォルダーを再帰的にチェックして、追加または変更したすべてのファイルをステージングすることを指定します。(すべての変更をコミットするのでない場合は、特定のファイルを追加できます。コミットを元に戻すこともできます。ヘルプを表示するには、「`git add -help`」または「`git status`」と入力してください。)

`commit` コマンドにより、ステージングされた変更がリポジトリに適用されます。`-m` はコマンド ラインでコミットのコメントを提供していることを示します。特定の発行日を対象としていない場合は、"できるだけ早い発行日" とすることができます。-v および -a スイッチは省略できます。-v スイッチはコマンドからの詳細 (verbose) 出力用で、-a スイッチは add コマンドですでに行ったことを行います。) 

作業の途中で複数回コミットするか、完了時まで待って 1 回だけコミットすることができます。

#### <a name="submit-a-pull-request-to-the-main-repository"></a>メイン リポジトリにプル要求を送信する

作業が完了し、中央リポジトリにマージする準備ができたら、以下の手順を実行します。

1.    GitBash で、コマンド プロンプトに `git push origin <new branch name>` を入力します。ローカル リポジトリにおいて、`origin` はローカル リポジトリの複製元である GitHub リポジトリを指します。このコマンドにより、前の手順で行ったすべてのコミットを含む新しい分岐の現在の状態が GitHub フォークにプッシュされます。
2.    GitHub サイト上のフォーク内で、新しい分岐まで移動します。
3.    ページの上部にある **[プル要求]** ボタンを選択します。
4.    Base 分岐が `microsoftgraph/microsoft-graph-docs@master` で、Head 分岐が `<your username>/microsoft-graph-docs@<branch name>` であることを確認します。
5.    **[コミット範囲の更新]** ボタンをクリックします。
6.    プル要求にタイトルを付けて、作成しているすべての変更についての説明を入力します。バグによる UserVoice 項目または GitHub に関する問題が修正される場合は、その問題を説明内で必ず参照してください。
7.    プル要求を提出します。

サイト管理者の 1 人がプル要求を処理します。プル要求は [問題] の下にある microsoftgraph/microsoft-graph-docs サイト上に表示されます。プル要求が承諾されると、問題は解決されます。

#### <a name="create-a-new-branch-after-merge"></a>マージの後に新しい分岐を作成する

分岐が正常にマージされた (つまり、プル要求が承諾された) 後は、正常にアップストリームがマージされたローカル分岐で作業を継続しないでください。別のプル要求を提出する場合にマージの競合が発生する可能性があります。代わりに、別の更新を行うには、正常にマージされたアップストリーム分岐から新しいローカル分岐を作成します。

たとえば、ローカル分岐 X が正常に microsoftgraph/microsoft-graph-docs マスター分岐にマージされた後、マージされた内容に追加の更新を行うとします。microsoftgraph/microsoft-graph-docs マスター分岐から新しいローカル分岐 X2 を作成します。これを行うには、GitBash を開き、次のコマンドを実行します。

    cd microsoft-graph-docs
    git pull upstream master:X2
    git push origin X2

これで、分岐 X で提出した作業のローカル コピーを (新しいローカル分岐内に) 作成できました。X2 ブランチには他のライターがマージしたすべての作業も含まれるため、自身の作業が他のライターの作業 (たとえば、共有画像) に依存している場合はその作業が新しい分岐で使用可能になります。以前の作業 (および他のライターの作業) が分岐にあることを確認するには、新しい分岐をチェックアウトして...

    git checkout X2

...内容を確認します。(`checkout` コマンドは、`C:\Users\<yourusername>\microsoft-graph-docs` 内のファイルを X2 分岐の現在の状態に更新します。新しい分岐をチェックアウトした後は、内容への更新を行って通常どおりにコミットすることができます。ただし、誤って作業することを避けるため、結合済みの分岐 (X) は削除することをお勧めします (次の「**分岐を削除する**」のセクションを参照してください)。

#### <a name="delete-a-branch"></a>分岐を削除する

変更内容が中央リポジトリにマージされたら、使用した分岐は不要になったので削除できます。すべての追加の作業には、新しい分岐が必要です。  

分岐を削除するには、次の手順を実行します。

1.    GitBash で、コマンド プロンプトに `git checkout master` を入力します。これにより、削除される分岐にいないことが保証されます (削除される分岐にいることは許可されません)。
2.    次に、コマンド プロンプトで `git branch -d <branch name>` と入力します。これにより、アップストリーム リポジトリに正常にマージ済みの場合にのみ、ローカル コンピューター上の分岐が削除されます。(この動作は `–D` フラグでオーバーライドすることができますが、最初にその必要があるかどうかを確かめてください。)
3.    最後に、コマンド プロンプトで `git push origin :<branch name>` (コロンの前にはスペースを 1 つ入れ、後にはスペースを入れません) と入力します。これにより、GitHub フォーク上の分岐が削除されます。  

これで、プロジェクトに正しく投稿できました。

## <a name="how-to-use-markdown-to-format-your-topic"></a>Markdown を使用してトピックを書式設定する方法

### <a name="standard-markdown"></a>標準の Markdown

このリポジトリ内のすべての記事では、Markdown を使用しています。完全な紹介 (およびすべての構文のリスト) は [[Markdown ホーム]] [] にありますが、必要な基本事項について説明します。

優れたエディターをお探しの場合は、[Markdown Pad][] をお試しください。


### <a name="markdown-basics"></a>Markdown の基本事項

最も一般的な Markdown 構文の一覧を以下に示します。

*     **改行と段落:**Markdown には、HTML `<br />` 要素はありません。代わりに、新しい段落がテキストの 2 つのブロック間に空白の行で指定されます。
*    **斜体:**HTML `<i>some text</i>` は、`*some text*` と記述されます。
*     **太字:**HTML `<strong>some text</strong>` 要素は、`**some text**` と記述されます。
*     **見出し:**HTML 見出しは、行の先頭の `#` 文字の数で指定されます。`#` 文字の数は、見出しの階層レベルに対応しています (たとえば、`#` = h1、`##` = h2、`###`= h3)。
*     **番号付きリスト**番号付き (順序指定された) リストを作成するには、`1. ` で行を開始します。単一のリスト要素内に複数の要素が必要な場合は、次のようにリストを書式設定します。
        
        1.    Notice that this line is tabbed over after the '.'
        
            Now notice that there is a line break between the two paragraphs in the list element, and that the indentation here matches the indentation of the line above.

*    **箇条書き:**箇条書き (順序指定のないリスト) は、`1. ` が `* `、`- `、または `+ ` のいずれかに置き換えられる点を除き、順序指定されたリストとほぼ同じです。複数の要素リストは、順序指定されたリストと同じように動作します。
*    **リンク:**リンクの基本構文は `[visible link text](link url)` です。

    リンクには参照も指定できます。これについては、以下の「**リンクとイメージ参照**」セクションで説明します。

*    **イメージ:**イメージの基本構文は `![alt text for the image](image url)` です。

    イメージには参照も指定できます。これについては、以下の「**リンクとイメージ参照**」セクションで説明します。

*    **インライン HTML:**Markdown では、HTML インラインを含めることができます。`<i>italic</i>` は<i>斜体</i>として Markdown によって正しく表示されます。

### <a name="link-and-image-references"></a>リンクとイメージ参照

Markdown には、ユーザーがイメージとリンクの URL の代わりに参照を挿入できるようにする、非常に便利な機能が用意されています。この機能を使用するための構文を以下に示します。

    The image below is from [Google][googleweb]
    
    ![Google's logo][logo]
    
    [googleweb]: http://www.google.com
    [logo]: https://www.google.com/images/srpr/logo3w.png

ファイルの下部でグループ化された参照を使用すると、リンクとイメージの URL を簡単に検索、編集、再利用することができます。 


## <a name="more-resources"></a>その他のリソース

* Markdown に関する詳細については、[サイト]の「[Markdown ホーム]」を参照してください。
* Git と GitHub の使用に関する詳細については、まず「[GitHub ヘルプ」セクション]の「 [GitHub ヘルプ]」を確認してから、必要に応じてサイト管理者に問い合わせてください。

[GitHub ホーム]: http://github.com
[GitHub ヘルプ]: http://help.github.com/
[Set Up Git]: http://help.github.com/win-set-up-git/
[Markdown ホーム]: http://daringfireball.net/projects/markdown/
[Markdown Pad]: http://markdownpad.com/
[microsoftgraph/microsoft-graph-docs issues]: https://github.com/microsoftgraph/microsoft-graph-docs/issues
