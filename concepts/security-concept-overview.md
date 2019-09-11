---
title: Microsoft Graph セキュリティ API の概要
description: Microsoft Graph セキュリティ API を使用して Microsoft のセキュリティ製品、サービス、パートナーに接続することで、セキュリティ運用の効率化を図り、脅威の防止、検出、対処の各機能を向上させることができます。 Microsoft Graph セキュリティ API は、単一のプログラム インターフェイスで複数の Microsoft Graph セキュリティ プロバイダー (セキュリティ プロバイダーまたはプロバイダーとも呼ばれる) を接続できる中継サービス (ブローカー) です。 Microsoft Graph セキュリティ API に対する要求は、適用可能なすべてのセキュリティ プロバイダーにフェデレーションされます。 次の図に示すように、結果は集計され、要求元のアプリケーションに共通のスキーマで返されます。 詳細については、「Microsoft Graph セキュリティ API のデータ フロー」を参照してください。
author: preetikr
localization_priority: Priority
ms.prod: security
scenarios: getting-started
ms.openlocfilehash: 7b12653382f88a3b16c370044fc3cb770aa2ac36
ms.sourcegitcommit: c68a83d28fa4bfca6e0618467934813a9ae17b12
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/07/2019
ms.locfileid: "36792969"
---
# <a name="microsoft-graph-security-api-overview"></a>Microsoft Graph セキュリティ API の概要

Microsoft Graph セキュリティ API を使用して Microsoft のセキュリティ製品、サービス、パートナーに接続することで、セキュリティ運用の効率化を図り、脅威の防止、検出、対処の各機能を向上させることができます。 Microsoft Graph セキュリティ API は、単一のプログラム インターフェイスで複数の [Microsoft Graph セキュリティ プロバイダー](/graph/api/resources/securityvendorinformation?view=graph-rest-1.0) (セキュリティ プロバイダーまたはプロバイダーとも呼ばれる) を接続できる中継サービス (ブローカー) です。 Microsoft Graph セキュリティ API に対する要求は、適用可能なすべてのセキュリティ プロバイダーにフェデレーションされます。 次の図に示すように、結果は集計され、要求元のアプリケーションに共通のスキーマで返されます。 詳細については、「[Microsoft Graph セキュリティ API のデータ フロー](security-dataflow.md)」を参照してください。

![security_overview_diagram_1.png](./images/security-overview-diagram-1.png)

承認については、「[承認と Microsoft Graph セキュリティ API](security-authorization.md)」を参照してください。 代理アクセス許可やアプリケーションのアクセス許可などのアクセス許可については、「[アクセス許可](permissions-reference.md#security-permissions)」を参照してください。

> [!VIDEO https://www.youtube-nocookie.com/embed/oYXPGwH9Ho0]

## <a name="why-use-the-microsoft-graph-security-api"></a>Microsoft Graph セキュリティ API を使用する理由

[Microsoft Graph Security API](/graph/api/resources/security-api-overview?view=graph-rest-1.0) を使用すると、Microsoft とパートナーのセキュリティ ソリューションとの接続を簡単に行えるようになります。 これにより、それらのソリューションの実現がさらに容易になり、その価値も高まります。 要件に応じて、次のいずれかの方法を使用することにより、Microsoft Graph Security API に簡単に接続できます。

- [コードを記述](https://aka.ms/graphsecuritysdk) – C#、Java、NodeJS などの[コード サンプル](https://aka.ms/graphsecurityapicode)を見つけます。
- [スクリプトを使用して接続](https://aka.ms/graphsecuritypowershellsampleblog) – [PowerShell サンプル](https://aka.ms/graphsecuritypowershellsample)を見つけます。
- [ワークフローとプレイブックにドラッグ アンド ドロップ](https://aka.ms/graphsecurityconnectorsblogpost) – [Azure Logic Apps](https://docs.microsoft.com/azure/logic-apps/logic-apps-overview)、[Microsoft Flow](https://flow.microsoft.com/)、[PowerApps](https://powerapps.microsoft.com/) 用の [Microsoft Graph セキュリティ コネクタ](https://aka.ms/graphsecurityconnectors)を使用します。
- [レポートとダッシュ ボードにデータを取得する](https://aka.ms/graphsecuritypowerbiconnectorblogpost) – [Power BI 用の Microsoft Graph セキュリティ コネクタ](https://aka.ms/graphsecuritypowerbiconnectordoc)を使用します。
- [Jupyter ノートブックを使用して接続](https://jupyter.org/) – [Jupyter ノートブック サンプル](https://aka.ms/graphsecurityjupyternotebooks)を検索します。  

### <a name="unify-and-standardize-alert-tracking"></a>警告追跡の統合と標準化

1 回接続すれば、Microsoft Graph 統合セキュリティ ソリューションからの警告を統合し、すべてのソリューション間で警告の状態と割り当ての同期を維持します。 また、Microsoft Graph Security API コネクタを使用して、Spluk などのセキュリティ情報およびイベント管理 (SIEM) ソリューションに警告をストリーミングすることができます。 セキュリティ API エンティティとのソリューション統合の詳細については、「[Microsoft Graph Security API を使用したセキュリティ ソリューションの統合](security-integration.md)」を参照してください。

### <a name="correlate-security-alerts-to-improve-threat-protection-and-response"></a>セキュリティの警告を関連付け、脅威の予防と対処を向上させる

複数のセキュリティ ソリューション間の警告を、統合された警告スキーマに簡単に関連付けることができます。 これにより、操作可能な警告情報を受け取れるだけでなく、セキュリティ アナリストがピボット分析を行い、資産やユーザーの情報で警告の質を高めることもでき、脅威への迅速な対処や資産保護を可能にします。  

### <a name="update-alert-tags-status-and-assignments"></a>警告のタグ、状態、割り当てを更新する

警告にタグ付けしてコンテキストや脅威インテリジェンスを追加し、対応や修復の情報を提供します。 警告へのコメントやフィードバックが確実にキャプチャされ、すべてのワークフローから参照できるようにします。 警告の状態と割り当ての同期状態を維持することで、すべての統合ソリューションに最新の状態が反映されます。 変更の通知を受け取るには、Webhook サブスクリプションを使用します。  

### <a name="unlock-security-context-to-drive-investigation"></a>セキュリティ コンテキストのロックを解除して調査を促進

関連するセキュリティ関連インベントリ (ユーザー、ホスト、アプリなど) を深く掘り下げ、Microsoft Graph の他のプロバイダー (Azure AD、Microsoft Intune、Office 365) からの組織コンテキストを追加することにより、ビジネス コンテキストとセキュリティ コンテキストをまとめて、脅威への対応を向上させます。

### <a name="automate-security-workflows-and-reporting"></a>セキュリティ ワークフローとレポート作成を自動化

セキュリティ管理、監視、調査を自動化し、運用効率と応答時間を向上させます。 Microsoft Graph セキュリティをレポートとダッシュ ボードに統合することによって、より深い分析情報とコンテキストが得られます。

### <a name="get-deep-insights-to-train-security-solutions"></a>深い分析情報を取得し、セキュリティ ソリューションをトレーニングする

組織で実行されている異なるセキュリティ製品にわたるデータを視覚化し、セキュリティに関するより深い分析情報を取得します。 データから学習し、セキュリティ ソリューションをトレーニングする機会を発見してください。 スキーマはピボット分析の対象となる複数のプロパティを提供し、セキュリティ データを使用して豊富な予備的なデータセットをビルドします。

### <a name="utilize-your-threat-intelligence-in-microsoft-security-solutions-preview"></a>Microsoft のセキュリティ ソリューション (プレビュー) で、自分の脅威インテリジェンスを活用する

脅威インジケーターを Microsoft のセキュリティ ソリューションに自動的に送信し、`alert`、`block`、`allow` アクションを有効にします。 Microsoft Graph Security API を直接使用するか、最新の脅威インテリジェンス プラットフォームとの統合を活用します。

### <a name="act-quickly-in-response-to-new-threats-preview"></a>新たな脅威に対してすばやく対応する (プレビュー)

新たな脅威に対して迅速な防御アクション (ファイル、URL、ドメイン、IP アドレスをブロックする操作など) をセキュリティ ツールおよびワークフロー内から行えるようにします。

### <a name="proactively-manage-security-risks-preview"></a>セキュリティ リスクをプロアクティブに管理 (プレビュー)

Microsoft Secure Score (プレビュー) を使用すると、組織のセキュリティ ニーズを視覚化して、セキュリティの強化方法に関する提案を受け取り、それを導入した後に見られるスコアの向上を予測することができます。 経時的な進捗状況を簡単に計測し、スコアの向上につながる特定の変更について分析情報を取得できます。

## <a name="benefits-of-using-the-microsoft-graph-security-api"></a>Microsoft Graph セキュリティ API を使用するメリット

次の表は、さまざまなセキュリティ ソリューションが Microsoft Graph セキュリティ API と統合することによって得られる利点の一覧を示します。  

|**領域**     | **メリット**|
|:---------------|:---------|
|**マネージド セキュリティ サービス プロバイダー (MSSP)**|<ul><li>セキュリティ運用ツール、ワークフロー、レポート作成の効率的な統合。</li> <li>展開および保守の時間と労力の削減。</li> <li>脅威に対するアクションを実行する、警告への自動応答。</li> <li>MSSP ユーザーにより多くの価値を提供。</li></ul>|
|**SIEM と IT リスク管理ソリューション**|<ul><li>Microsoft のセキュリティ ソリューションおよびエコシステム パートナーとのスムーズな統合。</li> <li>豊富な警告メタデータ。</li> <li>警告の関連付けの向上。</li></ul>|
|**アプリケーション** <br>(脅威インテリジェンス、モバイル、クラウド、IoT、不正検出、ID とアクセス、リスクとコンプライアンス、ファイアウォールなど)|<ul><li>さまざまなセキュリティ ソリューション全体で統合された脅威の管理と予防、リスク管理。</li> <li>Microsoft Graph を通じて公開される警告、アクション、顧客の脅威インテリジェンス。</li> <li>Microsoft Graph 対応ソリューションのクイック統合。</li> <li>他のセキュリティ ソリューションをトレーニングするための深いセキュリティ分析情報の取得。</li> </ul>|

## <a name="api-reference"></a>API リファレンス
このサービスの API リファレンスが必要な場合

- [Microsoft Graph v1.0 のセキュリティ API](/graph/api/resources/security-api-overview?view=graph-rest-1.0)
- [Microsoft Graph ベータ版のセキュリティ API](/graph/api/resources/security-api-overview?view=graph-rest-beta)

## <a name="next-steps"></a>次のステップ

- [Microsoft Graph セキュリティ API を使用する](/graph/api/resources/security-api-overview?view=graph-rest-1.0)
- セキュリティ プロバイダーに関心がある場合、 [Graphsecfeedback](mailto:graphsecfeedback@microsoft.com)にお問い合わせください。
