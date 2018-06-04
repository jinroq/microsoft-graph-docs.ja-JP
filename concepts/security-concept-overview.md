# <a name="overview-of-security-in-microsoft-graph-preview"></a>Microsoft Graph でのセキュリティの概要 (プレビュー) 

Microsoft Graph を使用することにより、Intelligent Security Graph に接続して Microsoft およびそのセキュリティ パートナーのリソースを活用して、脅威への対応ソリューションとしてより良いものを構築できます。 さらに Microsoft Graph は、Azure Active Directory (Azure AD) の Identity Protection サービスによって検出されるユーザーおよびアカウントのリスクへのアクセスも提供します。それにより、アカウント リスク データをセキュリティ アプリケーションに統合することができます。

## <a name="why-use-the-security-api-and-connect-with-microsoft-intelligent-security-graph"></a>セキュリティ API を使用して Microsoft Intelligent Security Graph に接続する理由

Intelligent Security Graph は、サイバー脅威と戦うための統一プラットフォームです。 これは、Microsoft のさまざまな製品やサービスを脅威から守るリアルタイム保護機能を提供し、統合ソリューションのエコシステムをサポートします。

それらのソリューションには、Intelligent Security Graph において [Microsoft Graph のセキュリティ API](https://aka.ms/graphsecuritydocs) により、容易に接続することができます。 それらのソリューションの実現がさらに容易になり、その価値が高まります。

### <a name="unify-and-standardize-alert-management"></a>警告管理の統一と標準化

複数のセキュリティ ソリューション間の警告を、一般的な警告スキーマに関連付けることが容易になります。 1 回のコーディングで Microsoft Graph 統合セキュリティ ソリューションからの警告を統合し、全ソリューション間で警告の状態と割り当ての同期を維持します。 また、[Azure Monitor](https://docs.microsoft.com/ja-JP/azure/monitoring-and-diagnostics/monitor-stream-monitoring-data-event-hubs#what-can-i-do-with-the-monitoring-data-being-sent-to-my-event-hub) により、Spluk や IBM QRadar など、セキュリティ情報およびイベント管理 (SIEM) ソリューションに警告をストリーミング処理することができます。

### <a name="federated-security-aggregation-service"></a>フェデレーション セキュリティ集約サービス

セキュリティ API をフェデレーション セキュリティ集約サービスとして使用することにより、オンボードのセキュリティ プロバイダーすべてに対してクエリを発行し、回答の集約情報を得ることができます。

### <a name="unlock-security-context-to-drive-investigation"></a>セキュリティ コンテキストをロックを解除して調査を促進

関連するセキュリティ関連インベントリ (ユーザー、ホスト、アプリなど) を深く掘り下げ、Microsoft Graph の他のプロバイダー (Azure AD、Microsoft Intune、Office 365) からの組織コンテキストを追加することにより、ビジネス コンテキストとセキュリティ コンテキストをまとめて、脅威への対応を向上させます。

## <a name="why-use-azure-ad-to-protect-identities-in-your-organization"></a>組織内の ID を保護するために Azure AD を使用する理由

ほとんどのセキュリティ侵害は、攻撃者がユーザーの ID を盗んだ結果としてなされており、第三者による侵害、パスワード スプレー攻撃、および高度なフィッシング攻撃を利用することで、ますます威力が増してきています。 したがって、ユーザー アカウントのすべてをそのような攻撃から保護し、無防備な ID が悪用されるのを事前に防ぐ必要があります。

Azure AD では、アカウントが無防備である可能性を示す異常を検出するために、アダプティブ機械学習アルゴリズムや経験則を使用します。 そのデータを使用することにより、Identity Protection は、リスク ベースの条件アクセス ポリシーでユーザーを保護し、レポートを生成し、検出された場合にはそれを通知します。

現在では、Microsoft Graph により、Azure AD Premium P1 および P2 のユーザーに容易にアクセスすることにより、Identity Protection によるリスク検出について問い合わせて、それらのイベントを SIEM システムおよびセキュリティ アプリケーションで使用することができます。

## <a name="next-steps"></a>次の手順

- [セキュリティ API を使用する](../api-reference/beta/resources/security-api-overview.md)
- [Azure AD Identity Protection API を使用する](../api-reference/beta/resources/identityprotection_root.md)

