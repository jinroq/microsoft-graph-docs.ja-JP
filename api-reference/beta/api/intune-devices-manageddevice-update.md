---
title: >
  managedDevice の更新
description: managedDevice オブジェクトのプロパティを更新します。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 31c1b1a497dcd5cabf4b7b97b56811dbbedb2a5a
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27858612"
---
# <a name="update-manageddevice"></a><span data-ttu-id="a743d-103">managedDevice の更新
</span><span class="sxs-lookup"><span data-stu-id="a743d-103">Update managedDevice</span></span>

> <span data-ttu-id="a743d-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="a743d-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a743d-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a743d-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="a743d-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="a743d-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="a743d-107">[managedDevice](../resources/intune-devices-manageddevice.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="a743d-107">Update the properties of a [managedDevice](../resources/intune-devices-manageddevice.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="a743d-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="a743d-108">Prerequisites</span></span>
<span data-ttu-id="a743d-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="a743d-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a743d-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="a743d-111">Permission type</span></span>|<span data-ttu-id="a743d-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="a743d-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a743d-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="a743d-113">Delegated (work or school account)</span></span>|<span data-ttu-id="a743d-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a743d-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="a743d-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="a743d-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a743d-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a743d-116">Not supported.</span></span>|
|<span data-ttu-id="a743d-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="a743d-117">Application</span></span>|<span data-ttu-id="a743d-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a743d-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a743d-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="a743d-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /users/{usersId}/managedDevices/{managedDeviceId}
PATCH /deviceManagement/managedDevices/{managedDeviceId}
PATCH /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice
PATCH /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/detectedApps/{detectedAppId}/managedDevices/{managedDeviceId}
```

## <a name="request-headers"></a><span data-ttu-id="a743d-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="a743d-120">Request headers</span></span>
|<span data-ttu-id="a743d-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="a743d-121">Header</span></span>|<span data-ttu-id="a743d-122">値</span><span class="sxs-lookup"><span data-stu-id="a743d-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a743d-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="a743d-123">Authorization</span></span>|<span data-ttu-id="a743d-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="a743d-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a743d-125">Accept</span><span class="sxs-lookup"><span data-stu-id="a743d-125">Accept</span></span>|<span data-ttu-id="a743d-126">application/json</span><span class="sxs-lookup"><span data-stu-id="a743d-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a743d-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="a743d-127">Request body</span></span>
<span data-ttu-id="a743d-128">要求本文で、[managedDevice](../resources/intune-devices-manageddevice.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="a743d-128">In the request body, supply a JSON representation for the [managedDevice](../resources/intune-devices-manageddevice.md) object.</span></span>

<span data-ttu-id="a743d-129">次の表に、[managedDevice](../resources/intune-devices-manageddevice.md) の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="a743d-129">The following table shows the properties that are required when you create the [managedDevice](../resources/intune-devices-manageddevice.md).</span></span>

|<span data-ttu-id="a743d-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="a743d-130">Property</span></span>|<span data-ttu-id="a743d-131">種類</span><span class="sxs-lookup"><span data-stu-id="a743d-131">Type</span></span>|<span data-ttu-id="a743d-132">説明</span><span class="sxs-lookup"><span data-stu-id="a743d-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a743d-133">ID</span><span class="sxs-lookup"><span data-stu-id="a743d-133">id</span></span>|<span data-ttu-id="a743d-134">String</span><span class="sxs-lookup"><span data-stu-id="a743d-134">String</span></span>|<span data-ttu-id="a743d-135">デバイスの一意識別子</span><span class="sxs-lookup"><span data-stu-id="a743d-135">Unique Identifier for the device</span></span>|
|<span data-ttu-id="a743d-136">userId</span><span class="sxs-lookup"><span data-stu-id="a743d-136">userId</span></span>|<span data-ttu-id="a743d-137">String</span><span class="sxs-lookup"><span data-stu-id="a743d-137">String</span></span>|<span data-ttu-id="a743d-138">デバイスに関連付けられているユーザーの一意の識別子</span><span class="sxs-lookup"><span data-stu-id="a743d-138">Unique Identifier for the user associated with the device</span></span>|
|<span data-ttu-id="a743d-139">deviceName</span><span class="sxs-lookup"><span data-stu-id="a743d-139">deviceName</span></span>|<span data-ttu-id="a743d-140">String</span><span class="sxs-lookup"><span data-stu-id="a743d-140">String</span></span>|<span data-ttu-id="a743d-141">デバイスの名前</span><span class="sxs-lookup"><span data-stu-id="a743d-141">Name of the device</span></span>|
|<span data-ttu-id="a743d-142">hardwareInformation</span><span class="sxs-lookup"><span data-stu-id="a743d-142">hardwareInformation</span></span>|[<span data-ttu-id="a743d-143">hardwareInformation</span><span class="sxs-lookup"><span data-stu-id="a743d-143">hardwareInformation</span></span>](../resources/intune-devices-hardwareinformation.md)|<span data-ttu-id="a743d-144">デバイスのハードウェアの詳細。</span><span class="sxs-lookup"><span data-stu-id="a743d-144">The hardward details for the device.</span></span>  <span data-ttu-id="a743d-145">記憶域の製造元、シリアル番号などの情報が含まれています。</span><span class="sxs-lookup"><span data-stu-id="a743d-145">Includes information such as storage space, manufacturer, serial number, etc.</span></span>|
|<span data-ttu-id="a743d-146">ownerType</span><span class="sxs-lookup"><span data-stu-id="a743d-146">ownerType</span></span>|[<span data-ttu-id="a743d-147">ownerType</span><span class="sxs-lookup"><span data-stu-id="a743d-147">ownerType</span></span>](../resources/intune-devices-ownertype.md)|<span data-ttu-id="a743d-148">デバイスの所有権。</span><span class="sxs-lookup"><span data-stu-id="a743d-148">Ownership of the device.</span></span> <span data-ttu-id="a743d-149">'会社' または '個人' にすることができます。</span><span class="sxs-lookup"><span data-stu-id="a743d-149">Can be 'company' or 'personal'.</span></span> <span data-ttu-id="a743d-150">可能な値は、`unknown`、`company`、`personal` です。</span><span class="sxs-lookup"><span data-stu-id="a743d-150">Possible values are: `unknown`, `company`, `personal`.</span></span>|
|<span data-ttu-id="a743d-151">managedDeviceOwnerType</span><span class="sxs-lookup"><span data-stu-id="a743d-151">managedDeviceOwnerType</span></span>|[<span data-ttu-id="a743d-152">managedDeviceOwnerType</span><span class="sxs-lookup"><span data-stu-id="a743d-152">managedDeviceOwnerType</span></span>](../resources/intune-devices-manageddeviceownertype.md)|<span data-ttu-id="a743d-153">デバイスの所有権。</span><span class="sxs-lookup"><span data-stu-id="a743d-153">Ownership of the device.</span></span> <span data-ttu-id="a743d-154">'会社' または '個人' にすることができます。</span><span class="sxs-lookup"><span data-stu-id="a743d-154">Can be 'company' or 'personal'.</span></span> <span data-ttu-id="a743d-155">可能な値は、`unknown`、`company`、`personal` です。</span><span class="sxs-lookup"><span data-stu-id="a743d-155">Possible values are: `unknown`, `company`, `personal`.</span></span>|
|<span data-ttu-id="a743d-156">deviceActionResults</span><span class="sxs-lookup"><span data-stu-id="a743d-156">deviceActionResults</span></span>|<span data-ttu-id="a743d-157">[deviceActionResult](../resources/intune-devices-deviceactionresult.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="a743d-157">[deviceActionResult](../resources/intune-devices-deviceactionresult.md) collection</span></span>|<span data-ttu-id="a743d-158">ComplexType deviceActionResult オブジェクトのリスト。</span><span class="sxs-lookup"><span data-stu-id="a743d-158">List of ComplexType deviceActionResult objects.</span></span>|
|<span data-ttu-id="a743d-159">managementState</span><span class="sxs-lookup"><span data-stu-id="a743d-159">managementState</span></span>|[<span data-ttu-id="a743d-160">managementState</span><span class="sxs-lookup"><span data-stu-id="a743d-160">managementState</span></span>](../resources/intune-devices-managementstate.md)|<span data-ttu-id="a743d-161">デバイスの状態を管理します。</span><span class="sxs-lookup"><span data-stu-id="a743d-161">Management state of the device.</span></span> <span data-ttu-id="a743d-162">可能な値は、`managed`、`retirePending`、`retireFailed`、`wipePending`、`wipeFailed`、`unhealthy`、`deletePending`、`retireIssued`、`wipeIssued`、`wipeCanceled`、`retireCanceled`、`discovered` です。</span><span class="sxs-lookup"><span data-stu-id="a743d-162">Possible values are: `managed`, `retirePending`, `retireFailed`, `wipePending`, `wipeFailed`, `unhealthy`, `deletePending`, `retireIssued`, `wipeIssued`, `wipeCanceled`, `retireCanceled`, `discovered`.</span></span>|
|<span data-ttu-id="a743d-163">enrolledDateTime</span><span class="sxs-lookup"><span data-stu-id="a743d-163">enrolledDateTime</span></span>|<span data-ttu-id="a743d-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a743d-164">DateTimeOffset</span></span>|<span data-ttu-id="a743d-165">デバイスの登録時刻。</span><span class="sxs-lookup"><span data-stu-id="a743d-165">Enrollment time of the device.</span></span>|
|<span data-ttu-id="a743d-166">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="a743d-166">lastSyncDateTime</span></span>|<span data-ttu-id="a743d-167">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a743d-167">DateTimeOffset</span></span>|<span data-ttu-id="a743d-168">デバイスが Intune との正常な同期を最終的に完了した日時。</span><span class="sxs-lookup"><span data-stu-id="a743d-168">The date and time that the device last completed a successful sync with Intune.</span></span>|
|<span data-ttu-id="a743d-169">chassisType</span><span class="sxs-lookup"><span data-stu-id="a743d-169">chassisType</span></span>|[<span data-ttu-id="a743d-170">chassisType</span><span class="sxs-lookup"><span data-stu-id="a743d-170">chassisType</span></span>](../resources/intune-devices-chassistype.md)|<span data-ttu-id="a743d-171">デバイスのシャーシの種類です。</span><span class="sxs-lookup"><span data-stu-id="a743d-171">Chassis type of the device.</span></span> <span data-ttu-id="a743d-172">可能な値は、`unknown`、`desktop`、`laptop`、`worksWorkstation`、`enterpriseServer`、`phone`、`tablet`、`mobileOther`、`mobileUnknown` です。</span><span class="sxs-lookup"><span data-stu-id="a743d-172">Possible values are: `unknown`, `desktop`, `laptop`, `worksWorkstation`, `enterpriseServer`, `phone`, `tablet`, `mobileOther`, `mobileUnknown`.</span></span>|
|<span data-ttu-id="a743d-173">operatingSystem</span><span class="sxs-lookup"><span data-stu-id="a743d-173">operatingSystem</span></span>|<span data-ttu-id="a743d-174">String</span><span class="sxs-lookup"><span data-stu-id="a743d-174">String</span></span>|<span data-ttu-id="a743d-175">デバイスのオペレーティング システム。</span><span class="sxs-lookup"><span data-stu-id="a743d-175">Operating system of the device.</span></span> <span data-ttu-id="a743d-176">Windows、iOS など。</span><span class="sxs-lookup"><span data-stu-id="a743d-176">Windows, iOS, etc.</span></span>|
|<span data-ttu-id="a743d-177">deviceType</span><span class="sxs-lookup"><span data-stu-id="a743d-177">deviceType</span></span>|[<span data-ttu-id="a743d-178">deviceType</span><span class="sxs-lookup"><span data-stu-id="a743d-178">deviceType</span></span>](../resources/intune-shared-devicetype.md)|<span data-ttu-id="a743d-179">デバイスのプラットフォームです。</span><span class="sxs-lookup"><span data-stu-id="a743d-179">Platform of the device.</span></span> <span data-ttu-id="a743d-180">使用可能な値: `desktop`、 `windowsRT`、 `winMO6`、 `nokia`、 `windowsPhone`、 `mac`、 `winCE`、 `winEmbedded`、 `iPhone`、 `iPad`、 `iPod`、 `android`、 `iSocConsumer`、 `unix`、 `macMDM`、 `holoLens`、 `surfaceHub`、 `androidForWork`、 `androidEnterprise`, `blackberry`, `palm`, `unknown`.</span><span class="sxs-lookup"><span data-stu-id="a743d-180">Possible values are: `desktop`, `windowsRT`, `winMO6`, `nokia`, `windowsPhone`, `mac`, `winCE`, `winEmbedded`, `iPhone`, `iPad`, `iPod`, `android`, `iSocConsumer`, `unix`, `macMDM`, `holoLens`, `surfaceHub`, `androidForWork`, `androidEnterprise`, `blackberry`, `palm`, `unknown`.</span></span>|
|<span data-ttu-id="a743d-181">complianceState</span><span class="sxs-lookup"><span data-stu-id="a743d-181">complianceState</span></span>|[<span data-ttu-id="a743d-182">complianceState</span><span class="sxs-lookup"><span data-stu-id="a743d-182">complianceState</span></span>](../resources/intune-devices-compliancestate.md)|<span data-ttu-id="a743d-183">デバイスのコンプライアンス状態。</span><span class="sxs-lookup"><span data-stu-id="a743d-183">Compliance state of the device.</span></span> <span data-ttu-id="a743d-184">可能な値は、`unknown`、`compliant`、`noncompliant`、`conflict`、`error`、`inGracePeriod`、`configManager` です。</span><span class="sxs-lookup"><span data-stu-id="a743d-184">Possible values are: `unknown`, `compliant`, `noncompliant`, `conflict`, `error`, `inGracePeriod`, `configManager`.</span></span>|
|<span data-ttu-id="a743d-185">jailBroken</span><span class="sxs-lookup"><span data-stu-id="a743d-185">jailBroken</span></span>|<span data-ttu-id="a743d-186">String</span><span class="sxs-lookup"><span data-stu-id="a743d-186">String</span></span>|<span data-ttu-id="a743d-187">デバイスが脱獄またはルート化されているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="a743d-187">whether the device is jail broken or rooted.</span></span>|
|<span data-ttu-id="a743d-188">managementAgent</span><span class="sxs-lookup"><span data-stu-id="a743d-188">managementAgent</span></span>|[<span data-ttu-id="a743d-189">managementAgentType</span><span class="sxs-lookup"><span data-stu-id="a743d-189">managementAgentType</span></span>](../resources/intune-devices-managementagenttype.md)|<span data-ttu-id="a743d-190">デバイスの管理チャネル。</span><span class="sxs-lookup"><span data-stu-id="a743d-190">Management channel of the device.</span></span> <span data-ttu-id="a743d-191">Intune、EA などです。使用可能な値: `eas`、 `mdm`、 `easMdm`、 `intuneClient`、 `easIntuneClient`、 `configurationManagerClient`、 `configurationManagerClientMdm`、 `configurationManagerClientMdmEas`、 `unknown`、 `jamf`、 `googleCloudDevicePolicyController`、 `microsoft365ManagedMdm`。</span><span class="sxs-lookup"><span data-stu-id="a743d-191">Intune, EAS, etc. Possible values are: `eas`, `mdm`, `easMdm`, `intuneClient`, `easIntuneClient`, `configurationManagerClient`, `configurationManagerClientMdm`, `configurationManagerClientMdmEas`, `unknown`, `jamf`, `googleCloudDevicePolicyController`, `microsoft365ManagedMdm`.</span></span>|
|<span data-ttu-id="a743d-192">osVersion</span><span class="sxs-lookup"><span data-stu-id="a743d-192">osVersion</span></span>|<span data-ttu-id="a743d-193">String</span><span class="sxs-lookup"><span data-stu-id="a743d-193">String</span></span>|<span data-ttu-id="a743d-194">デバイスのオペレーティング システムのバージョン。</span><span class="sxs-lookup"><span data-stu-id="a743d-194">Operating system version of the device.</span></span>|
|<span data-ttu-id="a743d-195">easActivated</span><span class="sxs-lookup"><span data-stu-id="a743d-195">easActivated</span></span>|<span data-ttu-id="a743d-196">Boolean</span><span class="sxs-lookup"><span data-stu-id="a743d-196">Boolean</span></span>|<span data-ttu-id="a743d-197">Exchange ActiveSync がアクティブになっているデバイスかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="a743d-197">Whether the device is Exchange ActiveSync activated.</span></span>|
|<span data-ttu-id="a743d-198">easDeviceId</span><span class="sxs-lookup"><span data-stu-id="a743d-198">easDeviceId</span></span>|<span data-ttu-id="a743d-199">String</span><span class="sxs-lookup"><span data-stu-id="a743d-199">String</span></span>|<span data-ttu-id="a743d-200">デバイスの Exchange ActiveSync の ID。</span><span class="sxs-lookup"><span data-stu-id="a743d-200">Exchange ActiveSync Id of the device.</span></span>|
|<span data-ttu-id="a743d-201">easActivationDateTime</span><span class="sxs-lookup"><span data-stu-id="a743d-201">easActivationDateTime</span></span>|<span data-ttu-id="a743d-202">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a743d-202">DateTimeOffset</span></span>|<span data-ttu-id="a743d-203">デバイスの Exchange ActivationSync のアクティブ化の時刻。</span><span class="sxs-lookup"><span data-stu-id="a743d-203">Exchange ActivationSync activation time of the device.</span></span>|
|<span data-ttu-id="a743d-204">aadRegistered</span><span class="sxs-lookup"><span data-stu-id="a743d-204">aadRegistered</span></span>|<span data-ttu-id="a743d-205">Boolean</span><span class="sxs-lookup"><span data-stu-id="a743d-205">Boolean</span></span>|<span data-ttu-id="a743d-206">Azure Active Directory が登録されているデバイスかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="a743d-206">Whether the device is Azure Active Directory registered.</span></span>|
|<span data-ttu-id="a743d-207">azureADRegistered</span><span class="sxs-lookup"><span data-stu-id="a743d-207">azureADRegistered</span></span>|<span data-ttu-id="a743d-208">Boolean</span><span class="sxs-lookup"><span data-stu-id="a743d-208">Boolean</span></span>|<span data-ttu-id="a743d-209">Azure Active Directory が登録されているデバイスかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="a743d-209">Whether the device is Azure Active Directory registered.</span></span>|
|<span data-ttu-id="a743d-210">deviceEnrollmentType</span><span class="sxs-lookup"><span data-stu-id="a743d-210">deviceEnrollmentType</span></span>|[<span data-ttu-id="a743d-211">deviceEnrollmentType</span><span class="sxs-lookup"><span data-stu-id="a743d-211">deviceEnrollmentType</span></span>](../resources/intune-shared-deviceenrollmenttype.md)|<span data-ttu-id="a743d-212">デバイスの登録の種類。</span><span class="sxs-lookup"><span data-stu-id="a743d-212">Enrollment type of the device.</span></span> <span data-ttu-id="a743d-213">可能な値は、`unknown`、`userEnrollment`、`deviceEnrollmentManager`、`appleBulkWithUser`、`appleBulkWithoutUser`、`windowsAzureADJoin`、`windowsBulkUserless`、`windowsAutoEnrollment`、`windowsBulkAzureDomainJoin`、`windowsCoManagement` です。</span><span class="sxs-lookup"><span data-stu-id="a743d-213">Possible values are: `unknown`, `userEnrollment`, `deviceEnrollmentManager`, `appleBulkWithUser`, `appleBulkWithoutUser`, `windowsAzureADJoin`, `windowsBulkUserless`, `windowsAutoEnrollment`, `windowsBulkAzureDomainJoin`, `windowsCoManagement`.</span></span>|
|<span data-ttu-id="a743d-214">lostModeState</span><span class="sxs-lookup"><span data-stu-id="a743d-214">lostModeState</span></span>|[<span data-ttu-id="a743d-215">lostModeState</span><span class="sxs-lookup"><span data-stu-id="a743d-215">lostModeState</span></span>](../resources/intune-devices-lostmodestate.md)|<span data-ttu-id="a743d-216">失われたモードが有効か無効を示します。</span><span class="sxs-lookup"><span data-stu-id="a743d-216">Indicates if Lost mode is enabled or disabled.</span></span> <span data-ttu-id="a743d-217">使用可能な値は、`disabled`、`enabled` です。</span><span class="sxs-lookup"><span data-stu-id="a743d-217">Possible values are: `disabled`, `enabled`.</span></span>|
|<span data-ttu-id="a743d-218">activationLockBypassCode</span><span class="sxs-lookup"><span data-stu-id="a743d-218">activationLockBypassCode</span></span>|<span data-ttu-id="a743d-219">String</span><span class="sxs-lookup"><span data-stu-id="a743d-219">String</span></span>|<span data-ttu-id="a743d-220">デバイスのアクティベーション ロックをバイパスするためのコード。</span><span class="sxs-lookup"><span data-stu-id="a743d-220">Code that allows the Activation Lock on a device to be bypassed.</span></span>|
|<span data-ttu-id="a743d-221">emailAddress</span><span class="sxs-lookup"><span data-stu-id="a743d-221">emailAddress</span></span>|<span data-ttu-id="a743d-222">String</span><span class="sxs-lookup"><span data-stu-id="a743d-222">String</span></span>|<span data-ttu-id="a743d-223">デバイスに関連付けられているユーザーの電子メール</span><span class="sxs-lookup"><span data-stu-id="a743d-223">Email(s) for the user associated with the device</span></span>|
|<span data-ttu-id="a743d-224">azureActiveDirectoryDeviceId</span><span class="sxs-lookup"><span data-stu-id="a743d-224">azureActiveDirectoryDeviceId</span></span>|<span data-ttu-id="a743d-225">String</span><span class="sxs-lookup"><span data-stu-id="a743d-225">String</span></span>|<span data-ttu-id="a743d-226">Azure Active Directory デバイスの一意識別子。</span><span class="sxs-lookup"><span data-stu-id="a743d-226">The unique identifier for the Azure Active Directory device.</span></span> <span data-ttu-id="a743d-227">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="a743d-227">Read only.</span></span>|
|<span data-ttu-id="a743d-228">azureADDeviceId</span><span class="sxs-lookup"><span data-stu-id="a743d-228">azureADDeviceId</span></span>|<span data-ttu-id="a743d-229">String</span><span class="sxs-lookup"><span data-stu-id="a743d-229">String</span></span>|<span data-ttu-id="a743d-230">Azure Active Directory デバイスの一意識別子。</span><span class="sxs-lookup"><span data-stu-id="a743d-230">The unique identifier for the Azure Active Directory device.</span></span> <span data-ttu-id="a743d-231">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="a743d-231">Read only.</span></span>|
|<span data-ttu-id="a743d-232">deviceRegistrationState</span><span class="sxs-lookup"><span data-stu-id="a743d-232">deviceRegistrationState</span></span>|[<span data-ttu-id="a743d-233">deviceRegistrationState</span><span class="sxs-lookup"><span data-stu-id="a743d-233">deviceRegistrationState</span></span>](../resources/intune-devices-deviceregistrationstate.md)|<span data-ttu-id="a743d-234">デバイスの登録状態。</span><span class="sxs-lookup"><span data-stu-id="a743d-234">Device registration state.</span></span> <span data-ttu-id="a743d-235">可能な値は、`notRegistered`、`registered`、`revoked`、`keyConflict`、`approvalPending`、`certificateReset`、`notRegisteredPendingEnrollment`、`unknown` です。</span><span class="sxs-lookup"><span data-stu-id="a743d-235">Possible values are: `notRegistered`, `registered`, `revoked`, `keyConflict`, `approvalPending`, `certificateReset`, `notRegisteredPendingEnrollment`, `unknown`.</span></span>|
|<span data-ttu-id="a743d-236">deviceCategoryDisplayName</span><span class="sxs-lookup"><span data-stu-id="a743d-236">deviceCategoryDisplayName</span></span>|<span data-ttu-id="a743d-237">String</span><span class="sxs-lookup"><span data-stu-id="a743d-237">String</span></span>|<span data-ttu-id="a743d-238">デバイス カテゴリの表示名</span><span class="sxs-lookup"><span data-stu-id="a743d-238">Device category display name</span></span>|
|<span data-ttu-id="a743d-239">isSupervised</span><span class="sxs-lookup"><span data-stu-id="a743d-239">isSupervised</span></span>|<span data-ttu-id="a743d-240">Boolean</span><span class="sxs-lookup"><span data-stu-id="a743d-240">Boolean</span></span>|<span data-ttu-id="a743d-241">デバイスの管理状況</span><span class="sxs-lookup"><span data-stu-id="a743d-241">Device supervised status</span></span>|
|<span data-ttu-id="a743d-242">exchangeLastSuccessfulSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="a743d-242">exchangeLastSuccessfulSyncDateTime</span></span>|<span data-ttu-id="a743d-243">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a743d-243">DateTimeOffset</span></span>|<span data-ttu-id="a743d-244">最後にデバイスが Exchange に接続した時刻。</span><span class="sxs-lookup"><span data-stu-id="a743d-244">Last time the device contacted Exchange.</span></span>|
|<span data-ttu-id="a743d-245">exchangeAccessState</span><span class="sxs-lookup"><span data-stu-id="a743d-245">exchangeAccessState</span></span>|[<span data-ttu-id="a743d-246">deviceManagementExchangeAccessState</span><span class="sxs-lookup"><span data-stu-id="a743d-246">deviceManagementExchangeAccessState</span></span>](../resources/intune-devices-devicemanagementexchangeaccessstate.md)|<span data-ttu-id="a743d-247">Exchange でのデバイスのアクセスの状態。</span><span class="sxs-lookup"><span data-stu-id="a743d-247">The Access State of the device in Exchange.</span></span> <span data-ttu-id="a743d-248">可能な値は、`none`、`unknown`、`allowed`、`blocked`、`quarantined` です。</span><span class="sxs-lookup"><span data-stu-id="a743d-248">Possible values are: `none`, `unknown`, `allowed`, `blocked`, `quarantined`.</span></span>|
|<span data-ttu-id="a743d-249">exchangeAccessStateReason</span><span class="sxs-lookup"><span data-stu-id="a743d-249">exchangeAccessStateReason</span></span>|[<span data-ttu-id="a743d-250">deviceManagementExchangeAccessStateReason</span><span class="sxs-lookup"><span data-stu-id="a743d-250">deviceManagementExchangeAccessStateReason</span></span>](../resources/intune-devices-devicemanagementexchangeaccessstatereason.md)|<span data-ttu-id="a743d-251">Exchange でのデバイスのアクセス状態の理由。
</span><span class="sxs-lookup"><span data-stu-id="a743d-251">The reason for the device's access state in Exchange.</span></span> <span data-ttu-id="a743d-252">可能な値は、`none`、`unknown`、`exchangeGlobalRule`、`exchangeIndividualRule`、`exchangeDeviceRule`、`exchangeUpgrade`、`exchangeMailboxPolicy`、`other`、`compliant`、`notCompliant`、`notEnrolled`、`unknownLocation`、`mfaRequired`、`azureADBlockDueToAccessPolicy`、`compromisedPassword`、`deviceNotKnownWithManagedApp` です。</span><span class="sxs-lookup"><span data-stu-id="a743d-252">Possible values are: `none`, `unknown`, `exchangeGlobalRule`, `exchangeIndividualRule`, `exchangeDeviceRule`, `exchangeUpgrade`, `exchangeMailboxPolicy`, `other`, `compliant`, `notCompliant`, `notEnrolled`, `unknownLocation`, `mfaRequired`, `azureADBlockDueToAccessPolicy`, `compromisedPassword`, `deviceNotKnownWithManagedApp`.</span></span>|
|<span data-ttu-id="a743d-253">remoteAssistanceSessionUrl</span><span class="sxs-lookup"><span data-stu-id="a743d-253">remoteAssistanceSessionUrl</span></span>|<span data-ttu-id="a743d-254">String</span><span class="sxs-lookup"><span data-stu-id="a743d-254">String</span></span>|<span data-ttu-id="a743d-255">デバイスとのリモート アシスタンス セッションを確立できるようにする URL。</span><span class="sxs-lookup"><span data-stu-id="a743d-255">Url that allows a Remote Assistance session to be established with the device.</span></span>|
|<span data-ttu-id="a743d-256">remoteAssistanceSessionErrorDetails</span><span class="sxs-lookup"><span data-stu-id="a743d-256">remoteAssistanceSessionErrorDetails</span></span>|<span data-ttu-id="a743d-257">String</span><span class="sxs-lookup"><span data-stu-id="a743d-257">String</span></span>|<span data-ttu-id="a743d-258">リモート アシスタンス セッション オブジェクトの作成時に問題を識別するエラー文字列。</span><span class="sxs-lookup"><span data-stu-id="a743d-258">An error string that identifies issues when creating Remote Assistance session objects.</span></span>|
|<span data-ttu-id="a743d-259">isEncrypted</span><span class="sxs-lookup"><span data-stu-id="a743d-259">isEncrypted</span></span>|<span data-ttu-id="a743d-260">Boolean</span><span class="sxs-lookup"><span data-stu-id="a743d-260">Boolean</span></span>|<span data-ttu-id="a743d-261">デバイスの暗号化の状態</span><span class="sxs-lookup"><span data-stu-id="a743d-261">Device encryption status</span></span>|
|<span data-ttu-id="a743d-262">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="a743d-262">userPrincipalName</span></span>|<span data-ttu-id="a743d-263">String</span><span class="sxs-lookup"><span data-stu-id="a743d-263">String</span></span>|<span data-ttu-id="a743d-264">デバイスのユーザー プリンシパル名。</span><span class="sxs-lookup"><span data-stu-id="a743d-264">Device user principal name</span></span>|
|<span data-ttu-id="a743d-265">model</span><span class="sxs-lookup"><span data-stu-id="a743d-265">model</span></span>|<span data-ttu-id="a743d-266">String</span><span class="sxs-lookup"><span data-stu-id="a743d-266">String</span></span>|<span data-ttu-id="a743d-267">デバイスのモデル</span><span class="sxs-lookup"><span data-stu-id="a743d-267">Model of the device</span></span>|
|<span data-ttu-id="a743d-268">manufacturer</span><span class="sxs-lookup"><span data-stu-id="a743d-268">manufacturer</span></span>|<span data-ttu-id="a743d-269">String</span><span class="sxs-lookup"><span data-stu-id="a743d-269">String</span></span>|<span data-ttu-id="a743d-270">デバイスのメーカー</span><span class="sxs-lookup"><span data-stu-id="a743d-270">Manufacturer of the device</span></span>|
|<span data-ttu-id="a743d-271">imei</span><span class="sxs-lookup"><span data-stu-id="a743d-271">imei</span></span>|<span data-ttu-id="a743d-272">String</span><span class="sxs-lookup"><span data-stu-id="a743d-272">String</span></span>|<span data-ttu-id="a743d-273">IMEI</span><span class="sxs-lookup"><span data-stu-id="a743d-273">IMEI</span></span>|
|<span data-ttu-id="a743d-274">complianceGracePeriodExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="a743d-274">complianceGracePeriodExpirationDateTime</span></span>|<span data-ttu-id="a743d-275">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a743d-275">DateTimeOffset</span></span>|<span data-ttu-id="a743d-276">デバイス コンプライアンスの猶予期間が経過する DateTime</span><span class="sxs-lookup"><span data-stu-id="a743d-276">The DateTime when device compliance grace period expires</span></span>|
|<span data-ttu-id="a743d-277">serialNumber</span><span class="sxs-lookup"><span data-stu-id="a743d-277">serialNumber</span></span>|<span data-ttu-id="a743d-278">String</span><span class="sxs-lookup"><span data-stu-id="a743d-278">String</span></span>|<span data-ttu-id="a743d-279">シリアル番号</span><span class="sxs-lookup"><span data-stu-id="a743d-279">SerialNumber</span></span>|
|<span data-ttu-id="a743d-280">phoneNumber</span><span class="sxs-lookup"><span data-stu-id="a743d-280">phoneNumber</span></span>|<span data-ttu-id="a743d-281">String</span><span class="sxs-lookup"><span data-stu-id="a743d-281">String</span></span>|<span data-ttu-id="a743d-282">デバイスの電話番号</span><span class="sxs-lookup"><span data-stu-id="a743d-282">Phone number of the device</span></span>|
|<span data-ttu-id="a743d-283">androidSecurityPatchLevel</span><span class="sxs-lookup"><span data-stu-id="a743d-283">androidSecurityPatchLevel</span></span>|<span data-ttu-id="a743d-284">String</span><span class="sxs-lookup"><span data-stu-id="a743d-284">String</span></span>|<span data-ttu-id="a743d-285">Android セキュリティ パッチのレベル</span><span class="sxs-lookup"><span data-stu-id="a743d-285">Android security patch level</span></span>|
|<span data-ttu-id="a743d-286">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="a743d-286">userDisplayName</span></span>|<span data-ttu-id="a743d-287">String</span><span class="sxs-lookup"><span data-stu-id="a743d-287">String</span></span>|<span data-ttu-id="a743d-288">ユーザーの表示名</span><span class="sxs-lookup"><span data-stu-id="a743d-288">User display name</span></span>|
|<span data-ttu-id="a743d-289">configurationManagerClientEnabledFeatures</span><span class="sxs-lookup"><span data-stu-id="a743d-289">configurationManagerClientEnabledFeatures</span></span>|[<span data-ttu-id="a743d-290">configurationManagerClientEnabledFeatures</span><span class="sxs-lookup"><span data-stu-id="a743d-290">configurationManagerClientEnabledFeatures</span></span>](../resources/intune-devices-configurationmanagerclientenabledfeatures.md)|<span data-ttu-id="a743d-291">ConfigrMgr クライアント対応機能
</span><span class="sxs-lookup"><span data-stu-id="a743d-291">ConfigrMgr client enabled features</span></span>|
|<span data-ttu-id="a743d-292">wiFiMacAddress</span><span class="sxs-lookup"><span data-stu-id="a743d-292">wiFiMacAddress</span></span>|<span data-ttu-id="a743d-293">String</span><span class="sxs-lookup"><span data-stu-id="a743d-293">String</span></span>|<span data-ttu-id="a743d-294">Wi-Fi MAC</span><span class="sxs-lookup"><span data-stu-id="a743d-294">Wi-Fi MAC</span></span>|
|<span data-ttu-id="a743d-295">deviceHealthAttestationState</span><span class="sxs-lookup"><span data-stu-id="a743d-295">deviceHealthAttestationState</span></span>|[<span data-ttu-id="a743d-296">deviceHealthAttestationState</span><span class="sxs-lookup"><span data-stu-id="a743d-296">deviceHealthAttestationState</span></span>](../resources/intune-devices-devicehealthattestationstate.md)|<span data-ttu-id="a743d-297">デバイスの正常性構成証明の状態。</span><span class="sxs-lookup"><span data-stu-id="a743d-297">The device health attestation state.</span></span>|
|<span data-ttu-id="a743d-298">subscriberCarrier</span><span class="sxs-lookup"><span data-stu-id="a743d-298">subscriberCarrier</span></span>|<span data-ttu-id="a743d-299">String</span><span class="sxs-lookup"><span data-stu-id="a743d-299">String</span></span>|<span data-ttu-id="a743d-300">サブスクライバー通信事業者</span><span class="sxs-lookup"><span data-stu-id="a743d-300">Subscriber Carrier</span></span>|
|<span data-ttu-id="a743d-301">meid</span><span class="sxs-lookup"><span data-stu-id="a743d-301">meid</span></span>|<span data-ttu-id="a743d-302">String</span><span class="sxs-lookup"><span data-stu-id="a743d-302">String</span></span>|<span data-ttu-id="a743d-303">MEID</span><span class="sxs-lookup"><span data-stu-id="a743d-303">MEID</span></span>|
|<span data-ttu-id="a743d-304">totalStorageSpaceInBytes</span><span class="sxs-lookup"><span data-stu-id="a743d-304">totalStorageSpaceInBytes</span></span>|<span data-ttu-id="a743d-305">Int64</span><span class="sxs-lookup"><span data-stu-id="a743d-305">Int64</span></span>|<span data-ttu-id="a743d-306">記憶域の合計 (バイト)</span><span class="sxs-lookup"><span data-stu-id="a743d-306">Total Storage in Bytes</span></span>|
|<span data-ttu-id="a743d-307">freeStorageSpaceInBytes</span><span class="sxs-lookup"><span data-stu-id="a743d-307">freeStorageSpaceInBytes</span></span>|<span data-ttu-id="a743d-308">Int64</span><span class="sxs-lookup"><span data-stu-id="a743d-308">Int64</span></span>|<span data-ttu-id="a743d-309">空き記憶域 (バイト)</span><span class="sxs-lookup"><span data-stu-id="a743d-309">Free Storage in Bytes</span></span>|
|<span data-ttu-id="a743d-310">managedDeviceName</span><span class="sxs-lookup"><span data-stu-id="a743d-310">managedDeviceName</span></span>|<span data-ttu-id="a743d-311">String</span><span class="sxs-lookup"><span data-stu-id="a743d-311">String</span></span>|<span data-ttu-id="a743d-312">デバイスを識別する名前が自動的に生成されます。</span><span class="sxs-lookup"><span data-stu-id="a743d-312">Automatically generated name to identify a device.</span></span> <span data-ttu-id="a743d-313">ユーザー フレンドリ名に上書きできます。</span><span class="sxs-lookup"><span data-stu-id="a743d-313">Can be overwritten to a user friendly name.</span></span>|
|<span data-ttu-id="a743d-314">partnerReportedThreatState</span><span class="sxs-lookup"><span data-stu-id="a743d-314">partnerReportedThreatState</span></span>|[<span data-ttu-id="a743d-315">managedDevicePartnerReportedHealthState</span><span class="sxs-lookup"><span data-stu-id="a743d-315">managedDevicePartnerReportedHealthState</span></span>](../resources/intune-devices-manageddevicepartnerreportedhealthstate.md)|<span data-ttu-id="a743d-316">Mobile Threat Defense パートナーがアカウントおよびデバイスで使用されている場合の、デバイスの脅威の状態を示します。</span><span class="sxs-lookup"><span data-stu-id="a743d-316">Indicates the threat state of a device when a Mobile Threat Defense partner is in use by the account and device.</span></span> <span data-ttu-id="a743d-317">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="a743d-317">Read Only.</span></span> <span data-ttu-id="a743d-318">可能な値は、`unknown`、`activated`、`deactivated`、`secured`、`lowSeverity`、`mediumSeverity`、`highSeverity`、`unresponsive`、`compromised`、`misconfigured` です。</span><span class="sxs-lookup"><span data-stu-id="a743d-318">Possible values are: `unknown`, `activated`, `deactivated`, `secured`, `lowSeverity`, `mediumSeverity`, `highSeverity`, `unresponsive`, `compromised`, `misconfigured`.</span></span>|
|<span data-ttu-id="a743d-319">usersLoggedOn</span><span class="sxs-lookup"><span data-stu-id="a743d-319">usersLoggedOn</span></span>|<span data-ttu-id="a743d-320">[loggedOnUser](../resources/intune-devices-loggedonuser.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="a743d-320">[loggedOnUser](../resources/intune-devices-loggedonuser.md) collection</span></span>|<span data-ttu-id="a743d-321">最後のデバイスのユーザーにログオンしていることを示します</span><span class="sxs-lookup"><span data-stu-id="a743d-321">Indicates the last logged on users of a device</span></span>|
|<span data-ttu-id="a743d-322">preferMdmOverGroupPolicyAppliedDateTime</span><span class="sxs-lookup"><span data-stu-id="a743d-322">preferMdmOverGroupPolicyAppliedDateTime</span></span>|<span data-ttu-id="a743d-323">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a743d-323">DateTimeOffset</span></span>|<span data-ttu-id="a743d-324">レポート preferMdmOverGroupPolicy 設定日付と時刻が設定されています。</span><span class="sxs-lookup"><span data-stu-id="a743d-324">Reports the DateTime the preferMdmOverGroupPolicy setting was set.</span></span>  <span data-ttu-id="a743d-325">設定すると、Intune MDM 設定が優先されますグループ ポリシー設定の競合がある場合。</span><span class="sxs-lookup"><span data-stu-id="a743d-325">When set, the Intune MDM settings will override Group Policy settings if there is a conflict.</span></span> <span data-ttu-id="a743d-326">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="a743d-326">Read Only.</span></span>|
|<span data-ttu-id="a743d-327">autopilotEnrolled</span><span class="sxs-lookup"><span data-stu-id="a743d-327">autopilotEnrolled</span></span>|<span data-ttu-id="a743d-328">ブール型</span><span class="sxs-lookup"><span data-stu-id="a743d-328">Boolean</span></span>|<span data-ttu-id="a743d-329">自動操縦を使用して管理対象のデバイスが登録されている場合にレポートします。</span><span class="sxs-lookup"><span data-stu-id="a743d-329">Reports if the managed device is enrolled via auto-pilot.</span></span>|
|<span data-ttu-id="a743d-330">requireUserEnrollmentApproval</span><span class="sxs-lookup"><span data-stu-id="a743d-330">requireUserEnrollmentApproval</span></span>|<span data-ttu-id="a743d-331">ブール型</span><span class="sxs-lookup"><span data-stu-id="a743d-331">Boolean</span></span>|<span data-ttu-id="a743d-332">マネージ iOS デバイスがユーザーの承認登録の場合にレポートします。</span><span class="sxs-lookup"><span data-stu-id="a743d-332">Reports if the managed iOS device is user approval enrollment.</span></span>|
|<span data-ttu-id="a743d-333">managementCertificateExpirationDate</span><span class="sxs-lookup"><span data-stu-id="a743d-333">managementCertificateExpirationDate</span></span>|<span data-ttu-id="a743d-334">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a743d-334">DateTimeOffset</span></span>|<span data-ttu-id="a743d-335">デバイスの管理の証明書の有効期限の日付をレポート</span><span class="sxs-lookup"><span data-stu-id="a743d-335">Reports device management certificate expiration date</span></span>|
|<span data-ttu-id="a743d-336">iccid</span><span class="sxs-lookup"><span data-stu-id="a743d-336">iccid</span></span>|<span data-ttu-id="a743d-337">String</span><span class="sxs-lookup"><span data-stu-id="a743d-337">String</span></span>|<span data-ttu-id="a743d-338">A SIM カードの一意の識別番号は集積回路カードの識別子です。</span><span class="sxs-lookup"><span data-stu-id="a743d-338">Integrated Circuit Card Identifier, it is A SIM card's unique identification number.</span></span>|
|<span data-ttu-id="a743d-339">udid</span><span class="sxs-lookup"><span data-stu-id="a743d-339">udid</span></span>|<span data-ttu-id="a743d-340">String</span><span class="sxs-lookup"><span data-stu-id="a743d-340">String</span></span>|<span data-ttu-id="a743d-341">IOS と macOS デバイスに一意のデバイス識別子です。</span><span class="sxs-lookup"><span data-stu-id="a743d-341">Unique Device Identifier for iOS and macOS devices.</span></span>|
|<span data-ttu-id="a743d-342">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="a743d-342">roleScopeTagIds</span></span>|<span data-ttu-id="a743d-343">String コレクション</span><span class="sxs-lookup"><span data-stu-id="a743d-343">String collection</span></span>|<span data-ttu-id="a743d-344">このデバイス インスタンスのスコープのタグ Id のリストです。</span><span class="sxs-lookup"><span data-stu-id="a743d-344">List of Scope Tag IDs for this Device instance.</span></span>|
|<span data-ttu-id="a743d-345">windowsActiveMalwareCount</span><span class="sxs-lookup"><span data-stu-id="a743d-345">windowsActiveMalwareCount</span></span>|<span data-ttu-id="a743d-346">Int32</span><span class="sxs-lookup"><span data-stu-id="a743d-346">Int32</span></span>|<span data-ttu-id="a743d-347">この windows デバイスのアクティブなマルウェアの数</span><span class="sxs-lookup"><span data-stu-id="a743d-347">Count of active malware for this windows device</span></span>|
|<span data-ttu-id="a743d-348">windowsRemediatedMalwareCount</span><span class="sxs-lookup"><span data-stu-id="a743d-348">windowsRemediatedMalwareCount</span></span>|<span data-ttu-id="a743d-349">Int32</span><span class="sxs-lookup"><span data-stu-id="a743d-349">Int32</span></span>|<span data-ttu-id="a743d-350">この windows デバイス用の修正されたマルウェアの数</span><span class="sxs-lookup"><span data-stu-id="a743d-350">Count of remediated malware for this windows device</span></span>|
|<span data-ttu-id="a743d-351">notes</span><span class="sxs-lookup"><span data-stu-id="a743d-351">notes</span></span>|<span data-ttu-id="a743d-352">String</span><span class="sxs-lookup"><span data-stu-id="a743d-352">String</span></span>|<span data-ttu-id="a743d-353">IT 管理者によって作成されたデバイスに関する注意事項</span><span class="sxs-lookup"><span data-stu-id="a743d-353">Notes on the device created by IT Admin</span></span>|
|<span data-ttu-id="a743d-354">configurationManagerClientHealthState</span><span class="sxs-lookup"><span data-stu-id="a743d-354">configurationManagerClientHealthState</span></span>|[<span data-ttu-id="a743d-355">configurationManagerClientHealthState</span><span class="sxs-lookup"><span data-stu-id="a743d-355">configurationManagerClientHealthState</span></span>](../resources/intune-devices-configurationmanagerclienthealthstate.md)|<span data-ttu-id="a743d-356">構成マネージャー クライアント正常性の状態、または構成マネージャーの MDM エージェントによって管理されるデバイスに対してのみ有効です。</span><span class="sxs-lookup"><span data-stu-id="a743d-356">Configuration manager client health state, valid only for devices managed by MDM/ConfigMgr Agent</span></span>|



## <a name="response"></a><span data-ttu-id="a743d-357">応答</span><span class="sxs-lookup"><span data-stu-id="a743d-357">Response</span></span>
<span data-ttu-id="a743d-358">成功した場合、このメソッドは `200 OK` 応答コードと、更新された [managedDevice](../resources/intune-devices-manageddevice.md) オブジェクトを応答本文で返します。</span><span class="sxs-lookup"><span data-stu-id="a743d-358">If successful, this method returns a `200 OK` response code and an updated [managedDevice](../resources/intune-devices-manageddevice.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a743d-359">例</span><span class="sxs-lookup"><span data-stu-id="a743d-359">Example</span></span>
### <a name="request"></a><span data-ttu-id="a743d-360">要求</span><span class="sxs-lookup"><span data-stu-id="a743d-360">Request</span></span>
<span data-ttu-id="a743d-361">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="a743d-361">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/users/{usersId}/managedDevices/{managedDeviceId}
Content-type: application/json
Content-length: 7114

{
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
  "partnerReportedThreatState": "activated",
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

### <a name="response"></a><span data-ttu-id="a743d-362">応答</span><span class="sxs-lookup"><span data-stu-id="a743d-362">Response</span></span>
<span data-ttu-id="a743d-p122">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="a743d-p122">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 7215

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
  "partnerReportedThreatState": "activated",
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





