---
title: 国内クラウドの展開
description: Microsoft のデータセンターのグローバル ネットワークに加えて、Microsoft クラウド サービスは 3 つの独立した国内クラウドで利用できます。 これらの国内クラウド バージョンは、Microsoft エンタープライズ クラウド サービスの物理的および論理的ネットワークの独立したインスタンスで、特定の国の地理的な境界内に限定され、ローカル スタッフによって運営されます。 詳細については、「Microsoft National Clouds」 (Microsoft の国内クラウド) を参照してください。
localization_priority: Priority
ms.openlocfilehash: b22fce675bc97d0f22833d89dab01afd18e06032
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27840419"
---
# <a name="national-cloud-deployments"></a>国内クラウドの展開


Microsoft のデータセンターのグローバル ネットワークに加えて、Microsoft クラウド サービスは 3 つの独立した国内クラウドで利用できます。 これらの国内クラウド バージョンは、Microsoft エンタープライズ クラウド サービスとは物理的および論理的に独立したネットワーク インスタンスで、特定の国の地理的な境界内に限定され、現地スタッフによって運営されます。 詳細については、「[Microsoft の国内クラウド](https://www.microsoft.com/ja-JP/TrustCenter/CloudServices/NationalCloud)」を参照してください。

現在の国内クラウドは、次のとおりです。

- Microsoft Cloud for US Government
- Microsoft Cloud Germany
- 21Vianet が中国で運用している Azure と Office 365

この記事では、Microsoft Graph のさまざまな国内クラウドの展開と、各展開において開発者が利用できる機能について示します。

## <a name="microsoft-graph-and-microsoft-graph-explorer-service-root-endpoints"></a>Microsoft Graph と Microsoft Graph Explorer のサービス ルート エンドポイント

次の表に、各国内クラウドの Microsoft Graph と Microsoft Graph Explorer のサービス ルート エンドポイントを示します。

| 国内クラウド | Microsoft Graph | Microsoft Graph Explorer
|---------------------------|----------------|----------------|
| 21Vianet によって運営されている Microsoft Graph China | https://microsoftgraph.chinacloudapi.cn | https://developer.microsoft.com/zh-cn/graph/graph-explorer-china |
| Microsoft Graph Germany | https://graph.microsoft.de | サポートされていません。 |
| 米国政府機関向け Microsoft Graph | https://graph.microsoft.com | サポートされていません。 |
| Microsoft Graph グローバル サービス | https://graph.microsoft.com | https://developer.microsoft.com/graph/graph-explorer |

> **メモ**: アプリから組織のデータへは、国内クラウド エンドポイント経由でのみアクセスできます。 つまり、特定の国内クラウドに登録されたテナント内のデータにのみアクセスできます。 Microsoft Graph を介して個人用 Microsoft アカウントに関連付けられているコンシューマー データにアクセスを試みるアプリには、グローバル サービス (https://graph.microsoft.com) を使用する必要があります。 国内クラウドの展開用に獲得したアクセス トークンは、グローバル サイト用に獲得したアクセス トークンと交換して使用することはできません。

## <a name="azure-ad-openid-connect-and-oauth20-endpoints"></a>Azure AD の OpenID Connect と OAuth2.0 のエンドポイント

次の表に、国内クラウドごとに Microsoft Graph を呼び出すためのトークンを獲得するときに使用される Azure Active Directory (Azure AD) エンドポイントのベース URL をまとめます。

| 国内クラウド | Azure AD ルート エンドポイント |
|---------------------------|----------------|
| 21Vianet によって運営されている Azure AD China |https://login.chinacloudapi.cn |
| Azure AD Germany | https://login.microsoftonline.de |
| 米国政府機関向け Azure AD | https://login.microsoftonline.us |
| Azure AD (グローバル サービス) | https://login.microsoftonline.com |

Azure AD 承認またはトークン エンドポイントへの要求は、該当する地域特有のベース URL を使用します。たとえば、ドイツの場合:

- 承認の共通エンドポイントは、https://login.microsoftonline.de/common/oauth2/authorize です。
- トークンの共通エンドポイントは、https://login.microsoftonline.de/common/oauth2/token です。

テナント特有のエンドポイントは、前述の URL の「common」の部分を、テナント ID またはテナントの検証済みドメインに置き換えて構成できます。共通エンドポイントまたはテナント特有のエンドポイントのどちらを使用するかは、アプリの要件と、トークンを取得するために使用している認証フローによって異なります。Azure AD のアクセス トークンと Microsoft Graph について詳しくは、「[認証トークンの取得](./auth-overview.md)」を参照してください。

> **注:** [Azure AD v2.0 認証エンドポイントとトークン エンドポイント](https://azure.microsoft.com/ja-JP/documentation/articles/active-directory-appmodel-v2-overview/)はグローバル サービスでのみ使用できます。国内クラウド展開での使用はまだサポートされていません。

## <a name="supported-features"></a>サポートされている機能

次の Microsoft Graph 機能が、注記されている場所を除くすべての国内クラウド展開で (`/v1.0` エンドポイント上で) 通常利用できます。

* ユーザー
* グループ
* Excel (中国で 21Vianet によって運営されている Microsoft Graph に限定してサポート)
* OneDrive (中国で 21Vianet によって運営されている Microsoft Graph に限定してサポート)
* Outlook メール
* Outlook カレンダー
* 個人用連絡先 
* SharePointl (中国で 21Vianet によって運営されている Microsoft Graph に限定してサポート)
* デルタ クエリ (各国内クラウド展開のさまざまなリソースにおいてサポートが異なります)。
* Webhook (各国内クラウド展開のさまざまなリソースにおいてサポートが異なります)。

次の Microsoft Graph 追加機能が、注記されている場所を除くすべての国内クラウド展開で通常、プレビュー段階として (`/beta` エンドポイント上で) 利用できます。

* 組織の連絡先
* アプリケーション
* サービス プリンシパル

次の Microsoft Graph 機能に関しては、国内クラウド展開ではまだサポートされていません。

* Microsoft Planner
* ディレクトリ スキーマの拡張
* オープン型の拡張機能
