---
title: >
  managedDevice の更新
description: managedDevice オブジェクトのプロパティを更新します。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 0dd5c42bd6dba6208ea06c2f85efce1e7972d6eb
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/11/2019
ms.locfileid: "33909590"
---
# <a name="update-manageddevice"></a><span data-ttu-id="58a40-103">managedDevice の更新
</span><span class="sxs-lookup"><span data-stu-id="58a40-103">Update managedDevice</span></span>

> <span data-ttu-id="58a40-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="58a40-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="58a40-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="58a40-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="58a40-106">[managedDevice](../resources/intune-devices-manageddevice.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="58a40-106">Update the properties of a [managedDevice](../resources/intune-devices-manageddevice.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="58a40-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="58a40-107">Prerequisites</span></span>
<span data-ttu-id="58a40-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="58a40-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="58a40-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="58a40-110">Permission type</span></span>|<span data-ttu-id="58a40-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="58a40-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="58a40-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="58a40-112">Delegated (work or school account)</span></span>|<span data-ttu-id="58a40-113">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="58a40-113">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="58a40-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="58a40-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="58a40-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="58a40-115">Not supported.</span></span>|
|<span data-ttu-id="58a40-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="58a40-116">Application</span></span>|<span data-ttu-id="58a40-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="58a40-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="58a40-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="58a40-118">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="58a40-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="58a40-119">Request headers</span></span>
|<span data-ttu-id="58a40-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="58a40-120">Header</span></span>|<span data-ttu-id="58a40-121">値</span><span class="sxs-lookup"><span data-stu-id="58a40-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="58a40-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="58a40-122">Authorization</span></span>|<span data-ttu-id="58a40-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="58a40-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="58a40-124">承諾</span><span class="sxs-lookup"><span data-stu-id="58a40-124">Accept</span></span>|<span data-ttu-id="58a40-125">application/json</span><span class="sxs-lookup"><span data-stu-id="58a40-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="58a40-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="58a40-126">Request body</span></span>
<span data-ttu-id="58a40-127">要求本文で、[managedDevice](../resources/intune-devices-manageddevice.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="58a40-127">In the request body, supply a JSON representation for the [managedDevice](../resources/intune-devices-manageddevice.md) object.</span></span>

<span data-ttu-id="58a40-128">次の表に、[managedDevice](../resources/intune-devices-manageddevice.md) の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="58a40-128">The following table shows the properties that are required when you create the [managedDevice](../resources/intune-devices-manageddevice.md).</span></span>

|<span data-ttu-id="58a40-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="58a40-129">Property</span></span>|<span data-ttu-id="58a40-130">型</span><span class="sxs-lookup"><span data-stu-id="58a40-130">Type</span></span>|<span data-ttu-id="58a40-131">説明</span><span class="sxs-lookup"><span data-stu-id="58a40-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="58a40-132">id</span><span class="sxs-lookup"><span data-stu-id="58a40-132">id</span></span>|<span data-ttu-id="58a40-133">文字列</span><span class="sxs-lookup"><span data-stu-id="58a40-133">String</span></span>|<span data-ttu-id="58a40-134">デバイスの一意識別子</span><span class="sxs-lookup"><span data-stu-id="58a40-134">Unique Identifier for the device</span></span>|
|<span data-ttu-id="58a40-135">userId</span><span class="sxs-lookup"><span data-stu-id="58a40-135">userId</span></span>|<span data-ttu-id="58a40-136">String</span><span class="sxs-lookup"><span data-stu-id="58a40-136">String</span></span>|<span data-ttu-id="58a40-137">デバイスに関連付けられているユーザーの一意の識別子</span><span class="sxs-lookup"><span data-stu-id="58a40-137">Unique Identifier for the user associated with the device</span></span>|
|<span data-ttu-id="58a40-138">deviceName</span><span class="sxs-lookup"><span data-stu-id="58a40-138">deviceName</span></span>|<span data-ttu-id="58a40-139">String</span><span class="sxs-lookup"><span data-stu-id="58a40-139">String</span></span>|<span data-ttu-id="58a40-140">デバイスの名前</span><span class="sxs-lookup"><span data-stu-id="58a40-140">Name of the device</span></span>|
|<span data-ttu-id="58a40-141">hardwareInformation</span><span class="sxs-lookup"><span data-stu-id="58a40-141">hardwareInformation</span></span>|[<span data-ttu-id="58a40-142">hardwareInformation</span><span class="sxs-lookup"><span data-stu-id="58a40-142">hardwareInformation</span></span>](../resources/intune-devices-hardwareinformation.md)|<span data-ttu-id="58a40-143">デバイスのハードワードの詳細。</span><span class="sxs-lookup"><span data-stu-id="58a40-143">The hardward details for the device.</span></span>  <span data-ttu-id="58a40-144">記憶領域、製造元、シリアル番号などの情報が含まれます。</span><span class="sxs-lookup"><span data-stu-id="58a40-144">Includes information such as storage space, manufacturer, serial number, etc.</span></span>|
|<span data-ttu-id="58a40-145">ownerType</span><span class="sxs-lookup"><span data-stu-id="58a40-145">ownerType</span></span>|[<span data-ttu-id="58a40-146">ownerType</span><span class="sxs-lookup"><span data-stu-id="58a40-146">ownerType</span></span>](../resources/intune-devices-ownertype.md)|<span data-ttu-id="58a40-147">デバイスの所有権。</span><span class="sxs-lookup"><span data-stu-id="58a40-147">Ownership of the device.</span></span> <span data-ttu-id="58a40-148">' Company ' または ' personal ' にすることができます。</span><span class="sxs-lookup"><span data-stu-id="58a40-148">Can be 'company' or 'personal'.</span></span> <span data-ttu-id="58a40-149">可能な値は、`unknown`、`company`、`personal` です。</span><span class="sxs-lookup"><span data-stu-id="58a40-149">Possible values are: `unknown`, `company`, `personal`.</span></span>|
|<span data-ttu-id="58a40-150">managedDeviceOwnerType</span><span class="sxs-lookup"><span data-stu-id="58a40-150">managedDeviceOwnerType</span></span>|[<span data-ttu-id="58a40-151">managedDeviceOwnerType</span><span class="sxs-lookup"><span data-stu-id="58a40-151">managedDeviceOwnerType</span></span>](../resources/intune-devices-manageddeviceownertype.md)|<span data-ttu-id="58a40-152">デバイスの所有権。</span><span class="sxs-lookup"><span data-stu-id="58a40-152">Ownership of the device.</span></span> <span data-ttu-id="58a40-153">' Company ' または ' personal ' にすることができます。</span><span class="sxs-lookup"><span data-stu-id="58a40-153">Can be 'company' or 'personal'.</span></span> <span data-ttu-id="58a40-154">可能な値は、`unknown`、`company`、`personal` です。</span><span class="sxs-lookup"><span data-stu-id="58a40-154">Possible values are: `unknown`, `company`, `personal`.</span></span>|
|<span data-ttu-id="58a40-155">deviceActionResults</span><span class="sxs-lookup"><span data-stu-id="58a40-155">deviceActionResults</span></span>|<span data-ttu-id="58a40-156">[deviceActionResult](../resources/intune-devices-deviceactionresult.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="58a40-156">[deviceActionResult](../resources/intune-devices-deviceactionresult.md) collection</span></span>|<span data-ttu-id="58a40-157">ComplexType deviceActionResult オブジェクトのリスト。</span><span class="sxs-lookup"><span data-stu-id="58a40-157">List of ComplexType deviceActionResult objects.</span></span>|
|<span data-ttu-id="58a40-158">managementState</span><span class="sxs-lookup"><span data-stu-id="58a40-158">managementState</span></span>|[<span data-ttu-id="58a40-159">managementState</span><span class="sxs-lookup"><span data-stu-id="58a40-159">managementState</span></span>](../resources/intune-devices-managementstate.md)|<span data-ttu-id="58a40-160">デバイスの管理状態。</span><span class="sxs-lookup"><span data-stu-id="58a40-160">Management state of the device.</span></span> <span data-ttu-id="58a40-161">可能な値は、`managed`、`retirePending`、`retireFailed`、`wipePending`、`wipeFailed`、`unhealthy`、`deletePending`、`retireIssued`、`wipeIssued`、`wipeCanceled`、`retireCanceled`、`discovered` です。</span><span class="sxs-lookup"><span data-stu-id="58a40-161">Possible values are: `managed`, `retirePending`, `retireFailed`, `wipePending`, `wipeFailed`, `unhealthy`, `deletePending`, `retireIssued`, `wipeIssued`, `wipeCanceled`, `retireCanceled`, `discovered`.</span></span>|
|<span data-ttu-id="58a40-162">enrolledDateTime</span><span class="sxs-lookup"><span data-stu-id="58a40-162">enrolledDateTime</span></span>|<span data-ttu-id="58a40-163">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="58a40-163">DateTimeOffset</span></span>|<span data-ttu-id="58a40-164">デバイスの登録時刻。</span><span class="sxs-lookup"><span data-stu-id="58a40-164">Enrollment time of the device.</span></span>|
|<span data-ttu-id="58a40-165">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="58a40-165">lastSyncDateTime</span></span>|<span data-ttu-id="58a40-166">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="58a40-166">DateTimeOffset</span></span>|<span data-ttu-id="58a40-167">デバイスが Intune との正常な同期を最終的に完了した日時。</span><span class="sxs-lookup"><span data-stu-id="58a40-167">The date and time that the device last completed a successful sync with Intune.</span></span>|
|<span data-ttu-id="58a40-168">chassisType</span><span class="sxs-lookup"><span data-stu-id="58a40-168">chassisType</span></span>|[<span data-ttu-id="58a40-169">chassisType</span><span class="sxs-lookup"><span data-stu-id="58a40-169">chassisType</span></span>](../resources/intune-devices-chassistype.md)|<span data-ttu-id="58a40-170">デバイスのシャーシの種類。</span><span class="sxs-lookup"><span data-stu-id="58a40-170">Chassis type of the device.</span></span> <span data-ttu-id="58a40-171">可能な値は、`unknown`、`desktop`、`laptop`、`worksWorkstation`、`enterpriseServer`、`phone`、`tablet`、`mobileOther`、`mobileUnknown` です。</span><span class="sxs-lookup"><span data-stu-id="58a40-171">Possible values are: `unknown`, `desktop`, `laptop`, `worksWorkstation`, `enterpriseServer`, `phone`, `tablet`, `mobileOther`, `mobileUnknown`.</span></span>|
|<span data-ttu-id="58a40-172">operatingSystem</span><span class="sxs-lookup"><span data-stu-id="58a40-172">operatingSystem</span></span>|<span data-ttu-id="58a40-173">文字列</span><span class="sxs-lookup"><span data-stu-id="58a40-173">String</span></span>|<span data-ttu-id="58a40-174">デバイスのオペレーティング システム。</span><span class="sxs-lookup"><span data-stu-id="58a40-174">Operating system of the device.</span></span> <span data-ttu-id="58a40-175">Windows、iOS など。</span><span class="sxs-lookup"><span data-stu-id="58a40-175">Windows, iOS, etc.</span></span>|
|<span data-ttu-id="58a40-176">deviceType</span><span class="sxs-lookup"><span data-stu-id="58a40-176">deviceType</span></span>|[<span data-ttu-id="58a40-177">deviceType</span><span class="sxs-lookup"><span data-stu-id="58a40-177">deviceType</span></span>](../resources/intune-shared-devicetype.md)|<span data-ttu-id="58a40-178">デバイスのプラットフォーム。</span><span class="sxs-lookup"><span data-stu-id="58a40-178">Platform of the device.</span></span> <span data-ttu-id="58a40-179">可能な値: `desktop`、 `windowsRT` `winMO6` `nokia` `windowsPhone` `mac` `winCE` `winEmbedded` `iPhone` `iPad` `iPod` `android`、、、、、、、、、、、、 `iSocConsumer` `unix` `macMDM` `holoLens` `surfaceHub` `androidForWork` `androidEnterprise`, `blackberry`, `palm`, `unknown`.</span><span class="sxs-lookup"><span data-stu-id="58a40-179">Possible values are: `desktop`, `windowsRT`, `winMO6`, `nokia`, `windowsPhone`, `mac`, `winCE`, `winEmbedded`, `iPhone`, `iPad`, `iPod`, `android`, `iSocConsumer`, `unix`, `macMDM`, `holoLens`, `surfaceHub`, `androidForWork`, `androidEnterprise`, `blackberry`, `palm`, `unknown`.</span></span>|
|<span data-ttu-id="58a40-180">complianceState</span><span class="sxs-lookup"><span data-stu-id="58a40-180">complianceState</span></span>|[<span data-ttu-id="58a40-181">complianceState</span><span class="sxs-lookup"><span data-stu-id="58a40-181">complianceState</span></span>](../resources/intune-devices-compliancestate.md)|<span data-ttu-id="58a40-182">デバイスのコンプライアンス状態。</span><span class="sxs-lookup"><span data-stu-id="58a40-182">Compliance state of the device.</span></span> <span data-ttu-id="58a40-183">可能な値は、`unknown`、`compliant`、`noncompliant`、`conflict`、`error`、`inGracePeriod`、`configManager` です。</span><span class="sxs-lookup"><span data-stu-id="58a40-183">Possible values are: `unknown`, `compliant`, `noncompliant`, `conflict`, `error`, `inGracePeriod`, `configManager`.</span></span>|
|<span data-ttu-id="58a40-184">jailBroken</span><span class="sxs-lookup"><span data-stu-id="58a40-184">jailBroken</span></span>|<span data-ttu-id="58a40-185">String</span><span class="sxs-lookup"><span data-stu-id="58a40-185">String</span></span>|<span data-ttu-id="58a40-186">デバイスが脱獄またはルート化されているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="58a40-186">whether the device is jail broken or rooted.</span></span>|
|<span data-ttu-id="58a40-187">managementAgent</span><span class="sxs-lookup"><span data-stu-id="58a40-187">managementAgent</span></span>|[<span data-ttu-id="58a40-188">managementAgentType</span><span class="sxs-lookup"><span data-stu-id="58a40-188">managementAgentType</span></span>](../resources/intune-devices-managementagenttype.md)|<span data-ttu-id="58a40-189">デバイスの管理チャネル。</span><span class="sxs-lookup"><span data-stu-id="58a40-189">Management channel of the device.</span></span> <span data-ttu-id="58a40-190">Intune、EAS など。可能な値は`eas`、 `mdm`、 `easMdm` `intuneClient` `easIntuneClient` `configurationManagerClient` `jamf` `googleCloudDevicePolicyController`、、、、、、、、、 `microsoft365ManagedMdm`、、です。 `configurationManagerClientMdm` `configurationManagerClientMdmEas` `unknown`</span><span class="sxs-lookup"><span data-stu-id="58a40-190">Intune, EAS, etc. Possible values are: `eas`, `mdm`, `easMdm`, `intuneClient`, `easIntuneClient`, `configurationManagerClient`, `configurationManagerClientMdm`, `configurationManagerClientMdmEas`, `unknown`, `jamf`, `googleCloudDevicePolicyController`, `microsoft365ManagedMdm`.</span></span>|
|<span data-ttu-id="58a40-191">osVersion</span><span class="sxs-lookup"><span data-stu-id="58a40-191">osVersion</span></span>|<span data-ttu-id="58a40-192">String</span><span class="sxs-lookup"><span data-stu-id="58a40-192">String</span></span>|<span data-ttu-id="58a40-193">デバイスのオペレーティング システムのバージョン。</span><span class="sxs-lookup"><span data-stu-id="58a40-193">Operating system version of the device.</span></span>|
|<span data-ttu-id="58a40-194">easActivated</span><span class="sxs-lookup"><span data-stu-id="58a40-194">easActivated</span></span>|<span data-ttu-id="58a40-195">Boolean</span><span class="sxs-lookup"><span data-stu-id="58a40-195">Boolean</span></span>|<span data-ttu-id="58a40-196">Exchange ActiveSync がアクティブになっているデバイスかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="58a40-196">Whether the device is Exchange ActiveSync activated.</span></span>|
|<span data-ttu-id="58a40-197">easDeviceId</span><span class="sxs-lookup"><span data-stu-id="58a40-197">easDeviceId</span></span>|<span data-ttu-id="58a40-198">String</span><span class="sxs-lookup"><span data-stu-id="58a40-198">String</span></span>|<span data-ttu-id="58a40-199">デバイスの Exchange ActiveSync の ID。</span><span class="sxs-lookup"><span data-stu-id="58a40-199">Exchange ActiveSync Id of the device.</span></span>|
|<span data-ttu-id="58a40-200">easActivationDateTime</span><span class="sxs-lookup"><span data-stu-id="58a40-200">easActivationDateTime</span></span>|<span data-ttu-id="58a40-201">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="58a40-201">DateTimeOffset</span></span>|<span data-ttu-id="58a40-202">デバイスの Exchange ActivationSync のアクティブ化の時刻。</span><span class="sxs-lookup"><span data-stu-id="58a40-202">Exchange ActivationSync activation time of the device.</span></span>|
|<span data-ttu-id="58a40-203">aadRegistered</span><span class="sxs-lookup"><span data-stu-id="58a40-203">aadRegistered</span></span>|<span data-ttu-id="58a40-204">Boolean</span><span class="sxs-lookup"><span data-stu-id="58a40-204">Boolean</span></span>|<span data-ttu-id="58a40-205">Azure Active Directory が登録されているデバイスかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="58a40-205">Whether the device is Azure Active Directory registered.</span></span>|
|<span data-ttu-id="58a40-206">azureADRegistered</span><span class="sxs-lookup"><span data-stu-id="58a40-206">azureADRegistered</span></span>|<span data-ttu-id="58a40-207">Boolean</span><span class="sxs-lookup"><span data-stu-id="58a40-207">Boolean</span></span>|<span data-ttu-id="58a40-208">Azure Active Directory が登録されているデバイスかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="58a40-208">Whether the device is Azure Active Directory registered.</span></span>|
|<span data-ttu-id="58a40-209">deviceEnrollmentType</span><span class="sxs-lookup"><span data-stu-id="58a40-209">deviceEnrollmentType</span></span>|[<span data-ttu-id="58a40-210">deviceEnrollmentType</span><span class="sxs-lookup"><span data-stu-id="58a40-210">deviceEnrollmentType</span></span>](../resources/intune-shared-deviceenrollmenttype.md)|<span data-ttu-id="58a40-211">デバイスの登録の種類。</span><span class="sxs-lookup"><span data-stu-id="58a40-211">Enrollment type of the device.</span></span> <span data-ttu-id="58a40-212">可能な値は、`unknown`、`userEnrollment`、`deviceEnrollmentManager`、`appleBulkWithUser`、`appleBulkWithoutUser`、`windowsAzureADJoin`、`windowsBulkUserless`、`windowsAutoEnrollment`、`windowsBulkAzureDomainJoin`、`windowsCoManagement` です。</span><span class="sxs-lookup"><span data-stu-id="58a40-212">Possible values are: `unknown`, `userEnrollment`, `deviceEnrollmentManager`, `appleBulkWithUser`, `appleBulkWithoutUser`, `windowsAzureADJoin`, `windowsBulkUserless`, `windowsAutoEnrollment`, `windowsBulkAzureDomainJoin`, `windowsCoManagement`.</span></span>|
|<span data-ttu-id="58a40-213">lostModeState</span><span class="sxs-lookup"><span data-stu-id="58a40-213">lostModeState</span></span>|[<span data-ttu-id="58a40-214">lostModeState</span><span class="sxs-lookup"><span data-stu-id="58a40-214">lostModeState</span></span>](../resources/intune-devices-lostmodestate.md)|<span data-ttu-id="58a40-215">失われたモードが有効か無効かを示します。</span><span class="sxs-lookup"><span data-stu-id="58a40-215">Indicates if Lost mode is enabled or disabled.</span></span> <span data-ttu-id="58a40-216">可能な値は、`disabled`、`enabled` です。</span><span class="sxs-lookup"><span data-stu-id="58a40-216">Possible values are: `disabled`, `enabled`.</span></span>|
|<span data-ttu-id="58a40-217">activationLockBypassCode</span><span class="sxs-lookup"><span data-stu-id="58a40-217">activationLockBypassCode</span></span>|<span data-ttu-id="58a40-218">String</span><span class="sxs-lookup"><span data-stu-id="58a40-218">String</span></span>|<span data-ttu-id="58a40-219">デバイスのアクティベーション ロックをバイパスするためのコード。</span><span class="sxs-lookup"><span data-stu-id="58a40-219">Code that allows the Activation Lock on a device to be bypassed.</span></span>|
|<span data-ttu-id="58a40-220">emailAddress</span><span class="sxs-lookup"><span data-stu-id="58a40-220">emailAddress</span></span>|<span data-ttu-id="58a40-221">String</span><span class="sxs-lookup"><span data-stu-id="58a40-221">String</span></span>|<span data-ttu-id="58a40-222">デバイスに関連付けられているユーザーの電子メール</span><span class="sxs-lookup"><span data-stu-id="58a40-222">Email(s) for the user associated with the device</span></span>|
|<span data-ttu-id="58a40-223">azureActiveDirectoryDeviceId</span><span class="sxs-lookup"><span data-stu-id="58a40-223">azureActiveDirectoryDeviceId</span></span>|<span data-ttu-id="58a40-224">String</span><span class="sxs-lookup"><span data-stu-id="58a40-224">String</span></span>|<span data-ttu-id="58a40-225">Azure Active Directory デバイスの一意識別子。</span><span class="sxs-lookup"><span data-stu-id="58a40-225">The unique identifier for the Azure Active Directory device.</span></span> <span data-ttu-id="58a40-226">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="58a40-226">Read only.</span></span>|
|<span data-ttu-id="58a40-227">azureADDeviceId</span><span class="sxs-lookup"><span data-stu-id="58a40-227">azureADDeviceId</span></span>|<span data-ttu-id="58a40-228">String</span><span class="sxs-lookup"><span data-stu-id="58a40-228">String</span></span>|<span data-ttu-id="58a40-229">Azure Active Directory デバイスの一意識別子。</span><span class="sxs-lookup"><span data-stu-id="58a40-229">The unique identifier for the Azure Active Directory device.</span></span> <span data-ttu-id="58a40-230">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="58a40-230">Read only.</span></span>|
|<span data-ttu-id="58a40-231">deviceRegistrationState</span><span class="sxs-lookup"><span data-stu-id="58a40-231">deviceRegistrationState</span></span>|[<span data-ttu-id="58a40-232">deviceRegistrationState</span><span class="sxs-lookup"><span data-stu-id="58a40-232">deviceRegistrationState</span></span>](../resources/intune-devices-deviceregistrationstate.md)|<span data-ttu-id="58a40-233">デバイスの登録状態。</span><span class="sxs-lookup"><span data-stu-id="58a40-233">Device registration state.</span></span> <span data-ttu-id="58a40-234">可能な値は、`notRegistered`、`registered`、`revoked`、`keyConflict`、`approvalPending`、`certificateReset`、`notRegisteredPendingEnrollment`、`unknown` です。</span><span class="sxs-lookup"><span data-stu-id="58a40-234">Possible values are: `notRegistered`, `registered`, `revoked`, `keyConflict`, `approvalPending`, `certificateReset`, `notRegisteredPendingEnrollment`, `unknown`.</span></span>|
|<span data-ttu-id="58a40-235">deviceCategoryDisplayName</span><span class="sxs-lookup"><span data-stu-id="58a40-235">deviceCategoryDisplayName</span></span>|<span data-ttu-id="58a40-236">String</span><span class="sxs-lookup"><span data-stu-id="58a40-236">String</span></span>|<span data-ttu-id="58a40-237">デバイス カテゴリの表示名</span><span class="sxs-lookup"><span data-stu-id="58a40-237">Device category display name</span></span>|
|<span data-ttu-id="58a40-238">isSupervised</span><span class="sxs-lookup"><span data-stu-id="58a40-238">isSupervised</span></span>|<span data-ttu-id="58a40-239">Boolean</span><span class="sxs-lookup"><span data-stu-id="58a40-239">Boolean</span></span>|<span data-ttu-id="58a40-240">デバイスの管理状況</span><span class="sxs-lookup"><span data-stu-id="58a40-240">Device supervised status</span></span>|
|<span data-ttu-id="58a40-241">exchangeLastSuccessfulSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="58a40-241">exchangeLastSuccessfulSyncDateTime</span></span>|<span data-ttu-id="58a40-242">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="58a40-242">DateTimeOffset</span></span>|<span data-ttu-id="58a40-243">最後にデバイスが Exchange に接続した時刻。</span><span class="sxs-lookup"><span data-stu-id="58a40-243">Last time the device contacted Exchange.</span></span>|
|<span data-ttu-id="58a40-244">exchangeAccessState</span><span class="sxs-lookup"><span data-stu-id="58a40-244">exchangeAccessState</span></span>|[<span data-ttu-id="58a40-245">deviceManagementExchangeAccessState</span><span class="sxs-lookup"><span data-stu-id="58a40-245">deviceManagementExchangeAccessState</span></span>](../resources/intune-devices-devicemanagementexchangeaccessstate.md)|<span data-ttu-id="58a40-246">Exchange でのデバイスのアクセスの状態。</span><span class="sxs-lookup"><span data-stu-id="58a40-246">The Access State of the device in Exchange.</span></span> <span data-ttu-id="58a40-247">可能な値は、`none`、`unknown`、`allowed`、`blocked`、`quarantined` です。</span><span class="sxs-lookup"><span data-stu-id="58a40-247">Possible values are: `none`, `unknown`, `allowed`, `blocked`, `quarantined`.</span></span>|
|<span data-ttu-id="58a40-248">exchangeAccessStateReason</span><span class="sxs-lookup"><span data-stu-id="58a40-248">exchangeAccessStateReason</span></span>|[<span data-ttu-id="58a40-249">deviceManagementExchangeAccessStateReason</span><span class="sxs-lookup"><span data-stu-id="58a40-249">deviceManagementExchangeAccessStateReason</span></span>](../resources/intune-devices-devicemanagementexchangeaccessstatereason.md)|<span data-ttu-id="58a40-250">Exchange でのデバイスのアクセス状態の理由。
</span><span class="sxs-lookup"><span data-stu-id="58a40-250">The reason for the device's access state in Exchange.</span></span> <span data-ttu-id="58a40-251">可能な値は、`none`、`unknown`、`exchangeGlobalRule`、`exchangeIndividualRule`、`exchangeDeviceRule`、`exchangeUpgrade`、`exchangeMailboxPolicy`、`other`、`compliant`、`notCompliant`、`notEnrolled`、`unknownLocation`、`mfaRequired`、`azureADBlockDueToAccessPolicy`、`compromisedPassword`、`deviceNotKnownWithManagedApp` です。</span><span class="sxs-lookup"><span data-stu-id="58a40-251">Possible values are: `none`, `unknown`, `exchangeGlobalRule`, `exchangeIndividualRule`, `exchangeDeviceRule`, `exchangeUpgrade`, `exchangeMailboxPolicy`, `other`, `compliant`, `notCompliant`, `notEnrolled`, `unknownLocation`, `mfaRequired`, `azureADBlockDueToAccessPolicy`, `compromisedPassword`, `deviceNotKnownWithManagedApp`.</span></span>|
|<span data-ttu-id="58a40-252">remoteAssistanceSessionUrl</span><span class="sxs-lookup"><span data-stu-id="58a40-252">remoteAssistanceSessionUrl</span></span>|<span data-ttu-id="58a40-253">String</span><span class="sxs-lookup"><span data-stu-id="58a40-253">String</span></span>|<span data-ttu-id="58a40-254">デバイスとのリモート アシスタンス セッションを確立できるようにする URL。</span><span class="sxs-lookup"><span data-stu-id="58a40-254">Url that allows a Remote Assistance session to be established with the device.</span></span>|
|<span data-ttu-id="58a40-255">remoteAssistanceSessionErrorDetails</span><span class="sxs-lookup"><span data-stu-id="58a40-255">remoteAssistanceSessionErrorDetails</span></span>|<span data-ttu-id="58a40-256">String</span><span class="sxs-lookup"><span data-stu-id="58a40-256">String</span></span>|<span data-ttu-id="58a40-257">リモート アシスタンス セッション オブジェクトの作成時に問題を識別するエラー文字列。</span><span class="sxs-lookup"><span data-stu-id="58a40-257">An error string that identifies issues when creating Remote Assistance session objects.</span></span>|
|<span data-ttu-id="58a40-258">isEncrypted</span><span class="sxs-lookup"><span data-stu-id="58a40-258">isEncrypted</span></span>|<span data-ttu-id="58a40-259">Boolean</span><span class="sxs-lookup"><span data-stu-id="58a40-259">Boolean</span></span>|<span data-ttu-id="58a40-260">デバイスの暗号化の状態</span><span class="sxs-lookup"><span data-stu-id="58a40-260">Device encryption status</span></span>|
|<span data-ttu-id="58a40-261">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="58a40-261">userPrincipalName</span></span>|<span data-ttu-id="58a40-262">String</span><span class="sxs-lookup"><span data-stu-id="58a40-262">String</span></span>|<span data-ttu-id="58a40-263">デバイスのユーザー プリンシパル名。</span><span class="sxs-lookup"><span data-stu-id="58a40-263">Device user principal name</span></span>|
|<span data-ttu-id="58a40-264">model</span><span class="sxs-lookup"><span data-stu-id="58a40-264">model</span></span>|<span data-ttu-id="58a40-265">String</span><span class="sxs-lookup"><span data-stu-id="58a40-265">String</span></span>|<span data-ttu-id="58a40-266">デバイスのモデル</span><span class="sxs-lookup"><span data-stu-id="58a40-266">Model of the device</span></span>|
|<span data-ttu-id="58a40-267">manufacturer</span><span class="sxs-lookup"><span data-stu-id="58a40-267">manufacturer</span></span>|<span data-ttu-id="58a40-268">String</span><span class="sxs-lookup"><span data-stu-id="58a40-268">String</span></span>|<span data-ttu-id="58a40-269">デバイスのメーカー</span><span class="sxs-lookup"><span data-stu-id="58a40-269">Manufacturer of the device</span></span>|
|<span data-ttu-id="58a40-270">imei</span><span class="sxs-lookup"><span data-stu-id="58a40-270">imei</span></span>|<span data-ttu-id="58a40-271">String</span><span class="sxs-lookup"><span data-stu-id="58a40-271">String</span></span>|<span data-ttu-id="58a40-272">IMEI</span><span class="sxs-lookup"><span data-stu-id="58a40-272">IMEI</span></span>|
|<span data-ttu-id="58a40-273">complianceGracePeriodExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="58a40-273">complianceGracePeriodExpirationDateTime</span></span>|<span data-ttu-id="58a40-274">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="58a40-274">DateTimeOffset</span></span>|<span data-ttu-id="58a40-275">デバイス コンプライアンスの猶予期間が経過する DateTime</span><span class="sxs-lookup"><span data-stu-id="58a40-275">The DateTime when device compliance grace period expires</span></span>|
|<span data-ttu-id="58a40-276">serialNumber</span><span class="sxs-lookup"><span data-stu-id="58a40-276">serialNumber</span></span>|<span data-ttu-id="58a40-277">String</span><span class="sxs-lookup"><span data-stu-id="58a40-277">String</span></span>|<span data-ttu-id="58a40-278">シリアル番号</span><span class="sxs-lookup"><span data-stu-id="58a40-278">SerialNumber</span></span>|
|<span data-ttu-id="58a40-279">phoneNumber</span><span class="sxs-lookup"><span data-stu-id="58a40-279">phoneNumber</span></span>|<span data-ttu-id="58a40-280">String</span><span class="sxs-lookup"><span data-stu-id="58a40-280">String</span></span>|<span data-ttu-id="58a40-281">デバイスの電話番号</span><span class="sxs-lookup"><span data-stu-id="58a40-281">Phone number of the device</span></span>|
|<span data-ttu-id="58a40-282">androidSecurityPatchLevel</span><span class="sxs-lookup"><span data-stu-id="58a40-282">androidSecurityPatchLevel</span></span>|<span data-ttu-id="58a40-283">String</span><span class="sxs-lookup"><span data-stu-id="58a40-283">String</span></span>|<span data-ttu-id="58a40-284">Android セキュリティ パッチのレベル</span><span class="sxs-lookup"><span data-stu-id="58a40-284">Android security patch level</span></span>|
|<span data-ttu-id="58a40-285">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="58a40-285">userDisplayName</span></span>|<span data-ttu-id="58a40-286">String</span><span class="sxs-lookup"><span data-stu-id="58a40-286">String</span></span>|<span data-ttu-id="58a40-287">ユーザーの表示名</span><span class="sxs-lookup"><span data-stu-id="58a40-287">User display name</span></span>|
|<span data-ttu-id="58a40-288">configurationManagerClientEnabledFeatures</span><span class="sxs-lookup"><span data-stu-id="58a40-288">configurationManagerClientEnabledFeatures</span></span>|[<span data-ttu-id="58a40-289">configurationManagerClientEnabledFeatures</span><span class="sxs-lookup"><span data-stu-id="58a40-289">configurationManagerClientEnabledFeatures</span></span>](../resources/intune-devices-configurationmanagerclientenabledfeatures.md)|<span data-ttu-id="58a40-290">ConfigrMgr クライアント対応機能
</span><span class="sxs-lookup"><span data-stu-id="58a40-290">ConfigrMgr client enabled features</span></span>|
|<span data-ttu-id="58a40-291">wiFiMacAddress</span><span class="sxs-lookup"><span data-stu-id="58a40-291">wiFiMacAddress</span></span>|<span data-ttu-id="58a40-292">String</span><span class="sxs-lookup"><span data-stu-id="58a40-292">String</span></span>|<span data-ttu-id="58a40-293">Wi-Fi MAC</span><span class="sxs-lookup"><span data-stu-id="58a40-293">Wi-Fi MAC</span></span>|
|<span data-ttu-id="58a40-294">deviceHealthAttestationState</span><span class="sxs-lookup"><span data-stu-id="58a40-294">deviceHealthAttestationState</span></span>|[<span data-ttu-id="58a40-295">deviceHealthAttestationState</span><span class="sxs-lookup"><span data-stu-id="58a40-295">deviceHealthAttestationState</span></span>](../resources/intune-devices-devicehealthattestationstate.md)|<span data-ttu-id="58a40-296">デバイスの正常性構成証明の状態。</span><span class="sxs-lookup"><span data-stu-id="58a40-296">The device health attestation state.</span></span>|
|<span data-ttu-id="58a40-297">subscriberCarrier</span><span class="sxs-lookup"><span data-stu-id="58a40-297">subscriberCarrier</span></span>|<span data-ttu-id="58a40-298">String</span><span class="sxs-lookup"><span data-stu-id="58a40-298">String</span></span>|<span data-ttu-id="58a40-299">サブスクライバー通信事業者</span><span class="sxs-lookup"><span data-stu-id="58a40-299">Subscriber Carrier</span></span>|
|<span data-ttu-id="58a40-300">meid</span><span class="sxs-lookup"><span data-stu-id="58a40-300">meid</span></span>|<span data-ttu-id="58a40-301">String</span><span class="sxs-lookup"><span data-stu-id="58a40-301">String</span></span>|<span data-ttu-id="58a40-302">MEID</span><span class="sxs-lookup"><span data-stu-id="58a40-302">MEID</span></span>|
|<span data-ttu-id="58a40-303">totalStorageSpaceInBytes</span><span class="sxs-lookup"><span data-stu-id="58a40-303">totalStorageSpaceInBytes</span></span>|<span data-ttu-id="58a40-304">Int64</span><span class="sxs-lookup"><span data-stu-id="58a40-304">Int64</span></span>|<span data-ttu-id="58a40-305">記憶域の合計 (バイト)</span><span class="sxs-lookup"><span data-stu-id="58a40-305">Total Storage in Bytes</span></span>|
|<span data-ttu-id="58a40-306">freeStorageSpaceInBytes</span><span class="sxs-lookup"><span data-stu-id="58a40-306">freeStorageSpaceInBytes</span></span>|<span data-ttu-id="58a40-307">Int64</span><span class="sxs-lookup"><span data-stu-id="58a40-307">Int64</span></span>|<span data-ttu-id="58a40-308">空き記憶域 (バイト)</span><span class="sxs-lookup"><span data-stu-id="58a40-308">Free Storage in Bytes</span></span>|
|<span data-ttu-id="58a40-309">managedDeviceName</span><span class="sxs-lookup"><span data-stu-id="58a40-309">managedDeviceName</span></span>|<span data-ttu-id="58a40-310">String</span><span class="sxs-lookup"><span data-stu-id="58a40-310">String</span></span>|<span data-ttu-id="58a40-311">デバイスを識別する名前が自動的に生成されます。</span><span class="sxs-lookup"><span data-stu-id="58a40-311">Automatically generated name to identify a device.</span></span> <span data-ttu-id="58a40-312">ユーザー フレンドリ名に上書きできます。</span><span class="sxs-lookup"><span data-stu-id="58a40-312">Can be overwritten to a user friendly name.</span></span>|
|<span data-ttu-id="58a40-313">partnerReportedThreatState</span><span class="sxs-lookup"><span data-stu-id="58a40-313">partnerReportedThreatState</span></span>|[<span data-ttu-id="58a40-314">managedDevicePartnerReportedHealthState</span><span class="sxs-lookup"><span data-stu-id="58a40-314">managedDevicePartnerReportedHealthState</span></span>](../resources/intune-devices-manageddevicepartnerreportedhealthstate.md)|<span data-ttu-id="58a40-315">Mobile Threat Defense パートナーがアカウントおよびデバイスで使用されている場合の、デバイスの脅威の状態を示します。</span><span class="sxs-lookup"><span data-stu-id="58a40-315">Indicates the threat state of a device when a Mobile Threat Defense partner is in use by the account and device.</span></span> <span data-ttu-id="58a40-316">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="58a40-316">Read Only.</span></span> <span data-ttu-id="58a40-317">可能な値は、`unknown`、`activated`、`deactivated`、`secured`、`lowSeverity`、`mediumSeverity`、`highSeverity`、`unresponsive`、`compromised`、`misconfigured` です。</span><span class="sxs-lookup"><span data-stu-id="58a40-317">Possible values are: `unknown`, `activated`, `deactivated`, `secured`, `lowSeverity`, `mediumSeverity`, `highSeverity`, `unresponsive`, `compromised`, `misconfigured`.</span></span>|
|<span data-ttu-id="58a40-318">retireAfterDateTime</span><span class="sxs-lookup"><span data-stu-id="58a40-318">retireAfterDateTime</span></span>|<span data-ttu-id="58a40-319">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="58a40-319">DateTimeOffset</span></span>|<span data-ttu-id="58a40-320">スケジュールされたアクションのためにデバイスが自動廃棄されるまでの時間を示します。</span><span class="sxs-lookup"><span data-stu-id="58a40-320">Indicates the time after when a device will be auto retired because of scheduled action.</span></span>|
|<span data-ttu-id="58a40-321">usersLoggedOn</span><span class="sxs-lookup"><span data-stu-id="58a40-321">usersLoggedOn</span></span>|<span data-ttu-id="58a40-322">[loggedOnUser](../resources/intune-devices-loggedonuser.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="58a40-322">[loggedOnUser](../resources/intune-devices-loggedonuser.md) collection</span></span>|<span data-ttu-id="58a40-323">デバイスの最後にログオンしたユーザーを示します</span><span class="sxs-lookup"><span data-stu-id="58a40-323">Indicates the last logged on users of a device</span></span>|
|<span data-ttu-id="58a40-324">preferMdmOverGroupPolicyAppliedDateTime</span><span class="sxs-lookup"><span data-stu-id="58a40-324">preferMdmOverGroupPolicyAppliedDateTime</span></span>|<span data-ttu-id="58a40-325">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="58a40-325">DateTimeOffset</span></span>|<span data-ttu-id="58a40-326">PreferMdmOverGroupPolicy の設定が設定された DateTime を報告します。</span><span class="sxs-lookup"><span data-stu-id="58a40-326">Reports the DateTime the preferMdmOverGroupPolicy setting was set.</span></span>  <span data-ttu-id="58a40-327">設定すると、競合がある場合に Intune MDM 設定がグループポリシー設定を上書きします。</span><span class="sxs-lookup"><span data-stu-id="58a40-327">When set, the Intune MDM settings will override Group Policy settings if there is a conflict.</span></span> <span data-ttu-id="58a40-328">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="58a40-328">Read Only.</span></span>|
|<span data-ttu-id="58a40-329">autopilotEnrolled</span><span class="sxs-lookup"><span data-stu-id="58a40-329">autopilotEnrolled</span></span>|<span data-ttu-id="58a40-330">Boolean</span><span class="sxs-lookup"><span data-stu-id="58a40-330">Boolean</span></span>|<span data-ttu-id="58a40-331">管理対象デバイスが自動パイロットで登録されているかどうかを報告します。</span><span class="sxs-lookup"><span data-stu-id="58a40-331">Reports if the managed device is enrolled via auto-pilot.</span></span>|
|<span data-ttu-id="58a40-332">requireUserEnrollmentApproval</span><span class="sxs-lookup"><span data-stu-id="58a40-332">requireUserEnrollmentApproval</span></span>|<span data-ttu-id="58a40-333">Boolean</span><span class="sxs-lookup"><span data-stu-id="58a40-333">Boolean</span></span>|<span data-ttu-id="58a40-334">管理対象 iOS デバイスがユーザー承認登録であるかどうかを報告します。</span><span class="sxs-lookup"><span data-stu-id="58a40-334">Reports if the managed iOS device is user approval enrollment.</span></span>|
|<span data-ttu-id="58a40-335">managementCertificateExpirationDate</span><span class="sxs-lookup"><span data-stu-id="58a40-335">managementCertificateExpirationDate</span></span>|<span data-ttu-id="58a40-336">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="58a40-336">DateTimeOffset</span></span>|<span data-ttu-id="58a40-337">デバイス管理証明書の有効期限を報告する</span><span class="sxs-lookup"><span data-stu-id="58a40-337">Reports device management certificate expiration date</span></span>|
|<span data-ttu-id="58a40-338">iccid</span><span class="sxs-lookup"><span data-stu-id="58a40-338">iccid</span></span>|<span data-ttu-id="58a40-339">String</span><span class="sxs-lookup"><span data-stu-id="58a40-339">String</span></span>|<span data-ttu-id="58a40-340">Ic カード識別子。 SIM カードの一意の識別番号です。</span><span class="sxs-lookup"><span data-stu-id="58a40-340">Integrated Circuit Card Identifier, it is A SIM card's unique identification number.</span></span>|
|<span data-ttu-id="58a40-341">udid</span><span class="sxs-lookup"><span data-stu-id="58a40-341">udid</span></span>|<span data-ttu-id="58a40-342">String</span><span class="sxs-lookup"><span data-stu-id="58a40-342">String</span></span>|<span data-ttu-id="58a40-343">IOS および macOS デバイスの一意のデバイス識別子。</span><span class="sxs-lookup"><span data-stu-id="58a40-343">Unique Device Identifier for iOS and macOS devices.</span></span>|
|<span data-ttu-id="58a40-344">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="58a40-344">roleScopeTagIds</span></span>|<span data-ttu-id="58a40-345">String collection</span><span class="sxs-lookup"><span data-stu-id="58a40-345">String collection</span></span>|<span data-ttu-id="58a40-346">このデバイスインスタンスの範囲タグ Id のリスト。</span><span class="sxs-lookup"><span data-stu-id="58a40-346">List of Scope Tag IDs for this Device instance.</span></span>|
|<span data-ttu-id="58a40-347">windowsActiveMalwareCount 再計算</span><span class="sxs-lookup"><span data-stu-id="58a40-347">windowsActiveMalwareCount</span></span>|<span data-ttu-id="58a40-348">Int32</span><span class="sxs-lookup"><span data-stu-id="58a40-348">Int32</span></span>|<span data-ttu-id="58a40-349">この windows デバイスのアクティブなマルウェアの数</span><span class="sxs-lookup"><span data-stu-id="58a40-349">Count of active malware for this windows device</span></span>|
|<span data-ttu-id="58a40-350">windowsRemediatedMalwareCount</span><span class="sxs-lookup"><span data-stu-id="58a40-350">windowsRemediatedMalwareCount</span></span>|<span data-ttu-id="58a40-351">Int32</span><span class="sxs-lookup"><span data-stu-id="58a40-351">Int32</span></span>|<span data-ttu-id="58a40-352">この windows デバイスの修復済みマルウェアの数</span><span class="sxs-lookup"><span data-stu-id="58a40-352">Count of remediated malware for this windows device</span></span>|
|<span data-ttu-id="58a40-353">notes</span><span class="sxs-lookup"><span data-stu-id="58a40-353">notes</span></span>|<span data-ttu-id="58a40-354">String</span><span class="sxs-lookup"><span data-stu-id="58a40-354">String</span></span>|<span data-ttu-id="58a40-355">IT 管理者によって作成されたデバイスのメモ</span><span class="sxs-lookup"><span data-stu-id="58a40-355">Notes on the device created by IT Admin</span></span>|
|<span data-ttu-id="58a40-356">configurationManagerClientHealthState</span><span class="sxs-lookup"><span data-stu-id="58a40-356">configurationManagerClientHealthState</span></span>|[<span data-ttu-id="58a40-357">configurationManagerClientHealthState</span><span class="sxs-lookup"><span data-stu-id="58a40-357">configurationManagerClientHealthState</span></span>](../resources/intune-devices-configurationmanagerclienthealthstate.md)|<span data-ttu-id="58a40-358">構成マネージャークライアントの正常性状態。 MDM/ConfigMgr エージェントによって管理されるデバイスに対してのみ有効です。</span><span class="sxs-lookup"><span data-stu-id="58a40-358">Configuration manager client health state, valid only for devices managed by MDM/ConfigMgr Agent</span></span>|



## <a name="response"></a><span data-ttu-id="58a40-359">応答</span><span class="sxs-lookup"><span data-stu-id="58a40-359">Response</span></span>
<span data-ttu-id="58a40-360">成功した場合、このメソッドは `200 OK` 応答コードと、更新された [managedDevice](../resources/intune-devices-manageddevice.md) オブジェクトを応答本文で返します。</span><span class="sxs-lookup"><span data-stu-id="58a40-360">If successful, this method returns a `200 OK` response code and an updated [managedDevice](../resources/intune-devices-manageddevice.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="58a40-361">例</span><span class="sxs-lookup"><span data-stu-id="58a40-361">Example</span></span>

### <a name="request"></a><span data-ttu-id="58a40-362">要求</span><span class="sxs-lookup"><span data-stu-id="58a40-362">Request</span></span>
<span data-ttu-id="58a40-363">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="58a40-363">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="58a40-364">応答</span><span class="sxs-lookup"><span data-stu-id="58a40-364">Response</span></span>
<span data-ttu-id="58a40-p121">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="58a40-p121">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




