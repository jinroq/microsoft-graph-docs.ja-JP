---
title: deviceManagement の更新
description: deviceManagement オブジェクトのプロパティを更新します。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: e0dc83489ede464eb9da000acb8db4e6af13f8d2
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32527050"
---
# <a name="update-devicemanagement"></a><span data-ttu-id="12cb3-103">deviceManagement の更新</span><span class="sxs-lookup"><span data-stu-id="12cb3-103">Update deviceManagement</span></span>

> <span data-ttu-id="12cb3-104">**重要:** Microsoft Graph の/ベータ版の api は変更される可能性があります。</span><span class="sxs-lookup"><span data-stu-id="12cb3-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="12cb3-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="12cb3-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="12cb3-106">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="12cb3-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="12cb3-107">[deviceManagement](../resources/intune-shared-devicemanagement.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="12cb3-107">Update the properties of a [deviceManagement](../resources/intune-shared-devicemanagement.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="12cb3-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="12cb3-108">Prerequisites</span></span>

<span data-ttu-id="12cb3-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="12cb3-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="12cb3-111">アクセス許可は、ワークフローによって異なることに注意してください。</span><span class="sxs-lookup"><span data-stu-id="12cb3-111">Note that the permission vary according to workflow.</span></span>

| <span data-ttu-id="12cb3-112">アクセス&nbsp;許可&nbsp;の種類&nbsp;(ワークフロー別)</span><span class="sxs-lookup"><span data-stu-id="12cb3-112">Permission&nbsp;type&nbsp;(by&nbsp;workflow)</span></span> | <span data-ttu-id="12cb3-113">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="12cb3-113">Permissions (from most to least privileged)</span></span> |
|:---|:---|
| <span data-ttu-id="12cb3-114">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="12cb3-114">Delegated (work or school account)</span></span> ||
| <span data-ttu-id="12cb3-115">&nbsp;&nbsp; **Android for Work**</span><span class="sxs-lookup"><span data-stu-id="12cb3-115">&nbsp; &nbsp; **Android for Work**</span></span> | <span data-ttu-id="12cb3-116">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="12cb3-116">DeviceManagementConfiguration.ReadWrite.All</span></span>  |
| <span data-ttu-id="12cb3-117">&nbsp; &nbsp; **監査**</span><span class="sxs-lookup"><span data-stu-id="12cb3-117">&nbsp; &nbsp; **Auditing**</span></span> | <span data-ttu-id="12cb3-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="12cb3-118">DeviceManagementApps.ReadWrite.All</span></span> |
| <span data-ttu-id="12cb3-119">&nbsp; &nbsp; **会社の用語**</span><span class="sxs-lookup"><span data-stu-id="12cb3-119">&nbsp; &nbsp; **Company terms**</span></span> | <span data-ttu-id="12cb3-120">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="12cb3-120">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="12cb3-121">&nbsp; &nbsp; **デバイス構成**</span><span class="sxs-lookup"><span data-stu-id="12cb3-121">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="12cb3-122">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="12cb3-122">DeviceManagementConfiguration.ReadWrite.All</span></span> |
| <span data-ttu-id="12cb3-123">&nbsp;&nbsp; **デバイスの目的**</span><span class="sxs-lookup"><span data-stu-id="12cb3-123">&nbsp; &nbsp; **Device intent**</span></span> | <span data-ttu-id="12cb3-124">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="12cb3-124">DeviceManagementConfiguration.ReadWrite.All</span></span>|
| <span data-ttu-id="12cb3-125">&nbsp;&nbsp; **デバイスの管理**</span><span class="sxs-lookup"><span data-stu-id="12cb3-125">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="12cb3-126">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="12cb3-126">DeviceManagementManagedDevices.ReadWrite.All</span></span> |
| <span data-ttu-id="12cb3-127">&nbsp;&nbsp; **電子 SIM**</span><span class="sxs-lookup"><span data-stu-id="12cb3-127">&nbsp; &nbsp; **Electronic SIM**</span></span> | <span data-ttu-id="12cb3-128">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="12cb3-128">DeviceManagementConfiguration.ReadWrite.All</span></span> |
| <span data-ttu-id="12cb3-129">&nbsp;&nbsp; **登録**</span><span class="sxs-lookup"><span data-stu-id="12cb3-129">&nbsp; &nbsp; **Enrollment**</span></span> | <span data-ttu-id="12cb3-130">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="12cb3-130">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="12cb3-131">&nbsp;&nbsp; **フェンス**</span><span class="sxs-lookup"><span data-stu-id="12cb3-131">&nbsp; &nbsp; **Fencing**</span></span> | <span data-ttu-id="12cb3-132">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="12cb3-132">DeviceManagementConfiguration.ReadWrite.All</span></span> |
| <span data-ttu-id="12cb3-133">&nbsp;&nbsp; **通知**</span><span class="sxs-lookup"><span data-stu-id="12cb3-133">&nbsp; &nbsp; **Notification**</span></span> | <span data-ttu-id="12cb3-134">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="12cb3-134">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="12cb3-135">&nbsp; &nbsp; **オンボーディング**</span><span class="sxs-lookup"><span data-stu-id="12cb3-135">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="12cb3-136">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="12cb3-136">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="12cb3-137">&nbsp; &nbsp; **役割ベースのアクセス制御 (RBAC)**</span><span class="sxs-lookup"><span data-stu-id="12cb3-137">&nbsp; &nbsp; **Role-based access control (RBAC)**</span></span> | <span data-ttu-id="12cb3-138">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="12cb3-138">DeviceManagementRBAC.ReadWrite.All</span></span> |
| <span data-ttu-id="12cb3-139">&nbsp; &nbsp; **リモート アクセス**</span><span class="sxs-lookup"><span data-stu-id="12cb3-139">&nbsp; &nbsp; **Remote access**</span></span> | <span data-ttu-id="12cb3-140">DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="12cb3-140">DeviceManagementConfiguration.Read.All</span></span> |
| <span data-ttu-id="12cb3-141">&nbsp;&nbsp; **リモートアシスタンス**</span><span class="sxs-lookup"><span data-stu-id="12cb3-141">&nbsp; &nbsp; **Remote assistance**</span></span> | <span data-ttu-id="12cb3-142">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="12cb3-142">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="12cb3-143">&nbsp;&nbsp; **通信経費管理**</span><span class="sxs-lookup"><span data-stu-id="12cb3-143">&nbsp; &nbsp; **Telecom expense management**</span></span> | <span data-ttu-id="12cb3-144">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="12cb3-144">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="12cb3-145">&nbsp;&nbsp; **Troublehooting**</span><span class="sxs-lookup"><span data-stu-id="12cb3-145">&nbsp; &nbsp; **Troublehooting**</span></span> | <span data-ttu-id="12cb3-146">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="12cb3-146">DeviceManagementManagedDevices.ReadWrite.All</span></span> |
| <span data-ttu-id="12cb3-147">&nbsp; &nbsp; **Windows 情報保護**</span><span class="sxs-lookup"><span data-stu-id="12cb3-147">&nbsp; &nbsp; **Windows Information Protection**</span></span> | <span data-ttu-id="12cb3-148">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="12cb3-148">DeviceManagementApps.ReadWrite.All</span></span> |
| <span data-ttu-id="12cb3-149">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="12cb3-149">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="12cb3-150">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="12cb3-150">Not supported.</span></span>|
| <span data-ttu-id="12cb3-151">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="12cb3-151">Application</span></span> | <span data-ttu-id="12cb3-152">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="12cb3-152">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="12cb3-153">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="12cb3-153">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement
```

## <a name="request-headers"></a><span data-ttu-id="12cb3-154">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="12cb3-154">Request headers</span></span>

|<span data-ttu-id="12cb3-155">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="12cb3-155">Header</span></span>|<span data-ttu-id="12cb3-156">値</span><span class="sxs-lookup"><span data-stu-id="12cb3-156">Value</span></span>|
|:---|:---|
|<span data-ttu-id="12cb3-157">Authorization</span><span class="sxs-lookup"><span data-stu-id="12cb3-157">Authorization</span></span>|<span data-ttu-id="12cb3-158">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="12cb3-158">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="12cb3-159">承諾</span><span class="sxs-lookup"><span data-stu-id="12cb3-159">Accept</span></span>|<span data-ttu-id="12cb3-160">application/json</span><span class="sxs-lookup"><span data-stu-id="12cb3-160">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="12cb3-161">要求本文</span><span class="sxs-lookup"><span data-stu-id="12cb3-161">Request body</span></span>

<span data-ttu-id="12cb3-162">要求本文で、[deviceManagement](../resources/intune-shared-devicemanagement.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="12cb3-162">In the request body, supply a JSON representation for the [deviceManagement](../resources/intune-shared-devicemanagement.md) object.</span></span>

<span data-ttu-id="12cb3-163">次の表に、[deviceManagement](../resources/intune-shared-devicemanagement.md) の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="12cb3-163">The following table shows the properties that are required when you create the [deviceManagement](../resources/intune-shared-devicemanagement.md).</span></span>

|<span data-ttu-id="12cb3-164">プロパティ</span><span class="sxs-lookup"><span data-stu-id="12cb3-164">Property</span></span>|<span data-ttu-id="12cb3-165">型</span><span class="sxs-lookup"><span data-stu-id="12cb3-165">Type</span></span>|<span data-ttu-id="12cb3-166">説明</span><span class="sxs-lookup"><span data-stu-id="12cb3-166">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="12cb3-167">id</span><span class="sxs-lookup"><span data-stu-id="12cb3-167">id</span></span>|<span data-ttu-id="12cb3-168">String</span><span class="sxs-lookup"><span data-stu-id="12cb3-168">String</span></span>|<span data-ttu-id="12cb3-169">デバイスの一意識別子。</span><span class="sxs-lookup"><span data-stu-id="12cb3-169">Unique identifier for the device.</span></span>|
|<span data-ttu-id="12cb3-170">**デバイス構成**</span><span class="sxs-lookup"><span data-stu-id="12cb3-170">**Device configuration**</span></span>|
|<span data-ttu-id="12cb3-171">int未指定 eaccountid</span><span class="sxs-lookup"><span data-stu-id="12cb3-171">intuneAccountId</span></span>|<span data-ttu-id="12cb3-172">GUID</span><span class="sxs-lookup"><span data-stu-id="12cb3-172">GUID</span></span>|<span data-ttu-id="12cb3-173">指定したテナントの Intune アカウント ID</span><span class="sxs-lookup"><span data-stu-id="12cb3-173">Intune Account ID for given tenant</span></span>|
|<span data-ttu-id="12cb3-174">legacyPcManangementEnabled</span><span class="sxs-lookup"><span data-stu-id="12cb3-174">legacyPcManangementEnabled</span></span>|<span data-ttu-id="12cb3-175">ブール値</span><span class="sxs-lookup"><span data-stu-id="12cb3-175">Boolean</span></span>|<span data-ttu-id="12cb3-176">このアカウントの非 MDM で管理されているレガシー PC 管理を有効にするプロパティ。</span><span class="sxs-lookup"><span data-stu-id="12cb3-176">The property to enable Non-MDM managed legacy PC management for this account.</span></span> <span data-ttu-id="12cb3-177">このプロパティに値を設定するには、 SetExtrusionDirection メソッドを適用します。</span><span class="sxs-lookup"><span data-stu-id="12cb3-177">This property is read-only.</span></span>|
|<span data-ttu-id="12cb3-178">maximumdeptokens</span><span class="sxs-lookup"><span data-stu-id="12cb3-178">maximumDepTokens</span></span>|<span data-ttu-id="12cb3-179">Int32</span><span class="sxs-lookup"><span data-stu-id="12cb3-179">Int32</span></span>|<span data-ttu-id="12cb3-180">テナントごとに許容される DEP トークンの最大数。</span><span class="sxs-lookup"><span data-stu-id="12cb3-180">Maximum number of DEP tokens allowed per-tenant.</span></span>|
|<span data-ttu-id="12cb3-181">settings</span><span class="sxs-lookup"><span data-stu-id="12cb3-181">settings</span></span>|[<span data-ttu-id="12cb3-182">deviceManagementSettings</span><span class="sxs-lookup"><span data-stu-id="12cb3-182">deviceManagementSettings</span></span>](../resources/intune-deviceconfig-devicemanagementsettings.md)|<span data-ttu-id="12cb3-183">アカウント レベルの設定。</span><span class="sxs-lookup"><span data-stu-id="12cb3-183">Account level settings.</span></span>|
|<span data-ttu-id="12cb3-184">**デバイスの管理**</span><span class="sxs-lookup"><span data-stu-id="12cb3-184">**Device management**</span></span>|
|<span data-ttu-id="12cb3-185">accountMoveCompletionDateTime</span><span class="sxs-lookup"><span data-stu-id="12cb3-185">accountMoveCompletionDateTime</span></span>|<span data-ttu-id="12cb3-186">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="12cb3-186">DateTimeOffset</span></span>|<span data-ttu-id="12cb3-187">& が、scaleunits 間でテナントデータを移動した日時です。</span><span class="sxs-lookup"><span data-stu-id="12cb3-187">The date & time when tenant data moved between scaleunits.</span></span>|
|<span data-ttu-id="12cb3-188">adminConsent</span><span class="sxs-lookup"><span data-stu-id="12cb3-188">adminConsent</span></span>|[<span data-ttu-id="12cb3-189">adminConsent</span><span class="sxs-lookup"><span data-stu-id="12cb3-189">adminConsent</span></span>](../resources/intune-devices-adminconsent.md)|<span data-ttu-id="12cb3-190">管理者の同意情報。</span><span class="sxs-lookup"><span data-stu-id="12cb3-190">Admin consent information.</span></span>|
|<span data-ttu-id="12cb3-191">deviceProtectionOverview</span><span class="sxs-lookup"><span data-stu-id="12cb3-191">deviceProtectionOverview</span></span>|[<span data-ttu-id="12cb3-192">deviceProtectionOverview</span><span class="sxs-lookup"><span data-stu-id="12cb3-192">deviceProtectionOverview</span></span>](../resources/intune-devices-deviceprotectionoverview.md)|<span data-ttu-id="12cb3-193">デバイス保護の概要。</span><span class="sxs-lookup"><span data-stu-id="12cb3-193">Device protection overview.</span></span>|
|<span data-ttu-id="12cb3-194">managedDeviceCleanupSettings</span><span class="sxs-lookup"><span data-stu-id="12cb3-194">managedDeviceCleanupSettings</span></span>|[<span data-ttu-id="12cb3-195">managedDeviceCleanupSettings</span><span class="sxs-lookup"><span data-stu-id="12cb3-195">managedDeviceCleanupSettings</span></span>](../resources/intune-devices-manageddevicecleanupsettings.md)|<span data-ttu-id="12cb3-196">デバイスクリーンアップルール</span><span class="sxs-lookup"><span data-stu-id="12cb3-196">Device cleanup rule</span></span>|
|<span data-ttu-id="12cb3-197">subscriptionState</span><span class="sxs-lookup"><span data-stu-id="12cb3-197">subscriptionState</span></span>|[<span data-ttu-id="12cb3-198">devicemanagementsubscriptionstate</span><span class="sxs-lookup"><span data-stu-id="12cb3-198">deviceManagementSubscriptionState</span></span>](../resources/intune-devices-devicemanagementsubscriptionstate.md)|<span data-ttu-id="12cb3-199">テナントのモバイル デバイス管理のサブスクリプション状態。</span><span class="sxs-lookup"><span data-stu-id="12cb3-199">Tenant mobile device management subscription state.</span></span> <span data-ttu-id="12cb3-200">可能な値は、`pending`、`active`、`warning`、`disabled`、`deleted`、`blocked`、`lockedOut` です。</span><span class="sxs-lookup"><span data-stu-id="12cb3-200">Possible values are: `pending`, `active`, `warning`, `disabled`, `deleted`, `blocked`, `lockedOut`.</span></span>|
|<span data-ttu-id="12cb3-201">subscriptions</span><span class="sxs-lookup"><span data-stu-id="12cb3-201">subscriptions</span></span>|[<span data-ttu-id="12cb3-202">devicemanagementsubscriptions</span><span class="sxs-lookup"><span data-stu-id="12cb3-202">deviceManagementSubscriptions</span></span>](../resources/intune-devices-devicemanagementsubscriptions.md)|<span data-ttu-id="12cb3-203">テナントのサブスクリプション。</span><span class="sxs-lookup"><span data-stu-id="12cb3-203">Tenant's Subscription.</span></span> <span data-ttu-id="12cb3-204">可能な値は `none`、`intune`、`office365`、`intunePremium`、`intune_EDU`、`intune_SMB` です。</span><span class="sxs-lookup"><span data-stu-id="12cb3-204">Possible values are: `none`, `intune`, `office365`, `intunePremium`, `intune_EDU`, `intune_SMB`.</span></span>|
|<span data-ttu-id="12cb3-205">windowsMalwareOverview</span><span class="sxs-lookup"><span data-stu-id="12cb3-205">windowsMalwareOverview</span></span>|[<span data-ttu-id="12cb3-206">windowsMalwareOverview</span><span class="sxs-lookup"><span data-stu-id="12cb3-206">windowsMalwareOverview</span></span>](../resources/intune-devices-windowsmalwareoverview.md)|<span data-ttu-id="12cb3-207">windows デバイスのマルウェアの概要。</span><span class="sxs-lookup"><span data-stu-id="12cb3-207">Malware overview for windows devices.</span></span>|
|<span data-ttu-id="12cb3-208">**オンボーディング**</span><span class="sxs-lookup"><span data-stu-id="12cb3-208">**Onboarding**</span></span>|
|<span data-ttu-id="12cb3-209">intuneBrand</span><span class="sxs-lookup"><span data-stu-id="12cb3-209">intuneBrand</span></span>|[<span data-ttu-id="12cb3-210">intuneBrand</span><span class="sxs-lookup"><span data-stu-id="12cb3-210">intuneBrand</span></span>](../resources/intune-onboarding-intunebrand.md)|<span data-ttu-id="12cb3-211">intuneBrand には、会社のポータル アプリケーションとエンド ユーザーの Web ポータルの外観のカスタマイズに使用するデータが含まれています。</span><span class="sxs-lookup"><span data-stu-id="12cb3-211">intuneBrand contains data which is used in customizing the appearance of the Company Portal applications as well as the end user web portal.</span></span>|

<span data-ttu-id="12cb3-212">要求本文のプロパティのサポートは、ワークフローによって異なります。</span><span class="sxs-lookup"><span data-stu-id="12cb3-212">Request body property support varies according to workflow.</span></span>

## <a name="response"></a><span data-ttu-id="12cb3-213">応答</span><span class="sxs-lookup"><span data-stu-id="12cb3-213">Response</span></span>
<span data-ttu-id="12cb3-214">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で更新された [deviceManagement](../resources/intune-shared-devicemanagement.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="12cb3-214">If successful, this method returns a `200 OK` response code and an updated [deviceManagement](../resources/intune-shared-devicemanagement.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="12cb3-215">例</span><span class="sxs-lookup"><span data-stu-id="12cb3-215">Example</span></span>

### <a name="request"></a><span data-ttu-id="12cb3-216">要求</span><span class="sxs-lookup"><span data-stu-id="12cb3-216">Request</span></span>

<span data-ttu-id="12cb3-217">以下は、デバイス管理ワークフローの後の要求の例です。</span><span class="sxs-lookup"><span data-stu-id="12cb3-217">Here is an example of a request following the device management workflow:</span></span>

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

### <a name="response"></a><span data-ttu-id="12cb3-218">応答</span><span class="sxs-lookup"><span data-stu-id="12cb3-218">Response</span></span>

<span data-ttu-id="12cb3-219">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="12cb3-219">Here is an example of the response.</span></span> 

<span data-ttu-id="12cb3-220">注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。</span><span class="sxs-lookup"><span data-stu-id="12cb3-220">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="12cb3-221">返されるプロパティは、ワークフローおよびコンテキストによって異なります。</span><span class="sxs-lookup"><span data-stu-id="12cb3-221">Returned properties vary according to workflow and context.</span></span>

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



