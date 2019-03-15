---
title: deviceManagement の更新
description: deviceManagement オブジェクトのプロパティを更新します。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: a71212652d789b08a8cb496b6b98c18b12d3e9c7
ms.sourcegitcommit: 8eb88cfb48b0eb8f992570caebef577dfa2f30d3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/14/2019
ms.locfileid: "30571054"
---
# <a name="update-devicemanagement"></a><span data-ttu-id="78f81-103">deviceManagement の更新</span><span class="sxs-lookup"><span data-stu-id="78f81-103">Update deviceManagement</span></span>

> <span data-ttu-id="78f81-104">**重要:** Microsoft Graph の/ベータ版の api は変更される可能性があります。</span><span class="sxs-lookup"><span data-stu-id="78f81-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="78f81-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="78f81-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="78f81-106">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="78f81-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="78f81-107">[deviceManagement](../resources/intune-shared-devicemanagement.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="78f81-107">Update the properties of a [deviceManagement](../resources/intune-shared-devicemanagement.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="78f81-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="78f81-108">Prerequisites</span></span>

<span data-ttu-id="78f81-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/concepts/permissions-reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="78f81-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

<span data-ttu-id="78f81-111">アクセス許可は、ワークフローによって異なることに注意してください。</span><span class="sxs-lookup"><span data-stu-id="78f81-111">Note that the permission vary according to workflow.</span></span>

| <span data-ttu-id="78f81-112">アクセス&nbsp;許可&nbsp;の種類&nbsp;(ワークフロー別)</span><span class="sxs-lookup"><span data-stu-id="78f81-112">Permission&nbsp;type&nbsp;(by&nbsp;workflow)</span></span> | <span data-ttu-id="78f81-113">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="78f81-113">Permissions (from most to least privileged)</span></span> |
|:---|:---|
| <span data-ttu-id="78f81-114">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="78f81-114">Delegated (work or school account)</span></span> ||
| <span data-ttu-id="78f81-115">&nbsp;&nbsp; **Android for Work**</span><span class="sxs-lookup"><span data-stu-id="78f81-115">&nbsp; &nbsp; **Android for Work**</span></span> | <span data-ttu-id="78f81-116">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="78f81-116">DeviceManagementConfiguration.ReadWrite.All</span></span>  |
| <span data-ttu-id="78f81-117">&nbsp; &nbsp; **監査**</span><span class="sxs-lookup"><span data-stu-id="78f81-117">&nbsp; &nbsp; **Auditing**</span></span> | <span data-ttu-id="78f81-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="78f81-118">DeviceManagementApps.ReadWrite.All</span></span> |
| <span data-ttu-id="78f81-119">&nbsp; &nbsp; **会社の用語**</span><span class="sxs-lookup"><span data-stu-id="78f81-119">&nbsp; &nbsp; **Company terms**</span></span> | <span data-ttu-id="78f81-120">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="78f81-120">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="78f81-121">&nbsp; &nbsp; **デバイス構成**</span><span class="sxs-lookup"><span data-stu-id="78f81-121">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="78f81-122">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="78f81-122">DeviceManagementConfiguration.ReadWrite.All</span></span> |
| <span data-ttu-id="78f81-123">&nbsp; &nbsp; **デバイスの管理**</span><span class="sxs-lookup"><span data-stu-id="78f81-123">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="78f81-124">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="78f81-124">DeviceManagementManagedDevices.ReadWrite.All</span></span> |
| <span data-ttu-id="78f81-125">&nbsp;&nbsp; **電子 SIM**</span><span class="sxs-lookup"><span data-stu-id="78f81-125">&nbsp; &nbsp; **Electronic SIM**</span></span> | <span data-ttu-id="78f81-126">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="78f81-126">DeviceManagementConfiguration.ReadWrite.All</span></span> |
| <span data-ttu-id="78f81-127">&nbsp;&nbsp; **登録**</span><span class="sxs-lookup"><span data-stu-id="78f81-127">&nbsp; &nbsp; **Enrollment**</span></span> | <span data-ttu-id="78f81-128">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="78f81-128">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="78f81-129">&nbsp;&nbsp; **フェンス**</span><span class="sxs-lookup"><span data-stu-id="78f81-129">&nbsp; &nbsp; **Fencing**</span></span> | <span data-ttu-id="78f81-130">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="78f81-130">DeviceManagementConfiguration.ReadWrite.All</span></span> |
| <span data-ttu-id="78f81-131">&nbsp; &nbsp; **通知**</span><span class="sxs-lookup"><span data-stu-id="78f81-131">&nbsp; &nbsp; **Notification**</span></span> | <span data-ttu-id="78f81-132">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="78f81-132">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="78f81-133">&nbsp; &nbsp; **オンボーディング**</span><span class="sxs-lookup"><span data-stu-id="78f81-133">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="78f81-134">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="78f81-134">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="78f81-135">&nbsp; &nbsp; **役割ベースのアクセス制御 (RBAC)**</span><span class="sxs-lookup"><span data-stu-id="78f81-135">&nbsp; &nbsp; **Role-based access control (RBAC)**</span></span> | <span data-ttu-id="78f81-136">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="78f81-136">DeviceManagementRBAC.ReadWrite.All</span></span> |
| <span data-ttu-id="78f81-137">&nbsp; &nbsp; **リモート アクセス**</span><span class="sxs-lookup"><span data-stu-id="78f81-137">&nbsp; &nbsp; **Remote access**</span></span> | <span data-ttu-id="78f81-138">DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="78f81-138">DeviceManagementConfiguration.Read.All</span></span> |
| <span data-ttu-id="78f81-139">&nbsp;&nbsp; **リモートアシスタンス**</span><span class="sxs-lookup"><span data-stu-id="78f81-139">&nbsp; &nbsp; **Remote assistance**</span></span> | <span data-ttu-id="78f81-140">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="78f81-140">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="78f81-141">&nbsp;&nbsp; **通信経費管理**</span><span class="sxs-lookup"><span data-stu-id="78f81-141">&nbsp; &nbsp; **Telecom expense management**</span></span> | <span data-ttu-id="78f81-142">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="78f81-142">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="78f81-143">&nbsp;&nbsp; **Troublehooting**</span><span class="sxs-lookup"><span data-stu-id="78f81-143">&nbsp; &nbsp; **Troublehooting**</span></span> | <span data-ttu-id="78f81-144">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="78f81-144">DeviceManagementManagedDevices.ReadWrite.All</span></span> |
| <span data-ttu-id="78f81-145">&nbsp;&nbsp; **Windows 情報保護**</span><span class="sxs-lookup"><span data-stu-id="78f81-145">&nbsp; &nbsp; **Windows Information Protection**</span></span> | <span data-ttu-id="78f81-146">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="78f81-146">DeviceManagementApps.ReadWrite.All</span></span> |
| <span data-ttu-id="78f81-147">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="78f81-147">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="78f81-148">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="78f81-148">Not supported.</span></span>|
| <span data-ttu-id="78f81-149">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="78f81-149">Application</span></span> | <span data-ttu-id="78f81-150">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="78f81-150">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="78f81-151">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="78f81-151">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement
```

## <a name="request-headers"></a><span data-ttu-id="78f81-152">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="78f81-152">Request headers</span></span>

|<span data-ttu-id="78f81-153">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="78f81-153">Header</span></span>|<span data-ttu-id="78f81-154">値</span><span class="sxs-lookup"><span data-stu-id="78f81-154">Value</span></span>|
|:---|:---|
|<span data-ttu-id="78f81-155">Authorization</span><span class="sxs-lookup"><span data-stu-id="78f81-155">Authorization</span></span>|<span data-ttu-id="78f81-156">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="78f81-156">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="78f81-157">承諾</span><span class="sxs-lookup"><span data-stu-id="78f81-157">Accept</span></span>|<span data-ttu-id="78f81-158">application/json</span><span class="sxs-lookup"><span data-stu-id="78f81-158">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="78f81-159">要求本文</span><span class="sxs-lookup"><span data-stu-id="78f81-159">Request body</span></span>

<span data-ttu-id="78f81-160">要求本文で、[deviceManagement](../resources/intune-shared-devicemanagement.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="78f81-160">In the request body, supply a JSON representation for the [deviceManagement](../resources/intune-shared-devicemanagement.md) object.</span></span>

<span data-ttu-id="78f81-161">次の表に、[deviceManagement](../resources/intune-shared-devicemanagement.md) の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="78f81-161">The following table shows the properties that are required when you create the [deviceManagement](../resources/intune-shared-devicemanagement.md).</span></span>

|<span data-ttu-id="78f81-162">プロパティ</span><span class="sxs-lookup"><span data-stu-id="78f81-162">Property</span></span>|<span data-ttu-id="78f81-163">型</span><span class="sxs-lookup"><span data-stu-id="78f81-163">Type</span></span>|<span data-ttu-id="78f81-164">説明</span><span class="sxs-lookup"><span data-stu-id="78f81-164">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="78f81-165">id</span><span class="sxs-lookup"><span data-stu-id="78f81-165">id</span></span>|<span data-ttu-id="78f81-166">String</span><span class="sxs-lookup"><span data-stu-id="78f81-166">String</span></span>|<span data-ttu-id="78f81-167">デバイスの一意識別子。</span><span class="sxs-lookup"><span data-stu-id="78f81-167">Unique identifier for the device.</span></span>|
|<span data-ttu-id="78f81-168">**デバイス構成**</span><span class="sxs-lookup"><span data-stu-id="78f81-168">**Device configuration**</span></span>|
|<span data-ttu-id="78f81-169">int未指定 eaccountid</span><span class="sxs-lookup"><span data-stu-id="78f81-169">intuneAccountId</span></span>|<span data-ttu-id="78f81-170">GUID</span><span class="sxs-lookup"><span data-stu-id="78f81-170">GUID</span></span>|<span data-ttu-id="78f81-171">指定したテナントの Intune アカウント ID</span><span class="sxs-lookup"><span data-stu-id="78f81-171">Intune Account ID for given tenant</span></span>|
|<span data-ttu-id="78f81-172">legacyPcManangementEnabled</span><span class="sxs-lookup"><span data-stu-id="78f81-172">legacyPcManangementEnabled</span></span>|<span data-ttu-id="78f81-173">Boolean</span><span class="sxs-lookup"><span data-stu-id="78f81-173">Boolean</span></span>|<span data-ttu-id="78f81-174">このアカウントの非 MDM で管理されているレガシー PC 管理を有効にするプロパティ。</span><span class="sxs-lookup"><span data-stu-id="78f81-174">The property to enable Non-MDM managed legacy PC management for this account.</span></span> <span data-ttu-id="78f81-175">このプロパティに値を設定するには、 SetExtrusionDirection メソッドを適用します。</span><span class="sxs-lookup"><span data-stu-id="78f81-175">This property is read-only.</span></span>|
|<span data-ttu-id="78f81-176">maximumdeptokens</span><span class="sxs-lookup"><span data-stu-id="78f81-176">maximumDepTokens</span></span>|<span data-ttu-id="78f81-177">Int32</span><span class="sxs-lookup"><span data-stu-id="78f81-177">Int32</span></span>|<span data-ttu-id="78f81-178">テナントごとに許容される DEP トークンの最大数。</span><span class="sxs-lookup"><span data-stu-id="78f81-178">Maximum number of DEP tokens allowed per-tenant.</span></span>|
|<span data-ttu-id="78f81-179">settings</span><span class="sxs-lookup"><span data-stu-id="78f81-179">settings</span></span>|[<span data-ttu-id="78f81-180">deviceManagementSettings</span><span class="sxs-lookup"><span data-stu-id="78f81-180">deviceManagementSettings</span></span>](../resources/intune-deviceconfig-devicemanagementsettings.md)|<span data-ttu-id="78f81-181">アカウント レベルの設定。</span><span class="sxs-lookup"><span data-stu-id="78f81-181">Account level settings.</span></span>|
|<span data-ttu-id="78f81-182">**デバイスの管理**</span><span class="sxs-lookup"><span data-stu-id="78f81-182">**Device management**</span></span>|
|<span data-ttu-id="78f81-183">accountMoveCompletionDateTime</span><span class="sxs-lookup"><span data-stu-id="78f81-183">accountMoveCompletionDateTime</span></span>|<span data-ttu-id="78f81-184">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="78f81-184">DateTimeOffset</span></span>|<span data-ttu-id="78f81-185">& が、scaleunits 間でテナントデータを移動した日時です。</span><span class="sxs-lookup"><span data-stu-id="78f81-185">The date & time when tenant data moved between scaleunits.</span></span>|
|<span data-ttu-id="78f81-186">adminConsent</span><span class="sxs-lookup"><span data-stu-id="78f81-186">adminConsent</span></span>|[<span data-ttu-id="78f81-187">adminConsent</span><span class="sxs-lookup"><span data-stu-id="78f81-187">adminConsent</span></span>](../resources/intune-devices-adminconsent.md)|<span data-ttu-id="78f81-188">管理者の同意情報。</span><span class="sxs-lookup"><span data-stu-id="78f81-188">Admin consent information.</span></span>|
|<span data-ttu-id="78f81-189">deviceProtectionOverview</span><span class="sxs-lookup"><span data-stu-id="78f81-189">deviceProtectionOverview</span></span>|[<span data-ttu-id="78f81-190">deviceProtectionOverview</span><span class="sxs-lookup"><span data-stu-id="78f81-190">deviceProtectionOverview</span></span>](../resources/intune-devices-deviceprotectionoverview.md)|<span data-ttu-id="78f81-191">デバイス保護の概要。</span><span class="sxs-lookup"><span data-stu-id="78f81-191">Device protection overview.</span></span>|
|<span data-ttu-id="78f81-192">managedDeviceCleanupSettings</span><span class="sxs-lookup"><span data-stu-id="78f81-192">managedDeviceCleanupSettings</span></span>|[<span data-ttu-id="78f81-193">managedDeviceCleanupSettings</span><span class="sxs-lookup"><span data-stu-id="78f81-193">managedDeviceCleanupSettings</span></span>](../resources/intune-devices-manageddevicecleanupsettings.md)|<span data-ttu-id="78f81-194">デバイスクリーンアップルール</span><span class="sxs-lookup"><span data-stu-id="78f81-194">Device cleanup rule</span></span>|
|<span data-ttu-id="78f81-195">subscriptionState</span><span class="sxs-lookup"><span data-stu-id="78f81-195">subscriptionState</span></span>|[<span data-ttu-id="78f81-196">devicemanagementsubscriptionstate</span><span class="sxs-lookup"><span data-stu-id="78f81-196">deviceManagementSubscriptionState</span></span>](../resources/intune-devices-devicemanagementsubscriptionstate.md)|<span data-ttu-id="78f81-197">テナントのモバイル デバイス管理のサブスクリプション状態。</span><span class="sxs-lookup"><span data-stu-id="78f81-197">Tenant mobile device management subscription state.</span></span> <span data-ttu-id="78f81-198">可能な値は、`pending`、`active`、`warning`、`disabled`、`deleted`、`blocked`、`lockedOut` です。</span><span class="sxs-lookup"><span data-stu-id="78f81-198">Possible values are: `pending`, `active`, `warning`, `disabled`, `deleted`, `blocked`, `lockedOut`.</span></span>|
|<span data-ttu-id="78f81-199">講読</span><span class="sxs-lookup"><span data-stu-id="78f81-199">subscriptions</span></span>|[<span data-ttu-id="78f81-200">devicemanagementsubscriptions</span><span class="sxs-lookup"><span data-stu-id="78f81-200">deviceManagementSubscriptions</span></span>](../resources/intune-devices-devicemanagementsubscriptions.md)|<span data-ttu-id="78f81-201">テナントのサブスクリプション。</span><span class="sxs-lookup"><span data-stu-id="78f81-201">Tenant's Subscription.</span></span> <span data-ttu-id="78f81-202">可能な値は `none`、`intune`、`office365`、`intunePremium`、`intune_EDU`、`intune_SMB` です。</span><span class="sxs-lookup"><span data-stu-id="78f81-202">Possible values are: `none`, `intune`, `office365`, `intunePremium`, `intune_EDU`, `intune_SMB`.</span></span>|
|<span data-ttu-id="78f81-203">windowsMalwareOverview</span><span class="sxs-lookup"><span data-stu-id="78f81-203">windowsMalwareOverview</span></span>|[<span data-ttu-id="78f81-204">windowsMalwareOverview</span><span class="sxs-lookup"><span data-stu-id="78f81-204">windowsMalwareOverview</span></span>](../resources/intune-devices-windowsmalwareoverview.md)|<span data-ttu-id="78f81-205">windows デバイスのマルウェアの概要。</span><span class="sxs-lookup"><span data-stu-id="78f81-205">Malware overview for windows devices.</span></span>|
|<span data-ttu-id="78f81-206">**オンボーディング**</span><span class="sxs-lookup"><span data-stu-id="78f81-206">**Onboarding**</span></span>|
|<span data-ttu-id="78f81-207">intuneBrand</span><span class="sxs-lookup"><span data-stu-id="78f81-207">intuneBrand</span></span>|[<span data-ttu-id="78f81-208">intuneBrand</span><span class="sxs-lookup"><span data-stu-id="78f81-208">intuneBrand</span></span>](../resources/intune-onboarding-intunebrand.md)|<span data-ttu-id="78f81-209">intuneBrand には、会社のポータル アプリケーションとエンド ユーザーの Web ポータルの外観のカスタマイズに使用するデータが含まれています。</span><span class="sxs-lookup"><span data-stu-id="78f81-209">intuneBrand contains data which is used in customizing the appearance of the Company Portal applications as well as the end user web portal.</span></span>|

<span data-ttu-id="78f81-210">要求本文のプロパティのサポートは、ワークフローによって異なります。</span><span class="sxs-lookup"><span data-stu-id="78f81-210">Request body property support varies according to workflow.</span></span>

## <a name="response"></a><span data-ttu-id="78f81-211">応答</span><span class="sxs-lookup"><span data-stu-id="78f81-211">Response</span></span>
<span data-ttu-id="78f81-212">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で更新された [deviceManagement](../resources/intune-shared-devicemanagement.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="78f81-212">If successful, this method returns a `200 OK` response code and an updated [deviceManagement](../resources/intune-shared-devicemanagement.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="78f81-213">例</span><span class="sxs-lookup"><span data-stu-id="78f81-213">Example</span></span>

### <a name="request"></a><span data-ttu-id="78f81-214">要求</span><span class="sxs-lookup"><span data-stu-id="78f81-214">Request</span></span>

<span data-ttu-id="78f81-215">以下は、デバイス管理ワークフローの後の要求の例です。</span><span class="sxs-lookup"><span data-stu-id="78f81-215">Here is an example of a request following the device management workflow:</span></span>

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

### <a name="response"></a><span data-ttu-id="78f81-216">応答</span><span class="sxs-lookup"><span data-stu-id="78f81-216">Response</span></span>

<span data-ttu-id="78f81-217">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="78f81-217">Here is an example of the response.</span></span> 

<span data-ttu-id="78f81-218">注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。</span><span class="sxs-lookup"><span data-stu-id="78f81-218">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="78f81-219">返されるプロパティは、ワークフローおよびコンテキストによって異なります。</span><span class="sxs-lookup"><span data-stu-id="78f81-219">Returned properties vary according to workflow and context.</span></span>

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



