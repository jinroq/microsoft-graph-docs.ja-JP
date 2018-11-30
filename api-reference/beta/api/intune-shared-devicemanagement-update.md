---
title: deviceManagement の更新
description: deviceManagement オブジェクトのプロパティを更新します。
ms.openlocfilehash: 7f73d3fc944dcbc36709cd7f1b46e61bca271152
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27069050"
---
# <a name="update-devicemanagement"></a><span data-ttu-id="bc0fb-103">deviceManagement の更新</span><span class="sxs-lookup"><span data-stu-id="bc0fb-103">Update deviceManagement</span></span>

> <span data-ttu-id="bc0fb-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="bc0fb-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="bc0fb-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="bc0fb-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="bc0fb-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="bc0fb-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="bc0fb-107">[deviceManagement](../resources/intune-shared-devicemanagement.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="bc0fb-107">Update the properties of a [deviceManagement](../resources/intune-shared-devicemanagement.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="bc0fb-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="bc0fb-108">Prerequisites</span></span>

<span data-ttu-id="bc0fb-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="bc0fb-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="bc0fb-111">ワークフローに応じて、[アクセス許可が異なることに注意してください。</span><span class="sxs-lookup"><span data-stu-id="bc0fb-111">Note that the permission vary according to workflow.</span></span>

| <span data-ttu-id="bc0fb-112">アクセス権&nbsp;型&nbsp;(によって&nbsp;ワークフロー)</span><span class="sxs-lookup"><span data-stu-id="bc0fb-112">Permission&nbsp;type&nbsp;(by&nbsp;workflow)</span></span> | <span data-ttu-id="bc0fb-113">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="bc0fb-113">Permissions (from most to least privileged)</span></span> |
|:---|:---|
| <span data-ttu-id="bc0fb-114">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="bc0fb-114">Delegated (work or school account)</span></span> ||
| <span data-ttu-id="bc0fb-115">&nbsp;&nbsp; **Android の作業**</span><span class="sxs-lookup"><span data-stu-id="bc0fb-115">&nbsp; &nbsp; **Android for Work**</span></span> | <span data-ttu-id="bc0fb-116">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bc0fb-116">DeviceManagementConfiguration.ReadWrite.All</span></span>  |
| <span data-ttu-id="bc0fb-117">&nbsp; &nbsp; **監査**</span><span class="sxs-lookup"><span data-stu-id="bc0fb-117">&nbsp; &nbsp; **Auditing**</span></span> | <span data-ttu-id="bc0fb-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bc0fb-118">DeviceManagementApps.ReadWrite.All</span></span> |
| <span data-ttu-id="bc0fb-119">&nbsp;&nbsp; **会社の用語**</span><span class="sxs-lookup"><span data-stu-id="bc0fb-119">&nbsp; &nbsp; **Company terms**</span></span> | <span data-ttu-id="bc0fb-120">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bc0fb-120">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="bc0fb-121">&nbsp; &nbsp; **デバイス構成**</span><span class="sxs-lookup"><span data-stu-id="bc0fb-121">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="bc0fb-122">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bc0fb-122">DeviceManagementConfiguration.ReadWrite.All</span></span> |
| <span data-ttu-id="bc0fb-123">&nbsp; &nbsp; **デバイスの管理**</span><span class="sxs-lookup"><span data-stu-id="bc0fb-123">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="bc0fb-124">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bc0fb-124">DeviceManagementManagedDevices.ReadWrite.All</span></span> |
| <span data-ttu-id="bc0fb-125">&nbsp;&nbsp; **電子 SIM**</span><span class="sxs-lookup"><span data-stu-id="bc0fb-125">&nbsp; &nbsp; **Electronic SIM**</span></span> | <span data-ttu-id="bc0fb-126">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bc0fb-126">DeviceManagementConfiguration.ReadWrite.All</span></span> |
| <span data-ttu-id="bc0fb-127">&nbsp; &nbsp; **登録**</span><span class="sxs-lookup"><span data-stu-id="bc0fb-127">&nbsp; &nbsp; **Enrollment**</span></span> | <span data-ttu-id="bc0fb-128">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bc0fb-128">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="bc0fb-129">&nbsp;&nbsp; **フェンス**</span><span class="sxs-lookup"><span data-stu-id="bc0fb-129">&nbsp; &nbsp; **Fencing**</span></span> | <span data-ttu-id="bc0fb-130">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bc0fb-130">DeviceManagementConfiguration.ReadWrite.All</span></span> |
| <span data-ttu-id="bc0fb-131">&nbsp;&nbsp; **の通知**</span><span class="sxs-lookup"><span data-stu-id="bc0fb-131">&nbsp; &nbsp; **Notification**</span></span> | <span data-ttu-id="bc0fb-132">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bc0fb-132">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="bc0fb-133">&nbsp;&nbsp; **契約時**</span><span class="sxs-lookup"><span data-stu-id="bc0fb-133">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="bc0fb-134">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bc0fb-134">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="bc0fb-135">&nbsp;&nbsp; **ロール ベースのアクセス制御 (RBAC)**</span><span class="sxs-lookup"><span data-stu-id="bc0fb-135">&nbsp; &nbsp; **Role-based access control (RBAC)**</span></span> | <span data-ttu-id="bc0fb-136">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bc0fb-136">DeviceManagementRBAC.ReadWrite.All</span></span> |
| <span data-ttu-id="bc0fb-137">&nbsp;&nbsp; **リモート アクセス**</span><span class="sxs-lookup"><span data-stu-id="bc0fb-137">&nbsp; &nbsp; **Remote access**</span></span> | <span data-ttu-id="bc0fb-138">DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="bc0fb-138">DeviceManagementConfiguration.Read.All</span></span> |
| <span data-ttu-id="bc0fb-139">&nbsp;&nbsp; **リモート アシスタンス**</span><span class="sxs-lookup"><span data-stu-id="bc0fb-139">&nbsp; &nbsp; **Remote assistance**</span></span> | <span data-ttu-id="bc0fb-140">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bc0fb-140">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="bc0fb-141">&nbsp;&nbsp; **通信経費の管理**</span><span class="sxs-lookup"><span data-stu-id="bc0fb-141">&nbsp; &nbsp; **Telecom expense management**</span></span> | <span data-ttu-id="bc0fb-142">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bc0fb-142">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="bc0fb-143">&nbsp;&nbsp; **Troublehooting**</span><span class="sxs-lookup"><span data-stu-id="bc0fb-143">&nbsp; &nbsp; **Troublehooting**</span></span> | <span data-ttu-id="bc0fb-144">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bc0fb-144">DeviceManagementManagedDevices.ReadWrite.All</span></span> |
| <span data-ttu-id="bc0fb-145">&nbsp;&nbsp; **Windows 情報の保護**</span><span class="sxs-lookup"><span data-stu-id="bc0fb-145">&nbsp; &nbsp; **Windows Information Protection**</span></span> | <span data-ttu-id="bc0fb-146">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bc0fb-146">DeviceManagementApps.ReadWrite.All</span></span> |
| <span data-ttu-id="bc0fb-147">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="bc0fb-147">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="bc0fb-148">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="bc0fb-148">Not supported.</span></span>|
| <span data-ttu-id="bc0fb-149">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="bc0fb-149">Application</span></span> | <span data-ttu-id="bc0fb-150">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="bc0fb-150">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="bc0fb-151">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="bc0fb-151">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement
```

## <a name="request-headers"></a><span data-ttu-id="bc0fb-152">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="bc0fb-152">Request headers</span></span>

|<span data-ttu-id="bc0fb-153">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="bc0fb-153">Header</span></span>|<span data-ttu-id="bc0fb-154">値</span><span class="sxs-lookup"><span data-stu-id="bc0fb-154">Value</span></span>|
|:---|:---|
|<span data-ttu-id="bc0fb-155">Authorization</span><span class="sxs-lookup"><span data-stu-id="bc0fb-155">Authorization</span></span>|<span data-ttu-id="bc0fb-156">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="bc0fb-156">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="bc0fb-157">Accept</span><span class="sxs-lookup"><span data-stu-id="bc0fb-157">Accept</span></span>|<span data-ttu-id="bc0fb-158">application/json</span><span class="sxs-lookup"><span data-stu-id="bc0fb-158">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="bc0fb-159">要求本文</span><span class="sxs-lookup"><span data-stu-id="bc0fb-159">Request body</span></span>

<span data-ttu-id="bc0fb-160">要求本文で、[deviceManagement](../resources/intune-shared-devicemanagement.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="bc0fb-160">In the request body, supply a JSON representation for the [deviceManagement](../resources/intune-shared-devicemanagement.md) object.</span></span>

<span data-ttu-id="bc0fb-161">次の表に、[deviceManagement](../resources/intune-shared-devicemanagement.md) の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="bc0fb-161">The following table shows the properties that are required when you create the [deviceManagement](../resources/intune-shared-devicemanagement.md).</span></span>

|<span data-ttu-id="bc0fb-162">プロパティ</span><span class="sxs-lookup"><span data-stu-id="bc0fb-162">Property</span></span>|<span data-ttu-id="bc0fb-163">型</span><span class="sxs-lookup"><span data-stu-id="bc0fb-163">Type</span></span>|<span data-ttu-id="bc0fb-164">説明</span><span class="sxs-lookup"><span data-stu-id="bc0fb-164">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bc0fb-165">id</span><span class="sxs-lookup"><span data-stu-id="bc0fb-165">id</span></span>|<span data-ttu-id="bc0fb-166">String</span><span class="sxs-lookup"><span data-stu-id="bc0fb-166">String</span></span>|<span data-ttu-id="bc0fb-167">デバイスの一意の識別子です。</span><span class="sxs-lookup"><span data-stu-id="bc0fb-167">Unique identifier for the device.</span></span>|
|<span data-ttu-id="bc0fb-168">**デバイス構成**</span><span class="sxs-lookup"><span data-stu-id="bc0fb-168">**Device configuration**</span></span>|
|<span data-ttu-id="bc0fb-169">intuneAccountId</span><span class="sxs-lookup"><span data-stu-id="bc0fb-169">intuneAccountId</span></span>|<span data-ttu-id="bc0fb-170">GUID</span><span class="sxs-lookup"><span data-stu-id="bc0fb-170">GUID</span></span>|<span data-ttu-id="bc0fb-171">Intune アカウント ID にはテナントが指定されました。</span><span class="sxs-lookup"><span data-stu-id="bc0fb-171">Intune Account ID for given tenant</span></span>|
|<span data-ttu-id="bc0fb-172">legacyPcManangementEnabled</span><span class="sxs-lookup"><span data-stu-id="bc0fb-172">legacyPcManangementEnabled</span></span>|<span data-ttu-id="bc0fb-173">ブール値</span><span class="sxs-lookup"><span data-stu-id="bc0fb-173">Boolean</span></span>|<span data-ttu-id="bc0fb-174">非 MDM を有効にするプロパティは、このアカウントの従来の PC の管理を管理します。</span><span class="sxs-lookup"><span data-stu-id="bc0fb-174">The property to enable Non-MDM managed legacy PC management for this account.</span></span> <span data-ttu-id="bc0fb-175">このプロパティは値の取得のみ可能です。</span><span class="sxs-lookup"><span data-stu-id="bc0fb-175">This property is read-only.</span></span>|
|<span data-ttu-id="bc0fb-176">maximumDepTokens</span><span class="sxs-lookup"><span data-stu-id="bc0fb-176">maximumDepTokens</span></span>|<span data-ttu-id="bc0fb-177">Int32</span><span class="sxs-lookup"><span data-stu-id="bc0fb-177">Int32</span></span>|<span data-ttu-id="bc0fb-178">DEP のトークンの最大数では、テナントごとに許可されます。</span><span class="sxs-lookup"><span data-stu-id="bc0fb-178">Maximum number of DEP tokens allowed per-tenant.</span></span>|
|<span data-ttu-id="bc0fb-179">settings</span><span class="sxs-lookup"><span data-stu-id="bc0fb-179">settings</span></span>|[<span data-ttu-id="bc0fb-180">deviceManagementSettings</span><span class="sxs-lookup"><span data-stu-id="bc0fb-180">deviceManagementSettings</span></span>](../resources/intune-deviceconfig-devicemanagementsettings.md)|<span data-ttu-id="bc0fb-181">アカウント レベルの設定。</span><span class="sxs-lookup"><span data-stu-id="bc0fb-181">Account level settings.</span></span>|
|<span data-ttu-id="bc0fb-182">**デバイスの管理**</span><span class="sxs-lookup"><span data-stu-id="bc0fb-182">**Device management**</span></span>|
|<span data-ttu-id="bc0fb-183">accountMoveCompletionDateTime</span><span class="sxs-lookup"><span data-stu-id="bc0fb-183">accountMoveCompletionDateTime</span></span>|<span data-ttu-id="bc0fb-184">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bc0fb-184">DateTimeOffset</span></span>|<span data-ttu-id="bc0fb-185">日付と時刻 scaleunits のテナントのデータを移動するときです。</span><span class="sxs-lookup"><span data-stu-id="bc0fb-185">The date & time when tenant data moved between scaleunits.</span></span>|
|<span data-ttu-id="bc0fb-186">adminConsent</span><span class="sxs-lookup"><span data-stu-id="bc0fb-186">adminConsent</span></span>|[<span data-ttu-id="bc0fb-187">adminConsent</span><span class="sxs-lookup"><span data-stu-id="bc0fb-187">adminConsent</span></span>](../resources/intune-devices-adminconsent.md)|<span data-ttu-id="bc0fb-188">同意の情報を管理します。</span><span class="sxs-lookup"><span data-stu-id="bc0fb-188">Admin consent information.</span></span>|
|<span data-ttu-id="bc0fb-189">deviceProtectionOverview</span><span class="sxs-lookup"><span data-stu-id="bc0fb-189">deviceProtectionOverview</span></span>|[<span data-ttu-id="bc0fb-190">deviceProtectionOverview</span><span class="sxs-lookup"><span data-stu-id="bc0fb-190">deviceProtectionOverview</span></span>](../resources/intune-devices-deviceprotectionoverview.md)|<span data-ttu-id="bc0fb-191">デバイス保護の概要です。</span><span class="sxs-lookup"><span data-stu-id="bc0fb-191">Device protection overview.</span></span>|
|<span data-ttu-id="bc0fb-192">managedDeviceCleanupSettings</span><span class="sxs-lookup"><span data-stu-id="bc0fb-192">managedDeviceCleanupSettings</span></span>|[<span data-ttu-id="bc0fb-193">managedDeviceCleanupSettings</span><span class="sxs-lookup"><span data-stu-id="bc0fb-193">managedDeviceCleanupSettings</span></span>](../resources/intune-devices-manageddevicecleanupsettings.md)|<span data-ttu-id="bc0fb-194">デバイスのクリーンアップ ・ ルール</span><span class="sxs-lookup"><span data-stu-id="bc0fb-194">Device cleanup rule</span></span>|
|<span data-ttu-id="bc0fb-195">subscriptionState</span><span class="sxs-lookup"><span data-stu-id="bc0fb-195">subscriptionState</span></span>|[<span data-ttu-id="bc0fb-196">deviceManagementSubscriptionState</span><span class="sxs-lookup"><span data-stu-id="bc0fb-196">deviceManagementSubscriptionState</span></span>](../resources/intune-devices-devicemanagementsubscriptionstate.md)|<span data-ttu-id="bc0fb-197">テナントのモバイル デバイス管理のサブスクリプション状態。</span><span class="sxs-lookup"><span data-stu-id="bc0fb-197">Tenant mobile device management subscription state.</span></span> <span data-ttu-id="bc0fb-198">可能な値は、`pending`、`active`、`warning`、`disabled`、`deleted`、`blocked`、`lockedOut` です。</span><span class="sxs-lookup"><span data-stu-id="bc0fb-198">Possible values are: `pending`, `active`, `warning`, `disabled`, `deleted`, `blocked`, `lockedOut`.</span></span>|
|<span data-ttu-id="bc0fb-199">サブスクリプション</span><span class="sxs-lookup"><span data-stu-id="bc0fb-199">subscriptions</span></span>|[<span data-ttu-id="bc0fb-200">deviceManagementSubscriptions</span><span class="sxs-lookup"><span data-stu-id="bc0fb-200">deviceManagementSubscriptions</span></span>](../resources/intune-devices-devicemanagementsubscriptions.md)|<span data-ttu-id="bc0fb-201">テナントのサブスクリプション。</span><span class="sxs-lookup"><span data-stu-id="bc0fb-201">Tenant's Subscription.</span></span> <span data-ttu-id="bc0fb-202">使用可能な値: `none`、`intune`、`office365`、`intunePremium`、`intune_EDU`、`intune_SMB`。</span><span class="sxs-lookup"><span data-stu-id="bc0fb-202">Possible values are: `none`, `intune`, `office365`, `intunePremium`, `intune_EDU`, `intune_SMB`.</span></span>|
|<span data-ttu-id="bc0fb-203">windowsMalwareOverview</span><span class="sxs-lookup"><span data-stu-id="bc0fb-203">windowsMalwareOverview</span></span>|[<span data-ttu-id="bc0fb-204">windowsMalwareOverview</span><span class="sxs-lookup"><span data-stu-id="bc0fb-204">windowsMalwareOverview</span></span>](../resources/intune-devices-windowsmalwareoverview.md)|<span data-ttu-id="bc0fb-205">Windows デバイスのマルウェアの概要です。</span><span class="sxs-lookup"><span data-stu-id="bc0fb-205">Malware overview for windows devices.</span></span>|
|<span data-ttu-id="bc0fb-206">**契約時**</span><span class="sxs-lookup"><span data-stu-id="bc0fb-206">**Onboarding**</span></span>|
|<span data-ttu-id="bc0fb-207">intuneBrand</span><span class="sxs-lookup"><span data-stu-id="bc0fb-207">intuneBrand</span></span>|[<span data-ttu-id="bc0fb-208">intuneBrand</span><span class="sxs-lookup"><span data-stu-id="bc0fb-208">intuneBrand</span></span>](../resources/intune-onboarding-intunebrand.md)|<span data-ttu-id="bc0fb-209">intuneBrand には、会社のポータル アプリケーションとエンド ユーザーの Web ポータルの外観のカスタマイズに使用するデータが含まれています。</span><span class="sxs-lookup"><span data-stu-id="bc0fb-209">intuneBrand contains data which is used in customizing the appearance of the Company Portal applications as well as the end user web portal.</span></span>|

<span data-ttu-id="bc0fb-210">要求本文のプロパティのサポートは、ワークフローによって異なります。</span><span class="sxs-lookup"><span data-stu-id="bc0fb-210">Request body property support varies according to workflow.</span></span>

## <a name="response"></a><span data-ttu-id="bc0fb-211">応答</span><span class="sxs-lookup"><span data-stu-id="bc0fb-211">Response</span></span>
<span data-ttu-id="bc0fb-212">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で更新された [deviceManagement](../resources/intune-shared-devicemanagement.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="bc0fb-212">If successful, this method returns a `200 OK` response code and an updated [deviceManagement](../resources/intune-shared-devicemanagement.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bc0fb-213">例</span><span class="sxs-lookup"><span data-stu-id="bc0fb-213">Example</span></span>

### <a name="request"></a><span data-ttu-id="bc0fb-214">要求</span><span class="sxs-lookup"><span data-stu-id="bc0fb-214">Request</span></span>

<span data-ttu-id="bc0fb-215">デバイス管理のワークフローを次の要求の例を以下に示します。</span><span class="sxs-lookup"><span data-stu-id="bc0fb-215">Here is an example of a request following the device management workflow:</span></span>

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

### <a name="response"></a><span data-ttu-id="bc0fb-216">応答</span><span class="sxs-lookup"><span data-stu-id="bc0fb-216">Response</span></span>

<span data-ttu-id="bc0fb-217">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="bc0fb-217">Here is an example of the response.</span></span> 

<span data-ttu-id="bc0fb-218">注: 簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。</span><span class="sxs-lookup"><span data-stu-id="bc0fb-218">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="bc0fb-219">返されるプロパティは、ワークフローおよびコンテキストによって異なります。</span><span class="sxs-lookup"><span data-stu-id="bc0fb-219">Returned properties vary according to workflow and context.</span></span>

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



