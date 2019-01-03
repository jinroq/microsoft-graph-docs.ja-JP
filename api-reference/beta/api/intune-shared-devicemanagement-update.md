---
title: deviceManagement の更新
description: deviceManagement オブジェクトのプロパティを更新します。
author: tfitzmac
ms.openlocfilehash: 1808c18fd5e305871e0be2e47def97938384488c
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27323766"
---
# <a name="update-devicemanagement"></a><span data-ttu-id="57519-103">deviceManagement の更新</span><span class="sxs-lookup"><span data-stu-id="57519-103">Update deviceManagement</span></span>

> <span data-ttu-id="57519-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="57519-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="57519-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="57519-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="57519-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="57519-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="57519-107">[deviceManagement](../resources/intune-shared-devicemanagement.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="57519-107">Update the properties of a [deviceManagement](../resources/intune-shared-devicemanagement.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="57519-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="57519-108">Prerequisites</span></span>

<span data-ttu-id="57519-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="57519-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="57519-111">ワークフローに応じて、[アクセス許可が異なることに注意してください。</span><span class="sxs-lookup"><span data-stu-id="57519-111">Note that the permission vary according to workflow.</span></span>

| <span data-ttu-id="57519-112">アクセス権&nbsp;型&nbsp;(によって&nbsp;ワークフロー)</span><span class="sxs-lookup"><span data-stu-id="57519-112">Permission&nbsp;type&nbsp;(by&nbsp;workflow)</span></span> | <span data-ttu-id="57519-113">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="57519-113">Permissions (from most to least privileged)</span></span> |
|:---|:---|
| <span data-ttu-id="57519-114">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="57519-114">Delegated (work or school account)</span></span> ||
| <span data-ttu-id="57519-115">&nbsp;&nbsp; **Android の作業**</span><span class="sxs-lookup"><span data-stu-id="57519-115">&nbsp; &nbsp; **Android for Work**</span></span> | <span data-ttu-id="57519-116">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="57519-116">DeviceManagementConfiguration.ReadWrite.All</span></span>  |
| <span data-ttu-id="57519-117">&nbsp; &nbsp; **監査**</span><span class="sxs-lookup"><span data-stu-id="57519-117">&nbsp; &nbsp; **Auditing**</span></span> | <span data-ttu-id="57519-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="57519-118">DeviceManagementApps.ReadWrite.All</span></span> |
| <span data-ttu-id="57519-119">&nbsp;&nbsp; **会社の用語**</span><span class="sxs-lookup"><span data-stu-id="57519-119">&nbsp; &nbsp; **Company terms**</span></span> | <span data-ttu-id="57519-120">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="57519-120">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="57519-121">&nbsp; &nbsp; **デバイス構成**</span><span class="sxs-lookup"><span data-stu-id="57519-121">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="57519-122">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="57519-122">DeviceManagementConfiguration.ReadWrite.All</span></span> |
| <span data-ttu-id="57519-123">&nbsp; &nbsp; **デバイスの管理**</span><span class="sxs-lookup"><span data-stu-id="57519-123">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="57519-124">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="57519-124">DeviceManagementManagedDevices.ReadWrite.All</span></span> |
| <span data-ttu-id="57519-125">&nbsp;&nbsp; **電子 SIM**</span><span class="sxs-lookup"><span data-stu-id="57519-125">&nbsp; &nbsp; **Electronic SIM**</span></span> | <span data-ttu-id="57519-126">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="57519-126">DeviceManagementConfiguration.ReadWrite.All</span></span> |
| <span data-ttu-id="57519-127">&nbsp; &nbsp; **登録**</span><span class="sxs-lookup"><span data-stu-id="57519-127">&nbsp; &nbsp; **Enrollment**</span></span> | <span data-ttu-id="57519-128">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="57519-128">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="57519-129">&nbsp;&nbsp; **フェンス**</span><span class="sxs-lookup"><span data-stu-id="57519-129">&nbsp; &nbsp; **Fencing**</span></span> | <span data-ttu-id="57519-130">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="57519-130">DeviceManagementConfiguration.ReadWrite.All</span></span> |
| <span data-ttu-id="57519-131">&nbsp;&nbsp; **の通知**</span><span class="sxs-lookup"><span data-stu-id="57519-131">&nbsp; &nbsp; **Notification**</span></span> | <span data-ttu-id="57519-132">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="57519-132">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="57519-133">&nbsp;&nbsp; **契約時**</span><span class="sxs-lookup"><span data-stu-id="57519-133">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="57519-134">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="57519-134">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="57519-135">&nbsp;&nbsp; **ロール ベースのアクセス制御 (RBAC)**</span><span class="sxs-lookup"><span data-stu-id="57519-135">&nbsp; &nbsp; **Role-based access control (RBAC)**</span></span> | <span data-ttu-id="57519-136">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="57519-136">DeviceManagementRBAC.ReadWrite.All</span></span> |
| <span data-ttu-id="57519-137">&nbsp;&nbsp; **リモート アクセス**</span><span class="sxs-lookup"><span data-stu-id="57519-137">&nbsp; &nbsp; **Remote access**</span></span> | <span data-ttu-id="57519-138">DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="57519-138">DeviceManagementConfiguration.Read.All</span></span> |
| <span data-ttu-id="57519-139">&nbsp;&nbsp; **リモート アシスタンス**</span><span class="sxs-lookup"><span data-stu-id="57519-139">&nbsp; &nbsp; **Remote assistance**</span></span> | <span data-ttu-id="57519-140">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="57519-140">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="57519-141">&nbsp;&nbsp; **通信経費の管理**</span><span class="sxs-lookup"><span data-stu-id="57519-141">&nbsp; &nbsp; **Telecom expense management**</span></span> | <span data-ttu-id="57519-142">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="57519-142">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="57519-143">&nbsp;&nbsp; **Troublehooting**</span><span class="sxs-lookup"><span data-stu-id="57519-143">&nbsp; &nbsp; **Troublehooting**</span></span> | <span data-ttu-id="57519-144">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="57519-144">DeviceManagementManagedDevices.ReadWrite.All</span></span> |
| <span data-ttu-id="57519-145">&nbsp;&nbsp; **Windows 情報の保護**</span><span class="sxs-lookup"><span data-stu-id="57519-145">&nbsp; &nbsp; **Windows Information Protection**</span></span> | <span data-ttu-id="57519-146">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="57519-146">DeviceManagementApps.ReadWrite.All</span></span> |
| <span data-ttu-id="57519-147">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="57519-147">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="57519-148">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="57519-148">Not supported.</span></span>|
| <span data-ttu-id="57519-149">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="57519-149">Application</span></span> | <span data-ttu-id="57519-150">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="57519-150">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="57519-151">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="57519-151">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement
```

## <a name="request-headers"></a><span data-ttu-id="57519-152">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="57519-152">Request headers</span></span>

|<span data-ttu-id="57519-153">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="57519-153">Header</span></span>|<span data-ttu-id="57519-154">値</span><span class="sxs-lookup"><span data-stu-id="57519-154">Value</span></span>|
|:---|:---|
|<span data-ttu-id="57519-155">Authorization</span><span class="sxs-lookup"><span data-stu-id="57519-155">Authorization</span></span>|<span data-ttu-id="57519-156">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="57519-156">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="57519-157">Accept</span><span class="sxs-lookup"><span data-stu-id="57519-157">Accept</span></span>|<span data-ttu-id="57519-158">application/json</span><span class="sxs-lookup"><span data-stu-id="57519-158">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="57519-159">要求本文</span><span class="sxs-lookup"><span data-stu-id="57519-159">Request body</span></span>

<span data-ttu-id="57519-160">要求本文で、[deviceManagement](../resources/intune-shared-devicemanagement.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="57519-160">In the request body, supply a JSON representation for the [deviceManagement](../resources/intune-shared-devicemanagement.md) object.</span></span>

<span data-ttu-id="57519-161">次の表に、[deviceManagement](../resources/intune-shared-devicemanagement.md) の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="57519-161">The following table shows the properties that are required when you create the [deviceManagement](../resources/intune-shared-devicemanagement.md).</span></span>

|<span data-ttu-id="57519-162">プロパティ</span><span class="sxs-lookup"><span data-stu-id="57519-162">Property</span></span>|<span data-ttu-id="57519-163">種類</span><span class="sxs-lookup"><span data-stu-id="57519-163">Type</span></span>|<span data-ttu-id="57519-164">説明</span><span class="sxs-lookup"><span data-stu-id="57519-164">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="57519-165">ID</span><span class="sxs-lookup"><span data-stu-id="57519-165">id</span></span>|<span data-ttu-id="57519-166">String</span><span class="sxs-lookup"><span data-stu-id="57519-166">String</span></span>|<span data-ttu-id="57519-167">デバイスの一意の識別子です。</span><span class="sxs-lookup"><span data-stu-id="57519-167">Unique identifier for the device.</span></span>|
|<span data-ttu-id="57519-168">**デバイス構成**</span><span class="sxs-lookup"><span data-stu-id="57519-168">**Device configuration**</span></span>|
|<span data-ttu-id="57519-169">intuneAccountId</span><span class="sxs-lookup"><span data-stu-id="57519-169">intuneAccountId</span></span>|<span data-ttu-id="57519-170">GUID</span><span class="sxs-lookup"><span data-stu-id="57519-170">GUID</span></span>|<span data-ttu-id="57519-171">Intune アカウント ID にはテナントが指定されました。</span><span class="sxs-lookup"><span data-stu-id="57519-171">Intune Account ID for given tenant</span></span>|
|<span data-ttu-id="57519-172">legacyPcManangementEnabled</span><span class="sxs-lookup"><span data-stu-id="57519-172">legacyPcManangementEnabled</span></span>|<span data-ttu-id="57519-173">ブール型</span><span class="sxs-lookup"><span data-stu-id="57519-173">Boolean</span></span>|<span data-ttu-id="57519-174">非 MDM を有効にするプロパティは、このアカウントの従来の PC の管理を管理します。</span><span class="sxs-lookup"><span data-stu-id="57519-174">The property to enable Non-MDM managed legacy PC management for this account.</span></span> <span data-ttu-id="57519-175">このプロパティは読み取りのみ可能です。</span><span class="sxs-lookup"><span data-stu-id="57519-175">This property is read-only.</span></span>|
|<span data-ttu-id="57519-176">maximumDepTokens</span><span class="sxs-lookup"><span data-stu-id="57519-176">maximumDepTokens</span></span>|<span data-ttu-id="57519-177">Int32</span><span class="sxs-lookup"><span data-stu-id="57519-177">Int32</span></span>|<span data-ttu-id="57519-178">DEP のトークンの最大数では、テナントごとに許可されます。</span><span class="sxs-lookup"><span data-stu-id="57519-178">Maximum number of DEP tokens allowed per-tenant.</span></span>|
|<span data-ttu-id="57519-179">settings</span><span class="sxs-lookup"><span data-stu-id="57519-179">settings</span></span>|[<span data-ttu-id="57519-180">deviceManagementSettings</span><span class="sxs-lookup"><span data-stu-id="57519-180">deviceManagementSettings</span></span>](../resources/intune-deviceconfig-devicemanagementsettings.md)|<span data-ttu-id="57519-181">アカウント レベルの設定。</span><span class="sxs-lookup"><span data-stu-id="57519-181">Account level settings.</span></span>|
|<span data-ttu-id="57519-182">**デバイスの管理**</span><span class="sxs-lookup"><span data-stu-id="57519-182">**Device management**</span></span>|
|<span data-ttu-id="57519-183">accountMoveCompletionDateTime</span><span class="sxs-lookup"><span data-stu-id="57519-183">accountMoveCompletionDateTime</span></span>|<span data-ttu-id="57519-184">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="57519-184">DateTimeOffset</span></span>|<span data-ttu-id="57519-185">日付と時刻 scaleunits のテナントのデータを移動するときです。</span><span class="sxs-lookup"><span data-stu-id="57519-185">The date & time when tenant data moved between scaleunits.</span></span>|
|<span data-ttu-id="57519-186">adminConsent</span><span class="sxs-lookup"><span data-stu-id="57519-186">adminConsent</span></span>|[<span data-ttu-id="57519-187">adminConsent</span><span class="sxs-lookup"><span data-stu-id="57519-187">adminConsent</span></span>](../resources/intune-devices-adminconsent.md)|<span data-ttu-id="57519-188">同意の情報を管理します。</span><span class="sxs-lookup"><span data-stu-id="57519-188">Admin consent information.</span></span>|
|<span data-ttu-id="57519-189">deviceProtectionOverview</span><span class="sxs-lookup"><span data-stu-id="57519-189">deviceProtectionOverview</span></span>|[<span data-ttu-id="57519-190">deviceProtectionOverview</span><span class="sxs-lookup"><span data-stu-id="57519-190">deviceProtectionOverview</span></span>](../resources/intune-devices-deviceprotectionoverview.md)|<span data-ttu-id="57519-191">デバイス保護の概要です。</span><span class="sxs-lookup"><span data-stu-id="57519-191">Device protection overview.</span></span>|
|<span data-ttu-id="57519-192">managedDeviceCleanupSettings</span><span class="sxs-lookup"><span data-stu-id="57519-192">managedDeviceCleanupSettings</span></span>|[<span data-ttu-id="57519-193">managedDeviceCleanupSettings</span><span class="sxs-lookup"><span data-stu-id="57519-193">managedDeviceCleanupSettings</span></span>](../resources/intune-devices-manageddevicecleanupsettings.md)|<span data-ttu-id="57519-194">デバイスのクリーンアップ ・ ルール</span><span class="sxs-lookup"><span data-stu-id="57519-194">Device cleanup rule</span></span>|
|<span data-ttu-id="57519-195">subscriptionState</span><span class="sxs-lookup"><span data-stu-id="57519-195">subscriptionState</span></span>|[<span data-ttu-id="57519-196">deviceManagementSubscriptionState</span><span class="sxs-lookup"><span data-stu-id="57519-196">deviceManagementSubscriptionState</span></span>](../resources/intune-devices-devicemanagementsubscriptionstate.md)|<span data-ttu-id="57519-197">テナントのモバイル デバイス管理のサブスクリプション状態。</span><span class="sxs-lookup"><span data-stu-id="57519-197">Tenant mobile device management subscription state.</span></span> <span data-ttu-id="57519-198">可能な値は、`pending`、`active`、`warning`、`disabled`、`deleted`、`blocked`、`lockedOut` です。</span><span class="sxs-lookup"><span data-stu-id="57519-198">Possible values are: `pending`, `active`, `warning`, `disabled`, `deleted`, `blocked`, `lockedOut`.</span></span>|
|<span data-ttu-id="57519-199">サブスクリプション</span><span class="sxs-lookup"><span data-stu-id="57519-199">subscriptions</span></span>|[<span data-ttu-id="57519-200">deviceManagementSubscriptions</span><span class="sxs-lookup"><span data-stu-id="57519-200">deviceManagementSubscriptions</span></span>](../resources/intune-devices-devicemanagementsubscriptions.md)|<span data-ttu-id="57519-201">テナントのサブスクリプション。</span><span class="sxs-lookup"><span data-stu-id="57519-201">Tenant's Subscription.</span></span> <span data-ttu-id="57519-202">使用可能な値: `none`、`intune`、`office365`、`intunePremium`、`intune_EDU`、`intune_SMB`。</span><span class="sxs-lookup"><span data-stu-id="57519-202">Possible values are: `none`, `intune`, `office365`, `intunePremium`, `intune_EDU`, `intune_SMB`.</span></span>|
|<span data-ttu-id="57519-203">windowsMalwareOverview</span><span class="sxs-lookup"><span data-stu-id="57519-203">windowsMalwareOverview</span></span>|[<span data-ttu-id="57519-204">windowsMalwareOverview</span><span class="sxs-lookup"><span data-stu-id="57519-204">windowsMalwareOverview</span></span>](../resources/intune-devices-windowsmalwareoverview.md)|<span data-ttu-id="57519-205">Windows デバイスのマルウェアの概要です。</span><span class="sxs-lookup"><span data-stu-id="57519-205">Malware overview for windows devices.</span></span>|
|<span data-ttu-id="57519-206">**契約時**</span><span class="sxs-lookup"><span data-stu-id="57519-206">**Onboarding**</span></span>|
|<span data-ttu-id="57519-207">intuneBrand</span><span class="sxs-lookup"><span data-stu-id="57519-207">intuneBrand</span></span>|[<span data-ttu-id="57519-208">intuneBrand</span><span class="sxs-lookup"><span data-stu-id="57519-208">intuneBrand</span></span>](../resources/intune-onboarding-intunebrand.md)|<span data-ttu-id="57519-209">intuneBrand には、会社のポータル アプリケーションとエンド ユーザーの Web ポータルの外観のカスタマイズに使用するデータが含まれています。</span><span class="sxs-lookup"><span data-stu-id="57519-209">intuneBrand contains data which is used in customizing the appearance of the Company Portal applications as well as the end user web portal.</span></span>|

<span data-ttu-id="57519-210">要求本文のプロパティのサポートは、ワークフローによって異なります。</span><span class="sxs-lookup"><span data-stu-id="57519-210">Request body property support varies according to workflow.</span></span>

## <a name="response"></a><span data-ttu-id="57519-211">応答</span><span class="sxs-lookup"><span data-stu-id="57519-211">Response</span></span>
<span data-ttu-id="57519-212">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で更新された [deviceManagement](../resources/intune-shared-devicemanagement.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="57519-212">If successful, this method returns a `200 OK` response code and an updated [deviceManagement](../resources/intune-shared-devicemanagement.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="57519-213">例</span><span class="sxs-lookup"><span data-stu-id="57519-213">Example</span></span>

### <a name="request"></a><span data-ttu-id="57519-214">要求</span><span class="sxs-lookup"><span data-stu-id="57519-214">Request</span></span>

<span data-ttu-id="57519-215">デバイス管理のワークフローを次の要求の例を以下に示します。</span><span class="sxs-lookup"><span data-stu-id="57519-215">Here is an example of a request following the device management workflow:</span></span>

``` http
PATCH https://graph.microsoft.com/beta/deviceManagement
Content-type: application/json
Content-length: 751

{
  "subscriptionState": "active",
  "subscriptions": "intune",
  "adminConsent": {
    "@odata.type": "microsoft.graph.adminConsent",
    "shareAPNSData": "granted"
  },
  "deviceProtectionOverview": {
    "@odata.type": "microsoft.graph.deviceProtectionOverview",
    "totalReportedDeviceCount": 8,
    "inactiveThreatAgentDeviceCount": 14,
    "unknownStateThreatAgentDeviceCount": 2,
    "pendingSignatureUpdateDeviceCount": 1,
    "cleanDeviceCount": 0,
    "pendingFullScanDeviceCount": 10,
    "pendingRestartDeviceCount": 9,
    "pendingManualStepsDeviceCount": 13,
    "pendingOfflineScanDeviceCount": 13,
    "criticalFailuresDeviceCount": 11
  },
  "accountMoveCompletionDateTime": "2017-01-01T00:01:17.9006709-08:00"
}
```

### <a name="response"></a><span data-ttu-id="57519-216">応答</span><span class="sxs-lookup"><span data-stu-id="57519-216">Response</span></span>

<span data-ttu-id="57519-217">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="57519-217">Here is an example of the response.</span></span> 

<span data-ttu-id="57519-218">注: 簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。</span><span class="sxs-lookup"><span data-stu-id="57519-218">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="57519-219">返されるプロパティは、ワークフローおよびコンテキストによって異なります。</span><span class="sxs-lookup"><span data-stu-id="57519-219">Returned properties vary according to workflow and context.</span></span>

``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 855

{
  "@odata.type": "#microsoft.graph.deviceManagement",
  "id": "0b283420-3420-0b28-2034-280b2034280b",
  "subscriptionState": "active",
  "subscriptions": "intune",
  "adminConsent": {
    "@odata.type": "microsoft.graph.adminConsent",
    "shareAPNSData": "granted"
  },
  "deviceProtectionOverview": {
    "@odata.type": "microsoft.graph.deviceProtectionOverview",
    "totalReportedDeviceCount": 8,
    "inactiveThreatAgentDeviceCount": 14,
    "unknownStateThreatAgentDeviceCount": 2,
    "pendingSignatureUpdateDeviceCount": 1,
    "cleanDeviceCount": 0,
    "pendingFullScanDeviceCount": 10,
    "pendingRestartDeviceCount": 9,
    "pendingManualStepsDeviceCount": 13,
    "pendingOfflineScanDeviceCount": 13,
    "criticalFailuresDeviceCount": 11
  },
  "accountMoveCompletionDateTime": "2017-01-01T00:01:17.9006709-08:00"
}
```


