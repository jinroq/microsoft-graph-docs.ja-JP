---
title: アプリケーションのアクセス許可を Exchange Online の特定のメールボックスにスコーピングする
description: アプリのアプリケーション アクセス許可を Exchange Online の特定のメールボックスにスコープ設定するには、アプリケーション アクセス ポリシーを作成する必要があります。
author: svpsiva
localization_priority: Priority
ms.prod: microsoft-identity-platform
ms.openlocfilehash: f9121ffad617d6901688718a8982b926959d8626
ms.sourcegitcommit: 56c0b609dfb1bc5d900956f407d107cdab7086e8
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/30/2019
ms.locfileid: "35932578"
---
# <a name="scoping-application-permissions-to-specific-exchange-online-mailboxes"></a><span data-ttu-id="7484e-103">アプリケーションのアクセス許可を Exchange Online の特定のメールボックスにスコーピングする</span><span class="sxs-lookup"><span data-stu-id="7484e-103">Scoping application permissions to specific Exchange Online mailboxes</span></span> 

<span data-ttu-id="7484e-104">一部のアプリは、ユーザーの代理としてではなく、独自の ID を使用して Microsoft Graph を呼び出します。</span><span class="sxs-lookup"><span data-stu-id="7484e-104">Some apps call Microsoft Graph with their own identity and not on behalf of a user.</span></span> <span data-ttu-id="7484e-105">通常、これに該当するものは、サーバーで実行される、サインインしているユーザーが存在しないバックグラウンド サービスやデーモン アプリです。</span><span class="sxs-lookup"><span data-stu-id="7484e-105">In many cases, these are background services or daemons that run on a server without the presence of a signed-in user.</span></span> <span data-ttu-id="7484e-106">こうしたアプリは、認証のために [OAuth 2.0 クライアント資格情報付与フロー](https://docs.microsoft.com/ja-JP/azure/active-directory/develop/v2-oauth2-client-creds-grant-flow)を使用し、アプリケーションのアクセス許可によって構成されています。これにより、そうしたアプリは Exchange Online の組織内のすべてのメールボックスにアクセスできるようになります。</span><span class="sxs-lookup"><span data-stu-id="7484e-106">These apps make use of [OAuth 2.0 client credentials grant flow](https://docs.microsoft.com/en-us/azure/active-directory/develop/v2-oauth2-client-creds-grant-flow) to authenticate and are configured with application permissions, which enable such apps to access all mailboxes in a organization on Exchange Online.</span></span> <span data-ttu-id="7484e-107">たとえば、アプリケーションのアクセス許可 Mail.Read により、サインインしているユーザーなしで、すべてのメールボックスのメールをアプリで読み取れるようになります。</span><span class="sxs-lookup"><span data-stu-id="7484e-107">For example, the Mail.Read application permission allows apps to read mail in all mailboxes without a signed-in user.</span></span> 

<span data-ttu-id="7484e-108">管理者は、アプリのアクセスを特定のメールボックスのセットに制限するために、PowerShell コマンドレット **New-ApplicationAccessPolicy** を使用してアクセス制御を構成できます。</span><span class="sxs-lookup"><span data-stu-id="7484e-108">Administrators who want to limit the app access to a specific set of mailboxes can use the **New-ApplicationAccessPolicy** PowerShell cmdlet to configure access control.</span></span> <span data-ttu-id="7484e-109">この記事では、アプリケーション アクセス ポリシーの基本的な構成手順について説明します。</span><span class="sxs-lookup"><span data-stu-id="7484e-109">This article covers the basic steps to configure an application access policy.</span></span>

<span data-ttu-id="7484e-110">この手順は Exchange Online のリソースに固有のものであり、その他の Microsoft Graph のワークロードには適用できません。</span><span class="sxs-lookup"><span data-stu-id="7484e-110">These steps are specific to Exchange Online resources and do not apply to other Microsoft Graph workloads.</span></span> 

## <a name="configure-applicationaccesspolicy"></a><span data-ttu-id="7484e-111">アプリケーション アクセス ポリシーの構成</span><span class="sxs-lookup"><span data-stu-id="7484e-111">Configure ApplicationAccessPolicy</span></span>

<span data-ttu-id="7484e-112">アプリケーション アクセス ポリシーを構成して、アプリケーションのアクセス許可のスコープを制限するには、次の操作を実行します。</span><span class="sxs-lookup"><span data-stu-id="7484e-112">To configure an application access policy and limit the scope of application permissions:</span></span>
1.  <span data-ttu-id="7484e-113">Exchange Online PowerShell に接続します。</span><span class="sxs-lookup"><span data-stu-id="7484e-113">Connect to Exchange Online PowerShell.</span></span> <span data-ttu-id="7484e-114">詳細については、「[Exchange Online PowerShell への接続](https://docs.microsoft.com/ja-JP/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="7484e-114">For details, see [Connect to Exchange Online Using Remote PowerShell](https://docs.microsoft.com/en-us/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps).</span></span>

2.  <span data-ttu-id="7484e-115">アプリのクライアント ID とメールが有効なセキュリティ グループを特定して、アプリのアクセス対象を制限します。</span><span class="sxs-lookup"><span data-stu-id="7484e-115">Identify the app’s client ID and a mail-enabled security group to restrict the app’s access to.</span></span>

    - <span data-ttu-id="7484e-116">[Azure のアプリの登録ポータル](https://portal.azure.com/#blade/Microsoft_AAD_RegisteredApps/ApplicationsListBlade)で、アプリのアプリケーション (クライアント) ID を特定します。</span><span class="sxs-lookup"><span data-stu-id="7484e-116">Identify the app’s application (client) ID in the [Azure app registration portal](https://portal.azure.com/#blade/Microsoft_AAD_RegisteredApps/ApplicationsListBlade).</span></span>
    - <span data-ttu-id="7484e-117">メールが有効な新しいセキュリティ グループを作成するか既存のグループを使用して、そのグループの電子メール アドレスを特定します。</span><span class="sxs-lookup"><span data-stu-id="7484e-117">Create a new mail-enabled security group or use an existing one and identify the email address for the group.</span></span> 

3.  <span data-ttu-id="7484e-118">アプリケーション アクセス ポリシーを作成します。</span><span class="sxs-lookup"><span data-stu-id="7484e-118">Create an application access policy.</span></span> 

    <span data-ttu-id="7484e-119">次のコマンドを実行します。ただし、引数の **AppId**、**PolicyScopeGroupId**、および **Description** は置き換えてください。</span><span class="sxs-lookup"><span data-stu-id="7484e-119">Run the following command, replacing the **AppId**, **PolicyScopeGroupId**, and **Description** arguments.</span></span>
    ```sh 
    New-ApplicationAccessPolicy -AppId e7e4dbfc-046f-4074-9b3b-2ae8f144f59b -PolicyScopeGroupId EvenUsers@contoso.com -AccessRight RestrictAccess -Description "Restrict this app to members of distribution group EvenUsers."
    ```
4.  <span data-ttu-id="7484e-120">新しく作成したアプリケーション アクセス ポリシーをテストします。</span><span class="sxs-lookup"><span data-stu-id="7484e-120">Test the newly created application access policy.</span></span>

    <span data-ttu-id="7484e-121">次のコマンドを実行します。ただし、引数の **AppId** および **Identity** は置き換えてください。</span><span class="sxs-lookup"><span data-stu-id="7484e-121">Run the following command, replacing the **AppId** and **Identity** arguments.</span></span>
    ```sh
    Test-ApplicationAccessPolicy -Identity user1@contoso.com -AppId e7e4dbfc-046-4074-9b3b-2ae8f144f59b 
    ```
    <span data-ttu-id="7484e-122">このコマンドの出力には、アプリが User1 のメールボックスにアクセスできるかどうかが示されます。</span><span class="sxs-lookup"><span data-stu-id="7484e-122">The output of this command will indicate whether the app has access to User1’s mailbox.</span></span>

<span data-ttu-id="7484e-123">注: アプリケーション アクセス ポリシーの変更が Microsoft Graph REST API の呼び出しに反映されるまでに、最長で 30 分かかることがあります。</span><span class="sxs-lookup"><span data-stu-id="7484e-123">Note: Changes to application access policies can take up to 30 minutes to take effect in Microsoft Graph REST API calls.</span></span>

## <a name="supported-permissions-and-additional-resources"></a><span data-ttu-id="7484e-124">サポートされるアクセス許可と追加のリソース</span><span class="sxs-lookup"><span data-stu-id="7484e-124">Supported app scenarios and additional resources</span></span>
<span data-ttu-id="7484e-125">管理者は、ApplicationAccessPolicy コマンドレットを使用して、次のいずれかのアプリケーションのアクセス許可が付与されているアプリのメールボックス アクセスを制御できます。</span><span class="sxs-lookup"><span data-stu-id="7484e-125">Administrators can use ApplicationAccessPolicy cmdlets to control mailbox access of an app that has been granted any of the following application permissions:</span></span> 
- <span data-ttu-id="7484e-126">Mail.Read</span><span class="sxs-lookup"><span data-stu-id="7484e-126">Mail.Read</span></span>
- <span data-ttu-id="7484e-127">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="7484e-127">Mail.ReadWrite</span></span>
- <span data-ttu-id="7484e-128">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="7484e-128">Mail.Send</span></span>
- <span data-ttu-id="7484e-129">MailboxSettings.Read</span><span class="sxs-lookup"><span data-stu-id="7484e-129">MailboxSettings.Read</span></span>  
- <span data-ttu-id="7484e-130">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="7484e-130">MailboxSettings.ReadWrite</span></span>
- <span data-ttu-id="7484e-131">Calendars.Read</span><span class="sxs-lookup"><span data-stu-id="7484e-131">Calendars.Read</span></span>
- <span data-ttu-id="7484e-132">Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="7484e-132">Calendars.ReadWrite</span></span>
- <span data-ttu-id="7484e-133">Contacts.Read</span><span class="sxs-lookup"><span data-stu-id="7484e-133">Contacts.Read</span></span>
- <span data-ttu-id="7484e-134">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="7484e-134">Contacts.ReadWrite</span></span>

<span data-ttu-id="7484e-135">アプリケーション アクセス ポリシーの構成の詳細については、[PowerShell コマンドレット リファレンスの New-ApplicationAccessPolicy](https://docs.microsoft.com/powershell/module/exchange/organization/new-applicationaccesspolicy)の項目を参照してください。</span><span class="sxs-lookup"><span data-stu-id="7484e-135">For more information about configuring application access policy, see the [PowerShell cmdlet reference for New-ApplicationAccessPolicy](https://docs.microsoft.com/powershell/module/exchange/organization/new-applicationaccesspolicy).</span></span> 

## <a name="handling-api-errors"></a><span data-ttu-id="7484e-136">API エラーの処理</span><span class="sxs-lookup"><span data-stu-id="7484e-136">Handling API errors</span></span>
<span data-ttu-id="7484e-137">構成済みのアプリケーション アクセス ポリシーによって API 呼び出しのアクセスが拒否されると、次のエラーが発生することがあります。</span><span class="sxs-lookup"><span data-stu-id="7484e-137">You might encounter the following error when an API call is denied access due to a configured application access policy.</span></span> 
```json
{
    "error": {
        "code": "ErrorAccessDenied",
        "message": "Access to OData is disabled.",
        "innerError": {
            "request-id": "2f038156-cf40-403d-8e46-831fe42a8229",
            "date": "2019-05-24T10:16:21"
        }
    }
}
```
<span data-ttu-id="7484e-138">このエラーがアプリからの Microsoft Graph API 呼び出しで返された場合は、組織の Exchange Online 管理者と協力して、メールボックス リソースにアクセスするためのアクセス許可をアプリに付与してください。</span><span class="sxs-lookup"><span data-stu-id="7484e-138">If Microsoft Graph API calls from your app return this error, work with the Exchange Online administrator for the organization to ensure that your app has permission to access the mailbox resource.</span></span>



## <a name="see-also"></a><span data-ttu-id="7484e-139">関連項目</span><span class="sxs-lookup"><span data-stu-id="7484e-139">See also</span></span>

- [<span data-ttu-id="7484e-140">アクセス許可リファレンス</span><span class="sxs-lookup"><span data-stu-id="7484e-140">Permissions reference</span></span>](permissions-reference.md)
- [<span data-ttu-id="7484e-141">New-ApplicationAccessPolicy</span><span class="sxs-lookup"><span data-stu-id="7484e-141">New-ApplicationAccessPolicy</span></span>](https://docs.microsoft.com/powershell/module/exchange/organization/new-applicationaccesspolicy)
- [<span data-ttu-id="7484e-142">Get-ApplicationAccessPolicy</span><span class="sxs-lookup"><span data-stu-id="7484e-142">Get-ApplicationAccessPolicy</span></span>](https://docs.microsoft.com/powershell/module/exchange/organization/get-applicationaccesspolicy)
- [<span data-ttu-id="7484e-143">Remove-ApplicationAccessPolicy</span><span class="sxs-lookup"><span data-stu-id="7484e-143">Remove-ApplicationAccessPolicy</span></span>](https://docs.microsoft.com/powershell/module/exchange/organization/remove-applicationaccesspolicy)
- [<span data-ttu-id="7484e-144">Set-ApplicationAccessPolicy</span><span class="sxs-lookup"><span data-stu-id="7484e-144">Set-ApplicationAccessPolicy</span></span>](https://docs.microsoft.com/powershell/module/exchange/organization/set-applicationaccesspolicy)
- [<span data-ttu-id="7484e-145">Test-ApplicationAccessPolicy</span><span class="sxs-lookup"><span data-stu-id="7484e-145">Test-ApplicationAccessPolicy</span></span>](https://docs.microsoft.com/powershell/module/exchange/organization/test-applicationaccesspolicy)
