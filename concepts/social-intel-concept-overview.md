# <a name="overview-of-social-intelligence-and-analytics-in-microsoft-graph"></a>Microsoft Graph におけるソーシャル インテリジェンスと分析の概要

Microsoft Graph では、Microsoft 365 のクラウド サービスを使用する何千万人ものユーザーが中核的な役割を果たします。 ユーザーのデータは、慎重に管理、保護されており、適切な権限があれば、Microsoft Graph サービスでビジネスの生産性や創造性を促進するために利用できます。 ユーザーのデータは Microsoft Graph のあらゆる部分に存在しますが、ユーザーの社会的な交流から得られたデータは特に興味深いものがあります。 たとえば、次のような質問への答えを導く知的なインサイトを得ることができます。

- 「このユーザーはこのトピックの情報を誰に問い合わせればよいか?」
- 「このユーザーにとって最も関心があるドキュメントはどれか?」

Microsoft Graph では、People API と Insights API を使用してユーザーに関連する人物とドキュメントにアクセスできる、よりスマートなアプリを構築できます。

People API は、人物をユーザーとの関連性が高い順に返します。これらの人物は、そのユーザーの連絡先、ソーシャル ネットワーク、組織の人名簿、およびメールや Skype で行われた最近のコミュニケーションに基づいて収集されます。 これは、人物を選択するシナリオで特に有用です。

Insights API は、高度な分析と機械学習を使用して、ユーザーが 1 日の作業時間を通して必要とする最も関連性の高いファイルを提供します。 この API により、Office Delve、SharePoint ホーム、OneDrive for Business の [Discover] ビュー、Outlook on the web などの使い慣れた Office 365 のエクスペリエンスが強化されます。

![People API と Insights API は、あるユーザーに関連する人物とドキュメントを返します](images/social-intel-concept-overview-data.png)

## <a name="why-integrate-with-people-data"></a>人物のデータと統合する理由

People API は、1 つのエンティティ ([person](../api-reference/v1.0/resources/person.md)) のデータを返します。このエンティティには、今日のビジネスの世界における個人の一般的なデータが含まれています。 Microsoft Graph ユーザーにとって、この **person** データを特に便利なものにしているのが、その_関連性_です。 関連性は、ユーザーのコミュニケーションやコラボレーションのパターン、およびビジネス リレーションシップに基づいて計算される各人物の関連性スコアで示されます。 この_関連性_データの用途には 3 つのタイプがあります。

### <a name="browse-people-by-relevance"></a>関連性による人物の参照

適切な[権限](people_example.md#authorization)を取得すると、サインインしているユーザー、またはサインインしているユーザーの組織内の他のユーザーに関連する人物を参照できます。 ユーザーは、関連性の順に並べられた **person** オブジェクトのコレクションを取得します。 応答で返された **person** オブジェクトのコレクションは、クエリ パラメーター `top`、`skip`、`orderby`、`select`、および `filter` を指定することでさらに[カスタマイズ](people_example.md#browse-people)できます。

### <a name="fuzzy-searches-based-on-people-criteria"></a>人物の抽出条件に基づくあいまい検索

アプリがサインインしているユーザーによるアクセス許可を取得している場合は、People API でそのユーザーに関連する人物を検索できます  (詳細については、「[People のアクセス許可](permissions_reference.md#people-permissions)」を参照してください)。

あいまい検索により、完全に一致する項目と、検索目的の推論に基づく結果が返されます。 これを具体的に示す次の例では、サインインしているユーザーに関連し、名前_またはメール アドレス_に「j」で始まる単語が含まれている **person** オブジェクトが返されます。

<!-- { "blockType": "ignored" } -->
```http
GET /me/people/?$search=j
```

### <a name="fuzzy-searches-based-on-topic-criteria"></a>トピックの抽出条件に基づくあいまい検索

People API では、サインインしているユーザーに関連し、そのユーザーと特定の「トピック」についてやり取りしたいと言っている人物を検索することもできます。 トピックとは、ユーザーが電子メールの会話で最もよく使用している単語のことです。 Microsoft はそのような単語を抽出し、コンテキストを取り除き、そのデータのインデックスを作成してあいまい検索を容易にします。

次の例は、「カブトムシ」というトピックの検索目的の推論を示しています。

<!-- { "blockType": "ignored" } -->
```http
GET /me/people/?$search="topic:beetle" 
```

トピック データのインデックスのあいまい検索により、昆虫のカブトムシ、フォルクス ワーゲンの象徴的な車であるビートル、バンドのビートルズ、およびその他の定義のインスタンスが返されます。


## <a name="why-integrate-with-document-based-insights-preview"></a>ドキュメントベースのインサイト (プレビュー) と統合する理由

### <a name="use-intelligence-to-improve-collaboration"></a>インテリジェンスを使用したコラボレーションの改善

ユーザーは多くの場合、通常の 1 日の作業時間中に、多くのドキュメントに保存されている大量の情報を操作し、さまざまな方法で他のユーザーと共同作業を行います。 必要な情報が必要なときに常に見つかることが重要です。

[trending](../api-reference/beta/resources/insights_trending.md)、[shared](../api-reference/beta/resources/insights_shared.md)、および [used](../api-reference/beta/resources/insights_used.md) API を含む Insights API を使用して、ユーザーの現在のコンテキストとニーズに基づいて Office 365 全体からファイルを抽出することにより、ユーザーの生産性が向上し、組織内のコラボレーションが改善されます。

アプリでは、Insights API の結果を簡単にレンダリングできます。 すべての結果には、プレビュー イメージの URL やプレビュー テキストなどの一般的な視覚化プロパティのセットが付属しています。

### <a name="make-relevant-content-visible"></a>関連するコンテンツの視覚化

Office 365 の Delve では、_trending_ のインサイトを使用して、ユーザーが現在最も興味を持っているドキュメントを見つけることができます。 図 1 を参照してください。

プログラムの中で Insights API の [trending](../api-reference/beta/resources/insights_trending.md) エンティティを使用すると、アプリの顧客に同じようなエクスペリエンスを提供できます。 **trending** エンティティを使用して、ユーザーが最近話題にしているドキュメントやユーザーに関連するドキュメントに接続します。 [人気上昇中のドキュメントの一覧表示](../api-reference/beta/api/insights_list_trending.md)では、OneDrive または SharePoint のチーム サイトに保存されているファイルが、関連性の最も高いものから順に並べ替えて返されます。 

**図 1 あるユーザーに人気のあるドキュメントが表示されている Office 365 の Delve**

![あるユーザーに人気のあるドキュメントが表示されている Office 365 の Delve のスクリーンショット](images/delve_concept.png)

### <a name="allow-users-to-collaborate-and-get-back-to-work"></a>ユーザーが共同作業の後で作業に戻れるようにする

新しい Office 365 の人物カードは、_used_ および _shared_ のインサイトを利用して人物と知識単位を結びます。 人物カードは、あるユーザーに関連するドキュメントを識別し、表示します。 ユーザーは、Outlook on the web など、スイート全体で人物カードを表示できます。 図 2 を参照してください。

Insights API は、[used](../api-reference/beta/resources/insights_used.md) および [shared](../api-reference/beta/resources/insights_shared.md) エンティティと同様の機能を提供します。 Office 365 で、あるユーザーが最近表示または操作したもの、または同僚が最近そのユーザーと共有したものが返されます。

**図 2 あるユーザーの人物カードが表示されている Outlook on the web**

![最近使用したファイルが表示されている、Outlook on the web のあるユーザーの人物カードのスクリーン ショット](images/peoplecard_concept.png)

## <a name="next-steps"></a>次の手順

* [Graph エクスプローラー](https://developer.microsoft.com/ja-JP/graph/graph-explorer)を使用して、自分のファイルで People および Insights API を試してみてください。 サインインして、左側の列の**サンプルをさらに表示**を選択します。 メニューを使用して **People** と **Insights (beta)** を有効にします。
* 詳細については、[People API](people_example.md) および [person](../api-reference/v1.0/resources/person.md) エンティティを参照してください。
* Insights API を使い始めるには、「[Insights API を使用する](../api-reference/beta/resources/insights.md)」を参照してください。
