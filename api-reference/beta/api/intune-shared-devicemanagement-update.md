---
title: deviceManagement の更新
description: deviceManagement オブジェクトのプロパティを更新します。
author: rolyon
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 43672e497640f64e8efb98edf8f752a0c2415d63
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35979765"
---
# <a name="update-devicemanagement"></a><span data-ttu-id="88150-103">deviceManagement の更新</span><span class="sxs-lookup"><span data-stu-id="88150-103">Update deviceManagement</span></span>

> <span data-ttu-id="88150-104">**重要:** Microsoft Graph の/ベータ版の Api は変更される可能性があります。</span><span class="sxs-lookup"><span data-stu-id="88150-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="88150-105">実稼働アプリケーションでは、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="88150-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="88150-106">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="88150-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="88150-107">[deviceManagement](../resources/intune-shared-devicemanagement.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="88150-107">Update the properties of a [deviceManagement](../resources/intune-shared-devicemanagement.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="88150-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="88150-108">Prerequisites</span></span>

<span data-ttu-id="88150-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="88150-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="88150-111">アクセス許可は、ワークフローによって異なることに注意してください。</span><span class="sxs-lookup"><span data-stu-id="88150-111">Note that the permission vary according to workflow.</span></span>

| <span data-ttu-id="88150-112">アクセス&nbsp;許可&nbsp;の種類&nbsp;(ワークフロー別)</span><span class="sxs-lookup"><span data-stu-id="88150-112">Permission&nbsp;type&nbsp;(by&nbsp;workflow)</span></span> | <span data-ttu-id="88150-113">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="88150-113">Permissions (from most to least privileged)</span></span> |
|:---|:---|
| <span data-ttu-id="88150-114">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="88150-114">Delegated (work or school account)</span></span> ||
| <span data-ttu-id="88150-115">&nbsp;&nbsp; **Android for Work**</span><span class="sxs-lookup"><span data-stu-id="88150-115">&nbsp; &nbsp; **Android for Work**</span></span> | <span data-ttu-id="88150-116">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="88150-116">DeviceManagementConfiguration.ReadWrite.All</span></span>  |
| <span data-ttu-id="88150-117">&nbsp; &nbsp; **監査**</span><span class="sxs-lookup"><span data-stu-id="88150-117">&nbsp; &nbsp; **Auditing**</span></span> | <span data-ttu-id="88150-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="88150-118">DeviceManagementApps.ReadWrite.All</span></span> |
| <span data-ttu-id="88150-119">&nbsp; &nbsp; **会社の用語**</span><span class="sxs-lookup"><span data-stu-id="88150-119">&nbsp; &nbsp; **Company terms**</span></span> | <span data-ttu-id="88150-120">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="88150-120">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="88150-121">&nbsp; &nbsp; **デバイス構成**</span><span class="sxs-lookup"><span data-stu-id="88150-121">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="88150-122">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="88150-122">DeviceManagementConfiguration.ReadWrite.All</span></span> |
| <span data-ttu-id="88150-123">&nbsp;&nbsp; **デバイスの目的**</span><span class="sxs-lookup"><span data-stu-id="88150-123">&nbsp; &nbsp; **Device intent**</span></span> | <span data-ttu-id="88150-124">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="88150-124">DeviceManagementConfiguration.ReadWrite.All</span></span>|
| <span data-ttu-id="88150-125">&nbsp;&nbsp; **デバイスの管理**</span><span class="sxs-lookup"><span data-stu-id="88150-125">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="88150-126">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="88150-126">DeviceManagementManagedDevices.ReadWrite.All</span></span> |
| <span data-ttu-id="88150-127">&nbsp;&nbsp; **電子 SIM**</span><span class="sxs-lookup"><span data-stu-id="88150-127">&nbsp; &nbsp; **Electronic SIM**</span></span> | <span data-ttu-id="88150-128">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="88150-128">DeviceManagementConfiguration.ReadWrite.All</span></span> |
| <span data-ttu-id="88150-129">&nbsp;&nbsp; **登録**</span><span class="sxs-lookup"><span data-stu-id="88150-129">&nbsp; &nbsp; **Enrollment**</span></span> | <span data-ttu-id="88150-130">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="88150-130">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="88150-131">&nbsp;&nbsp; **フェンス**</span><span class="sxs-lookup"><span data-stu-id="88150-131">&nbsp; &nbsp; **Fencing**</span></span> | <span data-ttu-id="88150-132">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="88150-132">DeviceManagementConfiguration.ReadWrite.All</span></span> |
| <span data-ttu-id="88150-133">&nbsp; &nbsp; **通知**</span><span class="sxs-lookup"><span data-stu-id="88150-133">&nbsp; &nbsp; **Notification**</span></span> | <span data-ttu-id="88150-134">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="88150-134">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="88150-135">&nbsp;&nbsp; **Odj**</span><span class="sxs-lookup"><span data-stu-id="88150-135">&nbsp; &nbsp; **Odj**</span></span> | <span data-ttu-id="88150-136">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="88150-136">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="88150-137">&nbsp; &nbsp; **オンボーディング**</span><span class="sxs-lookup"><span data-stu-id="88150-137">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="88150-138">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="88150-138">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="88150-139">&nbsp; &nbsp; **役割ベースのアクセス制御 (RBAC)**</span><span class="sxs-lookup"><span data-stu-id="88150-139">&nbsp; &nbsp; **Role-based access control (RBAC)**</span></span> | <span data-ttu-id="88150-140">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="88150-140">DeviceManagementRBAC.ReadWrite.All</span></span> |
| <span data-ttu-id="88150-141">&nbsp; &nbsp; **リモート アクセス**</span><span class="sxs-lookup"><span data-stu-id="88150-141">&nbsp; &nbsp; **Remote access**</span></span> | <span data-ttu-id="88150-142">DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="88150-142">DeviceManagementConfiguration.Read.All</span></span> |
| <span data-ttu-id="88150-143">&nbsp;&nbsp; **リモートアシスタンス**</span><span class="sxs-lookup"><span data-stu-id="88150-143">&nbsp; &nbsp; **Remote assistance**</span></span> | <span data-ttu-id="88150-144">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="88150-144">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="88150-145">&nbsp;&nbsp; **通信経費管理**</span><span class="sxs-lookup"><span data-stu-id="88150-145">&nbsp; &nbsp; **Telecom expense management**</span></span> | <span data-ttu-id="88150-146">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="88150-146">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="88150-147">&nbsp;&nbsp; **Troublehooting**</span><span class="sxs-lookup"><span data-stu-id="88150-147">&nbsp; &nbsp; **Troublehooting**</span></span> | <span data-ttu-id="88150-148">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="88150-148">DeviceManagementManagedDevices.ReadWrite.All</span></span> |
| <span data-ttu-id="88150-149">&nbsp; &nbsp; **Windows 情報保護**</span><span class="sxs-lookup"><span data-stu-id="88150-149">&nbsp; &nbsp; **Windows Information Protection**</span></span> | <span data-ttu-id="88150-150">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="88150-150">DeviceManagementApps.ReadWrite.All</span></span> |
| <span data-ttu-id="88150-151">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="88150-151">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="88150-152">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="88150-152">Not supported.</span></span>|
| <span data-ttu-id="88150-153">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="88150-153">Application</span></span> | <span data-ttu-id="88150-154">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="88150-154">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="88150-155">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="88150-155">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement
```

## <a name="request-headers"></a><span data-ttu-id="88150-156">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="88150-156">Request headers</span></span>

|<span data-ttu-id="88150-157">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="88150-157">Header</span></span>|<span data-ttu-id="88150-158">値</span><span class="sxs-lookup"><span data-stu-id="88150-158">Value</span></span>|
|:---|:---|
|<span data-ttu-id="88150-159">Authorization</span><span class="sxs-lookup"><span data-stu-id="88150-159">Authorization</span></span>|<span data-ttu-id="88150-160">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="88150-160">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="88150-161">承諾</span><span class="sxs-lookup"><span data-stu-id="88150-161">Accept</span></span>|<span data-ttu-id="88150-162">application/json</span><span class="sxs-lookup"><span data-stu-id="88150-162">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="88150-163">要求本文</span><span class="sxs-lookup"><span data-stu-id="88150-163">Request body</span></span>

<span data-ttu-id="88150-164">要求本文で、[deviceManagement](../resources/intune-shared-devicemanagement.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="88150-164">In the request body, supply a JSON representation for the [deviceManagement](../resources/intune-shared-devicemanagement.md) object.</span></span>

<span data-ttu-id="88150-165">次の表に、[deviceManagement](../resources/intune-shared-devicemanagement.md) の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="88150-165">The following table shows the properties that are required when you create the [deviceManagement](../resources/intune-shared-devicemanagement.md).</span></span>

|<span data-ttu-id="88150-166">プロパティ</span><span class="sxs-lookup"><span data-stu-id="88150-166">Property</span></span>|<span data-ttu-id="88150-167">型</span><span class="sxs-lookup"><span data-stu-id="88150-167">Type</span></span>|<span data-ttu-id="88150-168">説明</span><span class="sxs-lookup"><span data-stu-id="88150-168">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="88150-169">id</span><span class="sxs-lookup"><span data-stu-id="88150-169">id</span></span>|<span data-ttu-id="88150-170">String</span><span class="sxs-lookup"><span data-stu-id="88150-170">String</span></span>|<span data-ttu-id="88150-171">デバイスの一意識別子。</span><span class="sxs-lookup"><span data-stu-id="88150-171">Unique identifier for the device.</span></span>|
|<span data-ttu-id="88150-172">**デバイス構成**</span><span class="sxs-lookup"><span data-stu-id="88150-172">**Device configuration**</span></span>|
|<span data-ttu-id="88150-173">Int未指定 Eaccountid</span><span class="sxs-lookup"><span data-stu-id="88150-173">intuneAccountId</span></span>|<span data-ttu-id="88150-174">GUID</span><span class="sxs-lookup"><span data-stu-id="88150-174">GUID</span></span>|<span data-ttu-id="88150-175">指定したテナントの Intune アカウント ID</span><span class="sxs-lookup"><span data-stu-id="88150-175">Intune Account ID for given tenant</span></span>|
|<span data-ttu-id="88150-176">legacyPcManangementEnabled</span><span class="sxs-lookup"><span data-stu-id="88150-176">legacyPcManangementEnabled</span></span>|<span data-ttu-id="88150-177">Boolean</span><span class="sxs-lookup"><span data-stu-id="88150-177">Boolean</span></span>|<span data-ttu-id="88150-178">このアカウントの非 MDM で管理されているレガシー PC 管理を有効にするプロパティ。</span><span class="sxs-lookup"><span data-stu-id="88150-178">The property to enable Non-MDM managed legacy PC management for this account.</span></span> <span data-ttu-id="88150-179">このプロパティに値を設定するには、 SetExtrusionDirection メソッドを適用します。</span><span class="sxs-lookup"><span data-stu-id="88150-179">This property is read-only.</span></span>|
|<span data-ttu-id="88150-180">maximumDepTokens</span><span class="sxs-lookup"><span data-stu-id="88150-180">maximumDepTokens</span></span>|<span data-ttu-id="88150-181">Int32</span><span class="sxs-lookup"><span data-stu-id="88150-181">Int32</span></span>|<span data-ttu-id="88150-182">テナントごとに許容される DEP トークンの最大数。</span><span class="sxs-lookup"><span data-stu-id="88150-182">Maximum number of DEP tokens allowed per-tenant.</span></span>|
|<span data-ttu-id="88150-183">settings</span><span class="sxs-lookup"><span data-stu-id="88150-183">settings</span></span>|[<span data-ttu-id="88150-184">deviceManagementSettings</span><span class="sxs-lookup"><span data-stu-id="88150-184">deviceManagementSettings</span></span>](../resources/intune-deviceconfig-devicemanagementsettings.md)|<span data-ttu-id="88150-185">アカウント レベルの設定。</span><span class="sxs-lookup"><span data-stu-id="88150-185">Account level settings.</span></span>|
|<span data-ttu-id="88150-186">**デバイスの管理**</span><span class="sxs-lookup"><span data-stu-id="88150-186">**Device management**</span></span>|
|<span data-ttu-id="88150-187">accountMoveCompletionDateTime</span><span class="sxs-lookup"><span data-stu-id="88150-187">accountMoveCompletionDateTime</span></span>|<span data-ttu-id="88150-188">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="88150-188">DateTimeOffset</span></span>|<span data-ttu-id="88150-189">Scaleunits 間でテナントデータを移動したときの日付 & 時刻。</span><span class="sxs-lookup"><span data-stu-id="88150-189">The date & time when tenant data moved between scaleunits.</span></span>|
|<span data-ttu-id="88150-190">adminConsent</span><span class="sxs-lookup"><span data-stu-id="88150-190">adminConsent</span></span>|[<span data-ttu-id="88150-191">adminConsent</span><span class="sxs-lookup"><span data-stu-id="88150-191">adminConsent</span></span>](../resources/intune-devices-adminconsent.md)|<span data-ttu-id="88150-192">管理者の同意情報。</span><span class="sxs-lookup"><span data-stu-id="88150-192">Admin consent information.</span></span>|
|<span data-ttu-id="88150-193">deviceProtectionOverview</span><span class="sxs-lookup"><span data-stu-id="88150-193">deviceProtectionOverview</span></span>|[<span data-ttu-id="88150-194">deviceProtectionOverview</span><span class="sxs-lookup"><span data-stu-id="88150-194">deviceProtectionOverview</span></span>](../resources/intune-devices-deviceprotectionoverview.md)|<span data-ttu-id="88150-195">デバイス保護の概要。</span><span class="sxs-lookup"><span data-stu-id="88150-195">Device protection overview.</span></span>|
|<span data-ttu-id="88150-196">managedDeviceCleanupSettings</span><span class="sxs-lookup"><span data-stu-id="88150-196">managedDeviceCleanupSettings</span></span>|[<span data-ttu-id="88150-197">managedDeviceCleanupSettings</span><span class="sxs-lookup"><span data-stu-id="88150-197">managedDeviceCleanupSettings</span></span>](../resources/intune-devices-manageddevicecleanupsettings.md)|<span data-ttu-id="88150-198">デバイスクリーンアップルール</span><span class="sxs-lookup"><span data-stu-id="88150-198">Device cleanup rule</span></span>|
|<span data-ttu-id="88150-199">subscriptionState</span><span class="sxs-lookup"><span data-stu-id="88150-199">subscriptionState</span></span>|[<span data-ttu-id="88150-200">deviceManagementSubscriptionState</span><span class="sxs-lookup"><span data-stu-id="88150-200">deviceManagementSubscriptionState</span></span>](../resources/intune-devices-devicemanagementsubscriptionstate.md)|<span data-ttu-id="88150-201">テナントのモバイル デバイス管理のサブスクリプション状態。</span><span class="sxs-lookup"><span data-stu-id="88150-201">Tenant mobile device management subscription state.</span></span> <span data-ttu-id="88150-202">可能な値は、`pending`、`active`、`warning`、`disabled`、`deleted`、`blocked`、`lockedOut` です。</span><span class="sxs-lookup"><span data-stu-id="88150-202">Possible values are: `pending`, `active`, `warning`, `disabled`, `deleted`, `blocked`, `lockedOut`.</span></span>|
|<span data-ttu-id="88150-203">subscriptions</span><span class="sxs-lookup"><span data-stu-id="88150-203">subscriptions</span></span>|[<span data-ttu-id="88150-204">deviceManagementSubscriptions</span><span class="sxs-lookup"><span data-stu-id="88150-204">deviceManagementSubscriptions</span></span>](../resources/intune-devices-devicemanagementsubscriptions.md)|<span data-ttu-id="88150-205">テナントのサブスクリプション。</span><span class="sxs-lookup"><span data-stu-id="88150-205">Tenant's Subscription.</span></span> <span data-ttu-id="88150-206">使用可能な値: `none`、`intune`、`office365`、`intunePremium`、`intune_EDU`、`intune_SMB`。</span><span class="sxs-lookup"><span data-stu-id="88150-206">Possible values are: `none`, `intune`, `office365`, `intunePremium`, `intune_EDU`, `intune_SMB`.</span></span>|
|<span data-ttu-id="88150-207">windowsMalwareOverview</span><span class="sxs-lookup"><span data-stu-id="88150-207">windowsMalwareOverview</span></span>|[<span data-ttu-id="88150-208">windowsMalwareOverview</span><span class="sxs-lookup"><span data-stu-id="88150-208">windowsMalwareOverview</span></span>](../resources/intune-devices-windowsmalwareoverview.md)|<span data-ttu-id="88150-209">Windows デバイスのマルウェアの概要。</span><span class="sxs-lookup"><span data-stu-id="88150-209">Malware overview for windows devices.</span></span>|
|<span data-ttu-id="88150-210">**オンボーディング**</span><span class="sxs-lookup"><span data-stu-id="88150-210">**Onboarding**</span></span>|
|<span data-ttu-id="88150-211">intuneBrand</span><span class="sxs-lookup"><span data-stu-id="88150-211">intuneBrand</span></span>|[<span data-ttu-id="88150-212">intuneBrand</span><span class="sxs-lookup"><span data-stu-id="88150-212">intuneBrand</span></span>](../resources/intune-onboarding-intunebrand.md)|<span data-ttu-id="88150-213">intuneBrand には、会社のポータル アプリケーションとエンド ユーザーの Web ポータルの外観のカスタマイズに使用するデータが含まれています。</span><span class="sxs-lookup"><span data-stu-id="88150-213">intuneBrand contains data which is used in customizing the appearance of the Company Portal applications as well as the end user web portal.</span></span>|

<span data-ttu-id="88150-214">要求本文のプロパティのサポートは、ワークフローによって異なります。</span><span class="sxs-lookup"><span data-stu-id="88150-214">Request body property support varies according to workflow.</span></span>

## <a name="response"></a><span data-ttu-id="88150-215">応答</span><span class="sxs-lookup"><span data-stu-id="88150-215">Response</span></span>
<span data-ttu-id="88150-216">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で更新された [deviceManagement](../resources/intune-shared-devicemanagement.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="88150-216">If successful, this method returns a `200 OK` response code and an updated [deviceManagement](../resources/intune-shared-devicemanagement.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="88150-217">例</span><span class="sxs-lookup"><span data-stu-id="88150-217">Example</span></span>

### <a name="request"></a><span data-ttu-id="88150-218">要求</span><span class="sxs-lookup"><span data-stu-id="88150-218">Request</span></span>

<span data-ttu-id="88150-219">以下は、デバイス管理ワークフローの後の要求の例です。</span><span class="sxs-lookup"><span data-stu-id="88150-219">Here is an example of a request following the device management workflow:</span></span>

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

### <a name="response"></a><span data-ttu-id="88150-220">応答</span><span class="sxs-lookup"><span data-stu-id="88150-220">Response</span></span>

<span data-ttu-id="88150-221">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="88150-221">Here is an example of the response.</span></span> 

<span data-ttu-id="88150-222">注: 簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。</span><span class="sxs-lookup"><span data-stu-id="88150-222">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="88150-223">返されるプロパティは、ワークフローおよびコンテキストによって異なります。</span><span class="sxs-lookup"><span data-stu-id="88150-223">Returned properties vary according to workflow and context.</span></span>

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



