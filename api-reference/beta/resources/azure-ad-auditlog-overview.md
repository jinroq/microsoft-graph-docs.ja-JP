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
# <a name="azure-ad-audit-log-api-overview"></a><span data-ttu-id="cebdd-104">Azure AD 監査ログ API の概要</span><span class="sxs-lookup"><span data-stu-id="cebdd-104">Azure AD audit log API overview</span></span>

> <span data-ttu-id="cebdd-105">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="cebdd-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="cebdd-106">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="cebdd-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="cebdd-107">Azure Active Directory (AD の Azure) は、ユーザーの活動およびサインインのメトリックを追跡し、監査を作成、ユーザーのアクセスし、Azure AD サービスを活用するのに役立つログ レポートを理解します。</span><span class="sxs-lookup"><span data-stu-id="cebdd-107">Azure Active Directory (Azure AD) tracks user activity and sign-in metrics and creates audit log reports that help you understand how your users access and leverage Azure AD services.</span></span> <span data-ttu-id="cebdd-108">これらのレポートの基になるデータを分析して、組織の特定のニーズに合わせた独自のソリューションを作成するのには、Azure AD 用の Microsoft グラフ API を使用します。</span><span class="sxs-lookup"><span data-stu-id="cebdd-108">Use the Microsoft Graph API for Azure AD to analyze the data underlying these reports and to create custom solutions tailored to your organization's specific needs.</span></span>

## <a name="what-are-azure-ad-activity-logs"></a><span data-ttu-id="cebdd-109">Azure AD の活動は、何をログに記録しますか。</span><span class="sxs-lookup"><span data-stu-id="cebdd-109">What are Azure AD activity logs?</span></span>

<span data-ttu-id="cebdd-110">Azure AD には、動作状況のログの 2 種類が用意されています。</span><span class="sxs-lookup"><span data-stu-id="cebdd-110">Azure AD provides two types of activity logs:</span></span>

- <span data-ttu-id="cebdd-111">監査ログ</span><span class="sxs-lookup"><span data-stu-id="cebdd-111">audit logs</span></span> 
- <span data-ttu-id="cebdd-112">サインインのログ</span><span class="sxs-lookup"><span data-stu-id="cebdd-112">sign-in logs</span></span>

### <a name="audit-logs"></a><span data-ttu-id="cebdd-113">監査ログ</span><span class="sxs-lookup"><span data-stu-id="cebdd-113">Audit logs</span></span>

<span data-ttu-id="cebdd-114">監査ログの利用状況レポートは、テナントで実行されるすべてのタスクの履歴へのアクセスを提供します。</span><span class="sxs-lookup"><span data-stu-id="cebdd-114">The audit logs activity report provides you with access to the history of every task performed in your tenant.</span></span> <span data-ttu-id="cebdd-115">監査ログ レポートは、コンプライアンスのためのシステム ・ アクティビティの記録を提供します。</span><span class="sxs-lookup"><span data-stu-id="cebdd-115">The audit logs report provides you with records of system activities for compliance.</span></span> <span data-ttu-id="cebdd-116">、他のユーザーの間で提供されるデータには、一般的なシナリオを次のように対処することが有効にします。</span><span class="sxs-lookup"><span data-stu-id="cebdd-116">Amongst others, the provided data enables you to address common scenarios such as:</span></span>

- <span data-ttu-id="cebdd-117">ディレクトリ ユーザに管理者グループのアクセスを許可するか。</span><span class="sxs-lookup"><span data-stu-id="cebdd-117">Who granted admin group access to a directory user?</span></span>

- <span data-ttu-id="cebdd-118">ユーザーは、最近買収したアプリケーションへのをサインインがでしょうか。</span><span class="sxs-lookup"><span data-stu-id="cebdd-118">Which users are signing in to a recently acquired app?</span></span>

- <span data-ttu-id="cebdd-119">ディレクトリ内でどのように多くのパスワードのリセットが行われたでしょうか。</span><span class="sxs-lookup"><span data-stu-id="cebdd-119">How many passwords resets were made within the directory?</span></span>

### <a name="sign-in-logs"></a><span data-ttu-id="cebdd-120">ログを署名します。</span><span class="sxs-lookup"><span data-stu-id="cebdd-120">Sign in logs</span></span>

<span data-ttu-id="cebdd-121">サインインがアクティビティ ・ レポートでは、監査ログ レポートで報告されたタスクを実行したユーザーを確認できます。</span><span class="sxs-lookup"><span data-stu-id="cebdd-121">The sign-ins activity report helps you determine who performed the tasks reported by audit log reports.</span></span> <span data-ttu-id="cebdd-122">サインインがアクティビティ ・ レポートでは、質問に回答できます。</span><span class="sxs-lookup"><span data-stu-id="cebdd-122">The sign-ins activity report helps you answer questions like:</span></span>

- <span data-ttu-id="cebdd-123">パターン、ユーザーのサインインとは何ですか。</span><span class="sxs-lookup"><span data-stu-id="cebdd-123">What is the sign in pattern of a user?</span></span>
- <span data-ttu-id="cebdd-124">ユーザーの数は、最後の週でサインインがでしょうか。</span><span class="sxs-lookup"><span data-stu-id="cebdd-124">How many users have signed in during the last week?</span></span>
- <span data-ttu-id="cebdd-125">これらのサインインの状態とは何ですか。</span><span class="sxs-lookup"><span data-stu-id="cebdd-125">What's the status of these sign-ins?</span></span>

## <a name="what-can-i-do-with-audit-log-apis-in-microsoft-graph"></a><span data-ttu-id="cebdd-126">監査ログでは、Microsoft Graph Api では、どうすれば?</span><span class="sxs-lookup"><span data-stu-id="cebdd-126">What can I do with audit log APIs in Microsoft Graph?</span></span>

<span data-ttu-id="cebdd-127">監査ログのデータを操作するための一般的な要求を次に示します。</span><span class="sxs-lookup"><span data-stu-id="cebdd-127">Here are popular requests for working with audit log data:</span></span>

<span data-ttu-id="cebdd-128">操作</span><span class="sxs-lookup"><span data-stu-id="cebdd-128">Operation</span></span> | <span data-ttu-id="cebdd-129">URL</span><span class="sxs-lookup"><span data-stu-id="cebdd-129">URL</span></span>
:----------|:----
<span data-ttu-id="cebdd-130">テナント ユーザー ・ アクティビティを取得します。</span><span class="sxs-lookup"><span data-stu-id="cebdd-130">GET tenant user activities</span></span> | [https://graph.microsoft.com/beta/auditLogs/directoryAudits](https://developer.microsoft.com/graph/graph-explorer?request=auditLogs/directoryAudits&version=beta)
<span data-ttu-id="cebdd-131">テナント ユーザー サインインの問題を取得します。</span><span class="sxs-lookup"><span data-stu-id="cebdd-131">GET tenant user sign-ins</span></span> | [https://graph.microsoft.com/beta/auditLogs/signIns](https://developer.microsoft.com/graph/graph-explorer?request=auditLogs/signIns&version=beta)

## <a name="what-licenses-do-i-need"></a><span data-ttu-id="cebdd-132">どのようなライセンスが必要ですか。</span><span class="sxs-lookup"><span data-stu-id="cebdd-132">What licenses do I need?</span></span>

<span data-ttu-id="cebdd-133">監査ログ レポートは、ライセンスを取得している機能を使用できます。</span><span class="sxs-lookup"><span data-stu-id="cebdd-133">Audit log reports are available for features that you've licensed.</span></span>  <span data-ttu-id="cebdd-134">特定の機能のライセンスがあれば、その監査ログへのアクセスもあります。</span><span class="sxs-lookup"><span data-stu-id="cebdd-134">If you have a license for a specific feature, you also have access to its audit logs.</span></span>

<span data-ttu-id="cebdd-135">たとえば、パスワードのセルフ サービスの監査レポートにアクセスするのには Azure AD プレミアム P1 のライセンスが必要です。</span><span class="sxs-lookup"><span data-stu-id="cebdd-135">For example, you need an Azure AD Premium P1 license to access self-service password audit reports.</span></span>  <span data-ttu-id="cebdd-136">詳細については、 [Azure AD のライセンス](https://azure.microsoft.com/pricing/details/active-directory/)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="cebdd-136">To learn more, see [Azure AD licensing](https://azure.microsoft.com/pricing/details/active-directory/).</span></span>

<span data-ttu-id="cebdd-137">サインインのレポートでは、Azure AD のプレミアム ライセンスが必要です。</span><span class="sxs-lookup"><span data-stu-id="cebdd-137">Sign-in reports require an Azure AD Premium license.</span></span>

<span data-ttu-id="cebdd-138">詳細については、 [Azure AD の価格](https://azure.microsoft.com/pricing/details/active-directory/)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="cebdd-138">To learn more, see [Azure AD pricing](https://azure.microsoft.com/pricing/details/active-directory/).</span></span>

## <a name="next-steps"></a><span data-ttu-id="cebdd-139">次の手順</span><span class="sxs-lookup"><span data-stu-id="cebdd-139">Next Steps</span></span>

- <span data-ttu-id="cebdd-140">監査ログの必要条件を満たすためには、[アプリの登録](https://docs.microsoft.com/azure/active-directory/active-directory-reporting-api-prerequisites-azure-portal)をします。</span><span class="sxs-lookup"><span data-stu-id="cebdd-140">[Register your app](https://docs.microsoft.com/azure/active-directory/active-directory-reporting-api-prerequisites-azure-portal) to satisfy audit log prerequisites.</span></span> 
- <span data-ttu-id="cebdd-141">[ログを監査](https://docs.microsoft.com/azure/active-directory/active-directory-reporting-api-audit-samples)し、[サインイン用のサンプル](https://docs.microsoft.com/azure/active-directory/active-directory-reporting-api-sign-in-activity-samples)について説明します。</span><span class="sxs-lookup"><span data-stu-id="cebdd-141">Learn from [audit log](https://docs.microsoft.com/azure/active-directory/active-directory-reporting-api-audit-samples) and [sign-in samples](https://docs.microsoft.com/azure/active-directory/active-directory-reporting-api-sign-in-activity-samples).</span></span>  
- <span data-ttu-id="cebdd-142">[DirectoryAudit](directoryaudit.md)リソースと操作を確認します。</span><span class="sxs-lookup"><span data-stu-id="cebdd-142">Review [directoryAudit](directoryaudit.md) resource and actions.</span></span>
- <span data-ttu-id="cebdd-143">[サインイン](signin.md)リソースと操作を確認します。</span><span class="sxs-lookup"><span data-stu-id="cebdd-143">Review [signIn](signin.md) resource and actions.</span></span> 