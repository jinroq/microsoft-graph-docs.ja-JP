---
title: Azure AD 監査ログ API の概要
description: Azure Active Directory (Azure AD) は、ユーザーのアクティビティとサインインのメトリックを追跡し、ユーザーが Azure AD サービスにアクセスして使用する方法を把握するのに役立つ監査ログ レポートを作成します。 Azure AD 用の Microsoft Graph API を使用して、これらのレポートの基礎となるデータを分析したり、組織特有のニーズに合わせたカスタム ソリューションを作成したりします。
localization_priority: Priority
doc_type: conceptualPageType
ms.prod: ''
author: ''
ms.openlocfilehash: 9d739cbe711ad175e485ecb3d9d12173718a1b75
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35974242"
---
# <a name="azure-ad-audit-log-api-overview"></a>Azure AD 監査ログ API の概要

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Azure Active Directory (Azure AD) は、ユーザーのアクティビティとサインインのメトリックを追跡し、ユーザーが Azure AD サービスにアクセスして使用する方法を把握するのに役立つ監査ログ レポートを作成します。 Azure AD 用の Microsoft Graph API を使用して、これらのレポートの基礎となるデータを分析したり、組織特有のニーズに合わせたカスタム ソリューションを作成したりします。

## <a name="what-are-azure-ad-activity-logs"></a>Azure AD アクティビティ ログとは

Azure AD には、3 種類のアクティビティ ログが用意されています。

- 監査ログ 
- サインイン ログ
- プロビジョニング ログ

### <a name="audit-logs"></a>監査ログ

テナント内で実行されたすべてのタスクの履歴は、監査ログ アクティビティ レポートで把握できます。 監査ログ レポートから得られるシステム アクティビティの記録は、コンプライアンスに利用することができます。 特に、レポートから得たデータによって、日常的に発生する次のようなシナリオに対処することができます。

- ディレクトリのユーザーに管理者グループのアクセス権をだれが許可するか。

- 最近入手したアプリにサインインしているユーザーはだれか。

- ディレクトリ内でパスワードのリセットが何回行われたか。

### <a name="sign-in-logs"></a>サインイン ログ

監査ログ レポートによって報告されたタスクをだれが実行したかを把握するには、サインイン アクティビティ レポートが役立ちます。 サインイン アクティビティ レポートを利用すると、以下の事柄について把握できます。

- ユーザーのサインインにどのようなパターンがあるか。
- 先週、何人のユーザーがサインインを行ったか。
- これらのサインインはどのような状態か。

### <a name="provisioning-logs"></a>プロビジョニング ログ
プロビジョニング ログを使用すると、Azure AD のプロビジョニング サービスによって実行されるすべてのアクションを表示できます。 プロビジョニング ログを使うと、次のような質問に答えることができます。

- どのグループが ServiceNow で正常に作成されたか
- どのロールがアマゾン ウェブ サービスからインポートされたか
- どのユーザーが Workday で正常に作成されなかったか

## <a name="what-can-i-do-with-audit-log-apis-in-microsoft-graph"></a>Microsoft Graph の監査ログ API で実行できること

監査ログ データで行う一般的な要求を以下に示します。

Operation | URL
:----------|:----
テナント ユーザー アクティビティを取得する | [https://graph.microsoft.com/beta/auditLogs/directoryAudits](https://developer.microsoft.com/graph/graph-explorer?request=auditLogs/directoryAudits&version=beta)
テナント ユーザー サインインを取得する | [https://graph.microsoft.com/beta/auditLogs/signIns](https://developer.microsoft.com/graph/graph-explorer?request=auditLogs/signIns&version=beta)
プロビジョニング ログを取得する | [https://graph.microsoft.com/beta/auditLogs/directoryProvisioning](https://developer.microsoft.com/graph/graph-explorer?request=auditLogs/directoryProvisioning&version=beta)

## <a name="what-licenses-do-i-need"></a>必要なライセンス

監査ログ レポートは、ライセンスを取得した機能に関して利用できます。  特定の機能のライセンスがある場合、その機能の監査ログにもアクセスできます。

たとえば、セルフサービス パスワード監査レポートを利用するには、Azure AD Premium P1 ライセンスが必要です。  詳細については、[Azure AD ライセンス](https://azure.microsoft.com/pricing/details/active-directory/)をご覧ください。

サインイン レポートには、Azure AD Premium ライセンスが必要です。

詳細については、[Azure Active Directory の価格](https://azure.microsoft.com/pricing/details/active-directory/)をご覧ください。

## <a name="next-steps"></a>次の手順

- [アプリを登録](https://docs.microsoft.com/azure/active-directory/active-directory-reporting-api-prerequisites-azure-portal)して、監査ログの前提条件を満たします。 
- [監査ログ](https://docs.microsoft.com/azure/active-directory/active-directory-reporting-api-audit-samples)と[サインイン](https://docs.microsoft.com/azure/active-directory/active-directory-reporting-api-sign-in-activity-samples)のサンプルを参照して理解を深めます。  
- [ディレクトリ監査](directoryaudit.md) リソースとアクションを確認します。
- [サインイン](signin.md) リソースとアクションを確認します。 
- [プロビジョニング オブジェクト サマリー](provisioningobjectsummary.md)リソースを確認します。
