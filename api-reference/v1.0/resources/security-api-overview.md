# <a name="use-the-microsoft-graph-security-api"></a>Microsoft Graph API を使用

Microsoft グラフ セキュリティ API は、統一されたインタ フェースとマイクロソフトとエコシステムのパートナーからのセキュリティ ソリューションと統合するためにスキーマを提供します。 これは、セキュリティ ・ オペレーションを合理化し、サイバー脅威の増加が防御よりのお客様を支援します。 Microsoft Graph Security APIをフェデレーションセキュリティ集約サービスとして使用して、すべてのオンボードセキュリティプロバイダにクエリを送信し、集計応答を取得できます。 Microsoft Graph Security APIを使用して、次のようなアプリケーションを構築します。

- 統合し、複数のソースからのセキュリティの警告の相関関係
- コンテキストデータのロックを解除して調査を通知
- セキュリティ操作を自動化して効率を高める
- 積極的なリスク管理を可能にするセキュリティデータの可視性を提供

Microsoft Graph Security APIには、次のキーエンティティが含まれています。

## <a name="alerts"></a>アラート

通知は、マイクロソフトまたはパートナーのセキュリティ ・ ソリューションが既に特定し、アクションの通知フラグが設定されているお客様のテナント内で潜在的なセキュリティ上の問題です。 Microsoft Graph Security [ アラート](alert.md) エンティティを使用すると、統合されたすべてのソリューションでセキュリティの問題を統一し、合理化することができます。 これは、アプリケーションのアラートおよび脅威の保護とレスポンスを向上させるためにコンテキストを関連付けることもできます。 これらは、インシデントの解決方法を調査の時間と時間を減らすことでセキュリティの運用効率をアンロックします。 アラートの更新機能により、さまざまなセキュリティ製品およびサービスの [アラート](alert.md) のエンティティを更新することによって、Microsoft グラフ セキュリティ API と統合されている間、特定のアラートの状態を同期できます。

Microsoft Graph Security統合ソリューションは、次のセキュリティプロバイダからアラートを受信します。

- Azure のセキュリティ センター
- Azure Active Directory Id の保護
- Azure 情報保護
- Microsoftクラウドアプリケーションのセキュリティ
- Windows Defender 高度な脅威からの保護
- Microsoft Intune (プライベート プレビュー)
- Office 365 (準備中)
- Palo Alto Networks App Frameworkなどのパートナーソリューション

> **注:** 新しいプロバイダーは、Microsoft のグラフのセキュリティ エコシステムの契約時では継続的にします。

## <a name="common-use-cases"></a>一般的なユース ケース

以下は、Microsoft Graph Security APIを使用するための最も一般的な要求の一部です。

| **ユース ケース**   | **REST リソース** | **Graph エクスプローラーで試す** |
|:---------------|:--------|:----------|
| 警告の一覧表示 | [警告の一覧表示](../api/alert_list.md) | [https://graph.microsoft.com/v1.0/security/alerts](https://developer.microsoft.com/en-us/graph/graph-explorer?request=security/alerts&method=GET&version=v1.0&GraphUrl=https://graph.microsoft.com) |
| 通知を更新 | [警告の更新](../api/alert_update.md) | [https://graph.microsoft.com/v1.0/security/alerts/{alert-id}](https://developer.microsoft.com/en-us/graph/graph-explorer?request=security/alerts/{alert-id}&method=PATCH&version=v1.0&GraphUrl=https://graph.microsoft.com) |

購読して、Microsoft のグラフのセキュリティ エンティティの更新に関する通知を受け取るには、Graph [webhooks](../../../concepts/webhooks.md) を使用できます。

## <a name="resources"></a>リソース

コードを作成し、これらのMicrosoft Graph Security APIサンプルに寄稿：

- [ASP.NET (C#) のサンプル](https://github.com/microsoftgraph/aspnet-security-api-sample)
- [Python のサンプル](https://github.com/microsoftgraph/python-security-rest-sample)
- [Node.js (JavaScript) のサンプル](https://github.com/microsoftgraph/nodejs-security-sample)

コミュニティに参加。

- [技術コミュニティーに参加](https://aka.ms/graphsecuritycommunity)
- [StackOverflow を説明](https://stackoverflow.com/questions/tagged/microsoft-graph-security)

## <a name="next-steps"></a>次の手順

Microsoft グラフ セキュリティ API は、Microsoft およびパートナーからのさまざまなセキュリティ ソリューションと連携するための新しい方法を開くことができます。 開始するには、次の手順を実行します。

-  [アラート](alert.md)にドリル ・ ダウンします。
- [Graph エクスプローラー](https://developer.microsoft.com/graph/graph-explorer)で API をお試しください。 [ **サンプル クエリ**] は、 **多くのサンプルを表示する** を選択し、セキュリティ カテゴリを **オン**に設定します。
- エンティティの変更 [を購読して、受信通知](../../../concepts/webhooks.md) を実行してください。

さらに情報が必要な場合「[パートナーによる Microsoft Graph の活用方法](https://developer.microsoft.com/graph/graph/examples#partners)」を参照してください。
