---
title: Business Central API の概要
description: ソリューションをビジネス中央 api と統合する理由の概要。
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
ms.openlocfilehash: 0602b02592bec5210f243f77654a52ba96e6746a
ms.sourcegitcommit: f2444a37a719b87777bdddbd086f106746fa0a1c
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/02/2019
ms.locfileid: "30366803"
---
# <a name="dynamics-365-business-central-api-overview-preview"></a>Dynamics 365 Business Central API の概要 (プレビュー)
Dynamics 365 business Central は、簡単に使用および適応できる、オールインワンのビジネス管理ソリューションであり、ビジネスへの接続と高度な意思決定を支援します。 これにより、ビジネスのエンドツーエンドのビューが提供され、財務を管理し、サプライチェーンを自動化してセキュリティで保護し、顧客サービスをさらに向上させ、プロジェクトを時間と予算の下に保持し、運用を最適化することができます。

## <a name="why-integrate-with-dynamics-365-business-central"></a>Dynamics 365 Business Central と統合する理由
アプリケーションを Dynamics 365 Business Central に統合することで、ビジネスニーズにまたがるエクスペリエンスを作成できます。 ユーザーが主要なビジネスタスクおよび機能を実行できるようにするソリューションを作成できます。 Microsoft Graph を使用して、財務報告書にアクセスしたり、取引先担当者と連携したり、販売および購入するドキュメントを作成および送信したり、財務報告を取得したりすることができます。 

### <a name="synchronize-your-business-applications"></a>ビジネスアプリケーションを同期する
多くの企業では、さまざまな非接続のビジネスアプリケーションを使用して、ビジネスのさまざまな機能を管理しています。 Microsoft Graph を使用すると、データを接続してこれらのアプリケーションをまとめることができます。 これにより、給与アプリケーションを従業員レコードに接続したり、経費アプリケーションをベンダーレコードに接続したり、CRM アプリケーションで顧客レコードを最新の状態に保つことが容易になります。 データを接続して、アプリケーションの同期を維持します。

### <a name="create-custom-apps-to-manage-your-business-processes"></a>ビジネスプロセスを管理するためのカスタムアプリを作成する
すべてのビジネスは異なり、特化したビジネスプロセスを持つことができます。 これらのプロセスは、プロセスに合わせたカスタムアプリを使用して簡素化できます。 Microsoft Graph を使用すると、これらのアプリを財務データと統合するのが容易になります。 販売ドキュメント、購入ドキュメントを作成する経費アプリ、または総勘定元帳を作成する給与アプリを作成する sales または field service アプリを構築して、すべてのドキュメントを財務システムに保持できるようになります。

### <a name="gain-insights-from-your-financial-data"></a>財務データから洞察を得る
Microsoft Graph は、財務レポートへのアクセスを提供します。 bi ツールとアプリを貸借対照表、キャッシュフロー明細書、支払いおよび債権のエイジングレポート、および試用残高レポートに接続して、bi ダッシュボードを作成し、ユーザーが必要な情報にアクセスできるようにします。

## <a name="authorization"></a>Authorization
Azure AD v2.0 エンドポイントを使用して、Dynamics 365 Business Central api を認証します。 すべての api に`Authorization: Bearer {access-token}`は、要求ヘッダーが必要です。 承認の詳細については、「 [Microsoft Graph を呼び出せるようにアクセストークンを取得する](auth-overview.md)」を参照してください。

## <a name="api-reference"></a>API リファレンス
このサービスの API リファレンスをお探しですか?

「 [Dynamics 365 Business Central API in Microsoft Graph beta」を](/graph/api/resources/dynamics-graph-reference?view=graph-rest-beta)参照してください。


## <a name="next-steps"></a>次の手順
Microsoft Graph でサポートされている[ビジネスセンター API とユースケース](/graph/api/resources/dynamics-graph-reference?view=graph-rest-beta)の詳細については、こちらを参照してください。
