---
title: Azure AD 監査ログ API の概要
description: Azure Active Directory (Azure AD) は、ユーザーのアクティビティとサインインのメトリックを追跡し、ユーザーが Azure AD サービスにアクセスして活用する方法を把握するのに役立つ監査ログ レポートを作成します。 Azure AD 用の Microsoft Graph API を使用して、これらのレポートの基礎となるデータを分析したり、組織特有のニーズに合わせたカスタム ソリューションを作成したりします。
localization_priority: Priority
ms.openlocfilehash: 8bda9aff36ad8b46fbec3096008c2d5227058ef1
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33339075"
---
# <a name="azure-ad-audit-log-api-overview"></a><span data-ttu-id="d74b7-104">Azure AD 監査ログ API の概要</span><span class="sxs-lookup"><span data-stu-id="d74b7-104">Azure AD audit log API overview</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d74b7-105">Azure Active Directory (Azure AD) は、ユーザーのアクティビティとサインインのメトリックを追跡し、ユーザーが Azure AD サービスにアクセスして活用する方法を把握するのに役立つ監査ログ レポートを作成します。</span><span class="sxs-lookup"><span data-stu-id="d74b7-105">Azure Active Directory (Azure AD) tracks user activity and sign-in metrics and creates audit log reports that help you understand how your users access and leverage Azure AD services.</span></span> <span data-ttu-id="d74b7-106">Azure AD 用の Microsoft Graph API を使用して、これらのレポートの基礎となるデータを分析したり、組織特有のニーズに合わせたカスタム ソリューションを作成したりします。</span><span class="sxs-lookup"><span data-stu-id="d74b7-106">Use the Microsoft Graph API for Azure AD to analyze the data underlying these reports and to create custom solutions tailored to your organization's specific needs.</span></span>

## <a name="what-are-azure-ad-activity-logs"></a><span data-ttu-id="d74b7-107">Azure AD アクティビティ ログとは</span><span class="sxs-lookup"><span data-stu-id="d74b7-107">What are Azure AD activity logs?</span></span>

<span data-ttu-id="d74b7-108">Azure AD には、以下の 2 種類のアクティビティ ログがあります。</span><span class="sxs-lookup"><span data-stu-id="d74b7-108">Azure AD provides two types of activity logs:</span></span>

- <span data-ttu-id="d74b7-109">監査ログ</span><span class="sxs-lookup"><span data-stu-id="d74b7-109">Audit logs</span></span> 
- <span data-ttu-id="d74b7-110">サインイン ログ</span><span class="sxs-lookup"><span data-stu-id="d74b7-110">sign-in logs</span></span>

### <a name="audit-logs"></a><span data-ttu-id="d74b7-111">監査ログ</span><span class="sxs-lookup"><span data-stu-id="d74b7-111">Audit logs</span></span>

<span data-ttu-id="d74b7-112">テナント内で実行されたすべてのタスクの履歴は、監査ログ アクティビティ レポートで把握できます。</span><span class="sxs-lookup"><span data-stu-id="d74b7-112">The audit logs activity report provides you with access to the history of every task performed in your tenant.</span></span> <span data-ttu-id="d74b7-113">監査ログ レポートから得られるシステム アクティビティの記録は、コンプライアンスに利用することができます。</span><span class="sxs-lookup"><span data-stu-id="d74b7-113">The audit logs report provides you with records of system activities for compliance.</span></span> <span data-ttu-id="d74b7-114">特に、レポートから得たデータによって、日常的に発生する次のようなシナリオに対処することができます。</span><span class="sxs-lookup"><span data-stu-id="d74b7-114">Amongst others, the provided data enables you to address common scenarios such as:</span></span>

- <span data-ttu-id="d74b7-115">ディレクトリのユーザーに管理者グループのアクセス権をだれが許可するか。</span><span class="sxs-lookup"><span data-stu-id="d74b7-115">Who granted admin group access to a directory user?</span></span>

- <span data-ttu-id="d74b7-116">最近入手したアプリにサインインしているユーザーはだれか。</span><span class="sxs-lookup"><span data-stu-id="d74b7-116">Which users are signing in to a recently acquired app?</span></span>

- <span data-ttu-id="d74b7-117">ディレクトリ内でパスワードのリセットが何回行われたか。</span><span class="sxs-lookup"><span data-stu-id="d74b7-117">How many passwords resets were made within the directory?</span></span>

### <a name="sign-in-logs"></a><span data-ttu-id="d74b7-118">サインイン ログ</span><span class="sxs-lookup"><span data-stu-id="d74b7-118">Sign in logs</span></span>

<span data-ttu-id="d74b7-119">監査ログ レポートによって報告されたタスクをだれが実行したかを把握するには、サインイン アクティビティ レポートが役立ちます。</span><span class="sxs-lookup"><span data-stu-id="d74b7-119">The sign-ins activity report helps you determine who performed the tasks reported by audit log reports.</span></span> <span data-ttu-id="d74b7-120">サインイン アクティビティ レポートを利用すると、以下の事柄について把握できます。</span><span class="sxs-lookup"><span data-stu-id="d74b7-120">The sign-ins activity report helps you answer questions like:</span></span>

- <span data-ttu-id="d74b7-121">ユーザーのサインインにどのようなパターンがあるか。</span><span class="sxs-lookup"><span data-stu-id="d74b7-121">What is the sign in pattern of a user?</span></span>
- <span data-ttu-id="d74b7-122">先週、何人のユーザーがサインインを行ったか。</span><span class="sxs-lookup"><span data-stu-id="d74b7-122">How many users have signed in during the last week?</span></span>
- <span data-ttu-id="d74b7-123">これらのサインインはどのような状態か。</span><span class="sxs-lookup"><span data-stu-id="d74b7-123">What's the status of these sign-ins?</span></span>

## <a name="what-can-i-do-with-audit-log-apis-in-microsoft-graph"></a><span data-ttu-id="d74b7-124">Microsoft Graph の監査ログ API で実行できること</span><span class="sxs-lookup"><span data-stu-id="d74b7-124">What can I do with OneNote APIs in Microsoft Graph?</span></span>

<span data-ttu-id="d74b7-125">監査ログ データで行う一般的な要求を以下に示します。</span><span class="sxs-lookup"><span data-stu-id="d74b7-125">Here are popular requests for working with audit log data:</span></span>

<span data-ttu-id="d74b7-126">Operation</span><span class="sxs-lookup"><span data-stu-id="d74b7-126">Operation</span></span> | <span data-ttu-id="d74b7-127">URL</span><span class="sxs-lookup"><span data-stu-id="d74b7-127">URL</span></span>
:----------|:----
<span data-ttu-id="d74b7-128">テナント ユーザー アクティビティを取得する</span><span class="sxs-lookup"><span data-stu-id="d74b7-128">GET tenant user activities</span></span> | [https://graph.microsoft.com/beta/auditLogs/directoryAudits](https://developer.microsoft.com/graph/graph-explorer?request=auditLogs/directoryAudits&version=beta)
<span data-ttu-id="d74b7-129">テナント ユーザー サインインを取得する</span><span class="sxs-lookup"><span data-stu-id="d74b7-129">GET tenant user sign-ins</span></span> | [https://graph.microsoft.com/beta/auditLogs/signIns](https://developer.microsoft.com/graph/graph-explorer?request=auditLogs/signIns&version=beta)

## <a name="what-licenses-do-i-need"></a><span data-ttu-id="d74b7-130">必要なライセンス</span><span class="sxs-lookup"><span data-stu-id="d74b7-130">What do I need?</span></span>

<span data-ttu-id="d74b7-131">監査ログ レポートは、ライセンスを取得した機能に関して利用できます。</span><span class="sxs-lookup"><span data-stu-id="d74b7-131">Audit log reports are available for features that you've licensed.</span></span>  <span data-ttu-id="d74b7-132">特定の機能のライセンスがある場合、その機能の監査ログにもアクセスできます。</span><span class="sxs-lookup"><span data-stu-id="d74b7-132">If you have a license for a specific feature, you also have access to its audit logs.</span></span>

<span data-ttu-id="d74b7-133">たとえば、セルフサービス パスワード監査レポートを利用するには、Azure AD Premium P1 ライセンスが必要です。</span><span class="sxs-lookup"><span data-stu-id="d74b7-133">For example, you need an Azure AD Premium P1 license to access self-service password audit reports.</span></span>  <span data-ttu-id="d74b7-134">詳細については、[Azure AD ライセンス](https://azure.microsoft.com/pricing/details/active-directory/)をご覧ください。</span><span class="sxs-lookup"><span data-stu-id="d74b7-134">To learn more, see [Azure AD licensing](https://azure.microsoft.com/pricing/details/active-directory/).</span></span>

<span data-ttu-id="d74b7-135">サインイン レポートには、Azure AD Premium ライセンスが必要です。</span><span class="sxs-lookup"><span data-stu-id="d74b7-135">Sign-in reports require an Azure AD Premium license.</span></span>

<span data-ttu-id="d74b7-136">詳細については、[Azure Active Directory の価格](https://azure.microsoft.com/pricing/details/active-directory/)をご覧ください。</span><span class="sxs-lookup"><span data-stu-id="d74b7-136">To learn more, see [Azure AD pricing](https://azure.microsoft.com/pricing/details/active-directory/).</span></span>

## <a name="next-steps"></a><span data-ttu-id="d74b7-137">次のステップ</span><span class="sxs-lookup"><span data-stu-id="d74b7-137">Next Steps</span></span>

- <span data-ttu-id="d74b7-138">[アプリを登録](https://docs.microsoft.com/azure/active-directory/active-directory-reporting-api-prerequisites-azure-portal)して、監査ログの前提条件を満たします。</span><span class="sxs-lookup"><span data-stu-id="d74b7-138">[Register your app](https://docs.microsoft.com/azure/active-directory/active-directory-reporting-api-prerequisites-azure-portal) to satisfy audit log prerequisites.</span></span> 
- <span data-ttu-id="d74b7-139">[監査ログ](https://docs.microsoft.com/azure/active-directory/active-directory-reporting-api-audit-samples)と[サインイン](https://docs.microsoft.com/azure/active-directory/active-directory-reporting-api-sign-in-activity-samples)のサンプルを参照して理解を深めます。</span><span class="sxs-lookup"><span data-stu-id="d74b7-139">Learn from [audit log](https://docs.microsoft.com/azure/active-directory/active-directory-reporting-api-audit-samples) and [sign-in samples](https://docs.microsoft.com/azure/active-directory/active-directory-reporting-api-sign-in-activity-samples).</span></span>  
- <span data-ttu-id="d74b7-140">[directoryAudit](directoryaudit.md) リソースとアクションについて確認します。</span><span class="sxs-lookup"><span data-stu-id="d74b7-140">Review [directoryAudit](directoryaudit.md) resource and actions.</span></span>
- <span data-ttu-id="d74b7-141">[signIn](signin.md) リソースとアクションについて確認します。</span><span class="sxs-lookup"><span data-stu-id="d74b7-141">Review [signIn](signin.md) resource and actions.</span></span> 
