---
title: Graph セキュリティ API を使用します。
description: Microsoft グラフ セキュリティ API は、統一されたインタ フェースとマイクロソフトとエコシステムのパートナーからのセキュリティ ソリューションと統合するためにスキーマを提供します。 これは、セキュリティ ・ オペレーションを合理化し、サイバー脅威の増加が防御よりのお客様を支援します。 Microsoft グラフ セキュリティ API は、集約された応答を取得するすべての onboarded セキュリティ プロバイダーにクエリを発行するフェデレーション セキュリティ集約サービスとして使用できます。 Microsoft グラフ セキュリティ API を使用してアプリケーションを構築します。
ms.openlocfilehash: 511abbc6221ee9efb58cbfb36082514d98f9b918
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27024310"
---
# <a name="use-the-microsoft-graph-security-api"></a>Graph セキュリティ API を使用します。

Microsoft グラフ セキュリティ API は、統一されたインタ フェースとマイクロソフトとエコシステムのパートナーからのセキュリティ ソリューションと統合するためにスキーマを提供します。 これは、セキュリティ ・ オペレーションを合理化し、サイバー脅威の増加が防御よりのお客様を支援します。 Microsoft グラフ セキュリティ API は、集約された応答を取得するすべての onboarded セキュリティ プロバイダーにクエリを発行するフェデレーション セキュリティ集約サービスとして使用できます。 Microsoft グラフ セキュリティ API を使用してアプリケーションを構築します。

- 統合し、複数のソースからのセキュリティの警告の相関関係
- 調査を通知するためにコンテキストのデータのロックを解除します。
- 効率のセキュリティ ・ オペレーションを自動化します。
- プロアクティブ リスク管理を有効にするセキュリティ ・ データの可視性を提供します。

Microsoft グラフ セキュリティ API には、次のキーのエンティティが含まれています。

## <a name="alerts"></a>アラート

通知は、マイクロソフトまたはパートナーのセキュリティ ・ ソリューションが既に特定し、アクションの通知フラグが設定されているお客様のテナント内で潜在的なセキュリティ上の問題です。 Microsoft グラフのセキュリティの[警告](alert.md)のエンティティとを統合し、すべての統合されたソリューションのセキュリティの問題を合理化できます。 これは、アプリケーションのアラートおよび脅威の保護とレスポンスを向上させるためにコンテキストを関連付けることもできます。 これらは、インシデントの解決方法を調査の時間と時間を減らすことでセキュリティの運用効率をアンロックします。 アラートの更新機能により、さまざまなセキュリティ製品およびサービスの[アラート](alert.md)のエンティティを更新することによって、Microsoft グラフ セキュリティ API と統合されている間、特定のアラートの状態を同期できます。

グラフのセキュリティに統合されたソリューションの Microsoft 次のセキュリティ プロバイダーからのアラートが表示されます。

- Azure のセキュリティ センター
- Azure Active Directory Id の保護
- Azure の情報の保護
- マイクロソフト クラウド アプリケーションのセキュリティ
- Windows Defender の脅威保護の詳細
- Microsoft Intune (プライベート プレビュー)
- Office 365 の (準備中)
- Azure 高度な脅威の保護 (準備中)
- パートナー ・ ソリューション、パロアルトのネットワーク ・ アプリケーション ・ フレームワーク

> **注:** 新しいプロバイダーは、Microsoft のグラフのセキュリティ エコシステムの契約時では継続的にします。

## <a name="common-use-cases"></a>一般的なユース ケース

以下は、Microsoft グラフ セキュリティ API を使用するための最も一般的な要求の一部です。

| **ユース ケース**   | **REST リソース** | **グラフのエクスプ ローラーで試してみよう** |
|:---------------|:--------|:----------|
| 警告の一覧表示 | [警告の一覧表示](../api/alert-list.md) | [https://graph.microsoft.com/v1.0/security/alerts](https://developer.microsoft.com/graph/graph-explorer?request=security/alerts&method=GET&version=v1.0&GraphUrl=https://graph.microsoft.com) |
| アラートを更新します。 | [警告の更新](../api/alert-update.md) | [https://graph.microsoft.com/v1.0/security/alerts/{alert-id}](https://developer.microsoft.com/graph/graph-explorer?request=security/alerts/{alert-id}&method=PATCH&version=v1.0&GraphUrl=https://graph.microsoft.com) |

購読して、Microsoft のグラフのセキュリティ エンティティの更新に関する通知を受け取るには、Graph [webhooks](/graph/webhooks)を使用できます。

## <a name="resources"></a>リソース

コードされ、これらの Microsoft グラフ セキュリティ API のサンプル。

- [サンプルの ASP.NET (C#)](https://github.com/microsoftgraph/aspnet-security-api-sample)
- [Python のサンプル](https://github.com/microsoftgraph/python-security-rest-sample)
- [Node.js (JavaScript) のサンプル](https://github.com/microsoftgraph/nodejs-security-sample)

コミュニティに参加します。

- [テクニカル コミュニティに参加します。](https://aka.ms/graphsecuritycommunity)
- [StackOverflow を説明します。](https://stackoverflow.com/questions/tagged/microsoft-graph-security)

## <a name="next-steps"></a>次の手順

Microsoft グラフ セキュリティ API は、Microsoft およびパートナーからのさまざまなセキュリティ ソリューションと連携するための新しい方法を開くことができます。 開始する次の手順に従います。

- [アラート](alert.md)にドリル ・ ダウンします。
- [Graph エクスプローラー](https://developer.microsoft.com/graph/graph-explorer)で API をお試しください。 [**サンプル クエリ**] は、**多くのサンプルを表示する**を選択し、セキュリティ カテゴリを**オン**に設定します。
- エンティティの変更[をサブスクライブして、受信通知](/graph/webhooks)を実行してください。

さらに情報が必要な場合「[パートナーによる Microsoft Graph の活用方法](https://developer.microsoft.com/graph/graph/examples#partners)」を参照してください。
