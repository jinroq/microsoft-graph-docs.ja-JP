# <a name="microsoft-graph-security-api-overview"></a>Microsoft Graph Security API の概要

Microsoft Graph Security API は、Microsoft のセキュリティ製品、サービス、およびパートナーを接続し、セキュリティ オペレーションを合理化することで、脅威防御、検出、および応答機能を向上させます。 Microsoft Graph Security API は、 ひとつのプログラム インターフェイスにより複数の [Microsoft Graph Security プロバイダ](../api-reference/v1.0/resources/securityvendorinformation.md)  (セキュリティ プロバイダ、あるいはプロバイダ) を接続する、仲介サービス (ブローカー) です。 Microsoft Graph Security API  へのリクエストは、適用可能なすべてのセキュリティ プロバイダにフェデレーションされます。 次の図に示すように、結果を統合して、要求元のアプリケーションに共通のスキーマで返します。 詳細については、 [「Microsoft Graph Security のデータ フロー」](security-dataflow.md)　を参照してください。

![security_overview_diagram_1.png](./images/security_overview_diagram_1.png)

認証については、 [「認証、およびセキュリティ API」](security-authorization.md) を参照してください。 アクセス許可 (委任されたアクセス許可とアプリケーションのアクセス許可を含む) の詳細については、「 [アクセス許可](permissions_reference.md#security-permissions) 」を参照してください。

## <a name="why-use-the-microsoft-graph-security-api"></a>Microsoft Graph セキュリティ API を使用する理由

 [Microsoft グラフ セキュリティ API](../api-reference/v1.0/resources/security-api-overview.md) を使用すれば、Microsoft および Microsoft パートナーのさまざまなセキュリティ製品およびサービスの接続を簡単に行うことができます。 これらソリューションをより容易に、より高い価値で実現することができます。

### <a name="unify-and-standardize-alert-tracking"></a>アラート追跡の統一と標準化

1回のコーディングで Microsoft Graph 統合セキュリティ ソリューションからの警告を統合し、全ソリューション間で警告の状態と割り当ての同期を維持します。 また[Azure Monitor](https://docs.microsoft.com/en-us/azure/monitoring-and-diagnostics/monitor-stream-monitoring-data-event-hubs#what-can-i-do-with-the-monitoring-data-being-sent-to-my-event-hub) を使用して、Spluk や IBM QRadar などのセキュリティ情報およびイベント管理 (SIEM) ソリューションに、警告をストリーミング処理することができます。 SIEM のセキュリティ API エンティティとの統合についての詳細は、 [「SIEM との統合」](security_siemintegration.md) を参照してください。

### <a name="correlate-security-alerts-to-improve-threat-protection-and-response"></a>セキュリティの警告を関連させ、脅威に対する防御とレスポンスを向上させる

複数のセキュリティ ソリューション間の警告を、統合された警告スキーマに容易に関連付けることができます。 これにより、実践的な警告情報を受け取れるだけでなく、アセット、およびユーザー情報を使用してセキュリティ アナリストをピボットし、脅威とアセットの保護のより高速な応答を有効にする警告情報を追加することができます。  

### <a name="update-alert-tags-status-and-assignments"></a>警告タグ、ステータス、および割り当ての更新

追加のコンテキストまたは脅威インテリジェンスに警告を関連付け、応答と修復を通知します。 すべてのワークフローにおいて、警告に関するコメントやフィードバックが可視化されるようになります。 警告の状態および割り当てを最新に保つことにより、すべての統合ソリューションが現在の状態を反映するようにします。 Webhook サブスクリプションを使用すると、変更の通知を受け取ることができます。  

### <a name="unlock-security-context-to-drive-investigation"></a>セキュリティ コンテキストをロック解除してドライブを調査する

関連するセキュリティ関連インベントリ (ユーザー、ホスト、アプリなど) を深く掘り下げ、Microsoft Graph の他のプロバイダー (Azure AD、Microsoft Intune、Office 365) からの組織コンテキストを追加することにより、ビジネス コンテキストとセキュリティ コンテキストをまとめて、脅威への対応を向上させます。

### <a name="proactively-manage-security-risks-preview"></a>セキュリティ リスク (プレビュー) をプロアクティブに管理

Microsoft Secure Score (プレビュー) は組織のセキュリティのニーズを可視化して改善方法を提案し、解決策が組み込まれた後に改良されたスコアを実行します。 経時的な進行状況を簡単に計測し、スコアの向上につながっている特定の変更情報を取得します。

## <a name="benefits-of-using-the-microsoft-graph-security-api"></a>Microsoft Graph セキュリティ API を使用する利点

次の一覧表は、Microsoft Graph Security API を使用して統合することで得られる、さまざまなセキュリティ ソリューションです。  

|**領域**     | **利点**|
|:---------------|:---------|
|**マネージド セキュリティ サービス プロバイダ (MSSP)**|<ul><li>セキュリティ操作ツールとサービスの合理的な統合。</li> <li>展開と保守に要する時間を短縮し、作業を減らします。</li> <li>MSSP ユーザーにより多くの価値を提供する機能。</li></ul>|
|**SIEM と IT リスク管理ソリューション**|<ul><li>Microsoft のセキュリティ ソリューションとエコシステム パートナーをスムーズに統合します。</li> <li>豊富な警告メタデータ。</li> <li>警告の相関関係を向上します。</li></ul>|
|**アプリケーション** <br> (脅威インテリジェンス、モバイル、クラウド、IOT、詐欺検出、アイデンティティとアクセス、リスクとコンプライアンス、ファイアウォール、など)|<ul><li>さまざまなセキュリティ ・ ソリューションにまたがる脅威管理、防御、およびリスク管理の統合。</li> <li>警告、在庫、構成、および Microsoft Graph を通じて公開されるアクション。</li> <li>Microsoft Graph により有効化されたソリューションの即座の統合。</li></ul>|

## <a name="next-steps"></a>次の手順

- [Microsoft Graph セキュリティ API を使用する](../api-reference/v1.0/resources/security-api-overview.md)
- セキュリティ プロバイダになることに関心がありますか？  [「Graphsecfeedback」](mailto:graphsecfeedback@microsoft.com)にアクセスしてください。
