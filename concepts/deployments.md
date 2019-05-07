---
title: 国内クラウドの展開
description: Microsoft のデータセンターのグローバル ネットワークに加えて、Microsoft クラウド サービスは 3 つの独立した国内クラウドで利用できます。 これらの国内クラウドバージョンは、特定の国の地理的な境界内に限定され、ローカル担当者が運用している Microsoft エンタープライズクラウドサービスの物理的および論理的なネットワークの分離されたインスタンスです。
ms.openlocfilehash: 1eeb6c91f8c5162ae0b372e758a81d57aa0daa7a
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/06/2019
ms.locfileid: "33599829"
---
# <a name="national-cloud-deployments"></a>国内クラウドの展開

Microsoft のデータセンターのグローバル ネットワークに加えて、Microsoft クラウド サービスは 3 つの独立した国内クラウドで利用できます。 これらの国内クラウドバージョンは、特定の国の地理的な境界内に限定され、ローカル担当者が運用している Microsoft エンタープライズクラウドサービスの物理的および論理的なネットワークの分離されたインスタンスです。

現在の国内クラウドは、次のとおりです。

- Microsoft Cloud for US Government
- Microsoft Cloud Germany
- 21Vianet が中国で運用している Azure と Office 365

各 national クラウド環境は、Microsoft グローバル環境とは異なり、それぞれ異なるものです。 これらの主要な違いのいくつかは、各国のクラウド環境のアプリケーションを開発する際に知っておくことが重要です。たとえば、アプリケーションの登録、トークンの取得、および Microsoft Graph API の呼び出しは異なる場合があります。

この記事では、さまざまな Microsoft Graph 国内クラウド展開と、それぞれの開発者が使用できる機能について説明します。

>**注:**[Microsoft Graph データ接続](https://docs.microsoft.com/en-us/graph/data-connect-concept-overview?view=graph-rest-1.0)では、国内クラウド展開はサポートされていません。 

## <a name="app-registration-and-token-service-root-endpoints"></a>アプリの登録とトークンサービスのルートエンドポイント

Microsoft Graph Api を呼び出す前に、最初にアプリケーションを登録し、トークンを取得する必要があります。 次の表に、Azure Active Directory (Azure AD) エンドポイントのベース Url を示します。これにより、アプリケーションが登録され、各国立 cloud のトークンが取得されます。

| 国内クラウド | Azure AD ポータルエンドポイント| Azure AD エンドポイント|
|---------------------------|----------------|----------------|
|米国政府機関向け Azure AD |https://portal.azure.us|`https://login.microsoftonline.us`|
|Azure AD Germany |https://portal.microsoftazure.de|`https://login.microsoftonline.de`|
|21Vianet によって運営されている Azure AD China |https://portal.azure.cn|`https://login.chinacloudapi.cn`|
|Azure AD (グローバル サービス)|https://portal.azure.com |`https://login.microsoftonline.com`|

Azure AD のアクセストークンと Microsoft Graph の詳細については、「 [authentication の基礎](./auth/auth-concepts.md)」を参照してください。 Azure AD 認証のシナリオについては、「 [AZURE ad 認証の基礎](https://docs.microsoft.com/azure/active-directory/develop/authentication-scenarios)」を参照してください。

> **注:** [Azure AD v2.0 認証エンドポイントとトークン エンドポイント](https://docs.microsoft.com/azure/active-directory/develop/v2-overview)はグローバル サービスでのみ使用できます。国内クラウド展開での使用はまだサポートされていません。


## <a name="microsoft-graph-and-graph-explorer-service-root-endpoints"></a>Microsoft Graph および Graph エクスプローラサービスのルートエンドポイント

次の表に、各 national クラウドの Microsoft Graph および[Graph Explorer](https://developer.microsoft.com/graph/graph-explorer)のサービスルートエンドポイントを示します。

| 国内クラウド | Microsoft Graph | Graph エクスプローラー |
|---------------------------|----------------|----------------|
| US Government L4 の Microsoft Graph | https://graph.microsoft.us | サポートされていません。 |
| 米国政府の L5 (DOD) の Microsoft Graph | https://dod-graph.microsoft.us | サポートされていません。 |
| Microsoft Graph Germany | https://graph.microsoft.de | サポートされていません。 |
| 21Vianet によって運営されている Microsoft Graph China | https://microsoftgraph.chinacloudapi.cn | https://developer.microsoft.com/zh-cn/graph/graph-explorer-china |
| Microsoft Graph グローバル サービス | https://graph.microsoft.com | https://developer.microsoft.com/graph/graph-explorer |

>**重要:** 米国政府機関に既にアプリがあり、ワールドワイドエンドポイント`https://graph.microsoft.com`を使用している場合は、新しい`https://graph.microsoft.us`エンドポイントに切り替えることをお勧めします。 世界各地のエンドポイントを使用した米国政府データへのアクセスは現在機能していますが、近い将来は無効になります。

> **メモ**: アプリから組織のデータへは、国内クラウド エンドポイント経由でのみアクセスできます。 これは、アプリが特定の全国クラウドに登録されているテナントのデータにのみアクセスできることを意味します。 Microsoft Graph を使用して Microsoft 個人アカウントに関連付けられているコンシューマーデータにアクセスしよう`https://graph.microsoft.com`としているアプリには、グローバルサービスを使用する必要があります。 国内クラウド展開用に取得されたアクセストークンは、グローバルサービスまたはその他の全国クラウドで取得したものとは互換性がありません。

## <a name="supported-features"></a>サポートされている機能

次の Microsoft Graph 機能は、通常、すべて`/v1.0`の国内クラウド展開のエンドポイントで使用できます (記載されている場合を除く)。

| Microsoft Graph の機能 | Microsoft Cloud for US Government | 21Vianet が運用している Microsoft Cloud 中国 | Microsoft Cloud Germany |
|---------------------------|----------------|----------------|----------------|
| ユーザー | ✔ | ✔ | ✔ |
| グループ | ✔ | ✔ | ✔ |
| Excel | ✔| ✔* | ✔ |
| OneDrive | ✔ | ✔* | ✔ |
| Outlook メール | ✔ | ✔ | ✔ |
| Outlook の予定表 | ✔ | ✔ | ✔ |
| 個人用連絡先 | ✔ | ✔ | ✔ |
| SharePoint| ✔ | ✔ | ✔ |
| Planner|✔ |✔ |✔ |
| レポート  |➖| ✔ |➖|
| 変更通知 (webhooks)  | ➖|✔* |✔* |
| デルタ クエリ | ➖ | ➖| ➖ |
| ディレクトリ スキーマの拡張 |➖|➖|➖|
| オープン型の拡張機能|➖|➖|➖|
  
次に示すその他の Microsoft Graph 機能は、(エンド`/beta`ポイントの) すべての国内クラウド展開で使用できます (記載されている場合を除く)。

* 組織の連絡先
* アプリケーション
* サービス プリンシパル
* 変更通知 (webhooks)

(*)Exchange および OneDrive サービスのみのサポートが制限されています。 Azure AD サービスはサポートされていません。 

 > **重要:** グローバルサービスの特定の地域にある特定のサービスや機能は、国内のすべてのクラウドでは利用できない場合があります。 利用可能なサービスについては、「[利用可能な製品 (地域別](https://azure.microsoft.com/global-infrastructure/services/?products=all&regions=usgov-non-regional,us-dod-central,us-dod-east,usgov-arizona,usgov-iowa,usgov-texas,usgov-virginia,china-non-regional,china-east,china-east-2,china-north,china-north-2,germany-non-regional,germany-central,germany-northeast))」を参照してください。


各国の雲の詳細については、以下のトピックを参照してください。
- [Microsoft 国立クラウド](https://www.microsoft.com/TrustCenter/CloudServices/NationalCloud)
- [米国政府機関向け Office 365](https://docs.microsoft.com/office365/servicedescriptions/office-365-platform-service-description/office-365-us-government/office-365-us-government)
- [21Vianet が運用している Office 365](https://docs.microsoft.com/office365/servicedescriptions/office-365-platform-service-description/office-365-operated-by-21vianet)
- [Office 365 Germany](https://docs.microsoft.com/office365/servicedescriptions/office-365-platform-service-description/office-365-germany)
- [Azure Government](https://azure.microsoft.com/global-infrastructure/government/)
- [Azure 中国21Vianet](https://docs.microsoft.com/azure/china/)
- [Azure ドイツ](https://docs.microsoft.com/azure/germany/)
