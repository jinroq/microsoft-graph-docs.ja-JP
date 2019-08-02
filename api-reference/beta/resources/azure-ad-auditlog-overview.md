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
# <a name="azure-ad-audit-log-api-overview"></a><span data-ttu-id="66c10-104">Azure AD 監査ログ API の概要</span><span class="sxs-lookup"><span data-stu-id="66c10-104">Azure AD audit log API overview</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="66c10-105">Azure Active Directory (Azure AD) は、ユーザーのアクティビティとサインインのメトリックを追跡し、ユーザーが Azure AD サービスにアクセスして使用する方法を把握するのに役立つ監査ログ レポートを作成します。</span><span class="sxs-lookup"><span data-stu-id="66c10-105">Azure Active Directory (Azure AD) tracks user activity and sign-in metrics and creates audit log reports that help you understand how your users access and use Azure AD services.</span></span> <span data-ttu-id="66c10-106">Azure AD 用の Microsoft Graph API を使用して、これらのレポートの基礎となるデータを分析したり、組織特有のニーズに合わせたカスタム ソリューションを作成したりします。</span><span class="sxs-lookup"><span data-stu-id="66c10-106">Use the Microsoft Graph API for Azure AD to analyze the data underlying these reports and to create custom solutions tailored to your organization's specific needs.</span></span>

## <a name="what-are-azure-ad-activity-logs"></a><span data-ttu-id="66c10-107">Azure AD アクティビティ ログとは</span><span class="sxs-lookup"><span data-stu-id="66c10-107">What are Azure AD activity logs?</span></span>

<span data-ttu-id="66c10-108">Azure AD には、3 種類のアクティビティ ログが用意されています。</span><span class="sxs-lookup"><span data-stu-id="66c10-108">Azure AD provides two types of activity logs:</span></span>

- <span data-ttu-id="66c10-109">監査ログ</span><span class="sxs-lookup"><span data-stu-id="66c10-109">Audit logs</span></span> 
- <span data-ttu-id="66c10-110">サインイン ログ</span><span class="sxs-lookup"><span data-stu-id="66c10-110">Sign-in logs</span></span>
- <span data-ttu-id="66c10-111">プロビジョニング ログ</span><span class="sxs-lookup"><span data-stu-id="66c10-111">Provisioning logs</span></span>

### <a name="audit-logs"></a><span data-ttu-id="66c10-112">監査ログ</span><span class="sxs-lookup"><span data-stu-id="66c10-112">Audit logs</span></span>

<span data-ttu-id="66c10-113">テナント内で実行されたすべてのタスクの履歴は、監査ログ アクティビティ レポートで把握できます。</span><span class="sxs-lookup"><span data-stu-id="66c10-113">The audit logs activity report provides you with access to the history of every task performed in your tenant.</span></span> <span data-ttu-id="66c10-114">監査ログ レポートから得られるシステム アクティビティの記録は、コンプライアンスに利用することができます。</span><span class="sxs-lookup"><span data-stu-id="66c10-114">The audit logs report provides you with records of system activities for compliance.</span></span> <span data-ttu-id="66c10-115">特に、レポートから得たデータによって、日常的に発生する次のようなシナリオに対処することができます。</span><span class="sxs-lookup"><span data-stu-id="66c10-115">Amongst others, the provided data enables you to address common scenarios such as:</span></span>

- <span data-ttu-id="66c10-116">ディレクトリのユーザーに管理者グループのアクセス権をだれが許可するか。</span><span class="sxs-lookup"><span data-stu-id="66c10-116">Who granted admin group access to a directory user?</span></span>

- <span data-ttu-id="66c10-117">最近入手したアプリにサインインしているユーザーはだれか。</span><span class="sxs-lookup"><span data-stu-id="66c10-117">Which users are signing in to a recently acquired app?</span></span>

- <span data-ttu-id="66c10-118">ディレクトリ内でパスワードのリセットが何回行われたか。</span><span class="sxs-lookup"><span data-stu-id="66c10-118">How many passwords resets were made within the directory?</span></span>

### <a name="sign-in-logs"></a><span data-ttu-id="66c10-119">サインイン ログ</span><span class="sxs-lookup"><span data-stu-id="66c10-119">Sign-in logs</span></span>

<span data-ttu-id="66c10-120">監査ログ レポートによって報告されたタスクをだれが実行したかを把握するには、サインイン アクティビティ レポートが役立ちます。</span><span class="sxs-lookup"><span data-stu-id="66c10-120">The sign-ins activity report helps you determine who performed the tasks reported by audit log reports.</span></span> <span data-ttu-id="66c10-121">サインイン アクティビティ レポートを利用すると、以下の事柄について把握できます。</span><span class="sxs-lookup"><span data-stu-id="66c10-121">The sign-ins activity report helps you answer questions like:</span></span>

- <span data-ttu-id="66c10-122">ユーザーのサインインにどのようなパターンがあるか。</span><span class="sxs-lookup"><span data-stu-id="66c10-122">What is the sign in pattern of a user?</span></span>
- <span data-ttu-id="66c10-123">先週、何人のユーザーがサインインを行ったか。</span><span class="sxs-lookup"><span data-stu-id="66c10-123">How many users have signed in during the last week?</span></span>
- <span data-ttu-id="66c10-124">これらのサインインはどのような状態か。</span><span class="sxs-lookup"><span data-stu-id="66c10-124">What's the status of these sign-ins?</span></span>

### <a name="provisioning-logs"></a><span data-ttu-id="66c10-125">プロビジョニング ログ</span><span class="sxs-lookup"><span data-stu-id="66c10-125">Provisioning logs</span></span>
<span data-ttu-id="66c10-126">プロビジョニング ログを使用すると、Azure AD のプロビジョニング サービスによって実行されるすべてのアクションを表示できます。</span><span class="sxs-lookup"><span data-stu-id="66c10-126">The provisioning logs help you see all the actions performed by the Azure AD provisioning service.</span></span> <span data-ttu-id="66c10-127">プロビジョニング ログを使うと、次のような質問に答えることができます。</span><span class="sxs-lookup"><span data-stu-id="66c10-127">The provisioning logs help you answer questions like:</span></span>

- <span data-ttu-id="66c10-128">どのグループが ServiceNow で正常に作成されたか</span><span class="sxs-lookup"><span data-stu-id="66c10-128">What groups were successfully created in ServiceNow?</span></span>
- <span data-ttu-id="66c10-129">どのロールがアマゾン ウェブ サービスからインポートされたか</span><span class="sxs-lookup"><span data-stu-id="66c10-129">What roles were imported from Amazon Web Services?</span></span>
- <span data-ttu-id="66c10-130">どのユーザーが Workday で正常に作成されなかったか</span><span class="sxs-lookup"><span data-stu-id="66c10-130">What users were unsuccessfully created from Workday?</span></span>

## <a name="what-can-i-do-with-audit-log-apis-in-microsoft-graph"></a><span data-ttu-id="66c10-131">Microsoft Graph の監査ログ API で実行できること</span><span class="sxs-lookup"><span data-stu-id="66c10-131">What can I do with audit log APIs in Microsoft Graph?</span></span>

<span data-ttu-id="66c10-132">監査ログ データで行う一般的な要求を以下に示します。</span><span class="sxs-lookup"><span data-stu-id="66c10-132">Here are popular requests for working with audit log data:</span></span>

<span data-ttu-id="66c10-133">Operation</span><span class="sxs-lookup"><span data-stu-id="66c10-133">Operation</span></span> | <span data-ttu-id="66c10-134">URL</span><span class="sxs-lookup"><span data-stu-id="66c10-134">URL</span></span>
:----------|:----
<span data-ttu-id="66c10-135">テナント ユーザー アクティビティを取得する</span><span class="sxs-lookup"><span data-stu-id="66c10-135">GET tenant user activities</span></span> | [https://graph.microsoft.com/beta/auditLogs/directoryAudits](https://developer.microsoft.com/graph/graph-explorer?request=auditLogs/directoryAudits&version=beta)
<span data-ttu-id="66c10-136">テナント ユーザー サインインを取得する</span><span class="sxs-lookup"><span data-stu-id="66c10-136">GET tenant user sign-ins</span></span> | [https://graph.microsoft.com/beta/auditLogs/signIns](https://developer.microsoft.com/graph/graph-explorer?request=auditLogs/signIns&version=beta)
<span data-ttu-id="66c10-137">プロビジョニング ログを取得する</span><span class="sxs-lookup"><span data-stu-id="66c10-137">GET provisioning logs</span></span> | [https://graph.microsoft.com/beta/auditLogs/directoryProvisioning](https://developer.microsoft.com/graph/graph-explorer?request=auditLogs/directoryProvisioning&version=beta)

## <a name="what-licenses-do-i-need"></a><span data-ttu-id="66c10-138">必要なライセンス</span><span class="sxs-lookup"><span data-stu-id="66c10-138">What licenses do I need?</span></span>

<span data-ttu-id="66c10-139">監査ログ レポートは、ライセンスを取得した機能に関して利用できます。</span><span class="sxs-lookup"><span data-stu-id="66c10-139">Audit log reports are available for features that you've licensed.</span></span>  <span data-ttu-id="66c10-140">特定の機能のライセンスがある場合、その機能の監査ログにもアクセスできます。</span><span class="sxs-lookup"><span data-stu-id="66c10-140">If you have a license for a specific feature, you also have access to its audit logs.</span></span>

<span data-ttu-id="66c10-141">たとえば、セルフサービス パスワード監査レポートを利用するには、Azure AD Premium P1 ライセンスが必要です。</span><span class="sxs-lookup"><span data-stu-id="66c10-141">For example, you need an Azure AD Premium P1 license to access self-service password audit reports.</span></span>  <span data-ttu-id="66c10-142">詳細については、[Azure AD ライセンス](https://azure.microsoft.com/pricing/details/active-directory/)をご覧ください。</span><span class="sxs-lookup"><span data-stu-id="66c10-142">To learn more, see [Azure AD licensing](https://azure.microsoft.com/pricing/details/active-directory/).</span></span>

<span data-ttu-id="66c10-143">サインイン レポートには、Azure AD Premium ライセンスが必要です。</span><span class="sxs-lookup"><span data-stu-id="66c10-143">Sign-in reports require an Azure AD Premium license.</span></span>

<span data-ttu-id="66c10-144">詳細については、[Azure Active Directory の価格](https://azure.microsoft.com/pricing/details/active-directory/)をご覧ください。</span><span class="sxs-lookup"><span data-stu-id="66c10-144">To learn more, see [Azure AD pricing](https://azure.microsoft.com/pricing/details/active-directory/).</span></span>

## <a name="next-steps"></a><span data-ttu-id="66c10-145">次の手順</span><span class="sxs-lookup"><span data-stu-id="66c10-145">Next steps</span></span>

- <span data-ttu-id="66c10-146">[アプリを登録](https://docs.microsoft.com/azure/active-directory/active-directory-reporting-api-prerequisites-azure-portal)して、監査ログの前提条件を満たします。</span><span class="sxs-lookup"><span data-stu-id="66c10-146">[Register your app](https://docs.microsoft.com/azure/active-directory/active-directory-reporting-api-prerequisites-azure-portal) to satisfy audit log prerequisites.</span></span> 
- <span data-ttu-id="66c10-147">[監査ログ](https://docs.microsoft.com/azure/active-directory/active-directory-reporting-api-audit-samples)と[サインイン](https://docs.microsoft.com/azure/active-directory/active-directory-reporting-api-sign-in-activity-samples)のサンプルを参照して理解を深めます。</span><span class="sxs-lookup"><span data-stu-id="66c10-147">Learn from [audit log](https://docs.microsoft.com/azure/active-directory/active-directory-reporting-api-audit-samples) and [sign-in samples](https://docs.microsoft.com/azure/active-directory/active-directory-reporting-api-sign-in-activity-samples).</span></span>  
- <span data-ttu-id="66c10-148">[ディレクトリ監査](directoryaudit.md) リソースとアクションを確認します。</span><span class="sxs-lookup"><span data-stu-id="66c10-148">Review [directoryAudit](directoryaudit.md) resource and actions.</span></span>
- <span data-ttu-id="66c10-149">[サインイン](signin.md) リソースとアクションを確認します。</span><span class="sxs-lookup"><span data-stu-id="66c10-149">Review [signIn](signin.md) resource and actions.</span></span> 
- <span data-ttu-id="66c10-150">[プロビジョニング オブジェクト サマリー](provisioningobjectsummary.md)リソースを確認します。</span><span class="sxs-lookup"><span data-stu-id="66c10-150">Review the [provisioningObjectSummary](provisioningobjectsummary.md) resource.</span></span>
