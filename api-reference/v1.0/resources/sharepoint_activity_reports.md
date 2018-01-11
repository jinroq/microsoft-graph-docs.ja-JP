# <a name="sharepoint-activity-reports"></a>SharePoint アクティビティ レポート

SharePoint アクティビティ レポートを使用すると、ファイルの操作を参照して、SharePoint のすべてのライセンス ユーザーのアクティビティを取得できます。 共有されたファイル数に基づいて、進行中のコラボレーションのレベルを確認することもできます。

> **注:** 別のレポートのビューとレポート名についての詳細は、「[Office 365 レポート: SharePoint アクティビティ](https://support.office.com/client/SharePoint-activity-a91c958f-1279-499d-9959-12f0de08dc8f)」を参照してください。

## <a name="reports"></a>レポート

| 関数                                 | 戻り値の型 | 説明                              |
| :--------------------------------------- | :---------- | :--------------------------------------- |
| [ユーザーの詳細を取得する](../api/reportroot_getsharepointactivityuserdetail.md) | Stream      | ユーザー別の SharePoint アクティビティに関する詳細を取得します。 |
| [ファイルの数を取得する](../api/reportroot_getsharepointactivityfilecounts.md) | Stream      | SharePoint サイトに保存されているファイルを操作した、それぞれ別個のライセンス ユーザーの数を取得します。 |
| [ユーザーの数を取得する](../api/reportroot_getsharepointactivityusercounts.md) | Stream      | アクティブ ユーザーの数の傾向を取得します。 ユーザーが一定期間中にファイル アクティビティ (保存、同期、変更、共有) を実行するか、またはページにアクセスすると、そのユーザーはアクティブとみなされます。 |
| [ページを取得する](../api/reportroot_getsharepointactivitypages.md) | Stream      | ユーザーがアクセスしたそれぞれ別個のページ数を取得します。 |
