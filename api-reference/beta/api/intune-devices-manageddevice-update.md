---
title: >
  managedDevice の更新
description: managedDevice オブジェクトのプロパティを更新します。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: c86557fe2f80b8a61a1905d157ebce3eb7251f2a
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35987125"
---
# <a name="update-manageddevice"></a><span data-ttu-id="985ea-103">managedDevice の更新
</span><span class="sxs-lookup"><span data-stu-id="985ea-103">Update managedDevice</span></span>

> <span data-ttu-id="985ea-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="985ea-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="985ea-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="985ea-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="985ea-106">[managedDevice](../resources/intune-devices-manageddevice.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="985ea-106">Update the properties of a [managedDevice](../resources/intune-devices-manageddevice.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="985ea-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="985ea-107">Prerequisites</span></span>
<span data-ttu-id="985ea-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="985ea-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="985ea-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="985ea-110">Permission type</span></span>|<span data-ttu-id="985ea-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="985ea-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="985ea-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="985ea-112">Delegated (work or school account)</span></span>|<span data-ttu-id="985ea-113">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="985ea-113">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="985ea-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="985ea-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="985ea-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="985ea-115">Not supported.</span></span>|
|<span data-ttu-id="985ea-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="985ea-116">Application</span></span>|<span data-ttu-id="985ea-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="985ea-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="985ea-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="985ea-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/managedDevices/{managedDeviceId}
PATCH /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice
PATCH /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/users/{userId}/managedDevices/{managedDeviceId}
PATCH /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/detectedApps/{detectedAppId}/managedDevices/{managedDeviceId}
```

## <a name="request-headers"></a><span data-ttu-id="985ea-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="985ea-119">Request headers</span></span>
|<span data-ttu-id="985ea-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="985ea-120">Header</span></span>|<span data-ttu-id="985ea-121">値</span><span class="sxs-lookup"><span data-stu-id="985ea-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="985ea-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="985ea-122">Authorization</span></span>|<span data-ttu-id="985ea-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="985ea-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="985ea-124">承諾</span><span class="sxs-lookup"><span data-stu-id="985ea-124">Accept</span></span>|<span data-ttu-id="985ea-125">application/json</span><span class="sxs-lookup"><span data-stu-id="985ea-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="985ea-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="985ea-126">Request body</span></span>
<span data-ttu-id="985ea-127">要求本文で、[managedDevice](../resources/intune-devices-manageddevice.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="985ea-127">In the request body, supply a JSON representation for the [managedDevice](../resources/intune-devices-manageddevice.md) object.</span></span>

<span data-ttu-id="985ea-128">次の表に、[managedDevice](../resources/intune-devices-manageddevice.md) の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="985ea-128">The following table shows the properties that are required when you create the [managedDevice](../resources/intune-devices-manageddevice.md).</span></span>

|<span data-ttu-id="985ea-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="985ea-129">Property</span></span>|<span data-ttu-id="985ea-130">型</span><span class="sxs-lookup"><span data-stu-id="985ea-130">Type</span></span>|<span data-ttu-id="985ea-131">説明</span><span class="sxs-lookup"><span data-stu-id="985ea-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="985ea-132">id</span><span class="sxs-lookup"><span data-stu-id="985ea-132">id</span></span>|<span data-ttu-id="985ea-133">文字列</span><span class="sxs-lookup"><span data-stu-id="985ea-133">String</span></span>|<span data-ttu-id="985ea-134">デバイスの一意識別子</span><span class="sxs-lookup"><span data-stu-id="985ea-134">Unique Identifier for the device</span></span>|
|<span data-ttu-id="985ea-135">userId</span><span class="sxs-lookup"><span data-stu-id="985ea-135">userId</span></span>|<span data-ttu-id="985ea-136">String</span><span class="sxs-lookup"><span data-stu-id="985ea-136">String</span></span>|<span data-ttu-id="985ea-137">デバイスに関連付けられているユーザーの一意の識別子</span><span class="sxs-lookup"><span data-stu-id="985ea-137">Unique Identifier for the user associated with the device</span></span>|
|<span data-ttu-id="985ea-138">deviceName</span><span class="sxs-lookup"><span data-stu-id="985ea-138">deviceName</span></span>|<span data-ttu-id="985ea-139">String</span><span class="sxs-lookup"><span data-stu-id="985ea-139">String</span></span>|<span data-ttu-id="985ea-140">デバイスの名前</span><span class="sxs-lookup"><span data-stu-id="985ea-140">Name of the device</span></span>|
|<span data-ttu-id="985ea-141">hardwareInformation</span><span class="sxs-lookup"><span data-stu-id="985ea-141">hardwareInformation</span></span>|[<span data-ttu-id="985ea-142">hardwareInformation</span><span class="sxs-lookup"><span data-stu-id="985ea-142">hardwareInformation</span></span>](../resources/intune-devices-hardwareinformation.md)|<span data-ttu-id="985ea-143">デバイスのハードワードの詳細。</span><span class="sxs-lookup"><span data-stu-id="985ea-143">The hardward details for the device.</span></span>  <span data-ttu-id="985ea-144">記憶領域、製造元、シリアル番号などの情報が含まれます。</span><span class="sxs-lookup"><span data-stu-id="985ea-144">Includes information such as storage space, manufacturer, serial number, etc.</span></span>|
|<span data-ttu-id="985ea-145">ownerType</span><span class="sxs-lookup"><span data-stu-id="985ea-145">ownerType</span></span>|[<span data-ttu-id="985ea-146">ownerType</span><span class="sxs-lookup"><span data-stu-id="985ea-146">ownerType</span></span>](../resources/intune-devices-ownertype.md)|<span data-ttu-id="985ea-147">デバイスの所有権。</span><span class="sxs-lookup"><span data-stu-id="985ea-147">Ownership of the device.</span></span> <span data-ttu-id="985ea-148">' Company ' または ' personal ' にすることができます。</span><span class="sxs-lookup"><span data-stu-id="985ea-148">Can be 'company' or 'personal'.</span></span> <span data-ttu-id="985ea-149">可能な値は、`unknown`、`company`、`personal` です。</span><span class="sxs-lookup"><span data-stu-id="985ea-149">Possible values are: `unknown`, `company`, `personal`.</span></span>|
|<span data-ttu-id="985ea-150">managedDeviceOwnerType</span><span class="sxs-lookup"><span data-stu-id="985ea-150">managedDeviceOwnerType</span></span>|[<span data-ttu-id="985ea-151">managedDeviceOwnerType</span><span class="sxs-lookup"><span data-stu-id="985ea-151">managedDeviceOwnerType</span></span>](../resources/intune-devices-manageddeviceownertype.md)|<span data-ttu-id="985ea-152">デバイスの所有権。</span><span class="sxs-lookup"><span data-stu-id="985ea-152">Ownership of the device.</span></span> <span data-ttu-id="985ea-153">' Company ' または ' personal ' にすることができます。</span><span class="sxs-lookup"><span data-stu-id="985ea-153">Can be 'company' or 'personal'.</span></span> <span data-ttu-id="985ea-154">可能な値は、`unknown`、`company`、`personal` です。</span><span class="sxs-lookup"><span data-stu-id="985ea-154">Possible values are: `unknown`, `company`, `personal`.</span></span>|
|<span data-ttu-id="985ea-155">deviceActionResults</span><span class="sxs-lookup"><span data-stu-id="985ea-155">deviceActionResults</span></span>|<span data-ttu-id="985ea-156">[deviceActionResult](../resources/intune-devices-deviceactionresult.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="985ea-156">[deviceActionResult](../resources/intune-devices-deviceactionresult.md) collection</span></span>|<span data-ttu-id="985ea-157">ComplexType deviceActionResult オブジェクトのリスト。</span><span class="sxs-lookup"><span data-stu-id="985ea-157">List of ComplexType deviceActionResult objects.</span></span>|
|<span data-ttu-id="985ea-158">managementState</span><span class="sxs-lookup"><span data-stu-id="985ea-158">managementState</span></span>|[<span data-ttu-id="985ea-159">managementState</span><span class="sxs-lookup"><span data-stu-id="985ea-159">managementState</span></span>](../resources/intune-devices-managementstate.md)|<span data-ttu-id="985ea-160">デバイスの管理状態。</span><span class="sxs-lookup"><span data-stu-id="985ea-160">Management state of the device.</span></span> <span data-ttu-id="985ea-161">可能な値は、`managed`、`retirePending`、`retireFailed`、`wipePending`、`wipeFailed`、`unhealthy`、`deletePending`、`retireIssued`、`wipeIssued`、`wipeCanceled`、`retireCanceled`、`discovered` です。</span><span class="sxs-lookup"><span data-stu-id="985ea-161">Possible values are: `managed`, `retirePending`, `retireFailed`, `wipePending`, `wipeFailed`, `unhealthy`, `deletePending`, `retireIssued`, `wipeIssued`, `wipeCanceled`, `retireCanceled`, `discovered`.</span></span>|
|<span data-ttu-id="985ea-162">enrolledDateTime</span><span class="sxs-lookup"><span data-stu-id="985ea-162">enrolledDateTime</span></span>|<span data-ttu-id="985ea-163">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="985ea-163">DateTimeOffset</span></span>|<span data-ttu-id="985ea-164">デバイスの登録時刻。</span><span class="sxs-lookup"><span data-stu-id="985ea-164">Enrollment time of the device.</span></span>|
|<span data-ttu-id="985ea-165">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="985ea-165">lastSyncDateTime</span></span>|<span data-ttu-id="985ea-166">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="985ea-166">DateTimeOffset</span></span>|<span data-ttu-id="985ea-167">デバイスが Intune との正常な同期を最終的に完了した日時。</span><span class="sxs-lookup"><span data-stu-id="985ea-167">The date and time that the device last completed a successful sync with Intune.</span></span>|
|<span data-ttu-id="985ea-168">chassisType</span><span class="sxs-lookup"><span data-stu-id="985ea-168">chassisType</span></span>|[<span data-ttu-id="985ea-169">chassisType</span><span class="sxs-lookup"><span data-stu-id="985ea-169">chassisType</span></span>](../resources/intune-devices-chassistype.md)|<span data-ttu-id="985ea-170">デバイスのシャーシの種類。</span><span class="sxs-lookup"><span data-stu-id="985ea-170">Chassis type of the device.</span></span> <span data-ttu-id="985ea-171">可能な値は、`unknown`、`desktop`、`laptop`、`worksWorkstation`、`enterpriseServer`、`phone`、`tablet`、`mobileOther`、`mobileUnknown` です。</span><span class="sxs-lookup"><span data-stu-id="985ea-171">Possible values are: `unknown`, `desktop`, `laptop`, `worksWorkstation`, `enterpriseServer`, `phone`, `tablet`, `mobileOther`, `mobileUnknown`.</span></span>|
|<span data-ttu-id="985ea-172">operatingSystem</span><span class="sxs-lookup"><span data-stu-id="985ea-172">operatingSystem</span></span>|<span data-ttu-id="985ea-173">文字列</span><span class="sxs-lookup"><span data-stu-id="985ea-173">String</span></span>|<span data-ttu-id="985ea-174">デバイスのオペレーティング システム。</span><span class="sxs-lookup"><span data-stu-id="985ea-174">Operating system of the device.</span></span> <span data-ttu-id="985ea-175">Windows、iOS など。</span><span class="sxs-lookup"><span data-stu-id="985ea-175">Windows, iOS, etc.</span></span>|
|<span data-ttu-id="985ea-176">deviceType</span><span class="sxs-lookup"><span data-stu-id="985ea-176">deviceType</span></span>|[<span data-ttu-id="985ea-177">deviceType</span><span class="sxs-lookup"><span data-stu-id="985ea-177">deviceType</span></span>](../resources/intune-shared-devicetype.md)|<span data-ttu-id="985ea-178">デバイスのプラットフォーム。</span><span class="sxs-lookup"><span data-stu-id="985ea-178">Platform of the device.</span></span> <span data-ttu-id="985ea-179">可能な値: `desktop`、 `windowsRT` `winMO6` `nokia` `windowsPhone` `mac` `winCE` `winEmbedded` `iPhone` `iPad` `iPod` `android`、、、、、、、、、、、、 `iSocConsumer` `unix` `macMDM` `holoLens` `surfaceHub` `androidForWork` `androidEnterprise`, `blackberry`, `palm`, `unknown`.</span><span class="sxs-lookup"><span data-stu-id="985ea-179">Possible values are: `desktop`, `windowsRT`, `winMO6`, `nokia`, `windowsPhone`, `mac`, `winCE`, `winEmbedded`, `iPhone`, `iPad`, `iPod`, `android`, `iSocConsumer`, `unix`, `macMDM`, `holoLens`, `surfaceHub`, `androidForWork`, `androidEnterprise`, `blackberry`, `palm`, `unknown`.</span></span>|
|<span data-ttu-id="985ea-180">complianceState</span><span class="sxs-lookup"><span data-stu-id="985ea-180">complianceState</span></span>|[<span data-ttu-id="985ea-181">complianceState</span><span class="sxs-lookup"><span data-stu-id="985ea-181">complianceState</span></span>](../resources/intune-devices-compliancestate.md)|<span data-ttu-id="985ea-182">デバイスのコンプライアンス状態。</span><span class="sxs-lookup"><span data-stu-id="985ea-182">Compliance state of the device.</span></span> <span data-ttu-id="985ea-183">可能な値は、`unknown`、`compliant`、`noncompliant`、`conflict`、`error`、`inGracePeriod`、`configManager` です。</span><span class="sxs-lookup"><span data-stu-id="985ea-183">Possible values are: `unknown`, `compliant`, `noncompliant`, `conflict`, `error`, `inGracePeriod`, `configManager`.</span></span>|
|<span data-ttu-id="985ea-184">jailBroken</span><span class="sxs-lookup"><span data-stu-id="985ea-184">jailBroken</span></span>|<span data-ttu-id="985ea-185">String</span><span class="sxs-lookup"><span data-stu-id="985ea-185">String</span></span>|<span data-ttu-id="985ea-186">デバイスが脱獄またはルート化されているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="985ea-186">whether the device is jail broken or rooted.</span></span>|
|<span data-ttu-id="985ea-187">managementAgent</span><span class="sxs-lookup"><span data-stu-id="985ea-187">managementAgent</span></span>|[<span data-ttu-id="985ea-188">managementAgentType</span><span class="sxs-lookup"><span data-stu-id="985ea-188">managementAgentType</span></span>](../resources/intune-devices-managementagenttype.md)|<span data-ttu-id="985ea-189">デバイスの管理チャネル。</span><span class="sxs-lookup"><span data-stu-id="985ea-189">Management channel of the device.</span></span> <span data-ttu-id="985ea-190">Intune、EAS など。可能な値は`eas`、 `mdm`、 `easMdm` `intuneClient` `easIntuneClient` `configurationManagerClient` `jamf` `googleCloudDevicePolicyController`、、、、、、、、、 `microsoft365ManagedMdm`、、です。 `configurationManagerClientMdm` `configurationManagerClientMdmEas` `unknown`</span><span class="sxs-lookup"><span data-stu-id="985ea-190">Intune, EAS, etc. Possible values are: `eas`, `mdm`, `easMdm`, `intuneClient`, `easIntuneClient`, `configurationManagerClient`, `configurationManagerClientMdm`, `configurationManagerClientMdmEas`, `unknown`, `jamf`, `googleCloudDevicePolicyController`, `microsoft365ManagedMdm`.</span></span>|
|<span data-ttu-id="985ea-191">osVersion</span><span class="sxs-lookup"><span data-stu-id="985ea-191">osVersion</span></span>|<span data-ttu-id="985ea-192">String</span><span class="sxs-lookup"><span data-stu-id="985ea-192">String</span></span>|<span data-ttu-id="985ea-193">デバイスのオペレーティング システムのバージョン。</span><span class="sxs-lookup"><span data-stu-id="985ea-193">Operating system version of the device.</span></span>|
|<span data-ttu-id="985ea-194">easActivated</span><span class="sxs-lookup"><span data-stu-id="985ea-194">easActivated</span></span>|<span data-ttu-id="985ea-195">Boolean</span><span class="sxs-lookup"><span data-stu-id="985ea-195">Boolean</span></span>|<span data-ttu-id="985ea-196">Exchange ActiveSync がアクティブになっているデバイスかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="985ea-196">Whether the device is Exchange ActiveSync activated.</span></span>|
|<span data-ttu-id="985ea-197">easDeviceId</span><span class="sxs-lookup"><span data-stu-id="985ea-197">easDeviceId</span></span>|<span data-ttu-id="985ea-198">String</span><span class="sxs-lookup"><span data-stu-id="985ea-198">String</span></span>|<span data-ttu-id="985ea-199">デバイスの Exchange ActiveSync の ID。</span><span class="sxs-lookup"><span data-stu-id="985ea-199">Exchange ActiveSync Id of the device.</span></span>|
|<span data-ttu-id="985ea-200">easActivationDateTime</span><span class="sxs-lookup"><span data-stu-id="985ea-200">easActivationDateTime</span></span>|<span data-ttu-id="985ea-201">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="985ea-201">DateTimeOffset</span></span>|<span data-ttu-id="985ea-202">デバイスの Exchange ActivationSync のアクティブ化の時刻。</span><span class="sxs-lookup"><span data-stu-id="985ea-202">Exchange ActivationSync activation time of the device.</span></span>|
|<span data-ttu-id="985ea-203">aadRegistered</span><span class="sxs-lookup"><span data-stu-id="985ea-203">aadRegistered</span></span>|<span data-ttu-id="985ea-204">Boolean</span><span class="sxs-lookup"><span data-stu-id="985ea-204">Boolean</span></span>|<span data-ttu-id="985ea-205">Azure Active Directory が登録されているデバイスかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="985ea-205">Whether the device is Azure Active Directory registered.</span></span>|
|<span data-ttu-id="985ea-206">azureADRegistered</span><span class="sxs-lookup"><span data-stu-id="985ea-206">azureADRegistered</span></span>|<span data-ttu-id="985ea-207">Boolean</span><span class="sxs-lookup"><span data-stu-id="985ea-207">Boolean</span></span>|<span data-ttu-id="985ea-208">Azure Active Directory が登録されているデバイスかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="985ea-208">Whether the device is Azure Active Directory registered.</span></span>|
|<span data-ttu-id="985ea-209">deviceEnrollmentType</span><span class="sxs-lookup"><span data-stu-id="985ea-209">deviceEnrollmentType</span></span>|[<span data-ttu-id="985ea-210">deviceEnrollmentType</span><span class="sxs-lookup"><span data-stu-id="985ea-210">deviceEnrollmentType</span></span>](../resources/intune-shared-deviceenrollmenttype.md)|<span data-ttu-id="985ea-211">デバイスの登録の種類。</span><span class="sxs-lookup"><span data-stu-id="985ea-211">Enrollment type of the device.</span></span> <span data-ttu-id="985ea-212">可能な値は、`unknown`、`userEnrollment`、`deviceEnrollmentManager`、`appleBulkWithUser`、`appleBulkWithoutUser`、`windowsAzureADJoin`、`windowsBulkUserless`、`windowsAutoEnrollment`、`windowsBulkAzureDomainJoin`、`windowsCoManagement` です。</span><span class="sxs-lookup"><span data-stu-id="985ea-212">Possible values are: `unknown`, `userEnrollment`, `deviceEnrollmentManager`, `appleBulkWithUser`, `appleBulkWithoutUser`, `windowsAzureADJoin`, `windowsBulkUserless`, `windowsAutoEnrollment`, `windowsBulkAzureDomainJoin`, `windowsCoManagement`.</span></span>|
|<span data-ttu-id="985ea-213">lostModeState</span><span class="sxs-lookup"><span data-stu-id="985ea-213">lostModeState</span></span>|[<span data-ttu-id="985ea-214">lostModeState</span><span class="sxs-lookup"><span data-stu-id="985ea-214">lostModeState</span></span>](../resources/intune-devices-lostmodestate.md)|<span data-ttu-id="985ea-215">失われたモードが有効か無効かを示します。</span><span class="sxs-lookup"><span data-stu-id="985ea-215">Indicates if Lost mode is enabled or disabled.</span></span> <span data-ttu-id="985ea-216">可能な値は、`disabled`、`enabled` です。</span><span class="sxs-lookup"><span data-stu-id="985ea-216">Possible values are: `disabled`, `enabled`.</span></span>|
|<span data-ttu-id="985ea-217">activationLockBypassCode</span><span class="sxs-lookup"><span data-stu-id="985ea-217">activationLockBypassCode</span></span>|<span data-ttu-id="985ea-218">String</span><span class="sxs-lookup"><span data-stu-id="985ea-218">String</span></span>|<span data-ttu-id="985ea-219">デバイスのアクティベーション ロックをバイパスするためのコード。</span><span class="sxs-lookup"><span data-stu-id="985ea-219">Code that allows the Activation Lock on a device to be bypassed.</span></span>|
|<span data-ttu-id="985ea-220">emailAddress</span><span class="sxs-lookup"><span data-stu-id="985ea-220">emailAddress</span></span>|<span data-ttu-id="985ea-221">String</span><span class="sxs-lookup"><span data-stu-id="985ea-221">String</span></span>|<span data-ttu-id="985ea-222">デバイスに関連付けられているユーザーの電子メール</span><span class="sxs-lookup"><span data-stu-id="985ea-222">Email(s) for the user associated with the device</span></span>|
|<span data-ttu-id="985ea-223">azureActiveDirectoryDeviceId</span><span class="sxs-lookup"><span data-stu-id="985ea-223">azureActiveDirectoryDeviceId</span></span>|<span data-ttu-id="985ea-224">String</span><span class="sxs-lookup"><span data-stu-id="985ea-224">String</span></span>|<span data-ttu-id="985ea-225">Azure Active Directory デバイスの一意識別子。</span><span class="sxs-lookup"><span data-stu-id="985ea-225">The unique identifier for the Azure Active Directory device.</span></span> <span data-ttu-id="985ea-226">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="985ea-226">Read only.</span></span>|
|<span data-ttu-id="985ea-227">azureADDeviceId</span><span class="sxs-lookup"><span data-stu-id="985ea-227">azureADDeviceId</span></span>|<span data-ttu-id="985ea-228">String</span><span class="sxs-lookup"><span data-stu-id="985ea-228">String</span></span>|<span data-ttu-id="985ea-229">Azure Active Directory デバイスの一意識別子。</span><span class="sxs-lookup"><span data-stu-id="985ea-229">The unique identifier for the Azure Active Directory device.</span></span> <span data-ttu-id="985ea-230">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="985ea-230">Read only.</span></span>|
|<span data-ttu-id="985ea-231">deviceRegistrationState</span><span class="sxs-lookup"><span data-stu-id="985ea-231">deviceRegistrationState</span></span>|[<span data-ttu-id="985ea-232">deviceRegistrationState</span><span class="sxs-lookup"><span data-stu-id="985ea-232">deviceRegistrationState</span></span>](../resources/intune-devices-deviceregistrationstate.md)|<span data-ttu-id="985ea-233">デバイスの登録状態。</span><span class="sxs-lookup"><span data-stu-id="985ea-233">Device registration state.</span></span> <span data-ttu-id="985ea-234">可能な値は、`notRegistered`、`registered`、`revoked`、`keyConflict`、`approvalPending`、`certificateReset`、`notRegisteredPendingEnrollment`、`unknown` です。</span><span class="sxs-lookup"><span data-stu-id="985ea-234">Possible values are: `notRegistered`, `registered`, `revoked`, `keyConflict`, `approvalPending`, `certificateReset`, `notRegisteredPendingEnrollment`, `unknown`.</span></span>|
|<span data-ttu-id="985ea-235">deviceCategoryDisplayName</span><span class="sxs-lookup"><span data-stu-id="985ea-235">deviceCategoryDisplayName</span></span>|<span data-ttu-id="985ea-236">String</span><span class="sxs-lookup"><span data-stu-id="985ea-236">String</span></span>|<span data-ttu-id="985ea-237">デバイス カテゴリの表示名</span><span class="sxs-lookup"><span data-stu-id="985ea-237">Device category display name</span></span>|
|<span data-ttu-id="985ea-238">isSupervised</span><span class="sxs-lookup"><span data-stu-id="985ea-238">isSupervised</span></span>|<span data-ttu-id="985ea-239">Boolean</span><span class="sxs-lookup"><span data-stu-id="985ea-239">Boolean</span></span>|<span data-ttu-id="985ea-240">デバイスの管理状況</span><span class="sxs-lookup"><span data-stu-id="985ea-240">Device supervised status</span></span>|
|<span data-ttu-id="985ea-241">exchangeLastSuccessfulSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="985ea-241">exchangeLastSuccessfulSyncDateTime</span></span>|<span data-ttu-id="985ea-242">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="985ea-242">DateTimeOffset</span></span>|<span data-ttu-id="985ea-243">最後にデバイスが Exchange に接続した時刻。</span><span class="sxs-lookup"><span data-stu-id="985ea-243">Last time the device contacted Exchange.</span></span>|
|<span data-ttu-id="985ea-244">exchangeAccessState</span><span class="sxs-lookup"><span data-stu-id="985ea-244">exchangeAccessState</span></span>|[<span data-ttu-id="985ea-245">deviceManagementExchangeAccessState</span><span class="sxs-lookup"><span data-stu-id="985ea-245">deviceManagementExchangeAccessState</span></span>](../resources/intune-devices-devicemanagementexchangeaccessstate.md)|<span data-ttu-id="985ea-246">Exchange でのデバイスのアクセスの状態。</span><span class="sxs-lookup"><span data-stu-id="985ea-246">The Access State of the device in Exchange.</span></span> <span data-ttu-id="985ea-247">可能な値は、`none`、`unknown`、`allowed`、`blocked`、`quarantined` です。</span><span class="sxs-lookup"><span data-stu-id="985ea-247">Possible values are: `none`, `unknown`, `allowed`, `blocked`, `quarantined`.</span></span>|
|<span data-ttu-id="985ea-248">exchangeAccessStateReason</span><span class="sxs-lookup"><span data-stu-id="985ea-248">exchangeAccessStateReason</span></span>|[<span data-ttu-id="985ea-249">deviceManagementExchangeAccessStateReason</span><span class="sxs-lookup"><span data-stu-id="985ea-249">deviceManagementExchangeAccessStateReason</span></span>](../resources/intune-devices-devicemanagementexchangeaccessstatereason.md)|<span data-ttu-id="985ea-250">Exchange でのデバイスのアクセス状態の理由。
</span><span class="sxs-lookup"><span data-stu-id="985ea-250">The reason for the device's access state in Exchange.</span></span> <span data-ttu-id="985ea-251">可能な値は、`none`、`unknown`、`exchangeGlobalRule`、`exchangeIndividualRule`、`exchangeDeviceRule`、`exchangeUpgrade`、`exchangeMailboxPolicy`、`other`、`compliant`、`notCompliant`、`notEnrolled`、`unknownLocation`、`mfaRequired`、`azureADBlockDueToAccessPolicy`、`compromisedPassword`、`deviceNotKnownWithManagedApp` です。</span><span class="sxs-lookup"><span data-stu-id="985ea-251">Possible values are: `none`, `unknown`, `exchangeGlobalRule`, `exchangeIndividualRule`, `exchangeDeviceRule`, `exchangeUpgrade`, `exchangeMailboxPolicy`, `other`, `compliant`, `notCompliant`, `notEnrolled`, `unknownLocation`, `mfaRequired`, `azureADBlockDueToAccessPolicy`, `compromisedPassword`, `deviceNotKnownWithManagedApp`.</span></span>|
|<span data-ttu-id="985ea-252">remoteAssistanceSessionUrl</span><span class="sxs-lookup"><span data-stu-id="985ea-252">remoteAssistanceSessionUrl</span></span>|<span data-ttu-id="985ea-253">String</span><span class="sxs-lookup"><span data-stu-id="985ea-253">String</span></span>|<span data-ttu-id="985ea-254">デバイスとのリモート アシスタンス セッションを確立できるようにする URL。</span><span class="sxs-lookup"><span data-stu-id="985ea-254">Url that allows a Remote Assistance session to be established with the device.</span></span>|
|<span data-ttu-id="985ea-255">remoteAssistanceSessionErrorDetails</span><span class="sxs-lookup"><span data-stu-id="985ea-255">remoteAssistanceSessionErrorDetails</span></span>|<span data-ttu-id="985ea-256">String</span><span class="sxs-lookup"><span data-stu-id="985ea-256">String</span></span>|<span data-ttu-id="985ea-257">リモート アシスタンス セッション オブジェクトの作成時に問題を識別するエラー文字列。</span><span class="sxs-lookup"><span data-stu-id="985ea-257">An error string that identifies issues when creating Remote Assistance session objects.</span></span>|
|<span data-ttu-id="985ea-258">isEncrypted</span><span class="sxs-lookup"><span data-stu-id="985ea-258">isEncrypted</span></span>|<span data-ttu-id="985ea-259">Boolean</span><span class="sxs-lookup"><span data-stu-id="985ea-259">Boolean</span></span>|<span data-ttu-id="985ea-260">デバイスの暗号化の状態</span><span class="sxs-lookup"><span data-stu-id="985ea-260">Device encryption status</span></span>|
|<span data-ttu-id="985ea-261">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="985ea-261">userPrincipalName</span></span>|<span data-ttu-id="985ea-262">String</span><span class="sxs-lookup"><span data-stu-id="985ea-262">String</span></span>|<span data-ttu-id="985ea-263">デバイスのユーザー プリンシパル名。</span><span class="sxs-lookup"><span data-stu-id="985ea-263">Device user principal name</span></span>|
|<span data-ttu-id="985ea-264">model</span><span class="sxs-lookup"><span data-stu-id="985ea-264">model</span></span>|<span data-ttu-id="985ea-265">String</span><span class="sxs-lookup"><span data-stu-id="985ea-265">String</span></span>|<span data-ttu-id="985ea-266">デバイスのモデル</span><span class="sxs-lookup"><span data-stu-id="985ea-266">Model of the device</span></span>|
|<span data-ttu-id="985ea-267">manufacturer</span><span class="sxs-lookup"><span data-stu-id="985ea-267">manufacturer</span></span>|<span data-ttu-id="985ea-268">String</span><span class="sxs-lookup"><span data-stu-id="985ea-268">String</span></span>|<span data-ttu-id="985ea-269">デバイスのメーカー</span><span class="sxs-lookup"><span data-stu-id="985ea-269">Manufacturer of the device</span></span>|
|<span data-ttu-id="985ea-270">imei</span><span class="sxs-lookup"><span data-stu-id="985ea-270">imei</span></span>|<span data-ttu-id="985ea-271">String</span><span class="sxs-lookup"><span data-stu-id="985ea-271">String</span></span>|<span data-ttu-id="985ea-272">IMEI</span><span class="sxs-lookup"><span data-stu-id="985ea-272">IMEI</span></span>|
|<span data-ttu-id="985ea-273">complianceGracePeriodExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="985ea-273">complianceGracePeriodExpirationDateTime</span></span>|<span data-ttu-id="985ea-274">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="985ea-274">DateTimeOffset</span></span>|<span data-ttu-id="985ea-275">デバイス コンプライアンスの猶予期間が経過する DateTime</span><span class="sxs-lookup"><span data-stu-id="985ea-275">The DateTime when device compliance grace period expires</span></span>|
|<span data-ttu-id="985ea-276">serialNumber</span><span class="sxs-lookup"><span data-stu-id="985ea-276">serialNumber</span></span>|<span data-ttu-id="985ea-277">String</span><span class="sxs-lookup"><span data-stu-id="985ea-277">String</span></span>|<span data-ttu-id="985ea-278">シリアル番号</span><span class="sxs-lookup"><span data-stu-id="985ea-278">SerialNumber</span></span>|
|<span data-ttu-id="985ea-279">phoneNumber</span><span class="sxs-lookup"><span data-stu-id="985ea-279">phoneNumber</span></span>|<span data-ttu-id="985ea-280">String</span><span class="sxs-lookup"><span data-stu-id="985ea-280">String</span></span>|<span data-ttu-id="985ea-281">デバイスの電話番号</span><span class="sxs-lookup"><span data-stu-id="985ea-281">Phone number of the device</span></span>|
|<span data-ttu-id="985ea-282">androidSecurityPatchLevel</span><span class="sxs-lookup"><span data-stu-id="985ea-282">androidSecurityPatchLevel</span></span>|<span data-ttu-id="985ea-283">String</span><span class="sxs-lookup"><span data-stu-id="985ea-283">String</span></span>|<span data-ttu-id="985ea-284">Android セキュリティ パッチのレベル</span><span class="sxs-lookup"><span data-stu-id="985ea-284">Android security patch level</span></span>|
|<span data-ttu-id="985ea-285">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="985ea-285">userDisplayName</span></span>|<span data-ttu-id="985ea-286">String</span><span class="sxs-lookup"><span data-stu-id="985ea-286">String</span></span>|<span data-ttu-id="985ea-287">ユーザーの表示名</span><span class="sxs-lookup"><span data-stu-id="985ea-287">User display name</span></span>|
|<span data-ttu-id="985ea-288">configurationManagerClientEnabledFeatures</span><span class="sxs-lookup"><span data-stu-id="985ea-288">configurationManagerClientEnabledFeatures</span></span>|[<span data-ttu-id="985ea-289">configurationManagerClientEnabledFeatures</span><span class="sxs-lookup"><span data-stu-id="985ea-289">configurationManagerClientEnabledFeatures</span></span>](../resources/intune-devices-configurationmanagerclientenabledfeatures.md)|<span data-ttu-id="985ea-290">ConfigrMgr クライアント対応機能
</span><span class="sxs-lookup"><span data-stu-id="985ea-290">ConfigrMgr client enabled features</span></span>|
|<span data-ttu-id="985ea-291">wiFiMacAddress</span><span class="sxs-lookup"><span data-stu-id="985ea-291">wiFiMacAddress</span></span>|<span data-ttu-id="985ea-292">String</span><span class="sxs-lookup"><span data-stu-id="985ea-292">String</span></span>|<span data-ttu-id="985ea-293">Wi-Fi MAC</span><span class="sxs-lookup"><span data-stu-id="985ea-293">Wi-Fi MAC</span></span>|
|<span data-ttu-id="985ea-294">deviceHealthAttestationState</span><span class="sxs-lookup"><span data-stu-id="985ea-294">deviceHealthAttestationState</span></span>|[<span data-ttu-id="985ea-295">deviceHealthAttestationState</span><span class="sxs-lookup"><span data-stu-id="985ea-295">deviceHealthAttestationState</span></span>](../resources/intune-devices-devicehealthattestationstate.md)|<span data-ttu-id="985ea-296">デバイスの正常性構成証明の状態。</span><span class="sxs-lookup"><span data-stu-id="985ea-296">The device health attestation state.</span></span>|
|<span data-ttu-id="985ea-297">subscriberCarrier</span><span class="sxs-lookup"><span data-stu-id="985ea-297">subscriberCarrier</span></span>|<span data-ttu-id="985ea-298">String</span><span class="sxs-lookup"><span data-stu-id="985ea-298">String</span></span>|<span data-ttu-id="985ea-299">サブスクライバー通信事業者</span><span class="sxs-lookup"><span data-stu-id="985ea-299">Subscriber Carrier</span></span>|
|<span data-ttu-id="985ea-300">meid</span><span class="sxs-lookup"><span data-stu-id="985ea-300">meid</span></span>|<span data-ttu-id="985ea-301">String</span><span class="sxs-lookup"><span data-stu-id="985ea-301">String</span></span>|<span data-ttu-id="985ea-302">MEID</span><span class="sxs-lookup"><span data-stu-id="985ea-302">MEID</span></span>|
|<span data-ttu-id="985ea-303">totalStorageSpaceInBytes</span><span class="sxs-lookup"><span data-stu-id="985ea-303">totalStorageSpaceInBytes</span></span>|<span data-ttu-id="985ea-304">Int64</span><span class="sxs-lookup"><span data-stu-id="985ea-304">Int64</span></span>|<span data-ttu-id="985ea-305">記憶域の合計 (バイト)</span><span class="sxs-lookup"><span data-stu-id="985ea-305">Total Storage in Bytes</span></span>|
|<span data-ttu-id="985ea-306">freeStorageSpaceInBytes</span><span class="sxs-lookup"><span data-stu-id="985ea-306">freeStorageSpaceInBytes</span></span>|<span data-ttu-id="985ea-307">Int64</span><span class="sxs-lookup"><span data-stu-id="985ea-307">Int64</span></span>|<span data-ttu-id="985ea-308">空き記憶域 (バイト)</span><span class="sxs-lookup"><span data-stu-id="985ea-308">Free Storage in Bytes</span></span>|
|<span data-ttu-id="985ea-309">managedDeviceName</span><span class="sxs-lookup"><span data-stu-id="985ea-309">managedDeviceName</span></span>|<span data-ttu-id="985ea-310">String</span><span class="sxs-lookup"><span data-stu-id="985ea-310">String</span></span>|<span data-ttu-id="985ea-311">デバイスを識別する名前が自動的に生成されます。</span><span class="sxs-lookup"><span data-stu-id="985ea-311">Automatically generated name to identify a device.</span></span> <span data-ttu-id="985ea-312">ユーザー フレンドリ名に上書きできます。</span><span class="sxs-lookup"><span data-stu-id="985ea-312">Can be overwritten to a user friendly name.</span></span>|
|<span data-ttu-id="985ea-313">partnerReportedThreatState</span><span class="sxs-lookup"><span data-stu-id="985ea-313">partnerReportedThreatState</span></span>|[<span data-ttu-id="985ea-314">managedDevicePartnerReportedHealthState</span><span class="sxs-lookup"><span data-stu-id="985ea-314">managedDevicePartnerReportedHealthState</span></span>](../resources/intune-devices-manageddevicepartnerreportedhealthstate.md)|<span data-ttu-id="985ea-315">Mobile Threat Defense パートナーがアカウントおよびデバイスで使用されている場合の、デバイスの脅威の状態を示します。</span><span class="sxs-lookup"><span data-stu-id="985ea-315">Indicates the threat state of a device when a Mobile Threat Defense partner is in use by the account and device.</span></span> <span data-ttu-id="985ea-316">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="985ea-316">Read Only.</span></span> <span data-ttu-id="985ea-317">可能な値は、`unknown`、`activated`、`deactivated`、`secured`、`lowSeverity`、`mediumSeverity`、`highSeverity`、`unresponsive`、`compromised`、`misconfigured` です。</span><span class="sxs-lookup"><span data-stu-id="985ea-317">Possible values are: `unknown`, `activated`, `deactivated`, `secured`, `lowSeverity`, `mediumSeverity`, `highSeverity`, `unresponsive`, `compromised`, `misconfigured`.</span></span>|
|<span data-ttu-id="985ea-318">retireAfterDateTime</span><span class="sxs-lookup"><span data-stu-id="985ea-318">retireAfterDateTime</span></span>|<span data-ttu-id="985ea-319">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="985ea-319">DateTimeOffset</span></span>|<span data-ttu-id="985ea-320">スケジュールされたアクションのためにデバイスが自動廃棄されるまでの時間を示します。</span><span class="sxs-lookup"><span data-stu-id="985ea-320">Indicates the time after when a device will be auto retired because of scheduled action.</span></span>|
|<span data-ttu-id="985ea-321">usersLoggedOn</span><span class="sxs-lookup"><span data-stu-id="985ea-321">usersLoggedOn</span></span>|<span data-ttu-id="985ea-322">[loggedOnUser](../resources/intune-devices-loggedonuser.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="985ea-322">[loggedOnUser](../resources/intune-devices-loggedonuser.md) collection</span></span>|<span data-ttu-id="985ea-323">デバイスの最後にログオンしたユーザーを示します</span><span class="sxs-lookup"><span data-stu-id="985ea-323">Indicates the last logged on users of a device</span></span>|
|<span data-ttu-id="985ea-324">preferMdmOverGroupPolicyAppliedDateTime</span><span class="sxs-lookup"><span data-stu-id="985ea-324">preferMdmOverGroupPolicyAppliedDateTime</span></span>|<span data-ttu-id="985ea-325">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="985ea-325">DateTimeOffset</span></span>|<span data-ttu-id="985ea-326">PreferMdmOverGroupPolicy の設定が設定された DateTime を報告します。</span><span class="sxs-lookup"><span data-stu-id="985ea-326">Reports the DateTime the preferMdmOverGroupPolicy setting was set.</span></span>  <span data-ttu-id="985ea-327">設定すると、競合がある場合に Intune MDM 設定がグループポリシー設定を上書きします。</span><span class="sxs-lookup"><span data-stu-id="985ea-327">When set, the Intune MDM settings will override Group Policy settings if there is a conflict.</span></span> <span data-ttu-id="985ea-328">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="985ea-328">Read Only.</span></span>|
|<span data-ttu-id="985ea-329">autopilotEnrolled</span><span class="sxs-lookup"><span data-stu-id="985ea-329">autopilotEnrolled</span></span>|<span data-ttu-id="985ea-330">Boolean</span><span class="sxs-lookup"><span data-stu-id="985ea-330">Boolean</span></span>|<span data-ttu-id="985ea-331">管理対象デバイスが自動パイロットで登録されているかどうかを報告します。</span><span class="sxs-lookup"><span data-stu-id="985ea-331">Reports if the managed device is enrolled via auto-pilot.</span></span>|
|<span data-ttu-id="985ea-332">requireUserEnrollmentApproval</span><span class="sxs-lookup"><span data-stu-id="985ea-332">requireUserEnrollmentApproval</span></span>|<span data-ttu-id="985ea-333">Boolean</span><span class="sxs-lookup"><span data-stu-id="985ea-333">Boolean</span></span>|<span data-ttu-id="985ea-334">管理対象 iOS デバイスがユーザー承認登録であるかどうかを報告します。</span><span class="sxs-lookup"><span data-stu-id="985ea-334">Reports if the managed iOS device is user approval enrollment.</span></span>|
|<span data-ttu-id="985ea-335">managementCertificateExpirationDate</span><span class="sxs-lookup"><span data-stu-id="985ea-335">managementCertificateExpirationDate</span></span>|<span data-ttu-id="985ea-336">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="985ea-336">DateTimeOffset</span></span>|<span data-ttu-id="985ea-337">デバイス管理証明書の有効期限を報告する</span><span class="sxs-lookup"><span data-stu-id="985ea-337">Reports device management certificate expiration date</span></span>|
|<span data-ttu-id="985ea-338">iccid</span><span class="sxs-lookup"><span data-stu-id="985ea-338">iccid</span></span>|<span data-ttu-id="985ea-339">String</span><span class="sxs-lookup"><span data-stu-id="985ea-339">String</span></span>|<span data-ttu-id="985ea-340">Ic カード識別子。 SIM カードの一意の識別番号です。</span><span class="sxs-lookup"><span data-stu-id="985ea-340">Integrated Circuit Card Identifier, it is A SIM card's unique identification number.</span></span>|
|<span data-ttu-id="985ea-341">udid</span><span class="sxs-lookup"><span data-stu-id="985ea-341">udid</span></span>|<span data-ttu-id="985ea-342">String</span><span class="sxs-lookup"><span data-stu-id="985ea-342">String</span></span>|<span data-ttu-id="985ea-343">IOS および macOS デバイスの一意のデバイス識別子。</span><span class="sxs-lookup"><span data-stu-id="985ea-343">Unique Device Identifier for iOS and macOS devices.</span></span>|
|<span data-ttu-id="985ea-344">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="985ea-344">roleScopeTagIds</span></span>|<span data-ttu-id="985ea-345">文字列コレクション</span><span class="sxs-lookup"><span data-stu-id="985ea-345">String collection</span></span>|<span data-ttu-id="985ea-346">このデバイスインスタンスの範囲タグ Id のリスト。</span><span class="sxs-lookup"><span data-stu-id="985ea-346">List of Scope Tag IDs for this Device instance.</span></span>|
|<span data-ttu-id="985ea-347">windowsActiveMalwareCount 再計算</span><span class="sxs-lookup"><span data-stu-id="985ea-347">windowsActiveMalwareCount</span></span>|<span data-ttu-id="985ea-348">Int32</span><span class="sxs-lookup"><span data-stu-id="985ea-348">Int32</span></span>|<span data-ttu-id="985ea-349">この windows デバイスのアクティブなマルウェアの数</span><span class="sxs-lookup"><span data-stu-id="985ea-349">Count of active malware for this windows device</span></span>|
|<span data-ttu-id="985ea-350">windowsRemediatedMalwareCount</span><span class="sxs-lookup"><span data-stu-id="985ea-350">windowsRemediatedMalwareCount</span></span>|<span data-ttu-id="985ea-351">Int32</span><span class="sxs-lookup"><span data-stu-id="985ea-351">Int32</span></span>|<span data-ttu-id="985ea-352">この windows デバイスの修復済みマルウェアの数</span><span class="sxs-lookup"><span data-stu-id="985ea-352">Count of remediated malware for this windows device</span></span>|
|<span data-ttu-id="985ea-353">notes</span><span class="sxs-lookup"><span data-stu-id="985ea-353">notes</span></span>|<span data-ttu-id="985ea-354">String</span><span class="sxs-lookup"><span data-stu-id="985ea-354">String</span></span>|<span data-ttu-id="985ea-355">IT 管理者によって作成されたデバイスのメモ</span><span class="sxs-lookup"><span data-stu-id="985ea-355">Notes on the device created by IT Admin</span></span>|
|<span data-ttu-id="985ea-356">configurationManagerClientHealthState</span><span class="sxs-lookup"><span data-stu-id="985ea-356">configurationManagerClientHealthState</span></span>|[<span data-ttu-id="985ea-357">configurationManagerClientHealthState</span><span class="sxs-lookup"><span data-stu-id="985ea-357">configurationManagerClientHealthState</span></span>](../resources/intune-devices-configurationmanagerclienthealthstate.md)|<span data-ttu-id="985ea-358">構成マネージャークライアントの正常性状態。 MDM/ConfigMgr エージェントによって管理されるデバイスに対してのみ有効です。</span><span class="sxs-lookup"><span data-stu-id="985ea-358">Configuration manager client health state, valid only for devices managed by MDM/ConfigMgr Agent</span></span>|



## <a name="response"></a><span data-ttu-id="985ea-359">応答</span><span class="sxs-lookup"><span data-stu-id="985ea-359">Response</span></span>
<span data-ttu-id="985ea-360">成功した場合、このメソッドは `200 OK` 応答コードと、更新された [managedDevice](../resources/intune-devices-manageddevice.md) オブジェクトを応答本文で返します。</span><span class="sxs-lookup"><span data-stu-id="985ea-360">If successful, this method returns a `200 OK` response code and an updated [managedDevice](../resources/intune-devices-manageddevice.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="985ea-361">例</span><span class="sxs-lookup"><span data-stu-id="985ea-361">Example</span></span>

### <a name="request"></a><span data-ttu-id="985ea-362">要求</span><span class="sxs-lookup"><span data-stu-id="985ea-362">Request</span></span>
<span data-ttu-id="985ea-363">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="985ea-363">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/managedDevices/{managedDeviceId}
Content-type: application/json
Content-length: 7286

{
  "@odata.type": "#microsoft.graph.managedDevice",
  "userId": "User Id value",
  "deviceName": "Device Name value",
  "hardwareInformation": {
    "@odata.type": "microsoft.graph.hardwareInformation",
    "serialNumber": "Serial Number value",
    "totalStorageSpace": 1,
    "freeStorageSpace": 0,
    "imei": "Imei value",
    "meid": "Meid value",
    "manufacturer": "Manufacturer value",
    "model": "Model value",
    "phoneNumber": "Phone Number value",
    "subscriberCarrier": "Subscriber Carrier value",
    "cellularTechnology": "Cellular Technology value",
    "wifiMac": "Wifi Mac value",
    "operatingSystemLanguage": "Operating System Language value",
    "isSupervised": true,
    "isEncrypted": true,
    "isSharedDevice": true,
    "sharedDeviceCachedUsers": [
      {
        "@odata.type": "microsoft.graph.sharedAppleDeviceUser",
        "userPrincipalName": "User Principal Name value",
        "dataToSync": true,
        "dataQuota": 9,
        "dataUsed": 8
      }
    ],
    "tpmSpecificationVersion": "Tpm Specification Version value",
    "operatingSystemEdition": "Operating System Edition value",
    "deviceFullQualifiedDomainName": "Device Full Qualified Domain Name value",
    "deviceGuardVirtualizationBasedSecurityHardwareRequirementState": "secureBootRequired",
    "deviceGuardVirtualizationBasedSecurityState": "rebootRequired",
    "deviceGuardLocalSystemAuthorityCredentialGuardState": "rebootRequired"
  },
  "ownerType": "company",
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
  "managementState": "retirePending",
  "enrolledDateTime": "2016-12-31T23:59:43.797191-08:00",
  "lastSyncDateTime": "2017-01-01T00:02:49.3205976-08:00",
  "chassisType": "desktop",
  "operatingSystem": "Operating System value",
  "deviceType": "windowsRT",
  "complianceState": "compliant",
  "jailBroken": "Jail Broken value",
  "managementAgent": "mdm",
  "osVersion": "Os Version value",
  "easActivated": true,
  "easDeviceId": "Eas Device Id value",
  "easActivationDateTime": "2016-12-31T23:59:43.4878784-08:00",
  "aadRegistered": true,
  "azureADRegistered": true,
  "deviceEnrollmentType": "userEnrollment",
  "lostModeState": "enabled",
  "activationLockBypassCode": "Activation Lock Bypass Code value",
  "emailAddress": "Email Address value",
  "azureActiveDirectoryDeviceId": "Azure Active Directory Device Id value",
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
    "windowsUpdateForBusiness": true,
    "endpointProtection": true,
    "officeApps": true
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
  "partnerReportedThreatState": "activated",
  "retireAfterDateTime": "2016-12-31T23:57:37.576134-08:00",
  "usersLoggedOn": [
    {
      "@odata.type": "microsoft.graph.loggedOnUser",
      "userId": "User Id value",
      "lastLogOnDateTime": "2016-12-31T23:58:37.4262708-08:00"
    }
  ],
  "preferMdmOverGroupPolicyAppliedDateTime": "2016-12-31T23:57:34.4649887-08:00",
  "autopilotEnrolled": true,
  "requireUserEnrollmentApproval": true,
  "managementCertificateExpirationDate": "2016-12-31T23:57:59.9789653-08:00",
  "iccid": "Iccid value",
  "udid": "Udid value",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "windowsActiveMalwareCount": 9,
  "windowsRemediatedMalwareCount": 13,
  "notes": "Notes value",
  "configurationManagerClientHealthState": {
    "@odata.type": "microsoft.graph.configurationManagerClientHealthState",
    "state": "installed",
    "errorCode": 9,
    "lastSyncDateTime": "2017-01-01T00:02:49.3205976-08:00"
  }
}
```

### <a name="response"></a><span data-ttu-id="985ea-364">応答</span><span class="sxs-lookup"><span data-stu-id="985ea-364">Response</span></span>
<span data-ttu-id="985ea-p121">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="985ea-p121">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 7335

{
  "@odata.type": "#microsoft.graph.managedDevice",
  "id": "705c034c-034c-705c-4c03-5c704c035c70",
  "userId": "User Id value",
  "deviceName": "Device Name value",
  "hardwareInformation": {
    "@odata.type": "microsoft.graph.hardwareInformation",
    "serialNumber": "Serial Number value",
    "totalStorageSpace": 1,
    "freeStorageSpace": 0,
    "imei": "Imei value",
    "meid": "Meid value",
    "manufacturer": "Manufacturer value",
    "model": "Model value",
    "phoneNumber": "Phone Number value",
    "subscriberCarrier": "Subscriber Carrier value",
    "cellularTechnology": "Cellular Technology value",
    "wifiMac": "Wifi Mac value",
    "operatingSystemLanguage": "Operating System Language value",
    "isSupervised": true,
    "isEncrypted": true,
    "isSharedDevice": true,
    "sharedDeviceCachedUsers": [
      {
        "@odata.type": "microsoft.graph.sharedAppleDeviceUser",
        "userPrincipalName": "User Principal Name value",
        "dataToSync": true,
        "dataQuota": 9,
        "dataUsed": 8
      }
    ],
    "tpmSpecificationVersion": "Tpm Specification Version value",
    "operatingSystemEdition": "Operating System Edition value",
    "deviceFullQualifiedDomainName": "Device Full Qualified Domain Name value",
    "deviceGuardVirtualizationBasedSecurityHardwareRequirementState": "secureBootRequired",
    "deviceGuardVirtualizationBasedSecurityState": "rebootRequired",
    "deviceGuardLocalSystemAuthorityCredentialGuardState": "rebootRequired"
  },
  "ownerType": "company",
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
  "managementState": "retirePending",
  "enrolledDateTime": "2016-12-31T23:59:43.797191-08:00",
  "lastSyncDateTime": "2017-01-01T00:02:49.3205976-08:00",
  "chassisType": "desktop",
  "operatingSystem": "Operating System value",
  "deviceType": "windowsRT",
  "complianceState": "compliant",
  "jailBroken": "Jail Broken value",
  "managementAgent": "mdm",
  "osVersion": "Os Version value",
  "easActivated": true,
  "easDeviceId": "Eas Device Id value",
  "easActivationDateTime": "2016-12-31T23:59:43.4878784-08:00",
  "aadRegistered": true,
  "azureADRegistered": true,
  "deviceEnrollmentType": "userEnrollment",
  "lostModeState": "enabled",
  "activationLockBypassCode": "Activation Lock Bypass Code value",
  "emailAddress": "Email Address value",
  "azureActiveDirectoryDeviceId": "Azure Active Directory Device Id value",
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
    "windowsUpdateForBusiness": true,
    "endpointProtection": true,
    "officeApps": true
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
  "partnerReportedThreatState": "activated",
  "retireAfterDateTime": "2016-12-31T23:57:37.576134-08:00",
  "usersLoggedOn": [
    {
      "@odata.type": "microsoft.graph.loggedOnUser",
      "userId": "User Id value",
      "lastLogOnDateTime": "2016-12-31T23:58:37.4262708-08:00"
    }
  ],
  "preferMdmOverGroupPolicyAppliedDateTime": "2016-12-31T23:57:34.4649887-08:00",
  "autopilotEnrolled": true,
  "requireUserEnrollmentApproval": true,
  "managementCertificateExpirationDate": "2016-12-31T23:57:59.9789653-08:00",
  "iccid": "Iccid value",
  "udid": "Udid value",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "windowsActiveMalwareCount": 9,
  "windowsRemediatedMalwareCount": 13,
  "notes": "Notes value",
  "configurationManagerClientHealthState": {
    "@odata.type": "microsoft.graph.configurationManagerClientHealthState",
    "state": "installed",
    "errorCode": 9,
    "lastSyncDateTime": "2017-01-01T00:02:49.3205976-08:00"
  }
}
```





