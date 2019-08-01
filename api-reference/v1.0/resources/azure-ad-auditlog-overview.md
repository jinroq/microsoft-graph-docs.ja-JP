---
title: Azure AD 監査ログ API の概要
description: Azure Active Directory (Azure AD) は、ユーザーのアクティビティとサインインのメトリックを追跡し、ユーザーが Azure AD サービスにアクセスして使用する方法を把握するのに役立つ監査ログ レポートを作成します。
localization_priority: Priority
author: dhanyahk
ms.prod: microsoft-identity-platform
doc_type: conceptualPageType
ms.openlocfilehash: 7c91aea96c93065a469b64bb3088540928e2e1d3
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36033076"
---
# <a name="azure-ad-audit-log-api-overview"></a><span data-ttu-id="1294d-103">Azure AD 監査ログ API の概要</span><span class="sxs-lookup"><span data-stu-id="1294d-103">Azure AD audit log API overview</span></span>

<span data-ttu-id="1294d-104">Azure Active Directory (Azure AD) は、ユーザーのアクティビティとサインインのメトリックを追跡し、ユーザーが Azure AD サービスにアクセスして使用する方法を把握するのに役立つ監査ログ レポートを作成します。</span><span class="sxs-lookup"><span data-stu-id="1294d-104">Azure Active Directory (Azure AD) tracks user activity and sign-in metrics and creates audit log reports that help you understand how your users access and use Azure AD services.</span></span> <span data-ttu-id="1294d-105">Azure AD 用の Microsoft Graph API を使用して、これらのレポートの基礎となるデータを分析したり、組織特有のニーズに合わせたカスタム ソリューションを作成したりします。</span><span class="sxs-lookup"><span data-stu-id="1294d-105">Use the Microsoft Graph API for Azure AD to analyze the data underlying these reports and to create custom solutions tailored to your organization's specific needs.</span></span>

## <a name="what-are-azure-ad-activity-logs"></a><span data-ttu-id="1294d-106">Azure AD アクティビティ ログとは</span><span class="sxs-lookup"><span data-stu-id="1294d-106">What are Azure AD activity logs?</span></span>

<span data-ttu-id="1294d-107">Azure AD には、以下の 2 種類のアクティビティ ログがあります。</span><span class="sxs-lookup"><span data-stu-id="1294d-107">Azure AD provides two types of activity logs:</span></span>

- <span data-ttu-id="1294d-108">監査ログ</span><span class="sxs-lookup"><span data-stu-id="1294d-108">audit logs</span></span>
- <span data-ttu-id="1294d-109">サインイン ログ</span><span class="sxs-lookup"><span data-stu-id="1294d-109">sign-in logs</span></span>

### <a name="audit-logs"></a><span data-ttu-id="1294d-110">監査ログ</span><span class="sxs-lookup"><span data-stu-id="1294d-110">Audit logs</span></span>

<span data-ttu-id="1294d-111">テナント内で実行されたすべてのタスクの履歴は、監査ログ アクティビティ レポートで把握できます。</span><span class="sxs-lookup"><span data-stu-id="1294d-111">The audit logs activity report provides you with access to the history of every task performed in your tenant.</span></span> <span data-ttu-id="1294d-112">監査ログ レポートから得られるシステム アクティビティの記録は、コンプライアンスに利用することができます。</span><span class="sxs-lookup"><span data-stu-id="1294d-112">The audit logs report provides you with records of system activities for compliance.</span></span> <span data-ttu-id="1294d-113">特に、レポートから得たデータによって、日常的に発生する次のようなシナリオに対処することができます。</span><span class="sxs-lookup"><span data-stu-id="1294d-113">Amongst others, the provided data enables you to address common scenarios such as:</span></span>

- <span data-ttu-id="1294d-114">ディレクトリのユーザーに管理者グループのアクセス権をだれが許可するか。</span><span class="sxs-lookup"><span data-stu-id="1294d-114">Who granted admin group access to a directory user?</span></span>
- <span data-ttu-id="1294d-115">最近入手したアプリにサインインしているユーザーはだれか。</span><span class="sxs-lookup"><span data-stu-id="1294d-115">Which users are signing in to a recently acquired app?</span></span>
- <span data-ttu-id="1294d-116">ディレクトリ内でパスワードのリセットが何回行われたか。</span><span class="sxs-lookup"><span data-stu-id="1294d-116">How many passwords resets were made within the directory?</span></span>

### <a name="sign-in-logs"></a><span data-ttu-id="1294d-117">サインイン ログ</span><span class="sxs-lookup"><span data-stu-id="1294d-117">Sign-in logs</span></span>

<span data-ttu-id="1294d-118">監査ログ レポートによって報告されたタスクをだれが実行したかを把握するには、サインイン アクティビティ レポートが役立ちます。</span><span class="sxs-lookup"><span data-stu-id="1294d-118">The sign-ins activity report helps you determine who performed the tasks reported by audit log reports.</span></span> <span data-ttu-id="1294d-119">サインイン アクティビティ レポートを利用すると、以下の事柄について把握できます。</span><span class="sxs-lookup"><span data-stu-id="1294d-119">The sign-ins activity report helps you answer questions like:</span></span>

- <span data-ttu-id="1294d-120">ユーザーのサインインにどのようなパターンがあるか。</span><span class="sxs-lookup"><span data-stu-id="1294d-120">What is the sign in pattern of a user?</span></span>
- <span data-ttu-id="1294d-121">先週、何人のユーザーがサインインを行ったか。</span><span class="sxs-lookup"><span data-stu-id="1294d-121">How many users have signed in during the last week?</span></span>
- <span data-ttu-id="1294d-122">これらのサインインはどのような状態か。</span><span class="sxs-lookup"><span data-stu-id="1294d-122">What's the status of these sign-ins?</span></span>

## <a name="what-can-i-do-with-audit-log-apis-in-microsoft-graph"></a><span data-ttu-id="1294d-123">Microsoft Graph の監査ログ API で実行できること</span><span class="sxs-lookup"><span data-stu-id="1294d-123">What can I do with audit log APIs in Microsoft Graph?</span></span>

<span data-ttu-id="1294d-124">監査ログ データで行う一般的な要求を以下に示します。</span><span class="sxs-lookup"><span data-stu-id="1294d-124">The following are popular requests for working with audit log data:</span></span>

<span data-ttu-id="1294d-125">Operation</span><span class="sxs-lookup"><span data-stu-id="1294d-125">Operation</span></span> | <span data-ttu-id="1294d-126">URL</span><span class="sxs-lookup"><span data-stu-id="1294d-126">URL</span></span>
:----------|:----
<span data-ttu-id="1294d-127">テナント ユーザー アクティビティを取得する</span><span class="sxs-lookup"><span data-stu-id="1294d-127">GET tenant user activities</span></span> | [<span data-ttu-id="1294d-128">GET https://graph.microsoft.com/v1.0/auditLogs/directoryAudits</span><span class="sxs-lookup"><span data-stu-id="1294d-128">GET https://graph.microsoft.com/v1.0/auditLogs/directoryAudits</span></span>](https://developer.microsoft.com/graph/graph-explorer?request=auditLogs/directoryAudits&version=v1.0)
<span data-ttu-id="1294d-129">テナント ユーザー サインインを取得する</span><span class="sxs-lookup"><span data-stu-id="1294d-129">GET tenant user sign-ins</span></span> | [<span data-ttu-id="1294d-130">GET https://graph.microsoft.com/v1.0/auditLogs/signIns</span><span class="sxs-lookup"><span data-stu-id="1294d-130">GET https://graph.microsoft.com/v1.0/auditLogs/signIns</span></span>](https://developer.microsoft.com/graph/graph-explorer?request=auditLogs/signIns&version=v1.0)

## <a name="what-licenses-do-i-need"></a><span data-ttu-id="1294d-131">必要なライセンス</span><span class="sxs-lookup"><span data-stu-id="1294d-131">What licenses do I need?</span></span>

<span data-ttu-id="1294d-132">監査ログ レポートは、ライセンスを取得した機能に関して利用できます。</span><span class="sxs-lookup"><span data-stu-id="1294d-132">Audit log reports are available for features that you've licensed.</span></span>  <span data-ttu-id="1294d-133">特定の機能のライセンスがある場合、その機能の監査ログにもアクセスできます。</span><span class="sxs-lookup"><span data-stu-id="1294d-133">If you have a license for a specific feature, you also have access to its audit logs.</span></span>

<span data-ttu-id="1294d-134">たとえば、セルフサービス パスワード監査レポートを利用するには、Azure AD Premium P1 ライセンスが必要です。</span><span class="sxs-lookup"><span data-stu-id="1294d-134">For example, you need an Azure AD Premium P1 license to access self-service password audit reports.</span></span>  <span data-ttu-id="1294d-135">詳細については、[Azure AD ライセンス](https://azure.microsoft.com/pricing/details/active-directory/)をご覧ください。</span><span class="sxs-lookup"><span data-stu-id="1294d-135">To learn more, see [Azure AD licensing](https://azure.microsoft.com/pricing/details/active-directory/).</span></span>

<span data-ttu-id="1294d-136">サインイン レポートには、Azure AD Premium ライセンスが必要です。</span><span class="sxs-lookup"><span data-stu-id="1294d-136">Sign-in reports require an Azure AD Premium license.</span></span>

<span data-ttu-id="1294d-137">詳細については、[Azure Active Directory の価格](https://azure.microsoft.com/pricing/details/active-directory/)をご覧ください。</span><span class="sxs-lookup"><span data-stu-id="1294d-137">To learn more, see [Azure AD pricing](https://azure.microsoft.com/pricing/details/active-directory/).</span></span>

## <a name="next-steps"></a><span data-ttu-id="1294d-138">次のステップ</span><span class="sxs-lookup"><span data-stu-id="1294d-138">Next Steps</span></span>

- <span data-ttu-id="1294d-139">[アプリを登録](https://docs.microsoft.com/azure/active-directory/active-directory-reporting-api-prerequisites-azure-portal)して、監査ログの前提条件を満たします。</span><span class="sxs-lookup"><span data-stu-id="1294d-139">[Register your app](https://docs.microsoft.com/azure/active-directory/active-directory-reporting-api-prerequisites-azure-portal) to satisfy audit log prerequisites.</span></span> 
- <span data-ttu-id="1294d-140">[監査ログ](https://docs.microsoft.com/azure/active-directory/active-directory-reporting-api-audit-samples)と[サインイン](https://docs.microsoft.com/azure/active-directory/active-directory-reporting-api-sign-in-activity-samples)のサンプルを参照して理解を深めます。</span><span class="sxs-lookup"><span data-stu-id="1294d-140">Learn from [audit log](https://docs.microsoft.com/azure/active-directory/active-directory-reporting-api-audit-samples) and [sign-in samples](https://docs.microsoft.com/azure/active-directory/active-directory-reporting-api-sign-in-activity-samples).</span></span>  
- <span data-ttu-id="1294d-141">[directoryAudit](directoryaudit.md) リソースとアクションについて確認します。</span><span class="sxs-lookup"><span data-stu-id="1294d-141">Review [directoryAudit](directoryaudit.md) resource and actions.</span></span>
- <span data-ttu-id="1294d-142">[signIn](signin.md) リソースとアクションについて確認します。</span><span class="sxs-lookup"><span data-stu-id="1294d-142">Review [signIn](signin.md) resource and actions.</span></span> 
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/azure-ad-auditlog-overview.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
