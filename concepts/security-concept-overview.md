---
title: Microsoft Graph セキュリティ API の概要
description: Microsoft Graph セキュリティ API を使用して Microsoft のセキュリティ製品、サービス、パートナーに接続することで、セキュリティ運用の効率化を図り、脅威の防止、検出、対処の各機能を向上させることができます。 Microsoft Graph セキュリティ API は、単一のプログラム インターフェイスで複数の Microsoft Graph セキュリティ プロバイダー (セキュリティ プロバイダーまたはプロバイダーとも呼ばれる) を接続できる中継サービス (ブローカー) です。 Microsoft Graph セキュリティ API に対する要求は、適用可能なすべてのセキュリティ プロバイダーにフェデレーションされます。 次の図に示すように、結果は集計され、要求元のアプリケーションに共通のスキーマで返されます。 詳細については、「Microsoft Graph セキュリティ API のデータ フロー」を参照してください。
ms.openlocfilehash: b5e1fb3d60cfc55cb940a217aaba872175887297
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27092377"
---
# <a name="microsoft-graph-security-api-overview"></a>Microsoft Graph セキュリティ API の概要

Microsoft Graph セキュリティ API を使用して Microsoft のセキュリティ製品、サービス、パートナーに接続することで、セキュリティ運用の効率化を図り、脅威の防止、検出、対処の各機能を向上させることができます。 Microsoft Graph セキュリティ API は、単一のプログラム インターフェイスで複数の [Microsoft Graph セキュリティ プロバイダー](/graph/api/resources/securityvendorinformation?view=graph-rest-1.0) (セキュリティ プロバイダーまたはプロバイダーとも呼ばれる) を接続できる中継サービス (ブローカー) です。 Microsoft Graph セキュリティ API に対する要求は、適用可能なすべてのセキュリティ プロバイダーにフェデレーションされます。 次の図に示すように、結果は集計され、要求元のアプリケーションに共通のスキーマで返されます。 詳細については、「[Microsoft Graph セキュリティ API のデータ フロー](security-dataflow.md)」を参照してください。

![security_overview_diagram_1.png](./images/security-overview-diagram-1.png)

承認については、「[承認と Microsoft Graph セキュリティ API](security-authorization.md)」を参照してください。 代理アクセス許可やアプリケーションのアクセス許可などのアクセス許可については、「[アクセス許可](permissions-reference.md#security-permissions)」を参照してください。

## <a name="why-use-the-microsoft-graph-security-api"></a>Microsoft Graph セキュリティ API を使用する理由

[Microsoft Graph セキュリティ API](/graph/api/resources/security-api-overview?view=graph-rest-1.0) を使用すると、Microsoft および Microsoft パートナーのさまざまなセキュリティ製品やサービスと簡単に接続できます。 これにより、それらのソリューションの実現がさらに容易になり、その価値も高まります。

### <a name="unify-and-standardize-alert-tracking"></a>警告追跡の統合と標準化

1 回のコードの記述で Microsoft Graph 統合セキュリティ ソリューションからの警告を統合し、すべてのソリューション間で警告の状態と割り当ての同期を維持します。 また、[Azure Monitor](https://docs.microsoft.com/ja-JP/azure/monitoring-and-diagnostics/monitor-stream-monitoring-data-event-hubs#what-can-i-do-with-the-monitoring-data-being-sent-to-my-event-hub) を使用して、Spluk や IBM QRadar などのセキュリティ情報およびイベント管理 (SIEM) ソリューションに警告をストリーミングすることができます。 SIEM とセキュリティ API エンティティとの統合の詳細については、「[SIEM との統合](security-siemintegration.md)」を参照してください。

### <a name="correlate-security-alerts-to-improve-threat-protection-and-response"></a>セキュリティの警告を関連付け、脅威の予防と対処を向上させる

複数のセキュリティ ソリューション間の警告を、統合された警告スキーマに簡単に関連付けることができます。 これにより、操作可能な警告情報を受け取れるだけでなく、セキュリティ アナリストがピボット分析を行い、資産やユーザーの情報で警告の質を高めることもでき、脅威への迅速な対処や資産保護を可能にします。  

### <a name="update-alert-tags-status-and-assignments"></a>警告のタグ、状態、割り当てを更新する

警告にタグ付けしてコンテキストや脅威インテリジェンスを追加し、対応や修復の情報を提供します。 警告へのコメントやフィードバックが確実にキャプチャされ、すべてのワークフローから参照できるようにします。 警告の状態と割り当ての同期状態を維持することで、すべての統合ソリューションに最新の状態が反映されます。 変更の通知を受け取るには、Webhook サブスクリプションを使用します。  

### <a name="unlock-security-context-to-drive-investigation"></a>セキュリティ コンテキストのロックを解除して調査を促進

関連するセキュリティ関連インベントリ (ユーザー、ホスト、アプリなど) を深く掘り下げ、Microsoft Graph の他のプロバイダー (Azure AD、Microsoft Intune、Office 365) からの組織コンテキストを追加することにより、ビジネス コンテキストとセキュリティ コンテキストをまとめて、脅威への対応を向上させます。

### <a name="proactively-manage-security-risks-preview"></a>セキュリティ リスクをプロアクティブに管理 (プレビュー)

Microsoft Secure Score (プレビュー) を使用すると、組織のセキュリティ ニーズを視覚化して、セキュリティの強化方法に関する提案を受け取り、それを導入した後に見られるスコアの向上を予測することができます。 経時的な進捗状況を簡単に計測し、スコアの向上につながる特定の変更について分析情報を取得できます。

## <a name="benefits-of-using-the-microsoft-graph-security-api"></a>Microsoft Graph セキュリティ API を使用するメリット

次の表は、さまざまなセキュリティ ソリューションが Microsoft Graph セキュリティ API と統合することによって得られる利点の一覧を示します。  

|**領域**     | **メリット**|
|:---------------|:---------|
|**マネージド セキュリティ サービス プロバイダー (MSSP)**|<ul><li>セキュリティ運用ツールとサービスの効率的な統合。</li> <li>展開および保守の時間と労力の削減。</li> <li>MSSP ユーザーにより多くの価値を提供。</li></ul>|
|**SIEM と IT リスク管理ソリューション**|<ul><li>Microsoft のセキュリティ ソリューションおよびエコシステム パートナーとのスムーズな統合。</li> <li>豊富な警告メタデータ。</li> <li>警告の関連付けの向上。</li></ul>|
|**アプリケーション** <br>(脅威インテリジェンス、モバイル、クラウド、IoT、不正検出、ID とアクセス、リスクとコンプライアンス、ファイアウォールなど)|<ul><li>さまざまなセキュリティ ソリューション全体で統合された脅威の管理と予防、リスク管理。</li> <li>Microsoft Graph を通じて公開される警告、インベントリ、構成、アクション。</li> <li>Microsoft Graph 対応ソリューションのクイック統合。</li></ul>|

## <a name="api-reference"></a>API リファレンス
このサービスの API リファレンスが必要な場合

- [Microsoft Graph v1.0 のセキュリティ API](/graph/api/resources/security-api-overview?view=graph-rest-1.0)
- [Microsoft Graph ベータ版のセキュリティ API](/graph/api/resources/security-api-overview?view=graph-rest-beta)

## <a name="next-steps"></a>次のステップ

- [Microsoft Graph セキュリティ API を使用する](/graph/api/resources/security-api-overview?view=graph-rest-1.0)
- セキュリティ プロバイダーに関心がある場合、 [Graphsecfeedback](mailto:graphsecfeedback@microsoft.com)にお問い合わせください。
