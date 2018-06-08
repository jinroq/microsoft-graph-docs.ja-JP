# <a name="using-the-activity-feed-api-in-microsoft-graph-to-enable-cross-device-experiences"></a>Microsoft Graph のアクティビティ フィード API を使用してクロスデバイス エクスペリエンスを有効にする

さまざまなアクティビティは、デバイスが変わってもアプリでの作業をすばやく再開するのに役立ち、生産性が向上します。 Microsoft は、アクティビティ フィードを利用した Windows Timeline、Windows Sets、Cortana Pick up Where I left off、および Microsoft Launcher などのエクスペリエンスにより、アプリの生産性向上をサポートします。 アクティビティの利用で、それらの Microsoft エクスペリエンスによってアプリの利用が推進されます。 また、アプリでのアクティビティを表示することにより、Windows、Android、iOS など、どんなプラットフォームのどんなデバイス上でも、直前の作業の続きにすぐ取り掛かることができます。

## <a name="why-integrate-with-activities"></a>アクティビティを統合する理由
### <a name="enable-experiences-that-flow-seamlessly-between-windows-android-linux-and-ios-devices"></a>Windows、Android、Linux、および iOS のデバイスの間をシームレスに移ることのできるエクスペリエンスが可能になる 
優れたアプリケーションは、創造性、生産性、娯楽性の幅広いシナリオでユーザーが作業する上で大きな助けとなります。 作業に戻ることは挑戦となることがあります。その作業を別のデバイスや異なるプラットフォームで続行しようとする場合は、特にそう言えます。 アクティビティをアプリケーションに統合することにより、ユーザーは、近くにあるデバイスを使用してすぐに作業に戻ることができるようになります — Web、モバイル、デスクトップの間を自由に行き来できます。 履歴項目により、ユーザーは直前にどんなアクティビティを、いつ、どれほどの期間行っていたかを容易に確認できます。   

各ユーザー アクティビティは、アプリ内の 1 つの場所、つまり製品ページ、テレビ番組、ドキュメント、ゲームの現行キャンペーンなどを表します。 ディープ リンク 1 つにより、アプリのアクティビティを再開できます。 [[最近のアクティビティを取得する]](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/api/projectrome_get_recent_activities) を使用すれば、買い物アプリで最後に見ていた製品のリストや、現在読んでいる書籍やニュース記事のリストを取得できます。 

### <a name="create-richer-activities-for-any-experience-with-adaptive-cards"></a>アダプティブ カードを使用して任意のエクスペリエンスで動作する機能豊富なアクティビティを作成する
Windows Timeline などの Microsoft エクスペリエンスでアクティビティを表示すると、それらは、[[アダプティブ カード]](http://adaptivecards.io/) フレームワークを使用して表示されます。それにより、アプリのアクティビティを示す、見栄えが良くて機能豊富なカードを作成できます。 アダプティブ カード SDK を使用することにより、独自のアプリで機能豊富なカードを表示することもできます。 各アクティビティ用のアダプティブ カードが提供されていない場合、アプリケーションの名前とアイコン、必須タイトル フィールド、およびオプションの説明フィールドに基づいて自動的にシンプルなアクティビティ カードが作成されます。 

### <a name="let-microsoft-help-drive-app-usage-with-features-that-reach-hundreds-of-millions-of-customers"></a>Microsoft の機能利用により何億というユーザーに向けてアプリの利用を推進
ユーザー アクティビティ統合で可能になるのは、ユーザーは、アプリのアクティビティをシームレスに再開できることだけではありません。それにより、Windows、iOS、および Android のための Microsoft のエクスペリエンスを活用して、どんなデバイスでもアプリを利用できるようになり、ユーザーの生産性が向上するのです。 Microsoft Graph を利用すれば、ひとたびユーザー アクティビティを統合することで何億というユーザーに達することができ、さらには、Windows のみならず iOS や Android デバイス用の Microsoft 製品を使用する何千万という組織ユーザーにも達することができます。

![Windows Timeline のスクリーンショット](https://winblogs.azureedge.net/win/2017/05/22-591a3ec9833f4.jpg)

## <a name="see-also"></a>関連項目

- [Microsoft Graph のクロスデバイス エクスペリエンス](cross-device-concept-overview.md)
- [アクティビティ フィード API の利用によりデバイスが変わってもユーザー アクティビティを再開できる](../api-reference/v1.0/resources/activity-feed-api-overview.md)
- [ディープ挿入の利用により 1 回の要求でアクティビティと履歴項目を公開](https://developer.microsoft.com/ja-JP/graph/docs/api-reference/v1.0/api/projectrome_put_activity#example-2---deep-insert)
- [Project Rome に関する詳細情報](http://aka.ms/projectrome)
