---
title: deviceManagement の更新
description: deviceManagement オブジェクトのプロパティを更新します。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: f4ef1c7eb4711afd2aa29071f160f440dceefba3
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/29/2019
ms.locfileid: "30960406"
---
# <a name="update-devicemanagement"></a><span data-ttu-id="126da-103">deviceManagement の更新</span><span class="sxs-lookup"><span data-stu-id="126da-103">Update deviceManagement</span></span>

> <span data-ttu-id="126da-104">**重要:** Microsoft Graph の/ベータ版の api は変更される可能性があります。</span><span class="sxs-lookup"><span data-stu-id="126da-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="126da-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="126da-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="126da-106">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="126da-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="126da-107">[deviceManagement](../resources/intune-shared-devicemanagement.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="126da-107">Update the properties of a [deviceManagement](../resources/intune-shared-devicemanagement.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="126da-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="126da-108">Prerequisites</span></span>

<span data-ttu-id="126da-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="126da-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="126da-111">アクセス許可は、ワークフローによって異なることに注意してください。</span><span class="sxs-lookup"><span data-stu-id="126da-111">Note that the permission vary according to workflow.</span></span>

| <span data-ttu-id="126da-112">アクセス&nbsp;許可&nbsp;の種類&nbsp;(ワークフロー別)</span><span class="sxs-lookup"><span data-stu-id="126da-112">Permission&nbsp;type&nbsp;(by&nbsp;workflow)</span></span> | <span data-ttu-id="126da-113">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="126da-113">Permissions (from most to least privileged)</span></span> |
|:---|:---|
| <span data-ttu-id="126da-114">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="126da-114">Delegated (work or school account)</span></span> ||
| <span data-ttu-id="126da-115">&nbsp;&nbsp; **Android for Work**</span><span class="sxs-lookup"><span data-stu-id="126da-115">&nbsp; &nbsp; **Android for Work**</span></span> | <span data-ttu-id="126da-116">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="126da-116">DeviceManagementConfiguration.ReadWrite.All</span></span>  |
| <span data-ttu-id="126da-117">&nbsp; &nbsp; **監査**</span><span class="sxs-lookup"><span data-stu-id="126da-117">&nbsp; &nbsp; **Auditing**</span></span> | <span data-ttu-id="126da-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="126da-118">DeviceManagementApps.ReadWrite.All</span></span> |
| <span data-ttu-id="126da-119">&nbsp; &nbsp; **会社の用語**</span><span class="sxs-lookup"><span data-stu-id="126da-119">&nbsp; &nbsp; **Company terms**</span></span> | <span data-ttu-id="126da-120">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="126da-120">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="126da-121">&nbsp; &nbsp; **デバイス構成**</span><span class="sxs-lookup"><span data-stu-id="126da-121">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="126da-122">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="126da-122">DeviceManagementConfiguration.ReadWrite.All</span></span> |
| <span data-ttu-id="126da-123">&nbsp; &nbsp; **デバイスの管理**</span><span class="sxs-lookup"><span data-stu-id="126da-123">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="126da-124">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="126da-124">DeviceManagementManagedDevices.ReadWrite.All</span></span> |
| <span data-ttu-id="126da-125">&nbsp;&nbsp; **電子 SIM**</span><span class="sxs-lookup"><span data-stu-id="126da-125">&nbsp; &nbsp; **Electronic SIM**</span></span> | <span data-ttu-id="126da-126">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="126da-126">DeviceManagementConfiguration.ReadWrite.All</span></span> |
| <span data-ttu-id="126da-127">&nbsp;&nbsp; **登録**</span><span class="sxs-lookup"><span data-stu-id="126da-127">&nbsp; &nbsp; **Enrollment**</span></span> | <span data-ttu-id="126da-128">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="126da-128">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="126da-129">&nbsp;&nbsp; **フェンス**</span><span class="sxs-lookup"><span data-stu-id="126da-129">&nbsp; &nbsp; **Fencing**</span></span> | <span data-ttu-id="126da-130">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="126da-130">DeviceManagementConfiguration.ReadWrite.All</span></span> |
| <span data-ttu-id="126da-131">&nbsp; &nbsp; **通知**</span><span class="sxs-lookup"><span data-stu-id="126da-131">&nbsp; &nbsp; **Notification**</span></span> | <span data-ttu-id="126da-132">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="126da-132">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="126da-133">&nbsp; &nbsp; **オンボーディング**</span><span class="sxs-lookup"><span data-stu-id="126da-133">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="126da-134">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="126da-134">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="126da-135">&nbsp; &nbsp; **役割ベースのアクセス制御 (RBAC)**</span><span class="sxs-lookup"><span data-stu-id="126da-135">&nbsp; &nbsp; **Role-based access control (RBAC)**</span></span> | <span data-ttu-id="126da-136">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="126da-136">DeviceManagementRBAC.ReadWrite.All</span></span> |
| <span data-ttu-id="126da-137">&nbsp; &nbsp; **リモート アクセス**</span><span class="sxs-lookup"><span data-stu-id="126da-137">&nbsp; &nbsp; **Remote access**</span></span> | <span data-ttu-id="126da-138">DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="126da-138">DeviceManagementConfiguration.Read.All</span></span> |
| <span data-ttu-id="126da-139">&nbsp;&nbsp; **リモートアシスタンス**</span><span class="sxs-lookup"><span data-stu-id="126da-139">&nbsp; &nbsp; **Remote assistance**</span></span> | <span data-ttu-id="126da-140">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="126da-140">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="126da-141">&nbsp;&nbsp; **通信経費管理**</span><span class="sxs-lookup"><span data-stu-id="126da-141">&nbsp; &nbsp; **Telecom expense management**</span></span> | <span data-ttu-id="126da-142">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="126da-142">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="126da-143">&nbsp;&nbsp; **Troublehooting**</span><span class="sxs-lookup"><span data-stu-id="126da-143">&nbsp; &nbsp; **Troublehooting**</span></span> | <span data-ttu-id="126da-144">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="126da-144">DeviceManagementManagedDevices.ReadWrite.All</span></span> |
| <span data-ttu-id="126da-145">&nbsp;&nbsp; **Windows 情報保護**</span><span class="sxs-lookup"><span data-stu-id="126da-145">&nbsp; &nbsp; **Windows Information Protection**</span></span> | <span data-ttu-id="126da-146">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="126da-146">DeviceManagementApps.ReadWrite.All</span></span> |
| <span data-ttu-id="126da-147">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="126da-147">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="126da-148">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="126da-148">Not supported.</span></span>|
| <span data-ttu-id="126da-149">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="126da-149">Application</span></span> | <span data-ttu-id="126da-150">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="126da-150">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="126da-151">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="126da-151">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement
```

## <a name="request-headers"></a><span data-ttu-id="126da-152">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="126da-152">Request headers</span></span>

|<span data-ttu-id="126da-153">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="126da-153">Header</span></span>|<span data-ttu-id="126da-154">値</span><span class="sxs-lookup"><span data-stu-id="126da-154">Value</span></span>|
|:---|:---|
|<span data-ttu-id="126da-155">Authorization</span><span class="sxs-lookup"><span data-stu-id="126da-155">Authorization</span></span>|<span data-ttu-id="126da-156">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="126da-156">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="126da-157">承諾</span><span class="sxs-lookup"><span data-stu-id="126da-157">Accept</span></span>|<span data-ttu-id="126da-158">application/json</span><span class="sxs-lookup"><span data-stu-id="126da-158">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="126da-159">要求本文</span><span class="sxs-lookup"><span data-stu-id="126da-159">Request body</span></span>

<span data-ttu-id="126da-160">要求本文で、[deviceManagement](../resources/intune-shared-devicemanagement.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="126da-160">In the request body, supply a JSON representation for the [deviceManagement](../resources/intune-shared-devicemanagement.md) object.</span></span>

<span data-ttu-id="126da-161">次の表に、[deviceManagement](../resources/intune-shared-devicemanagement.md) の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="126da-161">The following table shows the properties that are required when you create the [deviceManagement](../resources/intune-shared-devicemanagement.md).</span></span>

|<span data-ttu-id="126da-162">プロパティ</span><span class="sxs-lookup"><span data-stu-id="126da-162">Property</span></span>|<span data-ttu-id="126da-163">型</span><span class="sxs-lookup"><span data-stu-id="126da-163">Type</span></span>|<span data-ttu-id="126da-164">説明</span><span class="sxs-lookup"><span data-stu-id="126da-164">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="126da-165">id</span><span class="sxs-lookup"><span data-stu-id="126da-165">id</span></span>|<span data-ttu-id="126da-166">String</span><span class="sxs-lookup"><span data-stu-id="126da-166">String</span></span>|<span data-ttu-id="126da-167">デバイスの一意識別子。</span><span class="sxs-lookup"><span data-stu-id="126da-167">Unique identifier for the device.</span></span>|
|<span data-ttu-id="126da-168">**デバイス構成**</span><span class="sxs-lookup"><span data-stu-id="126da-168">**Device configuration**</span></span>|
|<span data-ttu-id="126da-169">int未指定 eaccountid</span><span class="sxs-lookup"><span data-stu-id="126da-169">intuneAccountId</span></span>|<span data-ttu-id="126da-170">GUID</span><span class="sxs-lookup"><span data-stu-id="126da-170">GUID</span></span>|<span data-ttu-id="126da-171">指定したテナントの Intune アカウント ID</span><span class="sxs-lookup"><span data-stu-id="126da-171">Intune Account ID for given tenant</span></span>|
|<span data-ttu-id="126da-172">legacyPcManangementEnabled</span><span class="sxs-lookup"><span data-stu-id="126da-172">legacyPcManangementEnabled</span></span>|<span data-ttu-id="126da-173">Boolean</span><span class="sxs-lookup"><span data-stu-id="126da-173">Boolean</span></span>|<span data-ttu-id="126da-174">このアカウントの非 MDM で管理されているレガシー PC 管理を有効にするプロパティ。</span><span class="sxs-lookup"><span data-stu-id="126da-174">The property to enable Non-MDM managed legacy PC management for this account.</span></span> <span data-ttu-id="126da-175">このプロパティに値を設定するには、 SetExtrusionDirection メソッドを適用します。</span><span class="sxs-lookup"><span data-stu-id="126da-175">This property is read-only.</span></span>|
|<span data-ttu-id="126da-176">maximumdeptokens</span><span class="sxs-lookup"><span data-stu-id="126da-176">maximumDepTokens</span></span>|<span data-ttu-id="126da-177">Int32</span><span class="sxs-lookup"><span data-stu-id="126da-177">Int32</span></span>|<span data-ttu-id="126da-178">テナントごとに許容される DEP トークンの最大数。</span><span class="sxs-lookup"><span data-stu-id="126da-178">Maximum number of DEP tokens allowed per-tenant.</span></span>|
|<span data-ttu-id="126da-179">settings</span><span class="sxs-lookup"><span data-stu-id="126da-179">settings</span></span>|[<span data-ttu-id="126da-180">deviceManagementSettings</span><span class="sxs-lookup"><span data-stu-id="126da-180">deviceManagementSettings</span></span>](../resources/intune-deviceconfig-devicemanagementsettings.md)|<span data-ttu-id="126da-181">アカウント レベルの設定。</span><span class="sxs-lookup"><span data-stu-id="126da-181">Account level settings.</span></span>|
|<span data-ttu-id="126da-182">**デバイスの管理**</span><span class="sxs-lookup"><span data-stu-id="126da-182">**Device management**</span></span>|
|<span data-ttu-id="126da-183">accountMoveCompletionDateTime</span><span class="sxs-lookup"><span data-stu-id="126da-183">accountMoveCompletionDateTime</span></span>|<span data-ttu-id="126da-184">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="126da-184">DateTimeOffset</span></span>|<span data-ttu-id="126da-185">& が、scaleunits 間でテナントデータを移動した日時です。</span><span class="sxs-lookup"><span data-stu-id="126da-185">The date & time when tenant data moved between scaleunits.</span></span>|
|<span data-ttu-id="126da-186">adminConsent</span><span class="sxs-lookup"><span data-stu-id="126da-186">adminConsent</span></span>|[<span data-ttu-id="126da-187">adminConsent</span><span class="sxs-lookup"><span data-stu-id="126da-187">adminConsent</span></span>](../resources/intune-devices-adminconsent.md)|<span data-ttu-id="126da-188">管理者の同意情報。</span><span class="sxs-lookup"><span data-stu-id="126da-188">Admin consent information.</span></span>|
|<span data-ttu-id="126da-189">deviceProtectionOverview</span><span class="sxs-lookup"><span data-stu-id="126da-189">deviceProtectionOverview</span></span>|[<span data-ttu-id="126da-190">deviceProtectionOverview</span><span class="sxs-lookup"><span data-stu-id="126da-190">deviceProtectionOverview</span></span>](../resources/intune-devices-deviceprotectionoverview.md)|<span data-ttu-id="126da-191">デバイス保護の概要。</span><span class="sxs-lookup"><span data-stu-id="126da-191">Device protection overview.</span></span>|
|<span data-ttu-id="126da-192">managedDeviceCleanupSettings</span><span class="sxs-lookup"><span data-stu-id="126da-192">managedDeviceCleanupSettings</span></span>|[<span data-ttu-id="126da-193">managedDeviceCleanupSettings</span><span class="sxs-lookup"><span data-stu-id="126da-193">managedDeviceCleanupSettings</span></span>](../resources/intune-devices-manageddevicecleanupsettings.md)|<span data-ttu-id="126da-194">デバイスクリーンアップルール</span><span class="sxs-lookup"><span data-stu-id="126da-194">Device cleanup rule</span></span>|
|<span data-ttu-id="126da-195">subscriptionState</span><span class="sxs-lookup"><span data-stu-id="126da-195">subscriptionState</span></span>|[<span data-ttu-id="126da-196">devicemanagementsubscriptionstate</span><span class="sxs-lookup"><span data-stu-id="126da-196">deviceManagementSubscriptionState</span></span>](../resources/intune-devices-devicemanagementsubscriptionstate.md)|<span data-ttu-id="126da-197">テナントのモバイル デバイス管理のサブスクリプション状態。</span><span class="sxs-lookup"><span data-stu-id="126da-197">Tenant mobile device management subscription state.</span></span> <span data-ttu-id="126da-198">可能な値は、`pending`、`active`、`warning`、`disabled`、`deleted`、`blocked`、`lockedOut` です。</span><span class="sxs-lookup"><span data-stu-id="126da-198">Possible values are: `pending`, `active`, `warning`, `disabled`, `deleted`, `blocked`, `lockedOut`.</span></span>|
|<span data-ttu-id="126da-199">subscriptions</span><span class="sxs-lookup"><span data-stu-id="126da-199">subscriptions</span></span>|[<span data-ttu-id="126da-200">devicemanagementsubscriptions</span><span class="sxs-lookup"><span data-stu-id="126da-200">deviceManagementSubscriptions</span></span>](../resources/intune-devices-devicemanagementsubscriptions.md)|<span data-ttu-id="126da-201">テナントのサブスクリプション。</span><span class="sxs-lookup"><span data-stu-id="126da-201">Tenant's Subscription.</span></span> <span data-ttu-id="126da-202">可能な値は `none`、`intune`、`office365`、`intunePremium`、`intune_EDU`、`intune_SMB` です。</span><span class="sxs-lookup"><span data-stu-id="126da-202">Possible values are: `none`, `intune`, `office365`, `intunePremium`, `intune_EDU`, `intune_SMB`.</span></span>|
|<span data-ttu-id="126da-203">windowsMalwareOverview</span><span class="sxs-lookup"><span data-stu-id="126da-203">windowsMalwareOverview</span></span>|[<span data-ttu-id="126da-204">windowsMalwareOverview</span><span class="sxs-lookup"><span data-stu-id="126da-204">windowsMalwareOverview</span></span>](../resources/intune-devices-windowsmalwareoverview.md)|<span data-ttu-id="126da-205">windows デバイスのマルウェアの概要。</span><span class="sxs-lookup"><span data-stu-id="126da-205">Malware overview for windows devices.</span></span>|
|<span data-ttu-id="126da-206">**オンボーディング**</span><span class="sxs-lookup"><span data-stu-id="126da-206">**Onboarding**</span></span>|
|<span data-ttu-id="126da-207">intuneBrand</span><span class="sxs-lookup"><span data-stu-id="126da-207">intuneBrand</span></span>|[<span data-ttu-id="126da-208">intuneBrand</span><span class="sxs-lookup"><span data-stu-id="126da-208">intuneBrand</span></span>](../resources/intune-onboarding-intunebrand.md)|<span data-ttu-id="126da-209">intuneBrand には、会社のポータル アプリケーションとエンド ユーザーの Web ポータルの外観のカスタマイズに使用するデータが含まれています。</span><span class="sxs-lookup"><span data-stu-id="126da-209">intuneBrand contains data which is used in customizing the appearance of the Company Portal applications as well as the end user web portal.</span></span>|

<span data-ttu-id="126da-210">要求本文のプロパティのサポートは、ワークフローによって異なります。</span><span class="sxs-lookup"><span data-stu-id="126da-210">Request body property support varies according to workflow.</span></span>

## <a name="response"></a><span data-ttu-id="126da-211">応答</span><span class="sxs-lookup"><span data-stu-id="126da-211">Response</span></span>
<span data-ttu-id="126da-212">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で更新された [deviceManagement](../resources/intune-shared-devicemanagement.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="126da-212">If successful, this method returns a `200 OK` response code and an updated [deviceManagement](../resources/intune-shared-devicemanagement.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="126da-213">例</span><span class="sxs-lookup"><span data-stu-id="126da-213">Example</span></span>

### <a name="request"></a><span data-ttu-id="126da-214">要求</span><span class="sxs-lookup"><span data-stu-id="126da-214">Request</span></span>

<span data-ttu-id="126da-215">以下は、デバイス管理ワークフローの後の要求の例です。</span><span class="sxs-lookup"><span data-stu-id="126da-215">Here is an example of a request following the device management workflow:</span></span>

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

### <a name="response"></a><span data-ttu-id="126da-216">応答</span><span class="sxs-lookup"><span data-stu-id="126da-216">Response</span></span>

<span data-ttu-id="126da-217">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="126da-217">Here is an example of the response.</span></span> 

<span data-ttu-id="126da-218">注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。</span><span class="sxs-lookup"><span data-stu-id="126da-218">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="126da-219">返されるプロパティは、ワークフローおよびコンテキストによって異なります。</span><span class="sxs-lookup"><span data-stu-id="126da-219">Returned properties vary according to workflow and context.</span></span>

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



