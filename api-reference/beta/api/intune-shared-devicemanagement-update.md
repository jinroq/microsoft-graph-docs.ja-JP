---
title: deviceManagement の更新
description: deviceManagement オブジェクトのプロパティを更新します。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: e0dc83489ede464eb9da000acb8db4e6af13f8d2
ms.sourcegitcommit: 77f485ec03a8c917f59d2fbed4df1ec755f3da58
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/08/2019
ms.locfileid: "31518526"
---
# <a name="update-devicemanagement"></a><span data-ttu-id="68cb2-103">deviceManagement の更新</span><span class="sxs-lookup"><span data-stu-id="68cb2-103">Update deviceManagement</span></span>

> <span data-ttu-id="68cb2-104">**重要:** Microsoft Graph の/ベータ版の api は変更される可能性があります。</span><span class="sxs-lookup"><span data-stu-id="68cb2-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="68cb2-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="68cb2-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="68cb2-106">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="68cb2-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="68cb2-107">[deviceManagement](../resources/intune-shared-devicemanagement.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="68cb2-107">Update the properties of a [deviceManagement](../resources/intune-shared-devicemanagement.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="68cb2-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="68cb2-108">Prerequisites</span></span>

<span data-ttu-id="68cb2-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="68cb2-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="68cb2-111">アクセス許可は、ワークフローによって異なることに注意してください。</span><span class="sxs-lookup"><span data-stu-id="68cb2-111">Note that the permission vary according to workflow.</span></span>

| <span data-ttu-id="68cb2-112">アクセス&nbsp;許可&nbsp;の種類&nbsp;(ワークフロー別)</span><span class="sxs-lookup"><span data-stu-id="68cb2-112">Permission&nbsp;type&nbsp;(by&nbsp;workflow)</span></span> | <span data-ttu-id="68cb2-113">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="68cb2-113">Permissions (from most to least privileged)</span></span> |
|:---|:---|
| <span data-ttu-id="68cb2-114">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="68cb2-114">Delegated (work or school account)</span></span> ||
| <span data-ttu-id="68cb2-115">&nbsp;&nbsp; **Android for Work**</span><span class="sxs-lookup"><span data-stu-id="68cb2-115">&nbsp; &nbsp; **Android for Work**</span></span> | <span data-ttu-id="68cb2-116">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="68cb2-116">DeviceManagementConfiguration.ReadWrite.All</span></span>  |
| <span data-ttu-id="68cb2-117">&nbsp; &nbsp; **監査**</span><span class="sxs-lookup"><span data-stu-id="68cb2-117">&nbsp; &nbsp; **Auditing**</span></span> | <span data-ttu-id="68cb2-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="68cb2-118">DeviceManagementApps.ReadWrite.All</span></span> |
| <span data-ttu-id="68cb2-119">&nbsp; &nbsp; **会社の用語**</span><span class="sxs-lookup"><span data-stu-id="68cb2-119">&nbsp; &nbsp; **Company terms**</span></span> | <span data-ttu-id="68cb2-120">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="68cb2-120">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="68cb2-121">&nbsp; &nbsp; **デバイス構成**</span><span class="sxs-lookup"><span data-stu-id="68cb2-121">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="68cb2-122">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="68cb2-122">DeviceManagementConfiguration.ReadWrite.All</span></span> |
| <span data-ttu-id="68cb2-123">&nbsp;&nbsp; **デバイスの目的**</span><span class="sxs-lookup"><span data-stu-id="68cb2-123">&nbsp; &nbsp; **Device intent**</span></span> | <span data-ttu-id="68cb2-124">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="68cb2-124">DeviceManagementConfiguration.ReadWrite.All</span></span>|
| <span data-ttu-id="68cb2-125">&nbsp; &nbsp; **デバイスの管理**</span><span class="sxs-lookup"><span data-stu-id="68cb2-125">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="68cb2-126">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="68cb2-126">DeviceManagementManagedDevices.ReadWrite.All</span></span> |
| <span data-ttu-id="68cb2-127">&nbsp;&nbsp; **電子 SIM**</span><span class="sxs-lookup"><span data-stu-id="68cb2-127">&nbsp; &nbsp; **Electronic SIM**</span></span> | <span data-ttu-id="68cb2-128">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="68cb2-128">DeviceManagementConfiguration.ReadWrite.All</span></span> |
| <span data-ttu-id="68cb2-129">&nbsp;&nbsp; **登録**</span><span class="sxs-lookup"><span data-stu-id="68cb2-129">&nbsp; &nbsp; **Enrollment**</span></span> | <span data-ttu-id="68cb2-130">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="68cb2-130">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="68cb2-131">&nbsp;&nbsp; **フェンス**</span><span class="sxs-lookup"><span data-stu-id="68cb2-131">&nbsp; &nbsp; **Fencing**</span></span> | <span data-ttu-id="68cb2-132">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="68cb2-132">DeviceManagementConfiguration.ReadWrite.All</span></span> |
| <span data-ttu-id="68cb2-133">&nbsp; &nbsp; **通知**</span><span class="sxs-lookup"><span data-stu-id="68cb2-133">&nbsp; &nbsp; **Notification**</span></span> | <span data-ttu-id="68cb2-134">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="68cb2-134">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="68cb2-135">&nbsp; &nbsp; **オンボーディング**</span><span class="sxs-lookup"><span data-stu-id="68cb2-135">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="68cb2-136">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="68cb2-136">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="68cb2-137">&nbsp; &nbsp; **役割ベースのアクセス制御 (RBAC)**</span><span class="sxs-lookup"><span data-stu-id="68cb2-137">&nbsp; &nbsp; **Role-based access control (RBAC)**</span></span> | <span data-ttu-id="68cb2-138">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="68cb2-138">DeviceManagementRBAC.ReadWrite.All</span></span> |
| <span data-ttu-id="68cb2-139">&nbsp; &nbsp; **リモート アクセス**</span><span class="sxs-lookup"><span data-stu-id="68cb2-139">&nbsp; &nbsp; **Remote access**</span></span> | <span data-ttu-id="68cb2-140">DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="68cb2-140">DeviceManagementConfiguration.Read.All</span></span> |
| <span data-ttu-id="68cb2-141">&nbsp;&nbsp; **リモートアシスタンス**</span><span class="sxs-lookup"><span data-stu-id="68cb2-141">&nbsp; &nbsp; **Remote assistance**</span></span> | <span data-ttu-id="68cb2-142">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="68cb2-142">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="68cb2-143">&nbsp;&nbsp; **通信経費管理**</span><span class="sxs-lookup"><span data-stu-id="68cb2-143">&nbsp; &nbsp; **Telecom expense management**</span></span> | <span data-ttu-id="68cb2-144">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="68cb2-144">DeviceManagementServiceConfig.ReadWrite.All</span></span> |
| <span data-ttu-id="68cb2-145">&nbsp;&nbsp; **Troublehooting**</span><span class="sxs-lookup"><span data-stu-id="68cb2-145">&nbsp; &nbsp; **Troublehooting**</span></span> | <span data-ttu-id="68cb2-146">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="68cb2-146">DeviceManagementManagedDevices.ReadWrite.All</span></span> |
| <span data-ttu-id="68cb2-147">&nbsp;&nbsp; **Windows 情報保護**</span><span class="sxs-lookup"><span data-stu-id="68cb2-147">&nbsp; &nbsp; **Windows Information Protection**</span></span> | <span data-ttu-id="68cb2-148">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="68cb2-148">DeviceManagementApps.ReadWrite.All</span></span> |
| <span data-ttu-id="68cb2-149">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="68cb2-149">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="68cb2-150">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="68cb2-150">Not supported.</span></span>|
| <span data-ttu-id="68cb2-151">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="68cb2-151">Application</span></span> | <span data-ttu-id="68cb2-152">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="68cb2-152">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="68cb2-153">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="68cb2-153">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement
```

## <a name="request-headers"></a><span data-ttu-id="68cb2-154">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="68cb2-154">Request headers</span></span>

|<span data-ttu-id="68cb2-155">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="68cb2-155">Header</span></span>|<span data-ttu-id="68cb2-156">値</span><span class="sxs-lookup"><span data-stu-id="68cb2-156">Value</span></span>|
|:---|:---|
|<span data-ttu-id="68cb2-157">Authorization</span><span class="sxs-lookup"><span data-stu-id="68cb2-157">Authorization</span></span>|<span data-ttu-id="68cb2-158">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="68cb2-158">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="68cb2-159">承諾</span><span class="sxs-lookup"><span data-stu-id="68cb2-159">Accept</span></span>|<span data-ttu-id="68cb2-160">application/json</span><span class="sxs-lookup"><span data-stu-id="68cb2-160">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="68cb2-161">要求本文</span><span class="sxs-lookup"><span data-stu-id="68cb2-161">Request body</span></span>

<span data-ttu-id="68cb2-162">要求本文で、[deviceManagement](../resources/intune-shared-devicemanagement.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="68cb2-162">In the request body, supply a JSON representation for the [deviceManagement](../resources/intune-shared-devicemanagement.md) object.</span></span>

<span data-ttu-id="68cb2-163">次の表に、[deviceManagement](../resources/intune-shared-devicemanagement.md) の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="68cb2-163">The following table shows the properties that are required when you create the [deviceManagement](../resources/intune-shared-devicemanagement.md).</span></span>

|<span data-ttu-id="68cb2-164">プロパティ</span><span class="sxs-lookup"><span data-stu-id="68cb2-164">Property</span></span>|<span data-ttu-id="68cb2-165">型</span><span class="sxs-lookup"><span data-stu-id="68cb2-165">Type</span></span>|<span data-ttu-id="68cb2-166">説明</span><span class="sxs-lookup"><span data-stu-id="68cb2-166">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="68cb2-167">id</span><span class="sxs-lookup"><span data-stu-id="68cb2-167">id</span></span>|<span data-ttu-id="68cb2-168">String</span><span class="sxs-lookup"><span data-stu-id="68cb2-168">String</span></span>|<span data-ttu-id="68cb2-169">デバイスの一意識別子。</span><span class="sxs-lookup"><span data-stu-id="68cb2-169">Unique identifier for the device.</span></span>|
|**<span data-ttu-id="68cb2-170">デバイス構成</span><span class="sxs-lookup"><span data-stu-id="68cb2-170">Device configuration</span></span>**|
|<span data-ttu-id="68cb2-171">int未指定 eaccountid</span><span class="sxs-lookup"><span data-stu-id="68cb2-171">intuneAccountId</span></span>|<span data-ttu-id="68cb2-172">GUID</span><span class="sxs-lookup"><span data-stu-id="68cb2-172">GUID</span></span>|<span data-ttu-id="68cb2-173">指定したテナントの Intune アカウント ID</span><span class="sxs-lookup"><span data-stu-id="68cb2-173">Intune Account ID for given tenant</span></span>|
|<span data-ttu-id="68cb2-174">legacyPcManangementEnabled</span><span class="sxs-lookup"><span data-stu-id="68cb2-174">legacyPcManangementEnabled</span></span>|<span data-ttu-id="68cb2-175">Boolean</span><span class="sxs-lookup"><span data-stu-id="68cb2-175">Boolean</span></span>|<span data-ttu-id="68cb2-176">このアカウントの非 MDM で管理されているレガシー PC 管理を有効にするプロパティ。</span><span class="sxs-lookup"><span data-stu-id="68cb2-176">The property to enable Non-MDM managed legacy PC management for this account.</span></span> <span data-ttu-id="68cb2-177">このプロパティに値を設定するには、 SetExtrusionDirection メソッドを適用します。</span><span class="sxs-lookup"><span data-stu-id="68cb2-177">This property is read-only.</span></span>|
|<span data-ttu-id="68cb2-178">maximumdeptokens</span><span class="sxs-lookup"><span data-stu-id="68cb2-178">maximumDepTokens</span></span>|<span data-ttu-id="68cb2-179">Int32</span><span class="sxs-lookup"><span data-stu-id="68cb2-179">Int32</span></span>|<span data-ttu-id="68cb2-180">テナントごとに許容される DEP トークンの最大数。</span><span class="sxs-lookup"><span data-stu-id="68cb2-180">Maximum number of DEP tokens allowed per-tenant.</span></span>|
|<span data-ttu-id="68cb2-181">settings</span><span class="sxs-lookup"><span data-stu-id="68cb2-181">settings</span></span>|[<span data-ttu-id="68cb2-182">deviceManagementSettings</span><span class="sxs-lookup"><span data-stu-id="68cb2-182">deviceManagementSettings</span></span>](../resources/intune-deviceconfig-devicemanagementsettings.md)|<span data-ttu-id="68cb2-183">アカウント レベルの設定。</span><span class="sxs-lookup"><span data-stu-id="68cb2-183">Account level settings.</span></span>|
|**<span data-ttu-id="68cb2-184">デバイスの管理</span><span class="sxs-lookup"><span data-stu-id="68cb2-184">Device management</span></span>**|
|<span data-ttu-id="68cb2-185">accountMoveCompletionDateTime</span><span class="sxs-lookup"><span data-stu-id="68cb2-185">accountMoveCompletionDateTime</span></span>|<span data-ttu-id="68cb2-186">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="68cb2-186">DateTimeOffset</span></span>|<span data-ttu-id="68cb2-187">& が、scaleunits 間でテナントデータを移動した日時です。</span><span class="sxs-lookup"><span data-stu-id="68cb2-187">The date & time when tenant data moved between scaleunits.</span></span>|
|<span data-ttu-id="68cb2-188">adminConsent</span><span class="sxs-lookup"><span data-stu-id="68cb2-188">adminConsent</span></span>|[<span data-ttu-id="68cb2-189">adminConsent</span><span class="sxs-lookup"><span data-stu-id="68cb2-189">adminConsent</span></span>](../resources/intune-devices-adminconsent.md)|<span data-ttu-id="68cb2-190">管理者の同意情報。</span><span class="sxs-lookup"><span data-stu-id="68cb2-190">Admin consent information.</span></span>|
|<span data-ttu-id="68cb2-191">deviceProtectionOverview</span><span class="sxs-lookup"><span data-stu-id="68cb2-191">deviceProtectionOverview</span></span>|[<span data-ttu-id="68cb2-192">deviceProtectionOverview</span><span class="sxs-lookup"><span data-stu-id="68cb2-192">deviceProtectionOverview</span></span>](../resources/intune-devices-deviceprotectionoverview.md)|<span data-ttu-id="68cb2-193">デバイス保護の概要。</span><span class="sxs-lookup"><span data-stu-id="68cb2-193">Device protection overview.</span></span>|
|<span data-ttu-id="68cb2-194">managedDeviceCleanupSettings</span><span class="sxs-lookup"><span data-stu-id="68cb2-194">managedDeviceCleanupSettings</span></span>|[<span data-ttu-id="68cb2-195">managedDeviceCleanupSettings</span><span class="sxs-lookup"><span data-stu-id="68cb2-195">managedDeviceCleanupSettings</span></span>](../resources/intune-devices-manageddevicecleanupsettings.md)|<span data-ttu-id="68cb2-196">デバイスクリーンアップルール</span><span class="sxs-lookup"><span data-stu-id="68cb2-196">Device cleanup rule</span></span>|
|<span data-ttu-id="68cb2-197">subscriptionState</span><span class="sxs-lookup"><span data-stu-id="68cb2-197">subscriptionState</span></span>|[<span data-ttu-id="68cb2-198">devicemanagementsubscriptionstate</span><span class="sxs-lookup"><span data-stu-id="68cb2-198">deviceManagementSubscriptionState</span></span>](../resources/intune-devices-devicemanagementsubscriptionstate.md)|<span data-ttu-id="68cb2-199">テナントのモバイル デバイス管理のサブスクリプション状態。</span><span class="sxs-lookup"><span data-stu-id="68cb2-199">Tenant mobile device management subscription state.</span></span> <span data-ttu-id="68cb2-200">可能な値は、`pending`、`active`、`warning`、`disabled`、`deleted`、`blocked`、`lockedOut` です。</span><span class="sxs-lookup"><span data-stu-id="68cb2-200">Possible values are: `pending`, `active`, `warning`, `disabled`, `deleted`, `blocked`, `lockedOut`.</span></span>|
|<span data-ttu-id="68cb2-201">subscriptions</span><span class="sxs-lookup"><span data-stu-id="68cb2-201">subscriptions</span></span>|[<span data-ttu-id="68cb2-202">devicemanagementsubscriptions</span><span class="sxs-lookup"><span data-stu-id="68cb2-202">deviceManagementSubscriptions</span></span>](../resources/intune-devices-devicemanagementsubscriptions.md)|<span data-ttu-id="68cb2-203">テナントのサブスクリプション。</span><span class="sxs-lookup"><span data-stu-id="68cb2-203">Tenant's Subscription.</span></span> <span data-ttu-id="68cb2-204">可能な値は `none`、`intune`、`office365`、`intunePremium`、`intune_EDU`、`intune_SMB` です。</span><span class="sxs-lookup"><span data-stu-id="68cb2-204">Possible values are: `none`, `intune`, `office365`, `intunePremium`, `intune_EDU`, `intune_SMB`.</span></span>|
|<span data-ttu-id="68cb2-205">windowsMalwareOverview</span><span class="sxs-lookup"><span data-stu-id="68cb2-205">windowsMalwareOverview</span></span>|[<span data-ttu-id="68cb2-206">windowsMalwareOverview</span><span class="sxs-lookup"><span data-stu-id="68cb2-206">windowsMalwareOverview</span></span>](../resources/intune-devices-windowsmalwareoverview.md)|<span data-ttu-id="68cb2-207">windows デバイスのマルウェアの概要。</span><span class="sxs-lookup"><span data-stu-id="68cb2-207">Malware overview for windows devices.</span></span>|
|**<span data-ttu-id="68cb2-208">オンボーディング</span><span class="sxs-lookup"><span data-stu-id="68cb2-208">Onboarding</span></span>**|
|<span data-ttu-id="68cb2-209">intuneBrand</span><span class="sxs-lookup"><span data-stu-id="68cb2-209">intuneBrand</span></span>|[<span data-ttu-id="68cb2-210">intuneBrand</span><span class="sxs-lookup"><span data-stu-id="68cb2-210">intuneBrand</span></span>](../resources/intune-onboarding-intunebrand.md)|<span data-ttu-id="68cb2-211">intuneBrand には、会社のポータル アプリケーションとエンド ユーザーの Web ポータルの外観のカスタマイズに使用するデータが含まれています。</span><span class="sxs-lookup"><span data-stu-id="68cb2-211">intuneBrand contains data which is used in customizing the appearance of the Company Portal applications as well as the end user web portal.</span></span>|

<span data-ttu-id="68cb2-212">要求本文のプロパティのサポートは、ワークフローによって異なります。</span><span class="sxs-lookup"><span data-stu-id="68cb2-212">Request body property support varies according to workflow.</span></span>

## <a name="response"></a><span data-ttu-id="68cb2-213">応答</span><span class="sxs-lookup"><span data-stu-id="68cb2-213">Response</span></span>
<span data-ttu-id="68cb2-214">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で更新された [deviceManagement](../resources/intune-shared-devicemanagement.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="68cb2-214">If successful, this method returns a `200 OK` response code and an updated [deviceManagement](../resources/intune-shared-devicemanagement.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="68cb2-215">例</span><span class="sxs-lookup"><span data-stu-id="68cb2-215">Example</span></span>

### <a name="request"></a><span data-ttu-id="68cb2-216">要求</span><span class="sxs-lookup"><span data-stu-id="68cb2-216">Request</span></span>

<span data-ttu-id="68cb2-217">以下は、デバイス管理ワークフローの後の要求の例です。</span><span class="sxs-lookup"><span data-stu-id="68cb2-217">Here is an example of a request following the device management workflow:</span></span>

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

### <a name="response"></a><span data-ttu-id="68cb2-218">応答</span><span class="sxs-lookup"><span data-stu-id="68cb2-218">Response</span></span>

<span data-ttu-id="68cb2-219">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="68cb2-219">Here is an example of the response.</span></span> 

<span data-ttu-id="68cb2-220">注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。</span><span class="sxs-lookup"><span data-stu-id="68cb2-220">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="68cb2-221">返されるプロパティは、ワークフローおよびコンテキストによって異なります。</span><span class="sxs-lookup"><span data-stu-id="68cb2-221">Returned properties vary according to workflow and context.</span></span>

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



