---
title: Azure AD 監査ログ API の概要
description: Azure Active Directory (AD の Azure) は、ユーザーの活動およびサインインのメトリックを追跡し、監査を作成、ユーザーのアクセスし、Azure AD サービスを活用するのに役立つログ レポートを理解します。 これらのレポートの基になるデータを分析して、組織の特定のニーズに合わせた独自のソリューションを作成するのには、Azure AD 用の Microsoft グラフ API を使用します。
ms.openlocfilehash: b25e9820d4f6df0c6a38fc9784a37ce8a82ceeb1
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27067926"
---
# <a name="azure-ad-audit-log-api-overview"></a>Azure AD 監査ログ API の概要

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

Azure Active Directory (AD の Azure) は、ユーザーの活動およびサインインのメトリックを追跡し、監査を作成、ユーザーのアクセスし、Azure AD サービスを活用するのに役立つログ レポートを理解します。 これらのレポートの基になるデータを分析して、組織の特定のニーズに合わせた独自のソリューションを作成するのには、Azure AD 用の Microsoft グラフ API を使用します。

## <a name="what-are-azure-ad-activity-logs"></a>Azure AD の活動は、何をログに記録しますか。

Azure AD には、動作状況のログの 2 種類が用意されています。

- 監査ログ 
- サインインのログ

### <a name="audit-logs"></a>監査ログ

監査ログの利用状況レポートは、テナントで実行されるすべてのタスクの履歴へのアクセスを提供します。 監査ログ レポートは、コンプライアンスのためのシステム ・ アクティビティの記録を提供します。 、他のユーザーの間で提供されるデータには、一般的なシナリオを次のように対処することが有効にします。

- ディレクトリ ユーザに管理者グループのアクセスを許可するか。

- ユーザーは、最近買収したアプリケーションへのをサインインがでしょうか。

- ディレクトリ内でどのように多くのパスワードのリセットが行われたでしょうか。

### <a name="sign-in-logs"></a>ログを署名します。

サインインがアクティビティ ・ レポートでは、監査ログ レポートで報告されたタスクを実行したユーザーを確認できます。 サインインがアクティビティ ・ レポートでは、質問に回答できます。

- パターン、ユーザーのサインインとは何ですか。
- ユーザーの数は、最後の週でサインインがでしょうか。
- これらのサインインの状態とは何ですか。

## <a name="what-can-i-do-with-audit-log-apis-in-microsoft-graph"></a>監査ログでは、Microsoft Graph Api では、どうすれば?

監査ログのデータを操作するための一般的な要求を次に示します。

操作 | URL
:----------|:----
テナント ユーザー ・ アクティビティを取得します。 | [https://graph.microsoft.com/beta/auditLogs/directoryAudits](https://developer.microsoft.com/graph/graph-explorer?request=auditLogs/directoryAudits&version=beta)
テナント ユーザー サインインの問題を取得します。 | [https://graph.microsoft.com/beta/auditLogs/signIns](https://developer.microsoft.com/graph/graph-explorer?request=auditLogs/signIns&version=beta)

## <a name="what-licenses-do-i-need"></a>どのようなライセンスが必要ですか。

監査ログ レポートは、ライセンスを取得している機能を使用できます。  特定の機能のライセンスがあれば、その監査ログへのアクセスもあります。

たとえば、パスワードのセルフ サービスの監査レポートにアクセスするのには Azure AD プレミアム P1 のライセンスが必要です。  詳細については、 [Azure AD のライセンス](https://azure.microsoft.com/pricing/details/active-directory/)を参照してください。

サインインのレポートでは、Azure AD のプレミアム ライセンスが必要です。

詳細については、 [Azure AD の価格](https://azure.microsoft.com/pricing/details/active-directory/)を参照してください。

## <a name="next-steps"></a>次の手順

- 監査ログの必要条件を満たすためには、[アプリの登録](https://docs.microsoft.com/azure/active-directory/active-directory-reporting-api-prerequisites-azure-portal)をします。 
- [ログを監査](https://docs.microsoft.com/azure/active-directory/active-directory-reporting-api-audit-samples)し、[サインイン用のサンプル](https://docs.microsoft.com/azure/active-directory/active-directory-reporting-api-sign-in-activity-samples)について説明します。  
- [DirectoryAudit](directoryaudit.md)リソースと操作を確認します。
- [サインイン](signin.md)リソースと操作を確認します。 