---
title: >
  managedDevice の更新
description: managedDevice オブジェクトのプロパティを更新します。
author: tfitzmac
ms.openlocfilehash: 85803f6d5474ecc0e0e2f05cf974d705d4d47737
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27358752"
---
# <a name="update-manageddevice"></a><span data-ttu-id="1f95a-103">managedDevice の更新
</span><span class="sxs-lookup"><span data-stu-id="1f95a-103">Update managedDevice</span></span>

> <span data-ttu-id="1f95a-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="1f95a-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="1f95a-105">[managedDevice](../resources/intune-devices-manageddevice.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="1f95a-105">Update the properties of a [managedDevice](../resources/intune-devices-manageddevice.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="1f95a-106">前提条件</span><span class="sxs-lookup"><span data-stu-id="1f95a-106">Prerequisites</span></span>
<span data-ttu-id="1f95a-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="1f95a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1f95a-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="1f95a-109">Permission type</span></span>|<span data-ttu-id="1f95a-110">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="1f95a-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1f95a-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="1f95a-111">Delegated (work or school account)</span></span>|<span data-ttu-id="1f95a-112">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1f95a-112">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="1f95a-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="1f95a-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1f95a-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="1f95a-114">Not supported.</span></span>|
|<span data-ttu-id="1f95a-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="1f95a-115">Application</span></span>|<span data-ttu-id="1f95a-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="1f95a-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="1f95a-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="1f95a-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /users/{usersId}/managedDevices/{managedDeviceId}
PATCH /deviceManagement/managedDevices/{managedDeviceId}
PATCH /deviceManagement/detectedApps/{detectedAppId}/managedDevices/{managedDeviceId}
```

## <a name="request-headers"></a><span data-ttu-id="1f95a-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="1f95a-118">Request headers</span></span>
|<span data-ttu-id="1f95a-119">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="1f95a-119">Header</span></span>|<span data-ttu-id="1f95a-120">値</span><span class="sxs-lookup"><span data-stu-id="1f95a-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1f95a-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="1f95a-121">Authorization</span></span>|<span data-ttu-id="1f95a-122">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="1f95a-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1f95a-123">Accept</span><span class="sxs-lookup"><span data-stu-id="1f95a-123">Accept</span></span>|<span data-ttu-id="1f95a-124">application/json</span><span class="sxs-lookup"><span data-stu-id="1f95a-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1f95a-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="1f95a-125">Request body</span></span>
<span data-ttu-id="1f95a-126">要求本文で、[managedDevice](../resources/intune-devices-manageddevice.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="1f95a-126">In the request body, supply a JSON representation for the [managedDevice](../resources/intune-devices-manageddevice.md) object.</span></span>

<span data-ttu-id="1f95a-127">次の表に、[managedDevice](../resources/intune-devices-manageddevice.md) の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="1f95a-127">The following table shows the properties that are required when you create the [managedDevice](../resources/intune-devices-manageddevice.md).</span></span>

|<span data-ttu-id="1f95a-128">プロパティ</span><span class="sxs-lookup"><span data-stu-id="1f95a-128">Property</span></span>|<span data-ttu-id="1f95a-129">種類</span><span class="sxs-lookup"><span data-stu-id="1f95a-129">Type</span></span>|<span data-ttu-id="1f95a-130">説明</span><span class="sxs-lookup"><span data-stu-id="1f95a-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1f95a-131">ID</span><span class="sxs-lookup"><span data-stu-id="1f95a-131">id</span></span>|<span data-ttu-id="1f95a-132">String</span><span class="sxs-lookup"><span data-stu-id="1f95a-132">String</span></span>|<span data-ttu-id="1f95a-133">デバイスの一意識別子</span><span class="sxs-lookup"><span data-stu-id="1f95a-133">Unique Identifier for the device</span></span>|
|<span data-ttu-id="1f95a-134">userId</span><span class="sxs-lookup"><span data-stu-id="1f95a-134">userId</span></span>|<span data-ttu-id="1f95a-135">String</span><span class="sxs-lookup"><span data-stu-id="1f95a-135">String</span></span>|<span data-ttu-id="1f95a-136">デバイスに関連付けられているユーザーの一意の識別子</span><span class="sxs-lookup"><span data-stu-id="1f95a-136">Unique Identifier for the user associated with the device</span></span>|
|<span data-ttu-id="1f95a-137">deviceName</span><span class="sxs-lookup"><span data-stu-id="1f95a-137">deviceName</span></span>|<span data-ttu-id="1f95a-138">String</span><span class="sxs-lookup"><span data-stu-id="1f95a-138">String</span></span>|<span data-ttu-id="1f95a-139">デバイスの名前</span><span class="sxs-lookup"><span data-stu-id="1f95a-139">Name of the device</span></span>|
|<span data-ttu-id="1f95a-140">managedDeviceOwnerType</span><span class="sxs-lookup"><span data-stu-id="1f95a-140">managedDeviceOwnerType</span></span>|[<span data-ttu-id="1f95a-141">managedDeviceOwnerType</span><span class="sxs-lookup"><span data-stu-id="1f95a-141">managedDeviceOwnerType</span></span>](../resources/intune-devices-manageddeviceownertype.md)|<span data-ttu-id="1f95a-142">デバイスの所有権。</span><span class="sxs-lookup"><span data-stu-id="1f95a-142">Ownership of the device.</span></span> <span data-ttu-id="1f95a-143">'会社' または '個人' にすることができます。</span><span class="sxs-lookup"><span data-stu-id="1f95a-143">Can be 'company' or 'personal'.</span></span> <span data-ttu-id="1f95a-144">可能な値は、`unknown`、`company`、`personal` です。</span><span class="sxs-lookup"><span data-stu-id="1f95a-144">Possible values are: `unknown`, `company`, `personal`.</span></span>|
|<span data-ttu-id="1f95a-145">deviceActionResults</span><span class="sxs-lookup"><span data-stu-id="1f95a-145">deviceActionResults</span></span>|<span data-ttu-id="1f95a-146">[deviceActionResult](../resources/intune-devices-deviceactionresult.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="1f95a-146">[deviceActionResult](../resources/intune-devices-deviceactionresult.md) collection</span></span>|<span data-ttu-id="1f95a-147">ComplexType deviceActionResult オブジェクトのリスト。</span><span class="sxs-lookup"><span data-stu-id="1f95a-147">List of ComplexType deviceActionResult objects.</span></span>|
|<span data-ttu-id="1f95a-148">enrolledDateTime</span><span class="sxs-lookup"><span data-stu-id="1f95a-148">enrolledDateTime</span></span>|<span data-ttu-id="1f95a-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1f95a-149">DateTimeOffset</span></span>|<span data-ttu-id="1f95a-150">デバイスの登録時刻。</span><span class="sxs-lookup"><span data-stu-id="1f95a-150">Enrollment time of the device.</span></span>|
|<span data-ttu-id="1f95a-151">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="1f95a-151">lastSyncDateTime</span></span>|<span data-ttu-id="1f95a-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1f95a-152">DateTimeOffset</span></span>|<span data-ttu-id="1f95a-153">デバイスが Intune との正常な同期を最終的に完了した日時。</span><span class="sxs-lookup"><span data-stu-id="1f95a-153">The date and time that the device last completed a successful sync with Intune.</span></span>|
|<span data-ttu-id="1f95a-154">operatingSystem</span><span class="sxs-lookup"><span data-stu-id="1f95a-154">operatingSystem</span></span>|<span data-ttu-id="1f95a-155">String</span><span class="sxs-lookup"><span data-stu-id="1f95a-155">String</span></span>|<span data-ttu-id="1f95a-156">デバイスのオペレーティング システム。</span><span class="sxs-lookup"><span data-stu-id="1f95a-156">Operating system of the device.</span></span> <span data-ttu-id="1f95a-157">Windows、iOS など。</span><span class="sxs-lookup"><span data-stu-id="1f95a-157">Windows, iOS, etc.</span></span>|
|<span data-ttu-id="1f95a-158">complianceState</span><span class="sxs-lookup"><span data-stu-id="1f95a-158">complianceState</span></span>|[<span data-ttu-id="1f95a-159">complianceState</span><span class="sxs-lookup"><span data-stu-id="1f95a-159">complianceState</span></span>](../resources/intune-devices-compliancestate.md)|<span data-ttu-id="1f95a-160">デバイスのコンプライアンス状態。</span><span class="sxs-lookup"><span data-stu-id="1f95a-160">Compliance state of the device.</span></span> <span data-ttu-id="1f95a-161">可能な値は、`unknown`、`compliant`、`noncompliant`、`conflict`、`error`、`inGracePeriod`、`configManager` です。</span><span class="sxs-lookup"><span data-stu-id="1f95a-161">Possible values are: `unknown`, `compliant`, `noncompliant`, `conflict`, `error`, `inGracePeriod`, `configManager`.</span></span>|
|<span data-ttu-id="1f95a-162">jailBroken</span><span class="sxs-lookup"><span data-stu-id="1f95a-162">jailBroken</span></span>|<span data-ttu-id="1f95a-163">String</span><span class="sxs-lookup"><span data-stu-id="1f95a-163">String</span></span>|<span data-ttu-id="1f95a-164">デバイスが脱獄またはルート化されているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="1f95a-164">whether the device is jail broken or rooted.</span></span>|
|<span data-ttu-id="1f95a-165">managementAgent</span><span class="sxs-lookup"><span data-stu-id="1f95a-165">managementAgent</span></span>|[<span data-ttu-id="1f95a-166">managementAgentType</span><span class="sxs-lookup"><span data-stu-id="1f95a-166">managementAgentType</span></span>](../resources/intune-devices-managementagenttype.md)|<span data-ttu-id="1f95a-167">デバイスの管理チャネル。</span><span class="sxs-lookup"><span data-stu-id="1f95a-167">Management channel of the device.</span></span> <span data-ttu-id="1f95a-168">Intune、EAS など。可能な値は、`eas`、`mdm`、`easMdm`、`intuneClient`、`easIntuneClient`、`configurationManagerClient`、`configurationManagerClientMdm`、`configurationManagerClientMdmEas`、`unknown`、`jamf`、`googleCloudDevicePolicyController` です。</span><span class="sxs-lookup"><span data-stu-id="1f95a-168">Intune, EAS, etc. Possible values are: `eas`, `mdm`, `easMdm`, `intuneClient`, `easIntuneClient`, `configurationManagerClient`, `configurationManagerClientMdm`, `configurationManagerClientMdmEas`, `unknown`, `jamf`, `googleCloudDevicePolicyController`.</span></span>|
|<span data-ttu-id="1f95a-169">osVersion</span><span class="sxs-lookup"><span data-stu-id="1f95a-169">osVersion</span></span>|<span data-ttu-id="1f95a-170">String</span><span class="sxs-lookup"><span data-stu-id="1f95a-170">String</span></span>|<span data-ttu-id="1f95a-171">デバイスのオペレーティング システムのバージョン。</span><span class="sxs-lookup"><span data-stu-id="1f95a-171">Operating system version of the device.</span></span>|
|<span data-ttu-id="1f95a-172">easActivated</span><span class="sxs-lookup"><span data-stu-id="1f95a-172">easActivated</span></span>|<span data-ttu-id="1f95a-173">Boolean</span><span class="sxs-lookup"><span data-stu-id="1f95a-173">Boolean</span></span>|<span data-ttu-id="1f95a-174">Exchange ActiveSync がアクティブになっているデバイスかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="1f95a-174">Whether the device is Exchange ActiveSync activated.</span></span>|
|<span data-ttu-id="1f95a-175">easDeviceId</span><span class="sxs-lookup"><span data-stu-id="1f95a-175">easDeviceId</span></span>|<span data-ttu-id="1f95a-176">String</span><span class="sxs-lookup"><span data-stu-id="1f95a-176">String</span></span>|<span data-ttu-id="1f95a-177">デバイスの Exchange ActiveSync の ID。</span><span class="sxs-lookup"><span data-stu-id="1f95a-177">Exchange ActiveSync Id of the device.</span></span>|
|<span data-ttu-id="1f95a-178">easActivationDateTime</span><span class="sxs-lookup"><span data-stu-id="1f95a-178">easActivationDateTime</span></span>|<span data-ttu-id="1f95a-179">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1f95a-179">DateTimeOffset</span></span>|<span data-ttu-id="1f95a-180">デバイスの Exchange ActivationSync のアクティブ化の時刻。</span><span class="sxs-lookup"><span data-stu-id="1f95a-180">Exchange ActivationSync activation time of the device.</span></span>|
|<span data-ttu-id="1f95a-181">azureADRegistered</span><span class="sxs-lookup"><span data-stu-id="1f95a-181">azureADRegistered</span></span>|<span data-ttu-id="1f95a-182">Boolean</span><span class="sxs-lookup"><span data-stu-id="1f95a-182">Boolean</span></span>|<span data-ttu-id="1f95a-183">Azure Active Directory が登録されているデバイスかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="1f95a-183">Whether the device is Azure Active Directory registered.</span></span>|
|<span data-ttu-id="1f95a-184">deviceEnrollmentType</span><span class="sxs-lookup"><span data-stu-id="1f95a-184">deviceEnrollmentType</span></span>|[<span data-ttu-id="1f95a-185">deviceEnrollmentType</span><span class="sxs-lookup"><span data-stu-id="1f95a-185">deviceEnrollmentType</span></span>](../resources/intune-devices-deviceenrollmenttype.md)|<span data-ttu-id="1f95a-186">デバイスの登録の種類。</span><span class="sxs-lookup"><span data-stu-id="1f95a-186">Enrollment type of the device.</span></span> <span data-ttu-id="1f95a-187">可能な値は、`unknown`、`userEnrollment`、`deviceEnrollmentManager`、`appleBulkWithUser`、`appleBulkWithoutUser`、`windowsAzureADJoin`、`windowsBulkUserless`、`windowsAutoEnrollment`、`windowsBulkAzureDomainJoin`、`windowsCoManagement` です。</span><span class="sxs-lookup"><span data-stu-id="1f95a-187">Possible values are: `unknown`, `userEnrollment`, `deviceEnrollmentManager`, `appleBulkWithUser`, `appleBulkWithoutUser`, `windowsAzureADJoin`, `windowsBulkUserless`, `windowsAutoEnrollment`, `windowsBulkAzureDomainJoin`, `windowsCoManagement`.</span></span>|
|<span data-ttu-id="1f95a-188">activationLockBypassCode</span><span class="sxs-lookup"><span data-stu-id="1f95a-188">activationLockBypassCode</span></span>|<span data-ttu-id="1f95a-189">String</span><span class="sxs-lookup"><span data-stu-id="1f95a-189">String</span></span>|<span data-ttu-id="1f95a-190">デバイスのアクティベーション ロックをバイパスするためのコード。</span><span class="sxs-lookup"><span data-stu-id="1f95a-190">Code that allows the Activation Lock on a device to be bypassed.</span></span>|
|<span data-ttu-id="1f95a-191">emailAddress</span><span class="sxs-lookup"><span data-stu-id="1f95a-191">emailAddress</span></span>|<span data-ttu-id="1f95a-192">String</span><span class="sxs-lookup"><span data-stu-id="1f95a-192">String</span></span>|<span data-ttu-id="1f95a-193">デバイスに関連付けられているユーザーの電子メール</span><span class="sxs-lookup"><span data-stu-id="1f95a-193">Email(s) for the user associated with the device</span></span>|
|<span data-ttu-id="1f95a-194">azureADDeviceId</span><span class="sxs-lookup"><span data-stu-id="1f95a-194">azureADDeviceId</span></span>|<span data-ttu-id="1f95a-195">String</span><span class="sxs-lookup"><span data-stu-id="1f95a-195">String</span></span>|<span data-ttu-id="1f95a-196">Azure Active Directory デバイスの一意識別子。</span><span class="sxs-lookup"><span data-stu-id="1f95a-196">The unique identifier for the Azure Active Directory device.</span></span> <span data-ttu-id="1f95a-197">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="1f95a-197">Read only.</span></span>|
|<span data-ttu-id="1f95a-198">deviceRegistrationState</span><span class="sxs-lookup"><span data-stu-id="1f95a-198">deviceRegistrationState</span></span>|[<span data-ttu-id="1f95a-199">deviceRegistrationState</span><span class="sxs-lookup"><span data-stu-id="1f95a-199">deviceRegistrationState</span></span>](../resources/intune-devices-deviceregistrationstate.md)|<span data-ttu-id="1f95a-200">デバイスの登録状態。</span><span class="sxs-lookup"><span data-stu-id="1f95a-200">Device registration state.</span></span> <span data-ttu-id="1f95a-201">可能な値は、`notRegistered`、`registered`、`revoked`、`keyConflict`、`approvalPending`、`certificateReset`、`notRegisteredPendingEnrollment`、`unknown` です。</span><span class="sxs-lookup"><span data-stu-id="1f95a-201">Possible values are: `notRegistered`, `registered`, `revoked`, `keyConflict`, `approvalPending`, `certificateReset`, `notRegisteredPendingEnrollment`, `unknown`.</span></span>|
|<span data-ttu-id="1f95a-202">deviceCategoryDisplayName</span><span class="sxs-lookup"><span data-stu-id="1f95a-202">deviceCategoryDisplayName</span></span>|<span data-ttu-id="1f95a-203">String</span><span class="sxs-lookup"><span data-stu-id="1f95a-203">String</span></span>|<span data-ttu-id="1f95a-204">デバイス カテゴリの表示名</span><span class="sxs-lookup"><span data-stu-id="1f95a-204">Device category display name</span></span>|
|<span data-ttu-id="1f95a-205">isSupervised</span><span class="sxs-lookup"><span data-stu-id="1f95a-205">isSupervised</span></span>|<span data-ttu-id="1f95a-206">Boolean</span><span class="sxs-lookup"><span data-stu-id="1f95a-206">Boolean</span></span>|<span data-ttu-id="1f95a-207">デバイスの管理状況</span><span class="sxs-lookup"><span data-stu-id="1f95a-207">Device supervised status</span></span>|
|<span data-ttu-id="1f95a-208">exchangeLastSuccessfulSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="1f95a-208">exchangeLastSuccessfulSyncDateTime</span></span>|<span data-ttu-id="1f95a-209">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1f95a-209">DateTimeOffset</span></span>|<span data-ttu-id="1f95a-210">最後にデバイスが Exchange に接続した時刻。</span><span class="sxs-lookup"><span data-stu-id="1f95a-210">Last time the device contacted Exchange.</span></span>|
|<span data-ttu-id="1f95a-211">exchangeAccessState</span><span class="sxs-lookup"><span data-stu-id="1f95a-211">exchangeAccessState</span></span>|[<span data-ttu-id="1f95a-212">deviceManagementExchangeAccessState</span><span class="sxs-lookup"><span data-stu-id="1f95a-212">deviceManagementExchangeAccessState</span></span>](../resources/intune-devices-devicemanagementexchangeaccessstate.md)|<span data-ttu-id="1f95a-213">Exchange でのデバイスのアクセスの状態。</span><span class="sxs-lookup"><span data-stu-id="1f95a-213">The Access State of the device in Exchange.</span></span> <span data-ttu-id="1f95a-214">可能な値は、`none`、`unknown`、`allowed`、`blocked`、`quarantined` です。</span><span class="sxs-lookup"><span data-stu-id="1f95a-214">Possible values are: `none`, `unknown`, `allowed`, `blocked`, `quarantined`.</span></span>|
|<span data-ttu-id="1f95a-215">exchangeAccessStateReason</span><span class="sxs-lookup"><span data-stu-id="1f95a-215">exchangeAccessStateReason</span></span>|[<span data-ttu-id="1f95a-216">deviceManagementExchangeAccessStateReason</span><span class="sxs-lookup"><span data-stu-id="1f95a-216">deviceManagementExchangeAccessStateReason</span></span>](../resources/intune-devices-devicemanagementexchangeaccessstatereason.md)|<span data-ttu-id="1f95a-217">Exchange でのデバイスのアクセス状態の理由。
</span><span class="sxs-lookup"><span data-stu-id="1f95a-217">The reason for the device's access state in Exchange.</span></span> <span data-ttu-id="1f95a-218">可能な値は、`none`、`unknown`、`exchangeGlobalRule`、`exchangeIndividualRule`、`exchangeDeviceRule`、`exchangeUpgrade`、`exchangeMailboxPolicy`、`other`、`compliant`、`notCompliant`、`notEnrolled`、`unknownLocation`、`mfaRequired`、`azureADBlockDueToAccessPolicy`、`compromisedPassword`、`deviceNotKnownWithManagedApp` です。</span><span class="sxs-lookup"><span data-stu-id="1f95a-218">Possible values are: `none`, `unknown`, `exchangeGlobalRule`, `exchangeIndividualRule`, `exchangeDeviceRule`, `exchangeUpgrade`, `exchangeMailboxPolicy`, `other`, `compliant`, `notCompliant`, `notEnrolled`, `unknownLocation`, `mfaRequired`, `azureADBlockDueToAccessPolicy`, `compromisedPassword`, `deviceNotKnownWithManagedApp`.</span></span>|
|<span data-ttu-id="1f95a-219">remoteAssistanceSessionUrl</span><span class="sxs-lookup"><span data-stu-id="1f95a-219">remoteAssistanceSessionUrl</span></span>|<span data-ttu-id="1f95a-220">String</span><span class="sxs-lookup"><span data-stu-id="1f95a-220">String</span></span>|<span data-ttu-id="1f95a-221">デバイスとのリモート アシスタンス セッションを確立できるようにする URL。</span><span class="sxs-lookup"><span data-stu-id="1f95a-221">Url that allows a Remote Assistance session to be established with the device.</span></span>|
|<span data-ttu-id="1f95a-222">remoteAssistanceSessionErrorDetails</span><span class="sxs-lookup"><span data-stu-id="1f95a-222">remoteAssistanceSessionErrorDetails</span></span>|<span data-ttu-id="1f95a-223">String</span><span class="sxs-lookup"><span data-stu-id="1f95a-223">String</span></span>|<span data-ttu-id="1f95a-224">リモート アシスタンス セッション オブジェクトの作成時に問題を識別するエラー文字列。</span><span class="sxs-lookup"><span data-stu-id="1f95a-224">An error string that identifies issues when creating Remote Assistance session objects.</span></span>|
|<span data-ttu-id="1f95a-225">isEncrypted</span><span class="sxs-lookup"><span data-stu-id="1f95a-225">isEncrypted</span></span>|<span data-ttu-id="1f95a-226">Boolean</span><span class="sxs-lookup"><span data-stu-id="1f95a-226">Boolean</span></span>|<span data-ttu-id="1f95a-227">デバイスの暗号化の状態</span><span class="sxs-lookup"><span data-stu-id="1f95a-227">Device encryption status</span></span>|
|<span data-ttu-id="1f95a-228">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="1f95a-228">userPrincipalName</span></span>|<span data-ttu-id="1f95a-229">String</span><span class="sxs-lookup"><span data-stu-id="1f95a-229">String</span></span>|<span data-ttu-id="1f95a-230">デバイスのユーザー プリンシパル名。</span><span class="sxs-lookup"><span data-stu-id="1f95a-230">Device user principal name</span></span>|
|<span data-ttu-id="1f95a-231">model</span><span class="sxs-lookup"><span data-stu-id="1f95a-231">model</span></span>|<span data-ttu-id="1f95a-232">String</span><span class="sxs-lookup"><span data-stu-id="1f95a-232">String</span></span>|<span data-ttu-id="1f95a-233">デバイスのモデル</span><span class="sxs-lookup"><span data-stu-id="1f95a-233">Model of the device</span></span>|
|<span data-ttu-id="1f95a-234">manufacturer</span><span class="sxs-lookup"><span data-stu-id="1f95a-234">manufacturer</span></span>|<span data-ttu-id="1f95a-235">String</span><span class="sxs-lookup"><span data-stu-id="1f95a-235">String</span></span>|<span data-ttu-id="1f95a-236">デバイスのメーカー</span><span class="sxs-lookup"><span data-stu-id="1f95a-236">Manufacturer of the device</span></span>|
|<span data-ttu-id="1f95a-237">imei</span><span class="sxs-lookup"><span data-stu-id="1f95a-237">imei</span></span>|<span data-ttu-id="1f95a-238">String</span><span class="sxs-lookup"><span data-stu-id="1f95a-238">String</span></span>|<span data-ttu-id="1f95a-239">IMEI</span><span class="sxs-lookup"><span data-stu-id="1f95a-239">IMEI</span></span>|
|<span data-ttu-id="1f95a-240">complianceGracePeriodExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="1f95a-240">complianceGracePeriodExpirationDateTime</span></span>|<span data-ttu-id="1f95a-241">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1f95a-241">DateTimeOffset</span></span>|<span data-ttu-id="1f95a-242">デバイス コンプライアンスの猶予期間が経過する DateTime</span><span class="sxs-lookup"><span data-stu-id="1f95a-242">The DateTime when device compliance grace period expires</span></span>|
|<span data-ttu-id="1f95a-243">serialNumber</span><span class="sxs-lookup"><span data-stu-id="1f95a-243">serialNumber</span></span>|<span data-ttu-id="1f95a-244">String</span><span class="sxs-lookup"><span data-stu-id="1f95a-244">String</span></span>|<span data-ttu-id="1f95a-245">シリアル番号</span><span class="sxs-lookup"><span data-stu-id="1f95a-245">SerialNumber</span></span>|
|<span data-ttu-id="1f95a-246">phoneNumber</span><span class="sxs-lookup"><span data-stu-id="1f95a-246">phoneNumber</span></span>|<span data-ttu-id="1f95a-247">String</span><span class="sxs-lookup"><span data-stu-id="1f95a-247">String</span></span>|<span data-ttu-id="1f95a-248">デバイスの電話番号</span><span class="sxs-lookup"><span data-stu-id="1f95a-248">Phone number of the device</span></span>|
|<span data-ttu-id="1f95a-249">androidSecurityPatchLevel</span><span class="sxs-lookup"><span data-stu-id="1f95a-249">androidSecurityPatchLevel</span></span>|<span data-ttu-id="1f95a-250">String</span><span class="sxs-lookup"><span data-stu-id="1f95a-250">String</span></span>|<span data-ttu-id="1f95a-251">Android セキュリティ パッチのレベル</span><span class="sxs-lookup"><span data-stu-id="1f95a-251">Android security patch level</span></span>|
|<span data-ttu-id="1f95a-252">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="1f95a-252">userDisplayName</span></span>|<span data-ttu-id="1f95a-253">String</span><span class="sxs-lookup"><span data-stu-id="1f95a-253">String</span></span>|<span data-ttu-id="1f95a-254">ユーザーの表示名</span><span class="sxs-lookup"><span data-stu-id="1f95a-254">User display name</span></span>|
|<span data-ttu-id="1f95a-255">configurationManagerClientEnabledFeatures</span><span class="sxs-lookup"><span data-stu-id="1f95a-255">configurationManagerClientEnabledFeatures</span></span>|[<span data-ttu-id="1f95a-256">configurationManagerClientEnabledFeatures</span><span class="sxs-lookup"><span data-stu-id="1f95a-256">configurationManagerClientEnabledFeatures</span></span>](../resources/intune-devices-configurationmanagerclientenabledfeatures.md)|<span data-ttu-id="1f95a-257">ConfigrMgr クライアント対応機能
</span><span class="sxs-lookup"><span data-stu-id="1f95a-257">ConfigrMgr client enabled features</span></span>|
|<span data-ttu-id="1f95a-258">wiFiMacAddress</span><span class="sxs-lookup"><span data-stu-id="1f95a-258">wiFiMacAddress</span></span>|<span data-ttu-id="1f95a-259">String</span><span class="sxs-lookup"><span data-stu-id="1f95a-259">String</span></span>|<span data-ttu-id="1f95a-260">Wi-Fi MAC</span><span class="sxs-lookup"><span data-stu-id="1f95a-260">Wi-Fi MAC</span></span>|
|<span data-ttu-id="1f95a-261">deviceHealthAttestationState</span><span class="sxs-lookup"><span data-stu-id="1f95a-261">deviceHealthAttestationState</span></span>|[<span data-ttu-id="1f95a-262">deviceHealthAttestationState</span><span class="sxs-lookup"><span data-stu-id="1f95a-262">deviceHealthAttestationState</span></span>](../resources/intune-devices-devicehealthattestationstate.md)|<span data-ttu-id="1f95a-263">デバイスの正常性構成証明の状態。</span><span class="sxs-lookup"><span data-stu-id="1f95a-263">The device health attestation state.</span></span>|
|<span data-ttu-id="1f95a-264">subscriberCarrier</span><span class="sxs-lookup"><span data-stu-id="1f95a-264">subscriberCarrier</span></span>|<span data-ttu-id="1f95a-265">String</span><span class="sxs-lookup"><span data-stu-id="1f95a-265">String</span></span>|<span data-ttu-id="1f95a-266">サブスクライバー通信事業者</span><span class="sxs-lookup"><span data-stu-id="1f95a-266">Subscriber Carrier</span></span>|
|<span data-ttu-id="1f95a-267">meid</span><span class="sxs-lookup"><span data-stu-id="1f95a-267">meid</span></span>|<span data-ttu-id="1f95a-268">String</span><span class="sxs-lookup"><span data-stu-id="1f95a-268">String</span></span>|<span data-ttu-id="1f95a-269">MEID</span><span class="sxs-lookup"><span data-stu-id="1f95a-269">MEID</span></span>|
|<span data-ttu-id="1f95a-270">totalStorageSpaceInBytes</span><span class="sxs-lookup"><span data-stu-id="1f95a-270">totalStorageSpaceInBytes</span></span>|<span data-ttu-id="1f95a-271">Int64</span><span class="sxs-lookup"><span data-stu-id="1f95a-271">Int64</span></span>|<span data-ttu-id="1f95a-272">記憶域の合計 (バイト)</span><span class="sxs-lookup"><span data-stu-id="1f95a-272">Total Storage in Bytes</span></span>|
|<span data-ttu-id="1f95a-273">freeStorageSpaceInBytes</span><span class="sxs-lookup"><span data-stu-id="1f95a-273">freeStorageSpaceInBytes</span></span>|<span data-ttu-id="1f95a-274">Int64</span><span class="sxs-lookup"><span data-stu-id="1f95a-274">Int64</span></span>|<span data-ttu-id="1f95a-275">空き記憶域 (バイト)</span><span class="sxs-lookup"><span data-stu-id="1f95a-275">Free Storage in Bytes</span></span>|
|<span data-ttu-id="1f95a-276">managedDeviceName</span><span class="sxs-lookup"><span data-stu-id="1f95a-276">managedDeviceName</span></span>|<span data-ttu-id="1f95a-277">String</span><span class="sxs-lookup"><span data-stu-id="1f95a-277">String</span></span>|<span data-ttu-id="1f95a-278">デバイスを識別する名前が自動的に生成されます。</span><span class="sxs-lookup"><span data-stu-id="1f95a-278">Automatically generated name to identify a device.</span></span> <span data-ttu-id="1f95a-279">ユーザー フレンドリ名に上書きできます。</span><span class="sxs-lookup"><span data-stu-id="1f95a-279">Can be overwritten to a user friendly name.</span></span>|
|<span data-ttu-id="1f95a-280">partnerReportedThreatState</span><span class="sxs-lookup"><span data-stu-id="1f95a-280">partnerReportedThreatState</span></span>|[<span data-ttu-id="1f95a-281">managedDevicePartnerReportedHealthState</span><span class="sxs-lookup"><span data-stu-id="1f95a-281">managedDevicePartnerReportedHealthState</span></span>](../resources/intune-devices-manageddevicepartnerreportedhealthstate.md)|<span data-ttu-id="1f95a-282">Mobile Threat Defense パートナーがアカウントおよびデバイスで使用されている場合の、デバイスの脅威の状態を示します。</span><span class="sxs-lookup"><span data-stu-id="1f95a-282">Indicates the threat state of a device when a Mobile Threat Defense partner is in use by the account and device.</span></span> <span data-ttu-id="1f95a-283">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="1f95a-283">Read Only.</span></span> <span data-ttu-id="1f95a-284">可能な値は、`unknown`、`activated`、`deactivated`、`secured`、`lowSeverity`、`mediumSeverity`、`highSeverity`、`unresponsive`、`compromised`、`misconfigured` です。</span><span class="sxs-lookup"><span data-stu-id="1f95a-284">Possible values are: `unknown`, `activated`, `deactivated`, `secured`, `lowSeverity`, `mediumSeverity`, `highSeverity`, `unresponsive`, `compromised`, `misconfigured`.</span></span>|



## <a name="response"></a><span data-ttu-id="1f95a-285">応答</span><span class="sxs-lookup"><span data-stu-id="1f95a-285">Response</span></span>
<span data-ttu-id="1f95a-286">成功した場合、このメソッドは `200 OK` 応答コードと、更新された [managedDevice](../resources/intune-devices-manageddevice.md) オブジェクトを応答本文で返します。</span><span class="sxs-lookup"><span data-stu-id="1f95a-286">If successful, this method returns a `200 OK` response code and an updated [managedDevice](../resources/intune-devices-manageddevice.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1f95a-287">例</span><span class="sxs-lookup"><span data-stu-id="1f95a-287">Example</span></span>
### <a name="request"></a><span data-ttu-id="1f95a-288">要求</span><span class="sxs-lookup"><span data-stu-id="1f95a-288">Request</span></span>
<span data-ttu-id="1f95a-289">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="1f95a-289">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/users/{usersId}/managedDevices/{managedDeviceId}
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

### <a name="response"></a><span data-ttu-id="1f95a-290">応答</span><span class="sxs-lookup"><span data-stu-id="1f95a-290">Response</span></span>
<span data-ttu-id="1f95a-p113">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="1f95a-p113">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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


