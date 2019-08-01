---
title: Create managedDevice
description: 新しい managedDevice オブジェクトを作成します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 766274595966daeeb00b0802a92bb61c55a32e1f
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36018695"
---
# <a name="create-manageddevice"></a><span data-ttu-id="a9d4b-103">Create managedDevice</span><span class="sxs-lookup"><span data-stu-id="a9d4b-103">Create managedDevice</span></span>

> <span data-ttu-id="a9d4b-104">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="a9d4b-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a9d4b-105">新しい [managedDevice](../resources/intune-devices-manageddevice.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="a9d4b-105">Create a new [managedDevice](../resources/intune-devices-manageddevice.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a9d4b-106">前提条件</span><span class="sxs-lookup"><span data-stu-id="a9d4b-106">Prerequisites</span></span>
<span data-ttu-id="a9d4b-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="a9d4b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a9d4b-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="a9d4b-109">Permission type</span></span>|<span data-ttu-id="a9d4b-110">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="a9d4b-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a9d4b-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="a9d4b-111">Delegated (work or school account)</span></span>|<span data-ttu-id="a9d4b-112">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a9d4b-112">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="a9d4b-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="a9d4b-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a9d4b-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a9d4b-114">Not supported.</span></span>|
|<span data-ttu-id="a9d4b-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="a9d4b-115">Application</span></span>|<span data-ttu-id="a9d4b-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a9d4b-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a9d4b-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="a9d4b-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /users/{usersId}/managedDevices
POST /deviceManagement/managedDevices
POST /deviceManagement/detectedApps/{detectedAppId}/managedDevices
```

## <a name="request-headers"></a><span data-ttu-id="a9d4b-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="a9d4b-118">Request headers</span></span>
|<span data-ttu-id="a9d4b-119">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="a9d4b-119">Header</span></span>|<span data-ttu-id="a9d4b-120">値</span><span class="sxs-lookup"><span data-stu-id="a9d4b-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a9d4b-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="a9d4b-121">Authorization</span></span>|<span data-ttu-id="a9d4b-122">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="a9d4b-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a9d4b-123">承諾</span><span class="sxs-lookup"><span data-stu-id="a9d4b-123">Accept</span></span>|<span data-ttu-id="a9d4b-124">application/json</span><span class="sxs-lookup"><span data-stu-id="a9d4b-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a9d4b-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="a9d4b-125">Request body</span></span>
<span data-ttu-id="a9d4b-126">要求本文で、managedDevice オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="a9d4b-126">In the request body, supply a JSON representation for the managedDevice object.</span></span>

<span data-ttu-id="a9d4b-127">次の表に、managedDevice の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="a9d4b-127">The following table shows the properties that are required when you create the managedDevice.</span></span>

|<span data-ttu-id="a9d4b-128">プロパティ</span><span class="sxs-lookup"><span data-stu-id="a9d4b-128">Property</span></span>|<span data-ttu-id="a9d4b-129">型</span><span class="sxs-lookup"><span data-stu-id="a9d4b-129">Type</span></span>|<span data-ttu-id="a9d4b-130">説明</span><span class="sxs-lookup"><span data-stu-id="a9d4b-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a9d4b-131">id</span><span class="sxs-lookup"><span data-stu-id="a9d4b-131">id</span></span>|<span data-ttu-id="a9d4b-132">文字列</span><span class="sxs-lookup"><span data-stu-id="a9d4b-132">String</span></span>|<span data-ttu-id="a9d4b-133">デバイスの一意識別子</span><span class="sxs-lookup"><span data-stu-id="a9d4b-133">Unique Identifier for the device</span></span>|
|<span data-ttu-id="a9d4b-134">userId</span><span class="sxs-lookup"><span data-stu-id="a9d4b-134">userId</span></span>|<span data-ttu-id="a9d4b-135">String</span><span class="sxs-lookup"><span data-stu-id="a9d4b-135">String</span></span>|<span data-ttu-id="a9d4b-136">デバイスに関連付けられているユーザーの一意の識別子</span><span class="sxs-lookup"><span data-stu-id="a9d4b-136">Unique Identifier for the user associated with the device</span></span>|
|<span data-ttu-id="a9d4b-137">deviceName</span><span class="sxs-lookup"><span data-stu-id="a9d4b-137">deviceName</span></span>|<span data-ttu-id="a9d4b-138">String</span><span class="sxs-lookup"><span data-stu-id="a9d4b-138">String</span></span>|<span data-ttu-id="a9d4b-139">デバイスの名前</span><span class="sxs-lookup"><span data-stu-id="a9d4b-139">Name of the device</span></span>|
|<span data-ttu-id="a9d4b-140">managedDeviceOwnerType</span><span class="sxs-lookup"><span data-stu-id="a9d4b-140">managedDeviceOwnerType</span></span>|[<span data-ttu-id="a9d4b-141">managedDeviceOwnerType</span><span class="sxs-lookup"><span data-stu-id="a9d4b-141">managedDeviceOwnerType</span></span>](../resources/intune-devices-manageddeviceownertype.md)|<span data-ttu-id="a9d4b-142">デバイスの所有権。</span><span class="sxs-lookup"><span data-stu-id="a9d4b-142">Ownership of the device.</span></span> <span data-ttu-id="a9d4b-143">' Company ' または ' personal ' にすることができます。</span><span class="sxs-lookup"><span data-stu-id="a9d4b-143">Can be 'company' or 'personal'.</span></span> <span data-ttu-id="a9d4b-144">可能な値は、`unknown`、`company`、`personal` です。</span><span class="sxs-lookup"><span data-stu-id="a9d4b-144">Possible values are: `unknown`, `company`, `personal`.</span></span>|
|<span data-ttu-id="a9d4b-145">deviceActionResults</span><span class="sxs-lookup"><span data-stu-id="a9d4b-145">deviceActionResults</span></span>|<span data-ttu-id="a9d4b-146">[deviceActionResult](../resources/intune-devices-deviceactionresult.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="a9d4b-146">[deviceActionResult](../resources/intune-devices-deviceactionresult.md) collection</span></span>|<span data-ttu-id="a9d4b-147">ComplexType deviceActionResult オブジェクトのリスト。</span><span class="sxs-lookup"><span data-stu-id="a9d4b-147">List of ComplexType deviceActionResult objects.</span></span>|
|<span data-ttu-id="a9d4b-148">enrolledDateTime</span><span class="sxs-lookup"><span data-stu-id="a9d4b-148">enrolledDateTime</span></span>|<span data-ttu-id="a9d4b-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a9d4b-149">DateTimeOffset</span></span>|<span data-ttu-id="a9d4b-150">デバイスの登録時刻。</span><span class="sxs-lookup"><span data-stu-id="a9d4b-150">Enrollment time of the device.</span></span>|
|<span data-ttu-id="a9d4b-151">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="a9d4b-151">lastSyncDateTime</span></span>|<span data-ttu-id="a9d4b-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a9d4b-152">DateTimeOffset</span></span>|<span data-ttu-id="a9d4b-153">デバイスが Intune との正常な同期を最終的に完了した日時。</span><span class="sxs-lookup"><span data-stu-id="a9d4b-153">The date and time that the device last completed a successful sync with Intune.</span></span>|
|<span data-ttu-id="a9d4b-154">operatingSystem</span><span class="sxs-lookup"><span data-stu-id="a9d4b-154">operatingSystem</span></span>|<span data-ttu-id="a9d4b-155">文字列</span><span class="sxs-lookup"><span data-stu-id="a9d4b-155">String</span></span>|<span data-ttu-id="a9d4b-156">デバイスのオペレーティング システム。</span><span class="sxs-lookup"><span data-stu-id="a9d4b-156">Operating system of the device.</span></span> <span data-ttu-id="a9d4b-157">Windows、iOS など。</span><span class="sxs-lookup"><span data-stu-id="a9d4b-157">Windows, iOS, etc.</span></span>|
|<span data-ttu-id="a9d4b-158">complianceState</span><span class="sxs-lookup"><span data-stu-id="a9d4b-158">complianceState</span></span>|[<span data-ttu-id="a9d4b-159">complianceState</span><span class="sxs-lookup"><span data-stu-id="a9d4b-159">complianceState</span></span>](../resources/intune-devices-compliancestate.md)|<span data-ttu-id="a9d4b-160">デバイスのコンプライアンス状態。</span><span class="sxs-lookup"><span data-stu-id="a9d4b-160">Compliance state of the device.</span></span> <span data-ttu-id="a9d4b-161">可能な値は、`unknown`、`compliant`、`noncompliant`、`conflict`、`error`、`inGracePeriod`、`configManager` です。</span><span class="sxs-lookup"><span data-stu-id="a9d4b-161">Possible values are: `unknown`, `compliant`, `noncompliant`, `conflict`, `error`, `inGracePeriod`, `configManager`.</span></span>|
|<span data-ttu-id="a9d4b-162">jailBroken</span><span class="sxs-lookup"><span data-stu-id="a9d4b-162">jailBroken</span></span>|<span data-ttu-id="a9d4b-163">String</span><span class="sxs-lookup"><span data-stu-id="a9d4b-163">String</span></span>|<span data-ttu-id="a9d4b-164">デバイスが脱獄またはルート化されているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="a9d4b-164">whether the device is jail broken or rooted.</span></span>|
|<span data-ttu-id="a9d4b-165">managementAgent</span><span class="sxs-lookup"><span data-stu-id="a9d4b-165">managementAgent</span></span>|[<span data-ttu-id="a9d4b-166">managementAgentType</span><span class="sxs-lookup"><span data-stu-id="a9d4b-166">managementAgentType</span></span>](../resources/intune-devices-managementagenttype.md)|<span data-ttu-id="a9d4b-167">デバイスの管理チャネル。</span><span class="sxs-lookup"><span data-stu-id="a9d4b-167">Management channel of the device.</span></span> <span data-ttu-id="a9d4b-168">Intune、EAS など。可能な値は、`eas`、`mdm`、`easMdm`、`intuneClient`、`easIntuneClient`、`configurationManagerClient`、`configurationManagerClientMdm`、`configurationManagerClientMdmEas`、`unknown`、`jamf`、`googleCloudDevicePolicyController` です。</span><span class="sxs-lookup"><span data-stu-id="a9d4b-168">Intune, EAS, etc. Possible values are: `eas`, `mdm`, `easMdm`, `intuneClient`, `easIntuneClient`, `configurationManagerClient`, `configurationManagerClientMdm`, `configurationManagerClientMdmEas`, `unknown`, `jamf`, `googleCloudDevicePolicyController`.</span></span>|
|<span data-ttu-id="a9d4b-169">osVersion</span><span class="sxs-lookup"><span data-stu-id="a9d4b-169">osVersion</span></span>|<span data-ttu-id="a9d4b-170">String</span><span class="sxs-lookup"><span data-stu-id="a9d4b-170">String</span></span>|<span data-ttu-id="a9d4b-171">デバイスのオペレーティング システムのバージョン。</span><span class="sxs-lookup"><span data-stu-id="a9d4b-171">Operating system version of the device.</span></span>|
|<span data-ttu-id="a9d4b-172">easActivated</span><span class="sxs-lookup"><span data-stu-id="a9d4b-172">easActivated</span></span>|<span data-ttu-id="a9d4b-173">Boolean</span><span class="sxs-lookup"><span data-stu-id="a9d4b-173">Boolean</span></span>|<span data-ttu-id="a9d4b-174">Exchange ActiveSync がアクティブになっているデバイスかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="a9d4b-174">Whether the device is Exchange ActiveSync activated.</span></span>|
|<span data-ttu-id="a9d4b-175">easDeviceId</span><span class="sxs-lookup"><span data-stu-id="a9d4b-175">easDeviceId</span></span>|<span data-ttu-id="a9d4b-176">String</span><span class="sxs-lookup"><span data-stu-id="a9d4b-176">String</span></span>|<span data-ttu-id="a9d4b-177">デバイスの Exchange ActiveSync の ID。</span><span class="sxs-lookup"><span data-stu-id="a9d4b-177">Exchange ActiveSync Id of the device.</span></span>|
|<span data-ttu-id="a9d4b-178">easActivationDateTime</span><span class="sxs-lookup"><span data-stu-id="a9d4b-178">easActivationDateTime</span></span>|<span data-ttu-id="a9d4b-179">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a9d4b-179">DateTimeOffset</span></span>|<span data-ttu-id="a9d4b-180">デバイスの Exchange ActivationSync のアクティブ化の時刻。</span><span class="sxs-lookup"><span data-stu-id="a9d4b-180">Exchange ActivationSync activation time of the device.</span></span>|
|<span data-ttu-id="a9d4b-181">azureADRegistered</span><span class="sxs-lookup"><span data-stu-id="a9d4b-181">azureADRegistered</span></span>|<span data-ttu-id="a9d4b-182">Boolean</span><span class="sxs-lookup"><span data-stu-id="a9d4b-182">Boolean</span></span>|<span data-ttu-id="a9d4b-183">Azure Active Directory が登録されているデバイスかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="a9d4b-183">Whether the device is Azure Active Directory registered.</span></span>|
|<span data-ttu-id="a9d4b-184">deviceEnrollmentType</span><span class="sxs-lookup"><span data-stu-id="a9d4b-184">deviceEnrollmentType</span></span>|[<span data-ttu-id="a9d4b-185">deviceEnrollmentType</span><span class="sxs-lookup"><span data-stu-id="a9d4b-185">deviceEnrollmentType</span></span>](../resources/intune-shared-deviceenrollmenttype.md)|<span data-ttu-id="a9d4b-186">デバイスの登録の種類。</span><span class="sxs-lookup"><span data-stu-id="a9d4b-186">Enrollment type of the device.</span></span> <span data-ttu-id="a9d4b-187">可能な値は、`unknown`、`userEnrollment`、`deviceEnrollmentManager`、`appleBulkWithUser`、`appleBulkWithoutUser`、`windowsAzureADJoin`、`windowsBulkUserless`、`windowsAutoEnrollment`、`windowsBulkAzureDomainJoin`、`windowsCoManagement` です。</span><span class="sxs-lookup"><span data-stu-id="a9d4b-187">Possible values are: `unknown`, `userEnrollment`, `deviceEnrollmentManager`, `appleBulkWithUser`, `appleBulkWithoutUser`, `windowsAzureADJoin`, `windowsBulkUserless`, `windowsAutoEnrollment`, `windowsBulkAzureDomainJoin`, `windowsCoManagement`.</span></span>|
|<span data-ttu-id="a9d4b-188">activationLockBypassCode</span><span class="sxs-lookup"><span data-stu-id="a9d4b-188">activationLockBypassCode</span></span>|<span data-ttu-id="a9d4b-189">String</span><span class="sxs-lookup"><span data-stu-id="a9d4b-189">String</span></span>|<span data-ttu-id="a9d4b-190">デバイスのアクティベーション ロックをバイパスするためのコード。</span><span class="sxs-lookup"><span data-stu-id="a9d4b-190">Code that allows the Activation Lock on a device to be bypassed.</span></span>|
|<span data-ttu-id="a9d4b-191">emailAddress</span><span class="sxs-lookup"><span data-stu-id="a9d4b-191">emailAddress</span></span>|<span data-ttu-id="a9d4b-192">String</span><span class="sxs-lookup"><span data-stu-id="a9d4b-192">String</span></span>|<span data-ttu-id="a9d4b-193">デバイスに関連付けられているユーザーの電子メール</span><span class="sxs-lookup"><span data-stu-id="a9d4b-193">Email(s) for the user associated with the device</span></span>|
|<span data-ttu-id="a9d4b-194">azureADDeviceId</span><span class="sxs-lookup"><span data-stu-id="a9d4b-194">azureADDeviceId</span></span>|<span data-ttu-id="a9d4b-195">String</span><span class="sxs-lookup"><span data-stu-id="a9d4b-195">String</span></span>|<span data-ttu-id="a9d4b-196">Azure Active Directory デバイスの一意識別子。</span><span class="sxs-lookup"><span data-stu-id="a9d4b-196">The unique identifier for the Azure Active Directory device.</span></span> <span data-ttu-id="a9d4b-197">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="a9d4b-197">Read only.</span></span>|
|<span data-ttu-id="a9d4b-198">deviceRegistrationState</span><span class="sxs-lookup"><span data-stu-id="a9d4b-198">deviceRegistrationState</span></span>|[<span data-ttu-id="a9d4b-199">deviceRegistrationState</span><span class="sxs-lookup"><span data-stu-id="a9d4b-199">deviceRegistrationState</span></span>](../resources/intune-devices-deviceregistrationstate.md)|<span data-ttu-id="a9d4b-200">デバイスの登録状態。</span><span class="sxs-lookup"><span data-stu-id="a9d4b-200">Device registration state.</span></span> <span data-ttu-id="a9d4b-201">可能な値は、`notRegistered`、`registered`、`revoked`、`keyConflict`、`approvalPending`、`certificateReset`、`notRegisteredPendingEnrollment`、`unknown` です。</span><span class="sxs-lookup"><span data-stu-id="a9d4b-201">Possible values are: `notRegistered`, `registered`, `revoked`, `keyConflict`, `approvalPending`, `certificateReset`, `notRegisteredPendingEnrollment`, `unknown`.</span></span>|
|<span data-ttu-id="a9d4b-202">deviceCategoryDisplayName</span><span class="sxs-lookup"><span data-stu-id="a9d4b-202">deviceCategoryDisplayName</span></span>|<span data-ttu-id="a9d4b-203">String</span><span class="sxs-lookup"><span data-stu-id="a9d4b-203">String</span></span>|<span data-ttu-id="a9d4b-204">デバイス カテゴリの表示名</span><span class="sxs-lookup"><span data-stu-id="a9d4b-204">Device category display name</span></span>|
|<span data-ttu-id="a9d4b-205">isSupervised</span><span class="sxs-lookup"><span data-stu-id="a9d4b-205">isSupervised</span></span>|<span data-ttu-id="a9d4b-206">Boolean</span><span class="sxs-lookup"><span data-stu-id="a9d4b-206">Boolean</span></span>|<span data-ttu-id="a9d4b-207">デバイスの管理状況</span><span class="sxs-lookup"><span data-stu-id="a9d4b-207">Device supervised status</span></span>|
|<span data-ttu-id="a9d4b-208">exchangeLastSuccessfulSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="a9d4b-208">exchangeLastSuccessfulSyncDateTime</span></span>|<span data-ttu-id="a9d4b-209">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a9d4b-209">DateTimeOffset</span></span>|<span data-ttu-id="a9d4b-210">最後にデバイスが Exchange に接続した時刻。</span><span class="sxs-lookup"><span data-stu-id="a9d4b-210">Last time the device contacted Exchange.</span></span>|
|<span data-ttu-id="a9d4b-211">exchangeAccessState</span><span class="sxs-lookup"><span data-stu-id="a9d4b-211">exchangeAccessState</span></span>|[<span data-ttu-id="a9d4b-212">deviceManagementExchangeAccessState</span><span class="sxs-lookup"><span data-stu-id="a9d4b-212">deviceManagementExchangeAccessState</span></span>](../resources/intune-devices-devicemanagementexchangeaccessstate.md)|<span data-ttu-id="a9d4b-213">Exchange でのデバイスのアクセスの状態。</span><span class="sxs-lookup"><span data-stu-id="a9d4b-213">The Access State of the device in Exchange.</span></span> <span data-ttu-id="a9d4b-214">可能な値は、`none`、`unknown`、`allowed`、`blocked`、`quarantined` です。</span><span class="sxs-lookup"><span data-stu-id="a9d4b-214">Possible values are: `none`, `unknown`, `allowed`, `blocked`, `quarantined`.</span></span>|
|<span data-ttu-id="a9d4b-215">exchangeAccessStateReason</span><span class="sxs-lookup"><span data-stu-id="a9d4b-215">exchangeAccessStateReason</span></span>|[<span data-ttu-id="a9d4b-216">deviceManagementExchangeAccessStateReason</span><span class="sxs-lookup"><span data-stu-id="a9d4b-216">deviceManagementExchangeAccessStateReason</span></span>](../resources/intune-devices-devicemanagementexchangeaccessstatereason.md)|<span data-ttu-id="a9d4b-217">Exchange でのデバイスのアクセス状態の理由。
</span><span class="sxs-lookup"><span data-stu-id="a9d4b-217">The reason for the device's access state in Exchange.</span></span> <span data-ttu-id="a9d4b-218">可能な値は、`none`、`unknown`、`exchangeGlobalRule`、`exchangeIndividualRule`、`exchangeDeviceRule`、`exchangeUpgrade`、`exchangeMailboxPolicy`、`other`、`compliant`、`notCompliant`、`notEnrolled`、`unknownLocation`、`mfaRequired`、`azureADBlockDueToAccessPolicy`、`compromisedPassword`、`deviceNotKnownWithManagedApp` です。</span><span class="sxs-lookup"><span data-stu-id="a9d4b-218">Possible values are: `none`, `unknown`, `exchangeGlobalRule`, `exchangeIndividualRule`, `exchangeDeviceRule`, `exchangeUpgrade`, `exchangeMailboxPolicy`, `other`, `compliant`, `notCompliant`, `notEnrolled`, `unknownLocation`, `mfaRequired`, `azureADBlockDueToAccessPolicy`, `compromisedPassword`, `deviceNotKnownWithManagedApp`.</span></span>|
|<span data-ttu-id="a9d4b-219">remoteAssistanceSessionUrl</span><span class="sxs-lookup"><span data-stu-id="a9d4b-219">remoteAssistanceSessionUrl</span></span>|<span data-ttu-id="a9d4b-220">String</span><span class="sxs-lookup"><span data-stu-id="a9d4b-220">String</span></span>|<span data-ttu-id="a9d4b-221">デバイスとのリモート アシスタンス セッションを確立できるようにする URL。</span><span class="sxs-lookup"><span data-stu-id="a9d4b-221">Url that allows a Remote Assistance session to be established with the device.</span></span>|
|<span data-ttu-id="a9d4b-222">remoteAssistanceSessionErrorDetails</span><span class="sxs-lookup"><span data-stu-id="a9d4b-222">remoteAssistanceSessionErrorDetails</span></span>|<span data-ttu-id="a9d4b-223">String</span><span class="sxs-lookup"><span data-stu-id="a9d4b-223">String</span></span>|<span data-ttu-id="a9d4b-224">リモート アシスタンス セッション オブジェクトの作成時に問題を識別するエラー文字列。</span><span class="sxs-lookup"><span data-stu-id="a9d4b-224">An error string that identifies issues when creating Remote Assistance session objects.</span></span>|
|<span data-ttu-id="a9d4b-225">isEncrypted</span><span class="sxs-lookup"><span data-stu-id="a9d4b-225">isEncrypted</span></span>|<span data-ttu-id="a9d4b-226">Boolean</span><span class="sxs-lookup"><span data-stu-id="a9d4b-226">Boolean</span></span>|<span data-ttu-id="a9d4b-227">デバイスの暗号化の状態</span><span class="sxs-lookup"><span data-stu-id="a9d4b-227">Device encryption status</span></span>|
|<span data-ttu-id="a9d4b-228">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="a9d4b-228">userPrincipalName</span></span>|<span data-ttu-id="a9d4b-229">String</span><span class="sxs-lookup"><span data-stu-id="a9d4b-229">String</span></span>|<span data-ttu-id="a9d4b-230">デバイスのユーザー プリンシパル名。</span><span class="sxs-lookup"><span data-stu-id="a9d4b-230">Device user principal name</span></span>|
|<span data-ttu-id="a9d4b-231">model</span><span class="sxs-lookup"><span data-stu-id="a9d4b-231">model</span></span>|<span data-ttu-id="a9d4b-232">String</span><span class="sxs-lookup"><span data-stu-id="a9d4b-232">String</span></span>|<span data-ttu-id="a9d4b-233">デバイスのモデル</span><span class="sxs-lookup"><span data-stu-id="a9d4b-233">Model of the device</span></span>|
|<span data-ttu-id="a9d4b-234">manufacturer</span><span class="sxs-lookup"><span data-stu-id="a9d4b-234">manufacturer</span></span>|<span data-ttu-id="a9d4b-235">String</span><span class="sxs-lookup"><span data-stu-id="a9d4b-235">String</span></span>|<span data-ttu-id="a9d4b-236">デバイスのメーカー</span><span class="sxs-lookup"><span data-stu-id="a9d4b-236">Manufacturer of the device</span></span>|
|<span data-ttu-id="a9d4b-237">imei</span><span class="sxs-lookup"><span data-stu-id="a9d4b-237">imei</span></span>|<span data-ttu-id="a9d4b-238">String</span><span class="sxs-lookup"><span data-stu-id="a9d4b-238">String</span></span>|<span data-ttu-id="a9d4b-239">IMEI</span><span class="sxs-lookup"><span data-stu-id="a9d4b-239">IMEI</span></span>|
|<span data-ttu-id="a9d4b-240">complianceGracePeriodExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="a9d4b-240">complianceGracePeriodExpirationDateTime</span></span>|<span data-ttu-id="a9d4b-241">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a9d4b-241">DateTimeOffset</span></span>|<span data-ttu-id="a9d4b-242">デバイス コンプライアンスの猶予期間が経過する DateTime</span><span class="sxs-lookup"><span data-stu-id="a9d4b-242">The DateTime when device compliance grace period expires</span></span>|
|<span data-ttu-id="a9d4b-243">serialNumber</span><span class="sxs-lookup"><span data-stu-id="a9d4b-243">serialNumber</span></span>|<span data-ttu-id="a9d4b-244">String</span><span class="sxs-lookup"><span data-stu-id="a9d4b-244">String</span></span>|<span data-ttu-id="a9d4b-245">シリアル番号</span><span class="sxs-lookup"><span data-stu-id="a9d4b-245">SerialNumber</span></span>|
|<span data-ttu-id="a9d4b-246">phoneNumber</span><span class="sxs-lookup"><span data-stu-id="a9d4b-246">phoneNumber</span></span>|<span data-ttu-id="a9d4b-247">String</span><span class="sxs-lookup"><span data-stu-id="a9d4b-247">String</span></span>|<span data-ttu-id="a9d4b-248">デバイスの電話番号</span><span class="sxs-lookup"><span data-stu-id="a9d4b-248">Phone number of the device</span></span>|
|<span data-ttu-id="a9d4b-249">androidSecurityPatchLevel</span><span class="sxs-lookup"><span data-stu-id="a9d4b-249">androidSecurityPatchLevel</span></span>|<span data-ttu-id="a9d4b-250">String</span><span class="sxs-lookup"><span data-stu-id="a9d4b-250">String</span></span>|<span data-ttu-id="a9d4b-251">Android セキュリティ パッチのレベル</span><span class="sxs-lookup"><span data-stu-id="a9d4b-251">Android security patch level</span></span>|
|<span data-ttu-id="a9d4b-252">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="a9d4b-252">userDisplayName</span></span>|<span data-ttu-id="a9d4b-253">String</span><span class="sxs-lookup"><span data-stu-id="a9d4b-253">String</span></span>|<span data-ttu-id="a9d4b-254">ユーザーの表示名</span><span class="sxs-lookup"><span data-stu-id="a9d4b-254">User display name</span></span>|
|<span data-ttu-id="a9d4b-255">configurationManagerClientEnabledFeatures</span><span class="sxs-lookup"><span data-stu-id="a9d4b-255">configurationManagerClientEnabledFeatures</span></span>|[<span data-ttu-id="a9d4b-256">configurationManagerClientEnabledFeatures</span><span class="sxs-lookup"><span data-stu-id="a9d4b-256">configurationManagerClientEnabledFeatures</span></span>](../resources/intune-devices-configurationmanagerclientenabledfeatures.md)|<span data-ttu-id="a9d4b-257">ConfigrMgr クライアント対応機能
</span><span class="sxs-lookup"><span data-stu-id="a9d4b-257">ConfigrMgr client enabled features</span></span>|
|<span data-ttu-id="a9d4b-258">wiFiMacAddress</span><span class="sxs-lookup"><span data-stu-id="a9d4b-258">wiFiMacAddress</span></span>|<span data-ttu-id="a9d4b-259">String</span><span class="sxs-lookup"><span data-stu-id="a9d4b-259">String</span></span>|<span data-ttu-id="a9d4b-260">Wi-Fi MAC</span><span class="sxs-lookup"><span data-stu-id="a9d4b-260">Wi-Fi MAC</span></span>|
|<span data-ttu-id="a9d4b-261">deviceHealthAttestationState</span><span class="sxs-lookup"><span data-stu-id="a9d4b-261">deviceHealthAttestationState</span></span>|[<span data-ttu-id="a9d4b-262">deviceHealthAttestationState</span><span class="sxs-lookup"><span data-stu-id="a9d4b-262">deviceHealthAttestationState</span></span>](../resources/intune-devices-devicehealthattestationstate.md)|<span data-ttu-id="a9d4b-263">デバイスの正常性構成証明の状態。</span><span class="sxs-lookup"><span data-stu-id="a9d4b-263">The device health attestation state.</span></span>|
|<span data-ttu-id="a9d4b-264">subscriberCarrier</span><span class="sxs-lookup"><span data-stu-id="a9d4b-264">subscriberCarrier</span></span>|<span data-ttu-id="a9d4b-265">String</span><span class="sxs-lookup"><span data-stu-id="a9d4b-265">String</span></span>|<span data-ttu-id="a9d4b-266">サブスクライバー通信事業者</span><span class="sxs-lookup"><span data-stu-id="a9d4b-266">Subscriber Carrier</span></span>|
|<span data-ttu-id="a9d4b-267">meid</span><span class="sxs-lookup"><span data-stu-id="a9d4b-267">meid</span></span>|<span data-ttu-id="a9d4b-268">String</span><span class="sxs-lookup"><span data-stu-id="a9d4b-268">String</span></span>|<span data-ttu-id="a9d4b-269">MEID</span><span class="sxs-lookup"><span data-stu-id="a9d4b-269">MEID</span></span>|
|<span data-ttu-id="a9d4b-270">totalStorageSpaceInBytes</span><span class="sxs-lookup"><span data-stu-id="a9d4b-270">totalStorageSpaceInBytes</span></span>|<span data-ttu-id="a9d4b-271">Int64</span><span class="sxs-lookup"><span data-stu-id="a9d4b-271">Int64</span></span>|<span data-ttu-id="a9d4b-272">記憶域の合計 (バイト)</span><span class="sxs-lookup"><span data-stu-id="a9d4b-272">Total Storage in Bytes</span></span>|
|<span data-ttu-id="a9d4b-273">freeStorageSpaceInBytes</span><span class="sxs-lookup"><span data-stu-id="a9d4b-273">freeStorageSpaceInBytes</span></span>|<span data-ttu-id="a9d4b-274">Int64</span><span class="sxs-lookup"><span data-stu-id="a9d4b-274">Int64</span></span>|<span data-ttu-id="a9d4b-275">空き記憶域 (バイト)</span><span class="sxs-lookup"><span data-stu-id="a9d4b-275">Free Storage in Bytes</span></span>|
|<span data-ttu-id="a9d4b-276">managedDeviceName</span><span class="sxs-lookup"><span data-stu-id="a9d4b-276">managedDeviceName</span></span>|<span data-ttu-id="a9d4b-277">String</span><span class="sxs-lookup"><span data-stu-id="a9d4b-277">String</span></span>|<span data-ttu-id="a9d4b-278">デバイスを識別する名前が自動的に生成されます。</span><span class="sxs-lookup"><span data-stu-id="a9d4b-278">Automatically generated name to identify a device.</span></span> <span data-ttu-id="a9d4b-279">ユーザー フレンドリ名に上書きできます。</span><span class="sxs-lookup"><span data-stu-id="a9d4b-279">Can be overwritten to a user friendly name.</span></span>|
|<span data-ttu-id="a9d4b-280">partnerReportedThreatState</span><span class="sxs-lookup"><span data-stu-id="a9d4b-280">partnerReportedThreatState</span></span>|[<span data-ttu-id="a9d4b-281">managedDevicePartnerReportedHealthState</span><span class="sxs-lookup"><span data-stu-id="a9d4b-281">managedDevicePartnerReportedHealthState</span></span>](../resources/intune-devices-manageddevicepartnerreportedhealthstate.md)|<span data-ttu-id="a9d4b-282">Mobile Threat Defense パートナーがアカウントおよびデバイスで使用されている場合の、デバイスの脅威の状態を示します。</span><span class="sxs-lookup"><span data-stu-id="a9d4b-282">Indicates the threat state of a device when a Mobile Threat Defense partner is in use by the account and device.</span></span> <span data-ttu-id="a9d4b-283">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="a9d4b-283">Read Only.</span></span> <span data-ttu-id="a9d4b-284">可能な値は、`unknown`、`activated`、`deactivated`、`secured`、`lowSeverity`、`mediumSeverity`、`highSeverity`、`unresponsive`、`compromised`、`misconfigured` です。</span><span class="sxs-lookup"><span data-stu-id="a9d4b-284">Possible values are: `unknown`, `activated`, `deactivated`, `secured`, `lowSeverity`, `mediumSeverity`, `highSeverity`, `unresponsive`, `compromised`, `misconfigured`.</span></span>|



## <a name="response"></a><span data-ttu-id="a9d4b-285">応答</span><span class="sxs-lookup"><span data-stu-id="a9d4b-285">Response</span></span>
<span data-ttu-id="a9d4b-286">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [managedDevice](../resources/intune-devices-manageddevice.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="a9d4b-286">If successful, this method returns a `201 Created` response code and a [managedDevice](../resources/intune-devices-manageddevice.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a9d4b-287">例</span><span class="sxs-lookup"><span data-stu-id="a9d4b-287">Example</span></span>

### <a name="request"></a><span data-ttu-id="a9d4b-288">要求</span><span class="sxs-lookup"><span data-stu-id="a9d4b-288">Request</span></span>
<span data-ttu-id="a9d4b-289">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="a9d4b-289">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/users/{usersId}/managedDevices
Content-type: application/json
Content-length: 4656

{
  "@odata.type": "#microsoft.graph.managedDevice",
  "userId": "User Id value",
  "deviceName": "Device Name value",
  "managedDeviceOwnerType": "company",
  "deviceActionResults": [
    {
      "@odata.type": "microsoft.graph.deviceActionResult",
      "actionName": "Action Name value",
      "actionState": "pending",
      "startDateTime": "2016-12-31T23:58:46.7156189-08:00",
      "lastUpdatedDateTime": "2017-01-01T00:00:56.8321556-08:00"
    }
  ],
  "enrolledDateTime": "2016-12-31T23:59:43.797191-08:00",
  "lastSyncDateTime": "2017-01-01T00:02:49.3205976-08:00",
  "operatingSystem": "Operating System value",
  "complianceState": "compliant",
  "jailBroken": "Jail Broken value",
  "managementAgent": "mdm",
  "osVersion": "Os Version value",
  "easActivated": true,
  "easDeviceId": "Eas Device Id value",
  "easActivationDateTime": "2016-12-31T23:59:43.4878784-08:00",
  "azureADRegistered": true,
  "deviceEnrollmentType": "userEnrollment",
  "activationLockBypassCode": "Activation Lock Bypass Code value",
  "emailAddress": "Email Address value",
  "azureADDeviceId": "Azure ADDevice Id value",
  "deviceRegistrationState": "registered",
  "deviceCategoryDisplayName": "Device Category Display Name value",
  "isSupervised": true,
  "exchangeLastSuccessfulSyncDateTime": "2017-01-01T00:00:45.8803083-08:00",
  "exchangeAccessState": "unknown",
  "exchangeAccessStateReason": "unknown",
  "remoteAssistanceSessionUrl": "https://example.com/remoteAssistanceSessionUrl/",
  "remoteAssistanceSessionErrorDetails": "Remote Assistance Session Error Details value",
  "isEncrypted": true,
  "userPrincipalName": "User Principal Name value",
  "model": "Model value",
  "manufacturer": "Manufacturer value",
  "imei": "Imei value",
  "complianceGracePeriodExpirationDateTime": "2016-12-31T23:56:44.951111-08:00",
  "serialNumber": "Serial Number value",
  "phoneNumber": "Phone Number value",
  "androidSecurityPatchLevel": "Android Security Patch Level value",
  "userDisplayName": "User Display Name value",
  "configurationManagerClientEnabledFeatures": {
    "@odata.type": "microsoft.graph.configurationManagerClientEnabledFeatures",
    "inventory": true,
    "modernApps": true,
    "resourceAccess": true,
    "deviceConfiguration": true,
    "compliancePolicy": true,
    "windowsUpdateForBusiness": true
  },
  "wiFiMacAddress": "Wi Fi Mac Address value",
  "deviceHealthAttestationState": {
    "@odata.type": "microsoft.graph.deviceHealthAttestationState",
    "lastUpdateDateTime": "Last Update Date Time value",
    "contentNamespaceUrl": "https://example.com/contentNamespaceUrl/",
    "deviceHealthAttestationStatus": "Device Health Attestation Status value",
    "contentVersion": "Content Version value",
    "issuedDateTime": "2016-12-31T23:58:22.1231038-08:00",
    "attestationIdentityKey": "Attestation Identity Key value",
    "resetCount": 10,
    "restartCount": 12,
    "dataExcutionPolicy": "Data Excution Policy value",
    "bitLockerStatus": "Bit Locker Status value",
    "bootManagerVersion": "Boot Manager Version value",
    "codeIntegrityCheckVersion": "Code Integrity Check Version value",
    "secureBoot": "Secure Boot value",
    "bootDebugging": "Boot Debugging value",
    "operatingSystemKernelDebugging": "Operating System Kernel Debugging value",
    "codeIntegrity": "Code Integrity value",
    "testSigning": "Test Signing value",
    "safeMode": "Safe Mode value",
    "windowsPE": "Windows PE value",
    "earlyLaunchAntiMalwareDriverProtection": "Early Launch Anti Malware Driver Protection value",
    "virtualSecureMode": "Virtual Secure Mode value",
    "pcrHashAlgorithm": "Pcr Hash Algorithm value",
    "bootAppSecurityVersion": "Boot App Security Version value",
    "bootManagerSecurityVersion": "Boot Manager Security Version value",
    "tpmVersion": "Tpm Version value",
    "pcr0": "Pcr0 value",
    "secureBootConfigurationPolicyFingerPrint": "Secure Boot Configuration Policy Finger Print value",
    "codeIntegrityPolicy": "Code Integrity Policy value",
    "bootRevisionListInfo": "Boot Revision List Info value",
    "operatingSystemRevListInfo": "Operating System Rev List Info value",
    "healthStatusMismatchInfo": "Health Status Mismatch Info value",
    "healthAttestationSupportedStatus": "Health Attestation Supported Status value"
  },
  "subscriberCarrier": "Subscriber Carrier value",
  "meid": "Meid value",
  "totalStorageSpaceInBytes": 8,
  "freeStorageSpaceInBytes": 7,
  "managedDeviceName": "Managed Device Name value",
  "partnerReportedThreatState": "activated"
}
```

### <a name="response"></a><span data-ttu-id="a9d4b-290">応答</span><span class="sxs-lookup"><span data-stu-id="a9d4b-290">Response</span></span>
<span data-ttu-id="a9d4b-p113">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="a9d4b-p113">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 4705

{
  "@odata.type": "#microsoft.graph.managedDevice",
  "id": "705c034c-034c-705c-4c03-5c704c035c70",
  "userId": "User Id value",
  "deviceName": "Device Name value",
  "managedDeviceOwnerType": "company",
  "deviceActionResults": [
    {
      "@odata.type": "microsoft.graph.deviceActionResult",
      "actionName": "Action Name value",
      "actionState": "pending",
      "startDateTime": "2016-12-31T23:58:46.7156189-08:00",
      "lastUpdatedDateTime": "2017-01-01T00:00:56.8321556-08:00"
    }
  ],
  "enrolledDateTime": "2016-12-31T23:59:43.797191-08:00",
  "lastSyncDateTime": "2017-01-01T00:02:49.3205976-08:00",
  "operatingSystem": "Operating System value",
  "complianceState": "compliant",
  "jailBroken": "Jail Broken value",
  "managementAgent": "mdm",
  "osVersion": "Os Version value",
  "easActivated": true,
  "easDeviceId": "Eas Device Id value",
  "easActivationDateTime": "2016-12-31T23:59:43.4878784-08:00",
  "azureADRegistered": true,
  "deviceEnrollmentType": "userEnrollment",
  "activationLockBypassCode": "Activation Lock Bypass Code value",
  "emailAddress": "Email Address value",
  "azureADDeviceId": "Azure ADDevice Id value",
  "deviceRegistrationState": "registered",
  "deviceCategoryDisplayName": "Device Category Display Name value",
  "isSupervised": true,
  "exchangeLastSuccessfulSyncDateTime": "2017-01-01T00:00:45.8803083-08:00",
  "exchangeAccessState": "unknown",
  "exchangeAccessStateReason": "unknown",
  "remoteAssistanceSessionUrl": "https://example.com/remoteAssistanceSessionUrl/",
  "remoteAssistanceSessionErrorDetails": "Remote Assistance Session Error Details value",
  "isEncrypted": true,
  "userPrincipalName": "User Principal Name value",
  "model": "Model value",
  "manufacturer": "Manufacturer value",
  "imei": "Imei value",
  "complianceGracePeriodExpirationDateTime": "2016-12-31T23:56:44.951111-08:00",
  "serialNumber": "Serial Number value",
  "phoneNumber": "Phone Number value",
  "androidSecurityPatchLevel": "Android Security Patch Level value",
  "userDisplayName": "User Display Name value",
  "configurationManagerClientEnabledFeatures": {
    "@odata.type": "microsoft.graph.configurationManagerClientEnabledFeatures",
    "inventory": true,
    "modernApps": true,
    "resourceAccess": true,
    "deviceConfiguration": true,
    "compliancePolicy": true,
    "windowsUpdateForBusiness": true
  },
  "wiFiMacAddress": "Wi Fi Mac Address value",
  "deviceHealthAttestationState": {
    "@odata.type": "microsoft.graph.deviceHealthAttestationState",
    "lastUpdateDateTime": "Last Update Date Time value",
    "contentNamespaceUrl": "https://example.com/contentNamespaceUrl/",
    "deviceHealthAttestationStatus": "Device Health Attestation Status value",
    "contentVersion": "Content Version value",
    "issuedDateTime": "2016-12-31T23:58:22.1231038-08:00",
    "attestationIdentityKey": "Attestation Identity Key value",
    "resetCount": 10,
    "restartCount": 12,
    "dataExcutionPolicy": "Data Excution Policy value",
    "bitLockerStatus": "Bit Locker Status value",
    "bootManagerVersion": "Boot Manager Version value",
    "codeIntegrityCheckVersion": "Code Integrity Check Version value",
    "secureBoot": "Secure Boot value",
    "bootDebugging": "Boot Debugging value",
    "operatingSystemKernelDebugging": "Operating System Kernel Debugging value",
    "codeIntegrity": "Code Integrity value",
    "testSigning": "Test Signing value",
    "safeMode": "Safe Mode value",
    "windowsPE": "Windows PE value",
    "earlyLaunchAntiMalwareDriverProtection": "Early Launch Anti Malware Driver Protection value",
    "virtualSecureMode": "Virtual Secure Mode value",
    "pcrHashAlgorithm": "Pcr Hash Algorithm value",
    "bootAppSecurityVersion": "Boot App Security Version value",
    "bootManagerSecurityVersion": "Boot Manager Security Version value",
    "tpmVersion": "Tpm Version value",
    "pcr0": "Pcr0 value",
    "secureBootConfigurationPolicyFingerPrint": "Secure Boot Configuration Policy Finger Print value",
    "codeIntegrityPolicy": "Code Integrity Policy value",
    "bootRevisionListInfo": "Boot Revision List Info value",
    "operatingSystemRevListInfo": "Operating System Rev List Info value",
    "healthStatusMismatchInfo": "Health Status Mismatch Info value",
    "healthAttestationSupportedStatus": "Health Attestation Supported Status value"
  },
  "subscriberCarrier": "Subscriber Carrier value",
  "meid": "Meid value",
  "totalStorageSpaceInBytes": 8,
  "freeStorageSpaceInBytes": 7,
  "managedDeviceName": "Managed Device Name value",
  "partnerReportedThreatState": "activated"
}
```



