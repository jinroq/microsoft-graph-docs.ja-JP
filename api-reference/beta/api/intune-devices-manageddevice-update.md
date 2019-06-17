---
title: >
  managedDevice の更新
description: managedDevice オブジェクトのプロパティを更新します。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: c154be3a1691f125a8d2c8f68b28e4c246bb4b3c
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/14/2019
ms.locfileid: "34958201"
---
# <a name="update-manageddevice"></a><span data-ttu-id="53a69-103">managedDevice の更新
</span><span class="sxs-lookup"><span data-stu-id="53a69-103">Update managedDevice</span></span>

> <span data-ttu-id="53a69-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="53a69-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="53a69-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="53a69-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="53a69-106">[managedDevice](../resources/intune-devices-manageddevice.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="53a69-106">Update the properties of a [managedDevice](../resources/intune-devices-manageddevice.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="53a69-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="53a69-107">Prerequisites</span></span>
<span data-ttu-id="53a69-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="53a69-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="53a69-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="53a69-110">Permission type</span></span>|<span data-ttu-id="53a69-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="53a69-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="53a69-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="53a69-112">Delegated (work or school account)</span></span>|<span data-ttu-id="53a69-113">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="53a69-113">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="53a69-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="53a69-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="53a69-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="53a69-115">Not supported.</span></span>|
|<span data-ttu-id="53a69-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="53a69-116">Application</span></span>|<span data-ttu-id="53a69-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="53a69-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="53a69-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="53a69-118">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="53a69-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="53a69-119">Request headers</span></span>
|<span data-ttu-id="53a69-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="53a69-120">Header</span></span>|<span data-ttu-id="53a69-121">値</span><span class="sxs-lookup"><span data-stu-id="53a69-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="53a69-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="53a69-122">Authorization</span></span>|<span data-ttu-id="53a69-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="53a69-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="53a69-124">承諾</span><span class="sxs-lookup"><span data-stu-id="53a69-124">Accept</span></span>|<span data-ttu-id="53a69-125">application/json</span><span class="sxs-lookup"><span data-stu-id="53a69-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="53a69-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="53a69-126">Request body</span></span>
<span data-ttu-id="53a69-127">要求本文で、[managedDevice](../resources/intune-devices-manageddevice.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="53a69-127">In the request body, supply a JSON representation for the [managedDevice](../resources/intune-devices-manageddevice.md) object.</span></span>

<span data-ttu-id="53a69-128">次の表に、[managedDevice](../resources/intune-devices-manageddevice.md) の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="53a69-128">The following table shows the properties that are required when you create the [managedDevice](../resources/intune-devices-manageddevice.md).</span></span>

|<span data-ttu-id="53a69-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="53a69-129">Property</span></span>|<span data-ttu-id="53a69-130">型</span><span class="sxs-lookup"><span data-stu-id="53a69-130">Type</span></span>|<span data-ttu-id="53a69-131">説明</span><span class="sxs-lookup"><span data-stu-id="53a69-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="53a69-132">id</span><span class="sxs-lookup"><span data-stu-id="53a69-132">id</span></span>|<span data-ttu-id="53a69-133">文字列</span><span class="sxs-lookup"><span data-stu-id="53a69-133">String</span></span>|<span data-ttu-id="53a69-134">デバイスの一意識別子</span><span class="sxs-lookup"><span data-stu-id="53a69-134">Unique Identifier for the device</span></span>|
|<span data-ttu-id="53a69-135">userId</span><span class="sxs-lookup"><span data-stu-id="53a69-135">userId</span></span>|<span data-ttu-id="53a69-136">String</span><span class="sxs-lookup"><span data-stu-id="53a69-136">String</span></span>|<span data-ttu-id="53a69-137">デバイスに関連付けられているユーザーの一意の識別子</span><span class="sxs-lookup"><span data-stu-id="53a69-137">Unique Identifier for the user associated with the device</span></span>|
|<span data-ttu-id="53a69-138">deviceName</span><span class="sxs-lookup"><span data-stu-id="53a69-138">deviceName</span></span>|<span data-ttu-id="53a69-139">String</span><span class="sxs-lookup"><span data-stu-id="53a69-139">String</span></span>|<span data-ttu-id="53a69-140">デバイスの名前</span><span class="sxs-lookup"><span data-stu-id="53a69-140">Name of the device</span></span>|
|<span data-ttu-id="53a69-141">hardwareInformation</span><span class="sxs-lookup"><span data-stu-id="53a69-141">hardwareInformation</span></span>|[<span data-ttu-id="53a69-142">hardwareInformation</span><span class="sxs-lookup"><span data-stu-id="53a69-142">hardwareInformation</span></span>](../resources/intune-devices-hardwareinformation.md)|<span data-ttu-id="53a69-143">デバイスのハードワードの詳細。</span><span class="sxs-lookup"><span data-stu-id="53a69-143">The hardward details for the device.</span></span>  <span data-ttu-id="53a69-144">記憶領域、製造元、シリアル番号などの情報が含まれます。</span><span class="sxs-lookup"><span data-stu-id="53a69-144">Includes information such as storage space, manufacturer, serial number, etc.</span></span>|
|<span data-ttu-id="53a69-145">ownerType</span><span class="sxs-lookup"><span data-stu-id="53a69-145">ownerType</span></span>|[<span data-ttu-id="53a69-146">ownerType</span><span class="sxs-lookup"><span data-stu-id="53a69-146">ownerType</span></span>](../resources/intune-devices-ownertype.md)|<span data-ttu-id="53a69-147">デバイスの所有権。</span><span class="sxs-lookup"><span data-stu-id="53a69-147">Ownership of the device.</span></span> <span data-ttu-id="53a69-148">' Company ' または ' personal ' にすることができます。</span><span class="sxs-lookup"><span data-stu-id="53a69-148">Can be 'company' or 'personal'.</span></span> <span data-ttu-id="53a69-149">可能な値は、`unknown`、`company`、`personal` です。</span><span class="sxs-lookup"><span data-stu-id="53a69-149">Possible values are: `unknown`, `company`, `personal`.</span></span>|
|<span data-ttu-id="53a69-150">managedDeviceOwnerType</span><span class="sxs-lookup"><span data-stu-id="53a69-150">managedDeviceOwnerType</span></span>|[<span data-ttu-id="53a69-151">managedDeviceOwnerType</span><span class="sxs-lookup"><span data-stu-id="53a69-151">managedDeviceOwnerType</span></span>](../resources/intune-devices-manageddeviceownertype.md)|<span data-ttu-id="53a69-152">デバイスの所有権。</span><span class="sxs-lookup"><span data-stu-id="53a69-152">Ownership of the device.</span></span> <span data-ttu-id="53a69-153">' Company ' または ' personal ' にすることができます。</span><span class="sxs-lookup"><span data-stu-id="53a69-153">Can be 'company' or 'personal'.</span></span> <span data-ttu-id="53a69-154">可能な値は、`unknown`、`company`、`personal` です。</span><span class="sxs-lookup"><span data-stu-id="53a69-154">Possible values are: `unknown`, `company`, `personal`.</span></span>|
|<span data-ttu-id="53a69-155">deviceActionResults</span><span class="sxs-lookup"><span data-stu-id="53a69-155">deviceActionResults</span></span>|<span data-ttu-id="53a69-156">[deviceActionResult](../resources/intune-devices-deviceactionresult.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="53a69-156">[deviceActionResult](../resources/intune-devices-deviceactionresult.md) collection</span></span>|<span data-ttu-id="53a69-157">ComplexType deviceActionResult オブジェクトのリスト。</span><span class="sxs-lookup"><span data-stu-id="53a69-157">List of ComplexType deviceActionResult objects.</span></span>|
|<span data-ttu-id="53a69-158">managementState</span><span class="sxs-lookup"><span data-stu-id="53a69-158">managementState</span></span>|[<span data-ttu-id="53a69-159">managementState</span><span class="sxs-lookup"><span data-stu-id="53a69-159">managementState</span></span>](../resources/intune-devices-managementstate.md)|<span data-ttu-id="53a69-160">デバイスの管理状態。</span><span class="sxs-lookup"><span data-stu-id="53a69-160">Management state of the device.</span></span> <span data-ttu-id="53a69-161">可能な値は、`managed`、`retirePending`、`retireFailed`、`wipePending`、`wipeFailed`、`unhealthy`、`deletePending`、`retireIssued`、`wipeIssued`、`wipeCanceled`、`retireCanceled`、`discovered` です。</span><span class="sxs-lookup"><span data-stu-id="53a69-161">Possible values are: `managed`, `retirePending`, `retireFailed`, `wipePending`, `wipeFailed`, `unhealthy`, `deletePending`, `retireIssued`, `wipeIssued`, `wipeCanceled`, `retireCanceled`, `discovered`.</span></span>|
|<span data-ttu-id="53a69-162">enrolledDateTime</span><span class="sxs-lookup"><span data-stu-id="53a69-162">enrolledDateTime</span></span>|<span data-ttu-id="53a69-163">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="53a69-163">DateTimeOffset</span></span>|<span data-ttu-id="53a69-164">デバイスの登録時刻。</span><span class="sxs-lookup"><span data-stu-id="53a69-164">Enrollment time of the device.</span></span>|
|<span data-ttu-id="53a69-165">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="53a69-165">lastSyncDateTime</span></span>|<span data-ttu-id="53a69-166">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="53a69-166">DateTimeOffset</span></span>|<span data-ttu-id="53a69-167">デバイスが Intune との正常な同期を最終的に完了した日時。</span><span class="sxs-lookup"><span data-stu-id="53a69-167">The date and time that the device last completed a successful sync with Intune.</span></span>|
|<span data-ttu-id="53a69-168">chassisType</span><span class="sxs-lookup"><span data-stu-id="53a69-168">chassisType</span></span>|[<span data-ttu-id="53a69-169">chassisType</span><span class="sxs-lookup"><span data-stu-id="53a69-169">chassisType</span></span>](../resources/intune-devices-chassistype.md)|<span data-ttu-id="53a69-170">デバイスのシャーシの種類。</span><span class="sxs-lookup"><span data-stu-id="53a69-170">Chassis type of the device.</span></span> <span data-ttu-id="53a69-171">可能な値は、`unknown`、`desktop`、`laptop`、`worksWorkstation`、`enterpriseServer`、`phone`、`tablet`、`mobileOther`、`mobileUnknown` です。</span><span class="sxs-lookup"><span data-stu-id="53a69-171">Possible values are: `unknown`, `desktop`, `laptop`, `worksWorkstation`, `enterpriseServer`, `phone`, `tablet`, `mobileOther`, `mobileUnknown`.</span></span>|
|<span data-ttu-id="53a69-172">operatingSystem</span><span class="sxs-lookup"><span data-stu-id="53a69-172">operatingSystem</span></span>|<span data-ttu-id="53a69-173">文字列</span><span class="sxs-lookup"><span data-stu-id="53a69-173">String</span></span>|<span data-ttu-id="53a69-174">デバイスのオペレーティング システム。</span><span class="sxs-lookup"><span data-stu-id="53a69-174">Operating system of the device.</span></span> <span data-ttu-id="53a69-175">Windows、iOS など。</span><span class="sxs-lookup"><span data-stu-id="53a69-175">Windows, iOS, etc.</span></span>|
|<span data-ttu-id="53a69-176">deviceType</span><span class="sxs-lookup"><span data-stu-id="53a69-176">deviceType</span></span>|[<span data-ttu-id="53a69-177">deviceType</span><span class="sxs-lookup"><span data-stu-id="53a69-177">deviceType</span></span>](../resources/intune-shared-devicetype.md)|<span data-ttu-id="53a69-178">デバイスのプラットフォーム。</span><span class="sxs-lookup"><span data-stu-id="53a69-178">Platform of the device.</span></span> <span data-ttu-id="53a69-179">可能な値: `desktop`、 `windowsRT` `winMO6` `nokia` `windowsPhone` `mac` `winCE` `winEmbedded` `iPhone` `iPad` `iPod` `android`、、、、、、、、、、、、 `iSocConsumer` `unix` `macMDM` `holoLens` `surfaceHub` `androidForWork` `androidEnterprise`, `blackberry`, `palm`, `unknown`.</span><span class="sxs-lookup"><span data-stu-id="53a69-179">Possible values are: `desktop`, `windowsRT`, `winMO6`, `nokia`, `windowsPhone`, `mac`, `winCE`, `winEmbedded`, `iPhone`, `iPad`, `iPod`, `android`, `iSocConsumer`, `unix`, `macMDM`, `holoLens`, `surfaceHub`, `androidForWork`, `androidEnterprise`, `blackberry`, `palm`, `unknown`.</span></span>|
|<span data-ttu-id="53a69-180">complianceState</span><span class="sxs-lookup"><span data-stu-id="53a69-180">complianceState</span></span>|[<span data-ttu-id="53a69-181">complianceState</span><span class="sxs-lookup"><span data-stu-id="53a69-181">complianceState</span></span>](../resources/intune-devices-compliancestate.md)|<span data-ttu-id="53a69-182">デバイスのコンプライアンス状態。</span><span class="sxs-lookup"><span data-stu-id="53a69-182">Compliance state of the device.</span></span> <span data-ttu-id="53a69-183">可能な値は、`unknown`、`compliant`、`noncompliant`、`conflict`、`error`、`inGracePeriod`、`configManager` です。</span><span class="sxs-lookup"><span data-stu-id="53a69-183">Possible values are: `unknown`, `compliant`, `noncompliant`, `conflict`, `error`, `inGracePeriod`, `configManager`.</span></span>|
|<span data-ttu-id="53a69-184">jailBroken</span><span class="sxs-lookup"><span data-stu-id="53a69-184">jailBroken</span></span>|<span data-ttu-id="53a69-185">String</span><span class="sxs-lookup"><span data-stu-id="53a69-185">String</span></span>|<span data-ttu-id="53a69-186">デバイスが脱獄またはルート化されているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="53a69-186">whether the device is jail broken or rooted.</span></span>|
|<span data-ttu-id="53a69-187">managementAgent</span><span class="sxs-lookup"><span data-stu-id="53a69-187">managementAgent</span></span>|[<span data-ttu-id="53a69-188">managementAgentType</span><span class="sxs-lookup"><span data-stu-id="53a69-188">managementAgentType</span></span>](../resources/intune-devices-managementagenttype.md)|<span data-ttu-id="53a69-189">デバイスの管理チャネル。</span><span class="sxs-lookup"><span data-stu-id="53a69-189">Management channel of the device.</span></span> <span data-ttu-id="53a69-190">Intune、EAS など。可能な値は`eas`、 `mdm`、 `easMdm` `intuneClient` `easIntuneClient` `configurationManagerClient` `jamf` `googleCloudDevicePolicyController`、、、、、、、、、 `microsoft365ManagedMdm`、、です。 `configurationManagerClientMdm` `configurationManagerClientMdmEas` `unknown`</span><span class="sxs-lookup"><span data-stu-id="53a69-190">Intune, EAS, etc. Possible values are: `eas`, `mdm`, `easMdm`, `intuneClient`, `easIntuneClient`, `configurationManagerClient`, `configurationManagerClientMdm`, `configurationManagerClientMdmEas`, `unknown`, `jamf`, `googleCloudDevicePolicyController`, `microsoft365ManagedMdm`.</span></span>|
|<span data-ttu-id="53a69-191">osVersion</span><span class="sxs-lookup"><span data-stu-id="53a69-191">osVersion</span></span>|<span data-ttu-id="53a69-192">String</span><span class="sxs-lookup"><span data-stu-id="53a69-192">String</span></span>|<span data-ttu-id="53a69-193">デバイスのオペレーティング システムのバージョン。</span><span class="sxs-lookup"><span data-stu-id="53a69-193">Operating system version of the device.</span></span>|
|<span data-ttu-id="53a69-194">easActivated</span><span class="sxs-lookup"><span data-stu-id="53a69-194">easActivated</span></span>|<span data-ttu-id="53a69-195">Boolean</span><span class="sxs-lookup"><span data-stu-id="53a69-195">Boolean</span></span>|<span data-ttu-id="53a69-196">Exchange ActiveSync がアクティブになっているデバイスかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="53a69-196">Whether the device is Exchange ActiveSync activated.</span></span>|
|<span data-ttu-id="53a69-197">easDeviceId</span><span class="sxs-lookup"><span data-stu-id="53a69-197">easDeviceId</span></span>|<span data-ttu-id="53a69-198">String</span><span class="sxs-lookup"><span data-stu-id="53a69-198">String</span></span>|<span data-ttu-id="53a69-199">デバイスの Exchange ActiveSync の ID。</span><span class="sxs-lookup"><span data-stu-id="53a69-199">Exchange ActiveSync Id of the device.</span></span>|
|<span data-ttu-id="53a69-200">easActivationDateTime</span><span class="sxs-lookup"><span data-stu-id="53a69-200">easActivationDateTime</span></span>|<span data-ttu-id="53a69-201">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="53a69-201">DateTimeOffset</span></span>|<span data-ttu-id="53a69-202">デバイスの Exchange ActivationSync のアクティブ化の時刻。</span><span class="sxs-lookup"><span data-stu-id="53a69-202">Exchange ActivationSync activation time of the device.</span></span>|
|<span data-ttu-id="53a69-203">aadRegistered</span><span class="sxs-lookup"><span data-stu-id="53a69-203">aadRegistered</span></span>|<span data-ttu-id="53a69-204">Boolean</span><span class="sxs-lookup"><span data-stu-id="53a69-204">Boolean</span></span>|<span data-ttu-id="53a69-205">Azure Active Directory が登録されているデバイスかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="53a69-205">Whether the device is Azure Active Directory registered.</span></span>|
|<span data-ttu-id="53a69-206">azureADRegistered</span><span class="sxs-lookup"><span data-stu-id="53a69-206">azureADRegistered</span></span>|<span data-ttu-id="53a69-207">Boolean</span><span class="sxs-lookup"><span data-stu-id="53a69-207">Boolean</span></span>|<span data-ttu-id="53a69-208">Azure Active Directory が登録されているデバイスかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="53a69-208">Whether the device is Azure Active Directory registered.</span></span>|
|<span data-ttu-id="53a69-209">deviceEnrollmentType</span><span class="sxs-lookup"><span data-stu-id="53a69-209">deviceEnrollmentType</span></span>|[<span data-ttu-id="53a69-210">deviceEnrollmentType</span><span class="sxs-lookup"><span data-stu-id="53a69-210">deviceEnrollmentType</span></span>](../resources/intune-shared-deviceenrollmenttype.md)|<span data-ttu-id="53a69-211">デバイスの登録の種類。</span><span class="sxs-lookup"><span data-stu-id="53a69-211">Enrollment type of the device.</span></span> <span data-ttu-id="53a69-212">可能な値は、`unknown`、`userEnrollment`、`deviceEnrollmentManager`、`appleBulkWithUser`、`appleBulkWithoutUser`、`windowsAzureADJoin`、`windowsBulkUserless`、`windowsAutoEnrollment`、`windowsBulkAzureDomainJoin`、`windowsCoManagement` です。</span><span class="sxs-lookup"><span data-stu-id="53a69-212">Possible values are: `unknown`, `userEnrollment`, `deviceEnrollmentManager`, `appleBulkWithUser`, `appleBulkWithoutUser`, `windowsAzureADJoin`, `windowsBulkUserless`, `windowsAutoEnrollment`, `windowsBulkAzureDomainJoin`, `windowsCoManagement`.</span></span>|
|<span data-ttu-id="53a69-213">lostModeState</span><span class="sxs-lookup"><span data-stu-id="53a69-213">lostModeState</span></span>|[<span data-ttu-id="53a69-214">lostModeState</span><span class="sxs-lookup"><span data-stu-id="53a69-214">lostModeState</span></span>](../resources/intune-devices-lostmodestate.md)|<span data-ttu-id="53a69-215">失われたモードが有効か無効かを示します。</span><span class="sxs-lookup"><span data-stu-id="53a69-215">Indicates if Lost mode is enabled or disabled.</span></span> <span data-ttu-id="53a69-216">可能な値は、`disabled`、`enabled` です。</span><span class="sxs-lookup"><span data-stu-id="53a69-216">Possible values are: `disabled`, `enabled`.</span></span>|
|<span data-ttu-id="53a69-217">activationLockBypassCode</span><span class="sxs-lookup"><span data-stu-id="53a69-217">activationLockBypassCode</span></span>|<span data-ttu-id="53a69-218">String</span><span class="sxs-lookup"><span data-stu-id="53a69-218">String</span></span>|<span data-ttu-id="53a69-219">デバイスのアクティベーション ロックをバイパスするためのコード。</span><span class="sxs-lookup"><span data-stu-id="53a69-219">Code that allows the Activation Lock on a device to be bypassed.</span></span>|
|<span data-ttu-id="53a69-220">emailAddress</span><span class="sxs-lookup"><span data-stu-id="53a69-220">emailAddress</span></span>|<span data-ttu-id="53a69-221">String</span><span class="sxs-lookup"><span data-stu-id="53a69-221">String</span></span>|<span data-ttu-id="53a69-222">デバイスに関連付けられているユーザーの電子メール</span><span class="sxs-lookup"><span data-stu-id="53a69-222">Email(s) for the user associated with the device</span></span>|
|<span data-ttu-id="53a69-223">azureActiveDirectoryDeviceId</span><span class="sxs-lookup"><span data-stu-id="53a69-223">azureActiveDirectoryDeviceId</span></span>|<span data-ttu-id="53a69-224">String</span><span class="sxs-lookup"><span data-stu-id="53a69-224">String</span></span>|<span data-ttu-id="53a69-225">Azure Active Directory デバイスの一意識別子。</span><span class="sxs-lookup"><span data-stu-id="53a69-225">The unique identifier for the Azure Active Directory device.</span></span> <span data-ttu-id="53a69-226">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="53a69-226">Read only.</span></span>|
|<span data-ttu-id="53a69-227">azureADDeviceId</span><span class="sxs-lookup"><span data-stu-id="53a69-227">azureADDeviceId</span></span>|<span data-ttu-id="53a69-228">String</span><span class="sxs-lookup"><span data-stu-id="53a69-228">String</span></span>|<span data-ttu-id="53a69-229">Azure Active Directory デバイスの一意識別子。</span><span class="sxs-lookup"><span data-stu-id="53a69-229">The unique identifier for the Azure Active Directory device.</span></span> <span data-ttu-id="53a69-230">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="53a69-230">Read only.</span></span>|
|<span data-ttu-id="53a69-231">deviceRegistrationState</span><span class="sxs-lookup"><span data-stu-id="53a69-231">deviceRegistrationState</span></span>|[<span data-ttu-id="53a69-232">deviceRegistrationState</span><span class="sxs-lookup"><span data-stu-id="53a69-232">deviceRegistrationState</span></span>](../resources/intune-devices-deviceregistrationstate.md)|<span data-ttu-id="53a69-233">デバイスの登録状態。</span><span class="sxs-lookup"><span data-stu-id="53a69-233">Device registration state.</span></span> <span data-ttu-id="53a69-234">可能な値は、`notRegistered`、`registered`、`revoked`、`keyConflict`、`approvalPending`、`certificateReset`、`notRegisteredPendingEnrollment`、`unknown` です。</span><span class="sxs-lookup"><span data-stu-id="53a69-234">Possible values are: `notRegistered`, `registered`, `revoked`, `keyConflict`, `approvalPending`, `certificateReset`, `notRegisteredPendingEnrollment`, `unknown`.</span></span>|
|<span data-ttu-id="53a69-235">deviceCategoryDisplayName</span><span class="sxs-lookup"><span data-stu-id="53a69-235">deviceCategoryDisplayName</span></span>|<span data-ttu-id="53a69-236">String</span><span class="sxs-lookup"><span data-stu-id="53a69-236">String</span></span>|<span data-ttu-id="53a69-237">デバイス カテゴリの表示名</span><span class="sxs-lookup"><span data-stu-id="53a69-237">Device category display name</span></span>|
|<span data-ttu-id="53a69-238">isSupervised</span><span class="sxs-lookup"><span data-stu-id="53a69-238">isSupervised</span></span>|<span data-ttu-id="53a69-239">Boolean</span><span class="sxs-lookup"><span data-stu-id="53a69-239">Boolean</span></span>|<span data-ttu-id="53a69-240">デバイスの管理状況</span><span class="sxs-lookup"><span data-stu-id="53a69-240">Device supervised status</span></span>|
|<span data-ttu-id="53a69-241">exchangeLastSuccessfulSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="53a69-241">exchangeLastSuccessfulSyncDateTime</span></span>|<span data-ttu-id="53a69-242">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="53a69-242">DateTimeOffset</span></span>|<span data-ttu-id="53a69-243">最後にデバイスが Exchange に接続した時刻。</span><span class="sxs-lookup"><span data-stu-id="53a69-243">Last time the device contacted Exchange.</span></span>|
|<span data-ttu-id="53a69-244">exchangeAccessState</span><span class="sxs-lookup"><span data-stu-id="53a69-244">exchangeAccessState</span></span>|[<span data-ttu-id="53a69-245">deviceManagementExchangeAccessState</span><span class="sxs-lookup"><span data-stu-id="53a69-245">deviceManagementExchangeAccessState</span></span>](../resources/intune-devices-devicemanagementexchangeaccessstate.md)|<span data-ttu-id="53a69-246">Exchange でのデバイスのアクセスの状態。</span><span class="sxs-lookup"><span data-stu-id="53a69-246">The Access State of the device in Exchange.</span></span> <span data-ttu-id="53a69-247">可能な値は、`none`、`unknown`、`allowed`、`blocked`、`quarantined` です。</span><span class="sxs-lookup"><span data-stu-id="53a69-247">Possible values are: `none`, `unknown`, `allowed`, `blocked`, `quarantined`.</span></span>|
|<span data-ttu-id="53a69-248">exchangeAccessStateReason</span><span class="sxs-lookup"><span data-stu-id="53a69-248">exchangeAccessStateReason</span></span>|[<span data-ttu-id="53a69-249">deviceManagementExchangeAccessStateReason</span><span class="sxs-lookup"><span data-stu-id="53a69-249">deviceManagementExchangeAccessStateReason</span></span>](../resources/intune-devices-devicemanagementexchangeaccessstatereason.md)|<span data-ttu-id="53a69-250">Exchange でのデバイスのアクセス状態の理由。
</span><span class="sxs-lookup"><span data-stu-id="53a69-250">The reason for the device's access state in Exchange.</span></span> <span data-ttu-id="53a69-251">可能な値は、`none`、`unknown`、`exchangeGlobalRule`、`exchangeIndividualRule`、`exchangeDeviceRule`、`exchangeUpgrade`、`exchangeMailboxPolicy`、`other`、`compliant`、`notCompliant`、`notEnrolled`、`unknownLocation`、`mfaRequired`、`azureADBlockDueToAccessPolicy`、`compromisedPassword`、`deviceNotKnownWithManagedApp` です。</span><span class="sxs-lookup"><span data-stu-id="53a69-251">Possible values are: `none`, `unknown`, `exchangeGlobalRule`, `exchangeIndividualRule`, `exchangeDeviceRule`, `exchangeUpgrade`, `exchangeMailboxPolicy`, `other`, `compliant`, `notCompliant`, `notEnrolled`, `unknownLocation`, `mfaRequired`, `azureADBlockDueToAccessPolicy`, `compromisedPassword`, `deviceNotKnownWithManagedApp`.</span></span>|
|<span data-ttu-id="53a69-252">remoteAssistanceSessionUrl</span><span class="sxs-lookup"><span data-stu-id="53a69-252">remoteAssistanceSessionUrl</span></span>|<span data-ttu-id="53a69-253">String</span><span class="sxs-lookup"><span data-stu-id="53a69-253">String</span></span>|<span data-ttu-id="53a69-254">デバイスとのリモート アシスタンス セッションを確立できるようにする URL。</span><span class="sxs-lookup"><span data-stu-id="53a69-254">Url that allows a Remote Assistance session to be established with the device.</span></span>|
|<span data-ttu-id="53a69-255">remoteAssistanceSessionErrorDetails</span><span class="sxs-lookup"><span data-stu-id="53a69-255">remoteAssistanceSessionErrorDetails</span></span>|<span data-ttu-id="53a69-256">String</span><span class="sxs-lookup"><span data-stu-id="53a69-256">String</span></span>|<span data-ttu-id="53a69-257">リモート アシスタンス セッション オブジェクトの作成時に問題を識別するエラー文字列。</span><span class="sxs-lookup"><span data-stu-id="53a69-257">An error string that identifies issues when creating Remote Assistance session objects.</span></span>|
|<span data-ttu-id="53a69-258">isEncrypted</span><span class="sxs-lookup"><span data-stu-id="53a69-258">isEncrypted</span></span>|<span data-ttu-id="53a69-259">Boolean</span><span class="sxs-lookup"><span data-stu-id="53a69-259">Boolean</span></span>|<span data-ttu-id="53a69-260">デバイスの暗号化の状態</span><span class="sxs-lookup"><span data-stu-id="53a69-260">Device encryption status</span></span>|
|<span data-ttu-id="53a69-261">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="53a69-261">userPrincipalName</span></span>|<span data-ttu-id="53a69-262">String</span><span class="sxs-lookup"><span data-stu-id="53a69-262">String</span></span>|<span data-ttu-id="53a69-263">デバイスのユーザー プリンシパル名。</span><span class="sxs-lookup"><span data-stu-id="53a69-263">Device user principal name</span></span>|
|<span data-ttu-id="53a69-264">model</span><span class="sxs-lookup"><span data-stu-id="53a69-264">model</span></span>|<span data-ttu-id="53a69-265">String</span><span class="sxs-lookup"><span data-stu-id="53a69-265">String</span></span>|<span data-ttu-id="53a69-266">デバイスのモデル</span><span class="sxs-lookup"><span data-stu-id="53a69-266">Model of the device</span></span>|
|<span data-ttu-id="53a69-267">manufacturer</span><span class="sxs-lookup"><span data-stu-id="53a69-267">manufacturer</span></span>|<span data-ttu-id="53a69-268">String</span><span class="sxs-lookup"><span data-stu-id="53a69-268">String</span></span>|<span data-ttu-id="53a69-269">デバイスのメーカー</span><span class="sxs-lookup"><span data-stu-id="53a69-269">Manufacturer of the device</span></span>|
|<span data-ttu-id="53a69-270">imei</span><span class="sxs-lookup"><span data-stu-id="53a69-270">imei</span></span>|<span data-ttu-id="53a69-271">String</span><span class="sxs-lookup"><span data-stu-id="53a69-271">String</span></span>|<span data-ttu-id="53a69-272">IMEI</span><span class="sxs-lookup"><span data-stu-id="53a69-272">IMEI</span></span>|
|<span data-ttu-id="53a69-273">complianceGracePeriodExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="53a69-273">complianceGracePeriodExpirationDateTime</span></span>|<span data-ttu-id="53a69-274">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="53a69-274">DateTimeOffset</span></span>|<span data-ttu-id="53a69-275">デバイス コンプライアンスの猶予期間が経過する DateTime</span><span class="sxs-lookup"><span data-stu-id="53a69-275">The DateTime when device compliance grace period expires</span></span>|
|<span data-ttu-id="53a69-276">serialNumber</span><span class="sxs-lookup"><span data-stu-id="53a69-276">serialNumber</span></span>|<span data-ttu-id="53a69-277">String</span><span class="sxs-lookup"><span data-stu-id="53a69-277">String</span></span>|<span data-ttu-id="53a69-278">シリアル番号</span><span class="sxs-lookup"><span data-stu-id="53a69-278">SerialNumber</span></span>|
|<span data-ttu-id="53a69-279">phoneNumber</span><span class="sxs-lookup"><span data-stu-id="53a69-279">phoneNumber</span></span>|<span data-ttu-id="53a69-280">String</span><span class="sxs-lookup"><span data-stu-id="53a69-280">String</span></span>|<span data-ttu-id="53a69-281">デバイスの電話番号</span><span class="sxs-lookup"><span data-stu-id="53a69-281">Phone number of the device</span></span>|
|<span data-ttu-id="53a69-282">androidSecurityPatchLevel</span><span class="sxs-lookup"><span data-stu-id="53a69-282">androidSecurityPatchLevel</span></span>|<span data-ttu-id="53a69-283">String</span><span class="sxs-lookup"><span data-stu-id="53a69-283">String</span></span>|<span data-ttu-id="53a69-284">Android セキュリティ パッチのレベル</span><span class="sxs-lookup"><span data-stu-id="53a69-284">Android security patch level</span></span>|
|<span data-ttu-id="53a69-285">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="53a69-285">userDisplayName</span></span>|<span data-ttu-id="53a69-286">String</span><span class="sxs-lookup"><span data-stu-id="53a69-286">String</span></span>|<span data-ttu-id="53a69-287">ユーザーの表示名</span><span class="sxs-lookup"><span data-stu-id="53a69-287">User display name</span></span>|
|<span data-ttu-id="53a69-288">configurationManagerClientEnabledFeatures</span><span class="sxs-lookup"><span data-stu-id="53a69-288">configurationManagerClientEnabledFeatures</span></span>|[<span data-ttu-id="53a69-289">configurationManagerClientEnabledFeatures</span><span class="sxs-lookup"><span data-stu-id="53a69-289">configurationManagerClientEnabledFeatures</span></span>](../resources/intune-devices-configurationmanagerclientenabledfeatures.md)|<span data-ttu-id="53a69-290">ConfigrMgr クライアント対応機能
</span><span class="sxs-lookup"><span data-stu-id="53a69-290">ConfigrMgr client enabled features</span></span>|
|<span data-ttu-id="53a69-291">wiFiMacAddress</span><span class="sxs-lookup"><span data-stu-id="53a69-291">wiFiMacAddress</span></span>|<span data-ttu-id="53a69-292">String</span><span class="sxs-lookup"><span data-stu-id="53a69-292">String</span></span>|<span data-ttu-id="53a69-293">Wi-Fi MAC</span><span class="sxs-lookup"><span data-stu-id="53a69-293">Wi-Fi MAC</span></span>|
|<span data-ttu-id="53a69-294">deviceHealthAttestationState</span><span class="sxs-lookup"><span data-stu-id="53a69-294">deviceHealthAttestationState</span></span>|[<span data-ttu-id="53a69-295">deviceHealthAttestationState</span><span class="sxs-lookup"><span data-stu-id="53a69-295">deviceHealthAttestationState</span></span>](../resources/intune-devices-devicehealthattestationstate.md)|<span data-ttu-id="53a69-296">デバイスの正常性構成証明の状態。</span><span class="sxs-lookup"><span data-stu-id="53a69-296">The device health attestation state.</span></span>|
|<span data-ttu-id="53a69-297">subscriberCarrier</span><span class="sxs-lookup"><span data-stu-id="53a69-297">subscriberCarrier</span></span>|<span data-ttu-id="53a69-298">String</span><span class="sxs-lookup"><span data-stu-id="53a69-298">String</span></span>|<span data-ttu-id="53a69-299">サブスクライバー通信事業者</span><span class="sxs-lookup"><span data-stu-id="53a69-299">Subscriber Carrier</span></span>|
|<span data-ttu-id="53a69-300">meid</span><span class="sxs-lookup"><span data-stu-id="53a69-300">meid</span></span>|<span data-ttu-id="53a69-301">String</span><span class="sxs-lookup"><span data-stu-id="53a69-301">String</span></span>|<span data-ttu-id="53a69-302">MEID</span><span class="sxs-lookup"><span data-stu-id="53a69-302">MEID</span></span>|
|<span data-ttu-id="53a69-303">totalStorageSpaceInBytes</span><span class="sxs-lookup"><span data-stu-id="53a69-303">totalStorageSpaceInBytes</span></span>|<span data-ttu-id="53a69-304">Int64</span><span class="sxs-lookup"><span data-stu-id="53a69-304">Int64</span></span>|<span data-ttu-id="53a69-305">記憶域の合計 (バイト)</span><span class="sxs-lookup"><span data-stu-id="53a69-305">Total Storage in Bytes</span></span>|
|<span data-ttu-id="53a69-306">freeStorageSpaceInBytes</span><span class="sxs-lookup"><span data-stu-id="53a69-306">freeStorageSpaceInBytes</span></span>|<span data-ttu-id="53a69-307">Int64</span><span class="sxs-lookup"><span data-stu-id="53a69-307">Int64</span></span>|<span data-ttu-id="53a69-308">空き記憶域 (バイト)</span><span class="sxs-lookup"><span data-stu-id="53a69-308">Free Storage in Bytes</span></span>|
|<span data-ttu-id="53a69-309">managedDeviceName</span><span class="sxs-lookup"><span data-stu-id="53a69-309">managedDeviceName</span></span>|<span data-ttu-id="53a69-310">String</span><span class="sxs-lookup"><span data-stu-id="53a69-310">String</span></span>|<span data-ttu-id="53a69-311">デバイスを識別する名前が自動的に生成されます。</span><span class="sxs-lookup"><span data-stu-id="53a69-311">Automatically generated name to identify a device.</span></span> <span data-ttu-id="53a69-312">ユーザー フレンドリ名に上書きできます。</span><span class="sxs-lookup"><span data-stu-id="53a69-312">Can be overwritten to a user friendly name.</span></span>|
|<span data-ttu-id="53a69-313">partnerReportedThreatState</span><span class="sxs-lookup"><span data-stu-id="53a69-313">partnerReportedThreatState</span></span>|[<span data-ttu-id="53a69-314">managedDevicePartnerReportedHealthState</span><span class="sxs-lookup"><span data-stu-id="53a69-314">managedDevicePartnerReportedHealthState</span></span>](../resources/intune-devices-manageddevicepartnerreportedhealthstate.md)|<span data-ttu-id="53a69-315">Mobile Threat Defense パートナーがアカウントおよびデバイスで使用されている場合の、デバイスの脅威の状態を示します。</span><span class="sxs-lookup"><span data-stu-id="53a69-315">Indicates the threat state of a device when a Mobile Threat Defense partner is in use by the account and device.</span></span> <span data-ttu-id="53a69-316">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="53a69-316">Read Only.</span></span> <span data-ttu-id="53a69-317">可能な値は、`unknown`、`activated`、`deactivated`、`secured`、`lowSeverity`、`mediumSeverity`、`highSeverity`、`unresponsive`、`compromised`、`misconfigured` です。</span><span class="sxs-lookup"><span data-stu-id="53a69-317">Possible values are: `unknown`, `activated`, `deactivated`, `secured`, `lowSeverity`, `mediumSeverity`, `highSeverity`, `unresponsive`, `compromised`, `misconfigured`.</span></span>|
|<span data-ttu-id="53a69-318">retireAfterDateTime</span><span class="sxs-lookup"><span data-stu-id="53a69-318">retireAfterDateTime</span></span>|<span data-ttu-id="53a69-319">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="53a69-319">DateTimeOffset</span></span>|<span data-ttu-id="53a69-320">スケジュールされたアクションのためにデバイスが自動廃棄されるまでの時間を示します。</span><span class="sxs-lookup"><span data-stu-id="53a69-320">Indicates the time after when a device will be auto retired because of scheduled action.</span></span>|
|<span data-ttu-id="53a69-321">usersLoggedOn</span><span class="sxs-lookup"><span data-stu-id="53a69-321">usersLoggedOn</span></span>|<span data-ttu-id="53a69-322">[loggedOnUser](../resources/intune-devices-loggedonuser.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="53a69-322">[loggedOnUser](../resources/intune-devices-loggedonuser.md) collection</span></span>|<span data-ttu-id="53a69-323">デバイスの最後にログオンしたユーザーを示します</span><span class="sxs-lookup"><span data-stu-id="53a69-323">Indicates the last logged on users of a device</span></span>|
|<span data-ttu-id="53a69-324">preferMdmOverGroupPolicyAppliedDateTime</span><span class="sxs-lookup"><span data-stu-id="53a69-324">preferMdmOverGroupPolicyAppliedDateTime</span></span>|<span data-ttu-id="53a69-325">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="53a69-325">DateTimeOffset</span></span>|<span data-ttu-id="53a69-326">PreferMdmOverGroupPolicy の設定が設定された DateTime を報告します。</span><span class="sxs-lookup"><span data-stu-id="53a69-326">Reports the DateTime the preferMdmOverGroupPolicy setting was set.</span></span>  <span data-ttu-id="53a69-327">設定すると、競合がある場合に Intune MDM 設定がグループポリシー設定を上書きします。</span><span class="sxs-lookup"><span data-stu-id="53a69-327">When set, the Intune MDM settings will override Group Policy settings if there is a conflict.</span></span> <span data-ttu-id="53a69-328">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="53a69-328">Read Only.</span></span>|
|<span data-ttu-id="53a69-329">autopilotEnrolled</span><span class="sxs-lookup"><span data-stu-id="53a69-329">autopilotEnrolled</span></span>|<span data-ttu-id="53a69-330">Boolean</span><span class="sxs-lookup"><span data-stu-id="53a69-330">Boolean</span></span>|<span data-ttu-id="53a69-331">管理対象デバイスが自動パイロットで登録されているかどうかを報告します。</span><span class="sxs-lookup"><span data-stu-id="53a69-331">Reports if the managed device is enrolled via auto-pilot.</span></span>|
|<span data-ttu-id="53a69-332">requireUserEnrollmentApproval</span><span class="sxs-lookup"><span data-stu-id="53a69-332">requireUserEnrollmentApproval</span></span>|<span data-ttu-id="53a69-333">Boolean</span><span class="sxs-lookup"><span data-stu-id="53a69-333">Boolean</span></span>|<span data-ttu-id="53a69-334">管理対象 iOS デバイスがユーザー承認登録であるかどうかを報告します。</span><span class="sxs-lookup"><span data-stu-id="53a69-334">Reports if the managed iOS device is user approval enrollment.</span></span>|
|<span data-ttu-id="53a69-335">managementCertificateExpirationDate</span><span class="sxs-lookup"><span data-stu-id="53a69-335">managementCertificateExpirationDate</span></span>|<span data-ttu-id="53a69-336">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="53a69-336">DateTimeOffset</span></span>|<span data-ttu-id="53a69-337">デバイス管理証明書の有効期限を報告する</span><span class="sxs-lookup"><span data-stu-id="53a69-337">Reports device management certificate expiration date</span></span>|
|<span data-ttu-id="53a69-338">iccid</span><span class="sxs-lookup"><span data-stu-id="53a69-338">iccid</span></span>|<span data-ttu-id="53a69-339">String</span><span class="sxs-lookup"><span data-stu-id="53a69-339">String</span></span>|<span data-ttu-id="53a69-340">Ic カード識別子。 SIM カードの一意の識別番号です。</span><span class="sxs-lookup"><span data-stu-id="53a69-340">Integrated Circuit Card Identifier, it is A SIM card's unique identification number.</span></span>|
|<span data-ttu-id="53a69-341">udid</span><span class="sxs-lookup"><span data-stu-id="53a69-341">udid</span></span>|<span data-ttu-id="53a69-342">String</span><span class="sxs-lookup"><span data-stu-id="53a69-342">String</span></span>|<span data-ttu-id="53a69-343">IOS および macOS デバイスの一意のデバイス識別子。</span><span class="sxs-lookup"><span data-stu-id="53a69-343">Unique Device Identifier for iOS and macOS devices.</span></span>|
|<span data-ttu-id="53a69-344">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="53a69-344">roleScopeTagIds</span></span>|<span data-ttu-id="53a69-345">文字列コレクション</span><span class="sxs-lookup"><span data-stu-id="53a69-345">String collection</span></span>|<span data-ttu-id="53a69-346">このデバイスインスタンスの範囲タグ Id のリスト。</span><span class="sxs-lookup"><span data-stu-id="53a69-346">List of Scope Tag IDs for this Device instance.</span></span>|
|<span data-ttu-id="53a69-347">windowsActiveMalwareCount 再計算</span><span class="sxs-lookup"><span data-stu-id="53a69-347">windowsActiveMalwareCount</span></span>|<span data-ttu-id="53a69-348">Int32</span><span class="sxs-lookup"><span data-stu-id="53a69-348">Int32</span></span>|<span data-ttu-id="53a69-349">この windows デバイスのアクティブなマルウェアの数</span><span class="sxs-lookup"><span data-stu-id="53a69-349">Count of active malware for this windows device</span></span>|
|<span data-ttu-id="53a69-350">windowsRemediatedMalwareCount</span><span class="sxs-lookup"><span data-stu-id="53a69-350">windowsRemediatedMalwareCount</span></span>|<span data-ttu-id="53a69-351">Int32</span><span class="sxs-lookup"><span data-stu-id="53a69-351">Int32</span></span>|<span data-ttu-id="53a69-352">この windows デバイスの修復済みマルウェアの数</span><span class="sxs-lookup"><span data-stu-id="53a69-352">Count of remediated malware for this windows device</span></span>|
|<span data-ttu-id="53a69-353">notes</span><span class="sxs-lookup"><span data-stu-id="53a69-353">notes</span></span>|<span data-ttu-id="53a69-354">String</span><span class="sxs-lookup"><span data-stu-id="53a69-354">String</span></span>|<span data-ttu-id="53a69-355">IT 管理者によって作成されたデバイスのメモ</span><span class="sxs-lookup"><span data-stu-id="53a69-355">Notes on the device created by IT Admin</span></span>|
|<span data-ttu-id="53a69-356">configurationManagerClientHealthState</span><span class="sxs-lookup"><span data-stu-id="53a69-356">configurationManagerClientHealthState</span></span>|[<span data-ttu-id="53a69-357">configurationManagerClientHealthState</span><span class="sxs-lookup"><span data-stu-id="53a69-357">configurationManagerClientHealthState</span></span>](../resources/intune-devices-configurationmanagerclienthealthstate.md)|<span data-ttu-id="53a69-358">構成マネージャークライアントの正常性状態。 MDM/ConfigMgr エージェントによって管理されるデバイスに対してのみ有効です。</span><span class="sxs-lookup"><span data-stu-id="53a69-358">Configuration manager client health state, valid only for devices managed by MDM/ConfigMgr Agent</span></span>|



## <a name="response"></a><span data-ttu-id="53a69-359">応答</span><span class="sxs-lookup"><span data-stu-id="53a69-359">Response</span></span>
<span data-ttu-id="53a69-360">成功した場合、このメソッドは `200 OK` 応答コードと、更新された [managedDevice](../resources/intune-devices-manageddevice.md) オブジェクトを応答本文で返します。</span><span class="sxs-lookup"><span data-stu-id="53a69-360">If successful, this method returns a `200 OK` response code and an updated [managedDevice](../resources/intune-devices-manageddevice.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="53a69-361">例</span><span class="sxs-lookup"><span data-stu-id="53a69-361">Example</span></span>

### <a name="request"></a><span data-ttu-id="53a69-362">要求</span><span class="sxs-lookup"><span data-stu-id="53a69-362">Request</span></span>
<span data-ttu-id="53a69-363">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="53a69-363">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="53a69-364">応答</span><span class="sxs-lookup"><span data-stu-id="53a69-364">Response</span></span>
<span data-ttu-id="53a69-p121">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="53a69-p121">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





