---
title: Business Central API の概要
description: ソリューションをビジネス中央 Api と統合する理由の概要。
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
ms.openlocfilehash: aafc7e6f1f7a688d1f083c584ceedc8a11878866
ms.sourcegitcommit: 7c03131291113c343a98bb0234d31bd4535a4050
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/22/2019
ms.locfileid: "35133741"
---
# <a name="dynamics-365-business-central-api-overview-preview"></a>Dynamics 365 Business Central API の概要 (プレビュー)
Dynamics 365 Business Central は、簡単に使用および適応できる、オールインワンのビジネス管理ソリューションであり、ビジネスへの接続と高度な意思決定を支援します。 これにより、ビジネスのエンドツーエンドのビューが提供され、財務を管理し、サプライチェーンを自動化してセキュリティで保護し、顧客サービスをさらに向上させ、プロジェクトを時間と予算の下に保持し、運用を最適化することができます。

> [!VIDEO https://www.youtube-nocookie.com/embed/na1kFk53cbk]

## <a name="why-integrate-with-dynamics-365-business-central"></a>Dynamics 365 Business Central と統合する理由
アプリケーションを Dynamics 365 Business Central に統合することで、ビジネスニーズにまたがるエクスペリエンスを作成できます。 ユーザーが主要なビジネスタスクおよび機能を実行できるようにするソリューションを作成できます。 Microsoft Graph を使用して、財務報告書にアクセスしたり、取引先担当者と連携したり、販売および購入するドキュメントを作成および送信したり、財務報告を取得したりすることができます。

### <a name="synchronize-your-business-applications"></a>ビジネスアプリケーションを同期する
多くの企業では、さまざまな非接続のビジネスアプリケーションを使用して、ビジネスのさまざまな機能を管理しています。 Microsoft Graph を使用すると、データを接続してこれらのアプリケーションをまとめることができます。 これにより、給与アプリケーションを従業員レコードに接続したり、経費アプリケーションをベンダーレコードに接続したり、CRM アプリケーションで顧客レコードを最新の状態に保つことが容易になります。 データを接続して、アプリケーションの同期を維持します。

### <a name="create-custom-apps-to-manage-your-business-processes"></a>ビジネスプロセスを管理するためのカスタムアプリを作成する
すべてのビジネスは異なり、特化したビジネスプロセスを持つことができます。 これらのプロセスは、プロセスに合わせたカスタムアプリを使用して簡素化できます。 Microsoft Graph を使用すると、これらのアプリを財務データと統合するのが容易になります。 販売ドキュメント、購入ドキュメントを作成する経費アプリ、または総勘定元帳を作成する給与アプリを作成する sales または field service アプリを構築して、すべてのドキュメントを財務システムに保持できるようになります。

### <a name="gain-insights-from-your-financial-data"></a>財務データから洞察を得る
Microsoft Graph は、財務レポートへのアクセスを提供します。 BI ツールとアプリを貸借対照表、キャッシュフロー明細書、支払いおよび債権のエイジングレポート、および試用残高レポートに接続して、BI ダッシュボードを作成し、ユーザーが必要な情報にアクセスできるようにします。

## <a name="authorization"></a>Authorization
Azure AD v2.0 エンドポイントを使用して、Dynamics 365 Business Central Api を認証します。 すべての Api に`Authorization: Bearer {access-token}`は、要求ヘッダーが必要です。 承認の詳細については、「 [Microsoft Graph を呼び出せるようにアクセストークンを取得する](/graph/auth)」を参照してください。

## <a name="api-reference"></a>API リファレンス
このサービスの API リファレンスをお探しですか?

「 [Dynamics 365 Business CENTRAL API In Microsoft Graph beta」を](/graph/api/resources/dynamics-graph-reference?view=graph-rest-beta)参照してください。


## <a name="next-steps"></a>次のステップ
Microsoft Graph でサポートされている[ビジネスセンター API とユースケース](/graph/api/resources/dynamics-graph-reference?view=graph-rest-beta)の詳細については、こちらを参照してください。
