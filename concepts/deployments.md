---
title: 国内クラウドの展開
description: Microsoft のデータセンターのグローバル ネットワークに加えて、Microsoft クラウド サービスは 3 つの独立した国内クラウドで利用できます。 これらの国の雲のバージョンは、物理および論理ネットワークの分離のインスタンスを特定の国の地理的な境界の内部に限定され、ローカル スタッフによって運営されている Microsoft のエンタープライズのクラウド サービスです。
ms.openlocfilehash: 06ca3c24cba17e2d18fc4755f00a2c754e508f88
ms.sourcegitcommit: 597dfc95a44e0f2354d056b5567bcff2bb2837f1
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/12/2019
ms.locfileid: "29892499"
---
# <a name="national-cloud-deployments"></a>国内クラウドの展開

Microsoft のデータセンターのグローバル ネットワークに加えて、Microsoft クラウド サービスは 3 つの独立した国内クラウドで利用できます。 これらの国の雲のバージョンは、物理および論理ネットワークの分離のインスタンスを特定の国の地理的な境界の内部に限定され、ローカル スタッフによって運営されている Microsoft のエンタープライズのクラウド サービスです。

現在の国内クラウドは、次のとおりです。

- Microsoft Cloud for US Government
- Microsoft Cloud Germany
- 21Vianet が中国で運用している Azure と Office 365

各国内のクラウド環境では一意であり、マイクロソフトのグローバル環境とは異なります。 国内のクラウド環境向けのアプリケーションを開発するときにこれらの重要な違いがいくつかに注意する必要がなどのアプリケーションを登録して、トークンを取得する、Microsoft グラフ API を呼び出すことが異なることがあります。

この資料では、別の Microsoft Graph 国内クラウド展開し、各開発者に提供される機能についての情報を提供します。

## <a name="app-registration-and-token-service-root-endpoints"></a>アプリケーションの登録、トークン サービスのルート エンドポイント

Microsoft グラフ Api を呼び出す前にまず、アプリケーションを登録し、トークンを取得する必要があります。 アプリケーションを登録し、各国内のクラウド用のトークンを取得する Azure Active Directory (AD の Azure) エンドポイントのベース Url を次の表に一覧します。

| 国内クラウド | Azure AD ポータルのエンドポイント| Azure AD エンドポイント|
|---------------------------|----------------|----------------|
|米国政府機関向け Azure AD |https://portal.azure.us|`https://login.microsoftonline.us`|
|Azure AD Germany |https://portal.microsoftazure.de|`https://login.microsoftonline.de`|
|21Vianet によって運営されている Azure AD China |https://portal.azure.cn|`https://login.chinacloudapi.cn`|
|Azure AD (グローバル サービス)|https://portal.azure.com |`https://login.microsoftonline.com`|

Azure AD に関するその他のアクセス トークンと Microsoft のグラフについては、[認証トークンを取得する](./auth-overview.md)を参照してください。 Azure AD 認証シナリオでは、 [Azure AD の基本認証](https://docs.microsoft.com/azure/active-directory/develop/authentication-scenarios)を参照してください。

> **注:** [Azure AD v2.0 認証エンドポイントとトークン エンドポイント](https://docs.microsoft.com/azure/active-directory/develop/v2-overview)はグローバル サービスでのみ使用できます。国内クラウド展開での使用はまだサポートされていません。


## <a name="microsoft-graph-and-graph-explorer-service-root-endpoints"></a>グラフとグラフのエクスプ ローラーのサービスのルート エンドポイント

次の表は、グラフと[グラフのエクスプ ローラー](https://developer.microsoft.com/graph/graph-explorer)の各国内のクラウド サービスのルート エンドポイントを示します。

| 国内クラウド | Microsoft Graph | Graph エクスプローラー |
|---------------------------|----------------|----------------|
| 米国政府機関向け Microsoft Graph | https://graph.microsoft.us | サポートされていません。 |
| Microsoft Graph Germany | https://graph.microsoft.de | サポートされていません。 |
| 21Vianet によって運営されている Microsoft Graph China | https://microsoftgraph.chinacloudapi.cn | https://developer.microsoft.com/zh-cn/graph/graph-explorer-china |
| Microsoft Graph グローバル サービス | https://graph.microsoft.com | https://developer.microsoft.com/graph/graph-explorer |

> **メモ**: アプリから組織のデータへは、国内クラウド エンドポイント経由でのみアクセスできます。 つまり、アプリケーションは、特定の国のクラウドに登録されているテナントのデータにのみアクセスできます。 Graph での個人用の Microsoft アカウントに関連付けられたコンシューマー データにアクセスしようとしているアプリケーションはグローバル サービスを使用する必要があります`https://graph.microsoft.com`。 国内クラウド導入のための獲得、アクセス トークンは、グローバル ・ サービスまたはその他の国内クラウドのための獲得と交換可能ではありません。

## <a name="supported-features"></a>サポートされている機能

次のグラフ機能で一般に利用可能な`/v1.0`で示されている場合を除く、すべての国内クラウド展開のエンドポイントです。

| グラフ機能 | Microsoft Cloud for US Government | マイクロソフト クラウド中国の 21Vianet によって運営されて | Microsoft Cloud Germany |
|---------------------------|----------------|----------------|----------------|
| ユーザー | ✔ | ✔ | ✔ |
| グループ | ✔ | ✔ | ✔ |
| Excel | ✔| ✔* | ✔ |
| OneDrive | ✔ | ✔* | ✔ |
| Outlook メール | ✔ | ✔ | ✔ |
| Outlook カレンダー | ✔ | ✔ | ✔ |
| 個人用連絡先 | ✔ | ✔ | ✔ |
| SharePoint| ✔ | ✔* | ✔ |
| プランナー|✔ |✔ |✔ |
| レポート  |➖| ✔ |➖|
| デルタ クエリ | ➖ | ➖| ➖ |
| Webhook  | ➖| ➖| ➖
|ディレクトリ スキーマの拡張 |➖|➖|➖|
| オープン型の拡張機能|➖|➖|➖|
  
プレビューで次のようなグラフの追加の機能がある (で、`/beta`エンドポイント) で示されている場合を除く、すべての国内クラウド展開。

* 組織の連絡先
* アプリケーション
* サービス プリンシパル

(*)この雲の中には、この API の制限付きサポートします。

 > **重要:** 特定のサービスと、グローバル ・ サービスの特定の領域では機能できない可能性があります国内の雲の中のすべての。 利用できるどのようなサービスを調べるには、[地域で利用可能な製品](https://azure.microsoft.com/global-infrastructure/services/?products=all&regions=usgov-non-regional,us-dod-central,us-dod-east,usgov-arizona,usgov-iowa,usgov-texas,usgov-virginia,china-non-regional,china-east,china-east-2,china-north,china-north-2,germany-non-regional,germany-central,germany-northeast)を参照してください。


国内クラウドに関する詳細については、次のトピックを参照してください。
- [Microsoft 国立雲](https://www.microsoft.com/TrustCenter/CloudServices/NationalCloud)
- [米国政府の office 365](https://docs.microsoft.com/office365/servicedescriptions/office-365-platform-service-description/office-365-us-government/office-365-us-government)
- [21Vianet が運用している Office 365](https://docs.microsoft.com/office365/servicedescriptions/office-365-platform-service-description/office-365-operated-by-21vianet)
- [Office 365 のドイツ](https://docs.microsoft.com/office365/servicedescriptions/office-365-platform-service-description/office-365-germany)
- [Azure の政府](https://azure.microsoft.com/global-infrastructure/government/)
- [Azure の中国の 21Vianet](https://docs.microsoft.com/azure/china/)
- [Azure ドイツ](https://docs.microsoft.com/azure/germany/)
