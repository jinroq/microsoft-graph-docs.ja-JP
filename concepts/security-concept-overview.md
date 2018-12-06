---
title: Microsoft グラフ セキュリティ API の概要
description: Microsoft グラフ セキュリティ API を使用するにはマイクロソフトのセキュリティ製品、サービス、およびセキュリティ ・ オペレーションを合理化し、脅威の保護、検出、および応答の機能を向上させるためにパートナーを接続します。 Microsoft グラフ セキュリティ API は、仲介サービス (ブローカー) 複数の Microsoft のグラフのセキュリティ プロバイダーを接続する 1 つのプログラム インターフェイスを提供する (セキュリティとも呼ばれますプロバイダーまたはプロバイダー)。 Microsoft グラフ セキュリティ API への要求は、すべての適用可能なセキュリティ プロバイダーにフェデレーションします。 結果を統合して、次の図に示すように、共通のスキーマでは、要求元のアプリケーションに返されます。 詳細については、Microsoft グラフ セキュリティ API のデータ フローを参照してください。
ms.openlocfilehash: b5e1fb3d60cfc55cb940a217aaba872175887297
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27092377"
---
# <a name="microsoft-graph-security-api-overview"></a>Microsoft グラフ セキュリティ API の概要

Microsoft グラフ セキュリティ API を使用するにはマイクロソフトのセキュリティ製品、サービス、およびセキュリティ ・ オペレーションを合理化し、脅威の保護、検出、および応答の機能を向上させるためにパートナーを接続します。 Microsoft グラフ セキュリティ API は、仲介サービス (ブローカー) 複数の[Microsoft のグラフのセキュリティ プロバイダー](/graph/api/resources/securityvendorinformation?view=graph-rest-1.0)を接続する 1 つのプログラム インターフェイスを提供する (セキュリティとも呼ばれますプロバイダーまたはプロバイダー)。 Microsoft グラフ セキュリティ API への要求は、すべての適用可能なセキュリティ プロバイダーにフェデレーションします。 結果を統合して、次の図に示すように、共通のスキーマでは、要求元のアプリケーションに返されます。 詳細については、 [Microsoft グラフ セキュリティ API のデータ フロー](security-dataflow.md)を参照してください。

![security_overview_diagram_1.png](./images/security-overview-diagram-1.png)

承認については、[承認、および Microsoft のグラフのセキュリティ API](security-authorization.md)を参照してください。 アクセス許可については、委任など、アプリケーションのアクセス許可、[アクセス許可](permissions-reference.md#security-permissions)を参照してください。

## <a name="why-use-the-microsoft-graph-security-api"></a>Microsoft グラフ セキュリティ API を使用する理由

[Microsoft グラフ セキュリティ API](/graph/api/resources/security-api-overview?view=graph-rest-1.0)の違いを簡単に接続するマイクロソフトおよびマイクロソフトのセキュリティ製品およびサービスのパートナーです。 それらのソリューションの実現がさらに容易になり、その価値が高まります。

### <a name="unify-and-standardize-alert-tracking"></a>統一し、アラートの管理を標準化

1 回すべてのソリューションにわたって Microsoft のグラフに統合されたセキュリティ ソリューション、アラートの状態を維持する、および割り当ての同期からのアラートを統合するためにコードを記述します。 セキュリティ情報およびイベント管理 (SIEM) ソリューションでは、Splunk と[Azure のモニター](https://docs.microsoft.com/en-us/azure/monitoring-and-diagnostics/monitor-stream-monitoring-data-event-hubs#what-can-i-do-with-the-monitoring-data-being-sent-to-my-event-hub)を使用して、IBM QRadar のように警告をストリームすることもできます。 SIEM の統合セキュリティ API のエンティティについての詳細[と、SIEM の統合](security-siemintegration.md)を参照してください。

### <a name="correlate-security-alerts-to-improve-threat-protection-and-response"></a>脅威の保護とレスポンスを向上させるためにセキュリティの警告の相関関係します。

セキュリティ ・ ソリューションより簡単に統合された通知スキーマの間でアラートを相互に関連づける。 これにより、実践的な警告情報を受け取ることが可能だけでなく、セキュリティ アナリストをピボットして、資産、およびユーザー情報を使用して脅威と資産の保護をより高速な応答を有効にするアラートの情報を追加することができます。  

### <a name="update-alert-tags-status-and-assignments"></a>警告タグ、ステータス、および割り当てを更新します。

アラートの応答と改善策を通知するために追加のコンテキストまたは脅威インテリジェンスのタグです。 すべてのワークフローの可視性の警告に関するコメントやフィードバックを取得することを確認します。 アラートの状態および割り当ての同期を維持できるように、すべての統合ソリューションは、現在の状態を反映します。 Webhook サブスクリプションを使用すると、変更の通知を取得します。  

### <a name="unlock-security-context-to-drive-investigation"></a>セキュリティ コンテキストをロックを解除して調査を促進

関連するセキュリティ関連インベントリ (ユーザー、ホスト、アプリなど) を深く掘り下げ、Microsoft Graph の他のプロバイダー (Azure AD、Microsoft Intune、Office 365) からの組織コンテキストを追加することにより、ビジネス コンテキストとセキュリティ コンテキストをまとめて、脅威への対応を向上させます。

### <a name="proactively-manage-security-risks-preview"></a>(プレビュー) のセキュリティ リスクをプロアクティブに管理します。

マイクロソフト セキュリティで保護されたスコア (プレビュー)、組織のセキュリティの可視性を提供する必要があります、その改善方法についての提案を得るし、これらの解決策が組み込まれた後、改良されたスコアをプロジェクトに使用します。 簡単に時間の経過と共に、進行状況を測定し、スコアの向上につながっている特定の変更の情報を取得します。

## <a name="benefits-of-using-the-microsoft-graph-security-api"></a>Microsoft グラフ セキュリティ API を使用する利点

Microsoft グラフ セキュリティ API を使用して統合することでさまざまなセキュリティ ・ ソリューションにアクセスできる利点を次の表に一覧します。  

|**領域**     | **利点**|
|:---------------|:---------|
|**管理セキュリティ サービス プロバイダー (Mssp)**|<ul><li>セキュリティ操作のツールとサービスの合理化された統合。</li> <li>展開および保守に要する時間の短縮と作業します。</li> <li>MSSP のお客様により多くの価値を提供する機能。</li></ul>|
|**SIEM と IT リスク管理ソリューション**|<ul><li>マイクロソフト セキュリティ ソリューションとパートナーのエコシステムをスムーズに統合します。</li> <li>豊富なメタデータを警告します。</li> <li>アラートの相関関係が向上。</li></ul>|
|**アプリケーション** <br>(脅威インテリジェンス、モバイル、クラウド、IOT、詐欺検出、アイデンティティとアクセス、リスクとコンプライアンス、ファイアウォール、およびように)|<ul><li>セキュリティ ・ ソリューションをさまざまな脅威の管理、予防、およびリスク管理を統合します。</li> <li>警告、在庫、構成、および Microsoft Graph を通じて公開されるアクション。</li> <li>Microsoft グラフが有効なソリューションとインスタントの統合。</li></ul>|

## <a name="api-reference"></a>API リファレンス
このサービスの API リファレンスを検索してください。

- [セキュリティ API Graph v1.0 の](/graph/api/resources/security-api-overview?view=graph-rest-1.0)
- [ベータ版の Microsoft Graph では、セキュリティ API](/graph/api/resources/security-api-overview?view=graph-rest-beta)

## <a name="next-steps"></a>次のステップ

- [Graph セキュリティ API を使用します。](/graph/api/resources/security-api-overview?view=graph-rest-1.0)
- セキュリティ プロバイダーになることに関心があるでしょうか。 [Graphsecfeedback](mailto:graphsecfeedback@microsoft.com)にアクセスします。
