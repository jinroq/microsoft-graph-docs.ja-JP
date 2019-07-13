---
title: Microsoft Graph データ接続と Privileged Access Management の統合
description: Microsoft Graph データ接続は、Office 365 管理者がデータ移動の要求を承認できるようにするために、Privileged Access Management に依存しています。
author: tlenig
localization_priority: Priority
ms.prod: data-connect
ms.openlocfilehash: 439a5e50779888ff1ae7ccfb11311d8b3f6b8a14
ms.sourcegitcommit: ca55fc5f5711966eaa41da31cd1ae99820e9e586
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/13/2019
ms.locfileid: "35645269"
---
# <a name="microsoft-graph-data-connect-integration-with-privileged-access-management"></a><span data-ttu-id="ae6f2-103">Microsoft Graph データ接続と Privileged Access Management の統合</span><span class="sxs-lookup"><span data-stu-id="ae6f2-103">Microsoft Graph data connect integration with Privileged Access Management</span></span>

<span data-ttu-id="ae6f2-104">Microsoft Graph データ接続は、Office 365 管理者がデータ移動の要求を承認できるようにするために、Privileged Access Management (PAM) に依存しています。</span><span class="sxs-lookup"><span data-stu-id="ae6f2-104">Microsoft Graph data connect relies on Privileged Access Management (PAM) to allow Office 365 administrators to approve data movement requests.</span></span> <span data-ttu-id="ae6f2-105">データ接続のパイプラインは有効化中に、Office 365 管理者から指定されたデータ アクセス要求の承認者のメンバーによって承認される必要があります。</span><span class="sxs-lookup"><span data-stu-id="ae6f2-105">Data connect pipelines must be approved by a member of the data access request approver specified by the Office 365 administrator during enablement.</span></span> <span data-ttu-id="ae6f2-106">承認者グループを設定するには、「[はじめに](data-connect-get-started.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="ae6f2-106">To set up the approver group, see [Get started](data-connect-get-started.md).</span></span>

<span data-ttu-id="ae6f2-107">コピー アクティビティが Office 365 データを抽出するためのアクセスを要求したときに、承認要求メールが承認者グループの各メンバーに送信されます。</span><span class="sxs-lookup"><span data-stu-id="ae6f2-107">Approval request emails will be sent to each member of the approver group to notify them when copy activities request access to extract Office 365 data.</span></span> <span data-ttu-id="ae6f2-108">承認者は、これらの要求を承認または拒否したり、抽出されたデータから削除する必要があるユーザー グループを指定したりすることができます。また、以前に承認した要求を取り消すこともできます。</span><span class="sxs-lookup"><span data-stu-id="ae6f2-108">Approvers can approve or deny these requests, specify a user group that should be scrubbed out of extracted data, or revoke a previously approved request.</span></span> <span data-ttu-id="ae6f2-109">承認は 6 か月間有効となり、Azure Data Factory のパイプラインでのコピー アクティビティごとに 1 つの承認が必要となります。</span><span class="sxs-lookup"><span data-stu-id="ae6f2-109">Approvals persist for 6 months, and one approval is needed per copy activity in the Azure Data Factory pipeline.</span></span> 

<span data-ttu-id="ae6f2-110">すべての要求には、データセットと、データの抽出先のユーザーに関する以下の詳細が常に含まれます。</span><span class="sxs-lookup"><span data-stu-id="ae6f2-110">Every request will always include the following details about the dataset and the users about whom data is being extracted:</span></span>

* <span data-ttu-id="ae6f2-111">**要求者**: パイプラインを要求したユーザー。</span><span class="sxs-lookup"><span data-stu-id="ae6f2-111">**Requestor**: The user who requested the pipeline.</span></span>
* <span data-ttu-id="ae6f2-112">**期間**: 承認された場合の有効期間。</span><span class="sxs-lookup"><span data-stu-id="ae6f2-112">**Duration**: If approved, how long the approval will persist.</span></span> <span data-ttu-id="ae6f2-113">基本的に 4320 時間 (6 か月)。</span><span class="sxs-lookup"><span data-stu-id="ae6f2-113">Always 4320 hours (6 months).</span></span>
* <span data-ttu-id="ae6f2-114">**理由**: 要求の理由。「組織用にインストールされたアプリに、Office 365 データへのアクセスの承認が必要」が通常の理由となります。</span><span class="sxs-lookup"><span data-stu-id="ae6f2-114">**Reason**: Reason for the request, typically "An app installed for your organization requires approval for access to Office 365 Data."</span></span>
* <span data-ttu-id="ae6f2-115">**要求日時**: 要求の DateTime。</span><span class="sxs-lookup"><span data-stu-id="ae6f2-115">**Requested at**: The DateTime of the request.</span></span>
* <span data-ttu-id="ae6f2-116">**要求 ID**: 承認の目的で使用される要求の ID。</span><span class="sxs-lookup"><span data-stu-id="ae6f2-116">**Request id**: The ID of the request, used for approval purposes.</span></span>
* <span data-ttu-id="ae6f2-117">**DataTable**: 抽出されるデータ セット (例: 送信済みアイテムなど)。</span><span class="sxs-lookup"><span data-stu-id="ae6f2-117">**DataTable**: The data set being extracted (for example, Sent Items).</span></span>
* <span data-ttu-id="ae6f2-118">**列**: データ テーブルから抽出される列のリスト (例: SentDateTime など)。</span><span class="sxs-lookup"><span data-stu-id="ae6f2-118">**Columns**: The list of columns being extracted from the data table (for example, SentDateTime).</span></span>
* <span data-ttu-id="ae6f2-119">**AllowedGroups**: パイプラインによるデータ抽出の対象となるユーザーのグループ。</span><span class="sxs-lookup"><span data-stu-id="ae6f2-119">**AllowedGroups**: The group or groups of users against whom the pipeline is extracting data.</span></span> <span data-ttu-id="ae6f2-120">グループのリストが空の場合、パイプラインはテナント内の全ユーザーのデータへのアクセスを要求します。</span><span class="sxs-lookup"><span data-stu-id="ae6f2-120">If the list of groups is empty, the pipeline is requesting access to data from all users in the tenant.</span></span>
* <span data-ttu-id="ae6f2-121">**ユーザー スコープ クエリ**: ユーザーをフィルターで除外する場合に使用する述語。</span><span class="sxs-lookup"><span data-stu-id="ae6f2-121">**User Scope Query**: The predicate used to filter out users.</span></span> <span data-ttu-id="ae6f2-122">要求がテナント内のすべてのユーザーに対するものである場合にのみ適用されます。</span><span class="sxs-lookup"><span data-stu-id="ae6f2-122">Only applies if the request is for all users in the tenant.</span></span> <span data-ttu-id="ae6f2-123">これが空の場合は、フィルターは適用されません。</span><span class="sxs-lookup"><span data-stu-id="ae6f2-123">If this is empty, no filter is applied.</span></span> 
* <span data-ttu-id="ae6f2-124">**OutputUri**: 抽出されたデータが格納される出力パス。</span><span class="sxs-lookup"><span data-stu-id="ae6f2-124">**OutputUri**: The output path in which the extracted data will be stored.</span></span>
* <span data-ttu-id="ae6f2-125">**SourceTenantId**: データの抽出元のテナント ID。</span><span class="sxs-lookup"><span data-stu-id="ae6f2-125">**SourceTenantId**: The tenant ID from which data is being extracted.</span></span>
* <span data-ttu-id="ae6f2-126">**InstallerIdentity**: アプリのインストーラーの ID。</span><span class="sxs-lookup"><span data-stu-id="ae6f2-126">**InstallerIdentity**: The identity of the app installer.</span></span>

<span data-ttu-id="ae6f2-127">要求内の次のフィールドは、限られた場合にのみ使用可能となります。</span><span class="sxs-lookup"><span data-stu-id="ae6f2-127">The following fields in the request will be available only in some cases:</span></span>

* <span data-ttu-id="ae6f2-128">アプリケーション名と Marketplace URI (Azure Marketplace からインストールされたアプリケーションに対してのみ使用可能)。</span><span class="sxs-lookup"><span data-stu-id="ae6f2-128">Application Name and the Marketplace URI (available only for applications installed from the Azure marketplace).</span></span>
* <span data-ttu-id="ae6f2-129">アプリケーションのプライバシー ポリシーとサービス利用規約へのリンク (アプリケーションから提供されている場合にのみ使用可能)。</span><span class="sxs-lookup"><span data-stu-id="ae6f2-129">Links to the application's privacy policy and terms of service (available only if the application provides it).</span></span>
* <span data-ttu-id="ae6f2-130">出力の保管場所での保存データの暗号化など、アプリケーションが実施するコンプライアンス ポリシー (コンプライアンス ポリシーがアプリケーションから提供され、アプリケーションが Azure Marketplace からインストールされている場合にのみ使用可能)。</span><span class="sxs-lookup"><span data-stu-id="ae6f2-130">The compliance policies that the application enforces, such as data encryption at rest in the output storage location (available only if the application provides it and if the application is installed from the Azure marketplace).</span></span>
* <span data-ttu-id="ae6f2-131">拒否リスト - 抽出されたデータから削除できるユーザー グループ。</span><span class="sxs-lookup"><span data-stu-id="ae6f2-131">Deny List - The user group that can be scrubbed out of the extracted data.</span></span> <span data-ttu-id="ae6f2-132">このフィールドは、抽出されたデータのプライバシーに関するスクラブをサポートする要求の一環として、空となります。</span><span class="sxs-lookup"><span data-stu-id="ae6f2-132">This field is empty as a part of the request for datasets that support privacy scrubbing of extracted data.</span></span> <span data-ttu-id="ae6f2-133">要求を承認する承認者グループのメンバーが、承認の際にこのフィールドを設定できます。</span><span class="sxs-lookup"><span data-stu-id="ae6f2-133">It can be populated by the member of the approver group who approves the request at approval time.</span></span> 

## <a name="approving-requests"></a><span data-ttu-id="ae6f2-134">要求の承認</span><span class="sxs-lookup"><span data-stu-id="ae6f2-134">Approving requests</span></span>

<span data-ttu-id="ae6f2-135">データ接続のパイプラインは、データ アクセス要求の承認者グループのメンバーによって承認される必要があります。</span><span class="sxs-lookup"><span data-stu-id="ae6f2-135">Data connect pipelines must be approved by a member of a data access request approver group.</span></span> <span data-ttu-id="ae6f2-136">承認者は、Exchange Online PowerShell モジュールまたは PAM ユーザー エクスペリエンスを使用して、パイプラインの承認、拒否、あるいは取り消しを行うことができます。</span><span class="sxs-lookup"><span data-stu-id="ae6f2-136">Approvers can approve, deny, or revoke pipelines by using the Exchange Online PowerShell module or the PAM user experience.</span></span>

### <a name="approving-denying-and-revoking-requests-by-using-powershell"></a><span data-ttu-id="ae6f2-137">PowerShell を使用した要求の承認、拒否、取り消し</span><span class="sxs-lookup"><span data-stu-id="ae6f2-137">Approving, denying, and revoking requests by using PowerShell</span></span>

<span data-ttu-id="ae6f2-138">Exchange Online PowerShell モジュールを使用して要求を処理するには、次の手順を実行します。</span><span class="sxs-lookup"><span data-stu-id="ae6f2-138">Use the following steps to interact with a request using the Exchange Online PowerShell module:</span></span>

1. <span data-ttu-id="ae6f2-139">Exchange Online PowerShell モジュールをインストールします。</span><span class="sxs-lookup"><span data-stu-id="ae6f2-139">Install the Exchange Online Powershell module.</span></span> <span data-ttu-id="ae6f2-140">インストール方法の詳細については、「[多要素認証を使用して Exchange Online PowerShell に接続する](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/mfa-connect-to-exchange-online-powershell?view=exchange-ps)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="ae6f2-140">For installation instructions, see [Connect to Exchange Online PowerShell using multi-factor authentication](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/mfa-connect-to-exchange-online-powershell?view=exchange-ps).</span></span>

2. <span data-ttu-id="ae6f2-141">多要素認証 (MFA) を使用して Exchange Online PowerShell に接続します。</span><span class="sxs-lookup"><span data-stu-id="ae6f2-141">Connect to Exchange Online Powershell using multi-factor authentication (MFA).</span></span> <span data-ttu-id="ae6f2-142">詳細については、「[多要素認証を使用して Exchange Online PowerShell に接続する](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/mfa-connect-to-exchange-online-powershell?view=exchange-ps)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="ae6f2-142">For instructions, see [Connect to Exchange Online PowerShell using multi-factor authentication](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/mfa-connect-to-exchange-online-powershell?view=exchange-ps).</span></span>
    ><span data-ttu-id="ae6f2-143">**注**: Exchange Online PowerShell への接続中でなくても、組織で多要素認証を有効にしてこれらの手順を実行することができます。</span><span class="sxs-lookup"><span data-stu-id="ae6f2-143">**Note**: You do not need to enable multi-factor authentication for your organization to use these steps while connecting to Exchange Online PowerShell.</span></span> <span data-ttu-id="ae6f2-144">MFA と接続すると、要求への署名のために PAM によって使用される OAuth トークンが作成されます。</span><span class="sxs-lookup"><span data-stu-id="ae6f2-144">Connecting with MFA creates an OAuth token that is used by PAM for signing your requests.</span></span>

3. <span data-ttu-id="ae6f2-145">自分のアカウントでサインインします。</span><span class="sxs-lookup"><span data-stu-id="ae6f2-145">Sign in with your account.</span></span> <span data-ttu-id="ae6f2-146">要求の承認、拒否、または取り消しを行うには、構成済みのデータ アクセスの承認者グループのメンバーである必要があります。</span><span class="sxs-lookup"><span data-stu-id="ae6f2-146">Note that you must be part of the configured data access approver group in order to be able to approve, deny, or revoke requests.</span></span> <span data-ttu-id="ae6f2-147">ゲスト ユーザーは承認者グループであっても要求を承認することができません。</span><span class="sxs-lookup"><span data-stu-id="ae6f2-147">Guest users cannot approve requests, even if they are in the approver group.</span></span> 

   ```powershell
   Connect-EXOPSSession
   ```

4. <span data-ttu-id="ae6f2-148">保留中の要求を確認します。</span><span class="sxs-lookup"><span data-stu-id="ae6f2-148">Find all pending requests.</span></span>
   ><span data-ttu-id="ae6f2-149">**注:** 要求を識別して承認または拒否するには、**ID** プロパティの値を使用します。</span><span class="sxs-lookup"><span data-stu-id="ae6f2-149">**Note:** The value in the **Identity** property will be used to identify and approve or deny the request.</span></span> <span data-ttu-id="ae6f2-150">この値をメモして、-RequestId パラメーターで使用してください。</span><span class="sxs-lookup"><span data-stu-id="ae6f2-150">Note this value and use it in the -RequestId parameter.</span></span> 

   ```powershell
   Get-ElevatedAccessRequest | ?{$_.RequestStatus -eq 'Pending'}
   ```

4. <span data-ttu-id="ae6f2-151">関心のある要求の**コンテキスト** フィールドの詳細を確認します。</span><span class="sxs-lookup"><span data-stu-id="ae6f2-151">Take a closer look at the **context** field of the request you are interested in.</span></span> 
   ><span data-ttu-id="ae6f2-152">**注:** データ アクセスの要求のコンテキスト フィールドには、コピー アクティビティのパラメーターとプロパティが記述されます。</span><span class="sxs-lookup"><span data-stu-id="ae6f2-152">**Note:** The context field of the data access request describes the parameters and properties of the copy activity.</span></span>

   ```powershell
   (Get-ElevatedAccessRequest -RequestId $requestId).Context | ConvertFrom-Json
   ```

   <span data-ttu-id="ae6f2-153">次のような応答を受け取ります。</span><span class="sxs-lookup"><span data-stu-id="ae6f2-153">You'll get a response that looks like the following.</span></span>

   ```powershell
   Key                          Value
   ---                          -----
   ApplicationName
   ComplianceStatus             [{"Timestamp":"2018-05-02T18:29:21.5705664Z","RequirementName":"adlsEncryption","PolicyComplianceState":"Compliant","Violations":0},{"Timestamp":"2018-05-02T...
   ApplicationMarketPlaceUri
   OutputUri                    adl://myadlserumvrroyspmq.azuredatalakestore.net/targetFolder/Event
   ApplicationPrivacyPolicyUri  http://www.wkw.com/privacy
   ApplicationTermsOfServiceUri http://www.wkw.com/tos
   InstallerIdentity            a89885c3-4b0e-499e-86ed-14d7ed9147c2@942229f8-4656-4fb0-828b-e938dad4019a
   SourceTenantId               942229f8-4656-4fb0-828b-e938dad4019a
   UserScopeQuery               tenant in (942229f8-4656-4fb0-828b-e938dad4019a)
   ApplicationId
   DataTable                    Calendar Events
   DestinationTenantId          942229f8-4656-4fb0-828b-e938dad4019a
   Columns                      Subject:string, HasAttachments:bool, End:DateTime, Start:DateTime, ResponseStatus:string, Organizer:Object, Attendees:string, Importance:string, Sensitivity:...
   ```

5. <span data-ttu-id="ae6f2-154">-RequestId パラメーターに **ID** の値を使用して、要求の承認または拒否を行います。</span><span class="sxs-lookup"><span data-stu-id="ae6f2-154">Approve/deny the request using the value for **Identity** for the -RequestId parameter.</span></span>

   ```powershell
   Approve-ElevatedAccessRequest -RequestId $requestId -Comment "Yay!!"
   Deny-ElevatedAccessRequest -RequestId $requestId -Comment "Nay!!"
   ```

<span data-ttu-id="ae6f2-155">特定のユーザーからのデータが含まれないように、拒否リストを使用して要求を承認することもできます。</span><span class="sxs-lookup"><span data-stu-id="ae6f2-155">You can also approve the request with a deny list to ensure data from certain users is not included.</span></span> <span data-ttu-id="ae6f2-156">これを行うには、要求のコンテキストを変更して、除外するグループの `object Id` を追加してから要求を承認する必要があります。</span><span class="sxs-lookup"><span data-stu-id="ae6f2-156">To do so, you need to modify the context of the request to add the `object Id` of the group that you want to omit and then approve the request.</span></span> 

   ```powershell
   $request = Get-ElevatedAccessRequest -RequestId
   $hash = $request.Context
   $hash["DenyList"] = <Object ID of denied user group>;
   Approve-ElevatedAccessRequest -RequestId $requestId -Comment "Yay!!" -RequestContext $hash
   Deny-ElevatedAccessRequest -RequestId $requestId -Comment "Nay!!"
   ```
<span data-ttu-id="ae6f2-157">以前に承認した要求を取り消すこともできます。</span><span class="sxs-lookup"><span data-stu-id="ae6f2-157">You can also revoke requests that were previously approved.</span></span> <span data-ttu-id="ae6f2-158">要求の承認と同様に、**ID** の値は -RequestId パラメーターに必要となります。</span><span class="sxs-lookup"><span data-stu-id="ae6f2-158">Similar to approving requests, the value for **Identity** is what is required in the -RequestId parameter.</span></span> 

   ```powershell 
   Revoke-ElevatedAccessAuthorization -Comment "Revoking this request!" -RequestId $requestId
   ```
   <span data-ttu-id="ae6f2-159">次のような応答を受信します。</span><span class="sxs-lookup"><span data-stu-id="ae6f2-159">You'll see a response similar to the following.</span></span>
   
   ```powershell
   AuthorizedBy          : user@tenant.onmicrosoft.com
   Type                  : Task
   AuthorizedAccess      : Data Access Request
   StartTimeUtc          : 7/24/2018 6:02:42 PM
   EndTimeUtc            : 10/22/2018 6:02:42 PM
   Revoked               : True
   RevocationDateTimeUtc : 7/24/2018 9:12:55 PM
   RevokedBy             : NAMPR00A001.prod.outlook.com/Microsoft Exchange Hosted  Organizations/tenant.onmicrosoft.com/user
   RevocationComment     : Revoking this request!
   Identity              : bda75607-0d87-43cb-bdf1-284b18446b34
   DateCreatedUtc        : 1/1/0001 12:00:00 AM
   DateUpdatedUtc        : 7/24/2018 9:12:55 PM
   ```

### <a name="approving-denying-and-revoking-requests-by-using-the-pam-user-experience"></a><span data-ttu-id="ae6f2-160">PAM ユーザー エクスペリエンスを使用した要求の承認、拒否、取り消し</span><span class="sxs-lookup"><span data-stu-id="ae6f2-160">Approving, denying, and revoking requests by using the PAM user experience</span></span>

<span data-ttu-id="ae6f2-161">PAM Web エクスペリエンスを使用して要求を処理するには、次の手順を実行します。</span><span class="sxs-lookup"><span data-stu-id="ae6f2-161">Use the following steps to interact with a request using the PAM web experience:</span></span>

1. <span data-ttu-id="ae6f2-162">管理者の資格情報を使用して Office 365 管理ポータルにサインインし、[Privileged Access Management の承認ユーザー エクスペリエンス](https://admin.microsoft.com/AdminPortal/Home#/Settings/PrivilegedAccess)のページに移動します。</span><span class="sxs-lookup"><span data-stu-id="ae6f2-162">Sign in to the Office 365 admin portal using admin credentials and go to the [Privileged Access Managment approval user experience](https://admin.microsoft.com/AdminPortal/Home#/Settings/PrivilegedAccess) page.</span></span> <span data-ttu-id="ae6f2-163">ページに移動すると、すべてのアクセス要求 (保留中/承認済み/期限切れ/拒否) が表示されます。</span><span class="sxs-lookup"><span data-stu-id="ae6f2-163">This will show you all the access requests (pending/approved/expired/denied).</span></span>

<span data-ttu-id="ae6f2-164">表示されたページで、関心のある要求を選択します。</span><span class="sxs-lookup"><span data-stu-id="ae6f2-164">On the resulting page, select the request that you are interested in.</span></span> <span data-ttu-id="ae6f2-165">プライバシーに関するスクラブの拒否リストを選択するには、**[DenyList]** ドロップダウンをクリックし、スクラブを行うグループを選択して、**[承認]** を選択します。</span><span class="sxs-lookup"><span data-stu-id="ae6f2-165">To select deny list for privacy scrubbing, click the **DenyList** dropdown, select the group that needs to be scrubbed, and then select **Approve**.</span></span>

<span data-ttu-id="ae6f2-166">以前に承認した要求を取り消すには、取り消す必要がある承認済みの要求を選択し、**[取り消し]** を選択します。</span><span class="sxs-lookup"><span data-stu-id="ae6f2-166">To revoke a previously approved request, select the approved request that needs to be revoked, and choose **Revoke**.</span></span> <span data-ttu-id="ae6f2-167">この操作以降、取り消した承認でデータを移動することはできなくなります。</span><span class="sxs-lookup"><span data-stu-id="ae6f2-167">The next attempt to move data using that approval will fail.</span></span> 

### <a name="approval-behavior"></a><span data-ttu-id="ae6f2-168">承認の動作</span><span class="sxs-lookup"><span data-stu-id="ae6f2-168">Approval behavior</span></span>

<span data-ttu-id="ae6f2-169">データ接続の承認要求をする際には、以下の点に注意することが重要です。</span><span class="sxs-lookup"><span data-stu-id="ae6f2-169">Data conenct approval requests have particular characteristics that are important to be aware of:</span></span>

- <span data-ttu-id="ae6f2-170">承認要求は Azure Data Factory、パイプライン、コピー アクティビティの名前に基づきます。</span><span class="sxs-lookup"><span data-stu-id="ae6f2-170">Approval requests are based on the Azure Data Factory, pipeline and copy activity names.</span></span> <span data-ttu-id="ae6f2-171">コピー アクティビティを実行するたびに、Office 365 管理者が Office データへのアクセスに関するコピー アクティビティの要求を承認したかどうかが確認されます。また、承認のパラメーターに対するコピー アクティビティの重要なパラメーターが実行されているかどうかの検証も行われます。</span><span class="sxs-lookup"><span data-stu-id="ae6f2-171">Every copy activity run will verify that the Office 365 admin has approved the copy activity's request to access Office data, and will validate the important parameters of the copy activity run against the parameters of the approval.</span></span>
- <span data-ttu-id="ae6f2-172">特定の条件においては、新しい承認要求が自動的にトリガーされます。</span><span class="sxs-lookup"><span data-stu-id="ae6f2-172">Under certain conditions, a new approval request will automatically be triggered.</span></span> <span data-ttu-id="ae6f2-173">コピー アクティビティが Office 365 データにアクセスするには、データ接続の承認者が新しい要求を承認する必要があります。</span><span class="sxs-lookup"><span data-stu-id="ae6f2-173">A data connect approver will have to approve the new request before the copy activity can access Office 365 data.</span></span>
- <span data-ttu-id="ae6f2-174">コピー アクティビティ実行のパラメーターが変更されると、新しい承認要求がトリガーされます。</span><span class="sxs-lookup"><span data-stu-id="ae6f2-174">If the parameters of the copy activity run changes, a new approval request will be triggered.</span></span>
- <span data-ttu-id="ae6f2-175">Data Factory、パイプライン、コピー アクティビティの名前のパラメーターが変更されると、新しい承認要求がトリガーされます。</span><span class="sxs-lookup"><span data-stu-id="ae6f2-175">If the Data Factory, pipeline or copy activity names change, a new approval request will be triggered.</span></span>
- <span data-ttu-id="ae6f2-176">たとえば、コピー アクティビティがアクセスしているデータ テーブルまたは列のセットが変更された場合は、新しい承認が必要になります。</span><span class="sxs-lookup"><span data-stu-id="ae6f2-176">For example: A new approval will be required if the data table or set of columns that the copy activity is accessing changes.</span></span>
- <span data-ttu-id="ae6f2-177">コピー アクティビティは 6 か月に 1 回承認される必要があります。</span><span class="sxs-lookup"><span data-stu-id="ae6f2-177">Copy activities will have to be approved once every 6 months.</span></span> <span data-ttu-id="ae6f2-178">元の承認が 6 か月前に承認された場合は、新しい承認要求が自動的にトリガーされます。</span><span class="sxs-lookup"><span data-stu-id="ae6f2-178">If the original approval was approved 6 months ago, a new approval request will automatically be triggered.</span></span>
- <span data-ttu-id="ae6f2-179">Office 365 データへのアクセス承認者が承認要求を拒否したり、以前に承認した要求を取り消したりした場合、コピー アクティビティの実行ができなくなります。</span><span class="sxs-lookup"><span data-stu-id="ae6f2-179">If an Office 365 Data Access approver has denied an approval request or revoked a previously approved request, the copy activity will fail continually.</span></span> <span data-ttu-id="ae6f2-180">承認者と協力して、拒否または取り消しの理由を確認し、必要に応じてコピー アクティビティのパラメーターを修正する必要があります。</span><span class="sxs-lookup"><span data-stu-id="ae6f2-180">You should work with the approver to understand the reason for the denial or revocation and fix the parameters of the copy activity accordingly.</span></span> <span data-ttu-id="ae6f2-181">新しい承認要求をトリガーするためには、新しいコピー アクティビティを展開するか、既存のコピー アクティビティの名前を変更する必要があります。</span><span class="sxs-lookup"><span data-stu-id="ae6f2-181">A new copy activity will have to deployed, or the name of the existing copy activity will have to be changed in order to trigger a new approval request for approval.</span></span>
- <span data-ttu-id="ae6f2-182">Office 365 データへのアクセス承認者が要求を処理しない限り、承認要求は 24 時間で期限切れになります。</span><span class="sxs-lookup"><span data-stu-id="ae6f2-182">An approval request will expire in 24 hours unless an Office 365 data access approver acts on the request.</span></span> <span data-ttu-id="ae6f2-183">新しい承認要求は 24 時間ごとに 1 回送信されます。</span><span class="sxs-lookup"><span data-stu-id="ae6f2-183">A new request will be submitted once every 24 hours for approval.</span></span> <span data-ttu-id="ae6f2-184">コピー アクティビティが承認待ち (同意が保留中の段階) の場合は、Office 365 データへのアクセス承認者と協力して要求を承認する必要があります。</span><span class="sxs-lookup"><span data-stu-id="ae6f2-184">If you see your copy activity waiting for approval (in the Consent Pending stage), then work with Office 365 data access approvers to get your request approved.</span></span>

## <a name="privacy-scrubbing"></a><span data-ttu-id="ae6f2-185">プライバシーに関するスクラブ</span><span class="sxs-lookup"><span data-stu-id="ae6f2-185">Privacy scrubbing</span></span> 
<span data-ttu-id="ae6f2-186">要求を承認する承認者グループのメンバーは、抽出されたデータからデータを削除する 1 つのユーザー グループの名前を指定することができます。</span><span class="sxs-lookup"><span data-stu-id="ae6f2-186">The member of the approver group who approves the request can specify the name of one user group whose data would be scrubbed out of extracted data.</span></span> <span data-ttu-id="ae6f2-187">拒否されたグループのメンバーのメール アドレスを含む行は、抽出されたデータから削除されます。</span><span class="sxs-lookup"><span data-stu-id="ae6f2-187">The rows containing email addresses corresponding to the members of the denied group will be scrubbed out of extracted data.</span></span> <span data-ttu-id="ae6f2-188">拒否されたグループ内に入れ子になっているグループは展開され、ユーザーだけが削除されます。PowerShell または PAM UX を使用して承認中に拒否リストを適用する方法の詳細については、このトピックの「要求の承認」セクションを参照してください。</span><span class="sxs-lookup"><span data-stu-id="ae6f2-188">Groups nested within the denied group will be expanded and only users will be scrubbed out. Refer to the approving requests section of this topic for details on how to apply the deny list during approval, through either PowerShell or the PAM UX.</span></span> 

<span data-ttu-id="ae6f2-189">次の表は、データセットの名前と、プライバシーに関するスクラブ用にコンテンツの確認が行われる列を示しています。</span><span class="sxs-lookup"><span data-stu-id="ae6f2-189">The following table shows the names of the datasets and the columns for which the contents are checked for privacy scrubbing.</span></span>

| <span data-ttu-id="ae6f2-190">データセット名</span><span class="sxs-lookup"><span data-stu-id="ae6f2-190">Dataset name</span></span>                     | <span data-ttu-id="ae6f2-191">拒否リストに基づいたスクラブに使用される列</span><span class="sxs-lookup"><span data-stu-id="ae6f2-191">Columns used for deny list-based scrubbing</span></span>                                                  |
|---------------------------------------------------------------------|----------------------------------------------------------|
| <span data-ttu-id="ae6f2-192">**BasicDataSet_v0.Message_v0**</span><span class="sxs-lookup"><span data-stu-id="ae6f2-192">**BasicDataSet_v0.Message_v0**</span></span><br><span data-ttu-id="ae6f2-193">**BasicDataSet_v0.Message_v1**</span><span class="sxs-lookup"><span data-stu-id="ae6f2-193">**BasicDataSet_v0.Message_v1**</span></span>   | <span data-ttu-id="ae6f2-194">Sender、From、ToRecipients、CcRecipients、BccRecipients</span><span class="sxs-lookup"><span data-stu-id="ae6f2-194">Sender, From, ToRecipients, CcRecipients, BccRecipients</span></span>    |                                                                               
| <span data-ttu-id="ae6f2-195">**BasicDataSet_v0.SentItem_v0**</span><span class="sxs-lookup"><span data-stu-id="ae6f2-195">**BasicDataSet_v0.SentItem_v0**</span></span><br><span data-ttu-id="ae6f2-196">**BasicDataSet_v0.SentItem_v1**</span><span class="sxs-lookup"><span data-stu-id="ae6f2-196">**BasicDataSet_v0.SentItem_v1**</span></span>  | <span data-ttu-id="ae6f2-197">Sender、From、ToRecipients、CcRecipients、BccRecipients</span><span class="sxs-lookup"><span data-stu-id="ae6f2-197">Sender, From, ToRecipients, CcRecipients, BccRecipients</span></span>  |
| <span data-ttu-id="ae6f2-198">**BasicDataSet_v0.Event_v0**</span><span class="sxs-lookup"><span data-stu-id="ae6f2-198">**BasicDataSet_v0.Event_v0**</span></span><br><span data-ttu-id="ae6f2-199">**BasicDataSet_v0.Event_v1**</span><span class="sxs-lookup"><span data-stu-id="ae6f2-199">**BasicDataSet_v0.Event_v1**</span></span>     | <span data-ttu-id="ae6f2-200">Organizer、Attendees</span><span class="sxs-lookup"><span data-stu-id="ae6f2-200">Organizer, Attendees</span></span>                                        |
| <span data-ttu-id="ae6f2-201">**BasicDataSet_v0.Contact_v0**</span><span class="sxs-lookup"><span data-stu-id="ae6f2-201">**BasicDataSet_v0.Contact_v0**</span></span><br><span data-ttu-id="ae6f2-202">**BasicDataSet_v0.Contact_v1**</span><span class="sxs-lookup"><span data-stu-id="ae6f2-202">**BasicDataSet_v0.Contact_v1**</span></span>  | <span data-ttu-id="ae6f2-203">EmailAddresses</span><span class="sxs-lookup"><span data-stu-id="ae6f2-203">EmailAddresses</span></span>                                            |
| <span data-ttu-id="ae6f2-204">**BasicDataSet_v0.CalendarView_v0**</span><span class="sxs-lookup"><span data-stu-id="ae6f2-204">**BasicDataSet_v0.CalendarView_v0**</span></span>                                | <span data-ttu-id="ae6f2-205">Organizer、Attendees</span><span class="sxs-lookup"><span data-stu-id="ae6f2-205">Organizer, Attendees</span></span>                                      |

## <a name="next-steps"></a><span data-ttu-id="ae6f2-206">次の手順</span><span class="sxs-lookup"><span data-stu-id="ae6f2-206">Next Steps</span></span>

<span data-ttu-id="ae6f2-207">「[はじめに](data-connect-get-started.md)」の手順をすべて実行して、Microsoft Graph データが使用できるように Privileged Access Management が組織内で正しく構成されていることを確認します。</span><span class="sxs-lookup"><span data-stu-id="ae6f2-207">Ensure your organization has Privileged Access Management configured correctly for usage with Microsoft Graph data by completing the steps in [Get started](data-connect-get-started.md).</span></span>
