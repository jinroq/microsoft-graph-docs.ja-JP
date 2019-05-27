---
title: Microsoft Graph データ接続
description: 'Microsoft Graph データ接続は、コア データ パイプラインを通じてユーザーに Office 365 データや Microsoft Azure リソースを提供します。 Microsoft Graph データ接続を使用すると、Microsoft 提供の優れた開発ツールを使用して貴重なデータにアクセスするインテリジェントなアプリケーションを構築することができます。これらのツールはすべて、Microsoft のセキュリティで保護されたクラウド内にあります。 すべての企業が生産性の向上に関心を持っています。つまり、ナレッジ ワーカーの生産性を向上させる製品を構築することは、非常に大きなビジネス チャンスを意味します。 '
author: ajacks-msft
localization_priority: Priority
ms.prod: data-connect
ms.openlocfilehash: 10f5626a785e357677d6428b060e421a1bbf9138
ms.sourcegitcommit: 17eec88891d62b27dcc5d0abdff9fcff2186b31f
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/23/2019
ms.locfileid: "34407066"
---
# <a name="microsoft-graph-data-connect"></a>Microsoft Graph データ接続

Microsoft Graph データ接続は、ツールセットを使って Office 365 データおよび Microsoft Azure リソースをユーザーに提供します。 Microsoft Graph データ接続を使用すると、Microsoft 提供の優れた開発ツールを使用して貴重なデータにアクセスするインテリジェントなアプリケーションを構築することができます。これらのツールはすべて、Microsoft のセキュリティで保護されたクラウド内にあります。 すべての企業が生産性の向上に関心を持っています。つまり、ナレッジ ワーカーの生産性を向上させる製品を構築することは、非常に大きなビジネス チャンスを意味します。 

Microsoft Graph データ接続を活用する場合、「[Microsoft Graph 使用条件](https://developer.microsoft.com/ja-JP/graph/terms-of-use)」、「[Microsoft のプライバシーに関する声明](https://go.microsoft.com/fwlink/p/?LinkId=123161)」、および次に同意することになります。

- すべての Office 365 ユーザー向けにインテリジェントなアプリケーションを構築する ISV。
- Office 365 データにアクセスする組織内のユーザー向けにインテリジェントなアプリケーションを構築するエンタープライズ開発者。

## <a name="develop-a-pipeline-with-office-365-data"></a>Office 365 データによるパイプラインの開発
Microsoft Graph データ接続を使用すると、Microsoft Azure 内の最適なツールを利用して、Office 365 データに基づく新しい種類のアプリケーションを作成できます。 Azure Data Factory を使用して、よく使われる Azure データ ストア (Azure Data Lake Gen 1 / Gen 2 または Azure Blob Storage) に Office 365 データを移動できます。 この後、データを処理することも (たとえば、Azure Data Lake Analytics を使用)、Azure SQL Database などの別のストアに移動することもできます。 データは、アプリケーションのエンド ユーザー シナリオでサービスを提供するために使用できます。

Azure Data Factory パイプラインで Office 365 からデータを移動する前に、データ要求に対する承認依頼が、お客様の Office 365 管理者が指定したデータ承認者に送信されます。 データの移動は、データ承認者が承認した場合のみ開始されます。

## <a name="publish-your-app-as-an-azure-managed-application"></a>アプリを Azure 管理アプリケーションとして公開する
Microsoft Graph データ接続を使用してアプリケーションを開発したら、アプリケーションを他のユーザー (組織内のユーザーやより広い範囲のユーザー) が使用できるようにすることができます。 Microsoft Graph データ接続は、[Azure 管理アプリケーション](https://docs.microsoft.com/ja-JP/azure/managed-applications/overview)を使用して、他のユーザーが Microsoft Azure Marketplace を通じてこれらのアプリケーションを使用できるようにします。 Azure マネージド アプリケーション アプリケーションを使用すると、ISV およびエンタープライズ開発者は、顧客にターンキー ソリューションを提供することができます。 顧客はこれらのマネージド アプリケーションをサブスクリプションに展開し、ベンダー (ISV およびエンタープライズ開発者) はそのアプリケーションの管理とサポートを行います。 アプリケーション ベンダーが、保管中の暗号化などの[ポリシー](https://docs.microsoft.com/ja-JP/azure/managed-applications/overview#azure-policy)をアプリケーションに適用することにより、顧客は、データがより安全に取り扱われているという安心感を持つことができます。 アプリケーションは、[Azure Marketplace](https://docs.microsoft.com/ja-JP/azure/managed-applications/publish-marketplace-app)または [Azure サービス カタログ](https://docs.microsoft.com/ja-JP/azure/managed-applications/publish-service-catalog-app)のいずれかに公開できます。

アプリケーションをインストールする顧客は、サービスの使用条件、必要なデータ、各アプリケーション SKU の価格、リソース消費の概算コストを確認することができます。 購入者によって必要な展開プロパティが指定されると、リソースが提供されます。 これには、データの抽出を開始する Data Factory パイプラインが含まれます。 ベンダーは、インストール完了までの時間、アプリケーションの使用方法、サポートの受け方について説明した、アプリケーションの説明ファイルを提供します。

## <a name="next-steps"></a>次のステップ 
Microsoft Graph データ接続アプリケーションの開発を開始するには、「[Microsoft Graph データ接続の概要](data-connect-concept-overview.md)」を参照してください。
