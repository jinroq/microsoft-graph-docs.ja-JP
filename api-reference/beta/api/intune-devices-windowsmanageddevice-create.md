---
title: WindowsManagedDevice を作成します。
description: 新しい windowsManagedDevice オブジェクトを作成します。
ms.openlocfilehash: 79db6b0f2d5f8e918b42fb9b1c5a40b05983edae
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27070251"
---
# <a name="create-windowsmanageddevice"></a><span data-ttu-id="a9134-103">WindowsManagedDevice を作成します。</span><span class="sxs-lookup"><span data-stu-id="a9134-103">Create windowsManagedDevice</span></span>

> <span data-ttu-id="a9134-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="a9134-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a9134-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a9134-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="a9134-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="a9134-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="a9134-107">新しい[windowsManagedDevice](../resources/intune-devices-windowsmanageddevice.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="a9134-107">Create a new [windowsManagedDevice](../resources/intune-devices-windowsmanageddevice.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="a9134-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="a9134-108">Prerequisites</span></span>
<span data-ttu-id="a9134-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="a9134-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a9134-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="a9134-111">Permission type</span></span>|<span data-ttu-id="a9134-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="a9134-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a9134-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="a9134-113">Delegated (work or school account)</span></span>|<span data-ttu-id="a9134-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a9134-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="a9134-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="a9134-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a9134-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a9134-116">Not supported.</span></span>|
|<span data-ttu-id="a9134-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="a9134-117">Application</span></span>|<span data-ttu-id="a9134-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a9134-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a9134-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="a9134-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /users/{usersId}/managedDevices
POST /deviceManagement/managedDevices
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/detectedApps/{detectedAppId}/managedDevices
```

## <a name="request-headers"></a><span data-ttu-id="a9134-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="a9134-120">Request headers</span></span>
|<span data-ttu-id="a9134-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="a9134-121">Header</span></span>|<span data-ttu-id="a9134-122">値</span><span class="sxs-lookup"><span data-stu-id="a9134-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a9134-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="a9134-123">Authorization</span></span>|<span data-ttu-id="a9134-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="a9134-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a9134-125">Accept</span><span class="sxs-lookup"><span data-stu-id="a9134-125">Accept</span></span>|<span data-ttu-id="a9134-126">application/json</span><span class="sxs-lookup"><span data-stu-id="a9134-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a9134-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="a9134-127">Request body</span></span>
<span data-ttu-id="a9134-128">要求の本文に windowsManagedDevice オブジェクトの JSON の形式を指定します。</span><span class="sxs-lookup"><span data-stu-id="a9134-128">In the request body, supply a JSON representation for the windowsManagedDevice object.</span></span>

<span data-ttu-id="a9134-129">次の表は、windowsManagedDevice を作成するときに必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="a9134-129">The following table shows the properties that are required when you create the windowsManagedDevice.</span></span>

|<span data-ttu-id="a9134-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="a9134-130">Property</span></span>|<span data-ttu-id="a9134-131">型</span><span class="sxs-lookup"><span data-stu-id="a9134-131">Type</span></span>|<span data-ttu-id="a9134-132">説明</span><span class="sxs-lookup"><span data-stu-id="a9134-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a9134-133">id</span><span class="sxs-lookup"><span data-stu-id="a9134-133">id</span></span>|<span data-ttu-id="a9134-134">String</span><span class="sxs-lookup"><span data-stu-id="a9134-134">String</span></span>|<span data-ttu-id="a9134-135">[ManagedDevice](../resources/intune-devices-manageddevice.md)から継承されるデバイスの一意の識別子</span><span class="sxs-lookup"><span data-stu-id="a9134-135">Unique Identifier for the device Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="a9134-136">userId</span><span class="sxs-lookup"><span data-stu-id="a9134-136">userId</span></span>|<span data-ttu-id="a9134-137">String</span><span class="sxs-lookup"><span data-stu-id="a9134-137">String</span></span>|<span data-ttu-id="a9134-138">[ManagedDevice](../resources/intune-devices-manageddevice.md)から継承される、デバイスに関連付けられているユーザーの一意の識別子</span><span class="sxs-lookup"><span data-stu-id="a9134-138">Unique Identifier for the user associated with the device Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="a9134-139">deviceName</span><span class="sxs-lookup"><span data-stu-id="a9134-139">deviceName</span></span>|<span data-ttu-id="a9134-140">String</span><span class="sxs-lookup"><span data-stu-id="a9134-140">String</span></span>|<span data-ttu-id="a9134-141">[ManagedDevice](../resources/intune-devices-manageddevice.md)から継承されるデバイスの名前</span><span class="sxs-lookup"><span data-stu-id="a9134-141">Name of the device Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="a9134-142">hardwareInformation</span><span class="sxs-lookup"><span data-stu-id="a9134-142">hardwareInformation</span></span>|[<span data-ttu-id="a9134-143">hardwareInformation</span><span class="sxs-lookup"><span data-stu-id="a9134-143">hardwareInformation</span></span>](../resources/intune-devices-hardwareinformation.md)|<span data-ttu-id="a9134-144">デバイスのハードウェアの詳細。</span><span class="sxs-lookup"><span data-stu-id="a9134-144">The hardward details for the device.</span></span>  <span data-ttu-id="a9134-145">記憶域の製造元、シリアル番号などの情報が含まれています。[ManagedDevice](../resources/intune-devices-manageddevice.md)から継承されました。</span><span class="sxs-lookup"><span data-stu-id="a9134-145">Includes information such as storage space, manufacturer, serial number, etc. Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="a9134-146">ownerType</span><span class="sxs-lookup"><span data-stu-id="a9134-146">ownerType</span></span>|[<span data-ttu-id="a9134-147">ownerType</span><span class="sxs-lookup"><span data-stu-id="a9134-147">ownerType</span></span>](../resources/intune-devices-ownertype.md)|<span data-ttu-id="a9134-148">デバイスの所有権。</span><span class="sxs-lookup"><span data-stu-id="a9134-148">Ownership of the device.</span></span> <span data-ttu-id="a9134-149">'会社' または[managedDevice](../resources/intune-devices-manageddevice.md)からの '個人' の継承を使用できます。</span><span class="sxs-lookup"><span data-stu-id="a9134-149">Can be 'company' or 'personal' Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="a9134-150">可能な値は、`unknown`、`company`、`personal` です。</span><span class="sxs-lookup"><span data-stu-id="a9134-150">Possible values are: `unknown`, `company`, `personal`.</span></span>|
|<span data-ttu-id="a9134-151">managedDeviceOwnerType</span><span class="sxs-lookup"><span data-stu-id="a9134-151">managedDeviceOwnerType</span></span>|[<span data-ttu-id="a9134-152">managedDeviceOwnerType</span><span class="sxs-lookup"><span data-stu-id="a9134-152">managedDeviceOwnerType</span></span>](../resources/intune-devices-manageddeviceownertype.md)|<span data-ttu-id="a9134-153">デバイスの所有権。</span><span class="sxs-lookup"><span data-stu-id="a9134-153">Ownership of the device.</span></span> <span data-ttu-id="a9134-154">'会社' または[managedDevice](../resources/intune-devices-manageddevice.md)からの '個人' の継承を使用できます。</span><span class="sxs-lookup"><span data-stu-id="a9134-154">Can be 'company' or 'personal' Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="a9134-155">可能な値は、`unknown`、`company`、`personal` です。</span><span class="sxs-lookup"><span data-stu-id="a9134-155">Possible values are: `unknown`, `company`, `personal`.</span></span>|
|<span data-ttu-id="a9134-156">deviceActionResults</span><span class="sxs-lookup"><span data-stu-id="a9134-156">deviceActionResults</span></span>|<span data-ttu-id="a9134-157">[deviceActionResult](../resources/intune-devices-deviceactionresult.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="a9134-157">[deviceActionResult](../resources/intune-devices-deviceactionresult.md) collection</span></span>|<span data-ttu-id="a9134-158">ComplexType deviceActionResult オブジェクトのリスト。</span><span class="sxs-lookup"><span data-stu-id="a9134-158">List of ComplexType deviceActionResult objects.</span></span> <span data-ttu-id="a9134-159">[ManagedDevice](../resources/intune-devices-manageddevice.md)から継承されました。</span><span class="sxs-lookup"><span data-stu-id="a9134-159">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="a9134-160">managementState</span><span class="sxs-lookup"><span data-stu-id="a9134-160">managementState</span></span>|[<span data-ttu-id="a9134-161">managementState</span><span class="sxs-lookup"><span data-stu-id="a9134-161">managementState</span></span>](../resources/intune-devices-managementstate.md)|<span data-ttu-id="a9134-162">デバイスの状態を管理します。</span><span class="sxs-lookup"><span data-stu-id="a9134-162">Management state of the device.</span></span> <span data-ttu-id="a9134-163">[ManagedDevice](../resources/intune-devices-manageddevice.md)から継承されます。</span><span class="sxs-lookup"><span data-stu-id="a9134-163">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="a9134-164">可能な値は、`managed`、`retirePending`、`retireFailed`、`wipePending`、`wipeFailed`、`unhealthy`、`deletePending`、`retireIssued`、`wipeIssued`、`wipeCanceled`、`retireCanceled`、`discovered` です。</span><span class="sxs-lookup"><span data-stu-id="a9134-164">Possible values are: `managed`, `retirePending`, `retireFailed`, `wipePending`, `wipeFailed`, `unhealthy`, `deletePending`, `retireIssued`, `wipeIssued`, `wipeCanceled`, `retireCanceled`, `discovered`.</span></span>|
|<span data-ttu-id="a9134-165">enrolledDateTime</span><span class="sxs-lookup"><span data-stu-id="a9134-165">enrolledDateTime</span></span>|<span data-ttu-id="a9134-166">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a9134-166">DateTimeOffset</span></span>|<span data-ttu-id="a9134-167">デバイスの登録時刻。</span><span class="sxs-lookup"><span data-stu-id="a9134-167">Enrollment time of the device.</span></span> <span data-ttu-id="a9134-168">[ManagedDevice](../resources/intune-devices-manageddevice.md)から継承されました。</span><span class="sxs-lookup"><span data-stu-id="a9134-168">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="a9134-169">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="a9134-169">lastSyncDateTime</span></span>|<span data-ttu-id="a9134-170">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a9134-170">DateTimeOffset</span></span>|<span data-ttu-id="a9134-171">デバイスが Intune との正常な同期を最終的に完了した日時。</span><span class="sxs-lookup"><span data-stu-id="a9134-171">The date and time that the device last completed a successful sync with Intune.</span></span> <span data-ttu-id="a9134-172">[ManagedDevice](../resources/intune-devices-manageddevice.md)から継承されました。</span><span class="sxs-lookup"><span data-stu-id="a9134-172">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="a9134-173">chassisType</span><span class="sxs-lookup"><span data-stu-id="a9134-173">chassisType</span></span>|[<span data-ttu-id="a9134-174">chassisType</span><span class="sxs-lookup"><span data-stu-id="a9134-174">chassisType</span></span>](../resources/intune-devices-chassistype.md)|<span data-ttu-id="a9134-175">デバイスのシャーシの種類です。</span><span class="sxs-lookup"><span data-stu-id="a9134-175">Chassis type of the device.</span></span> <span data-ttu-id="a9134-176">[ManagedDevice](../resources/intune-devices-manageddevice.md)から継承されます。</span><span class="sxs-lookup"><span data-stu-id="a9134-176">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="a9134-177">可能な値は、`unknown`、`desktop`、`laptop`、`worksWorkstation`、`enterpriseServer`、`phone`、`tablet`、`mobileOther`、`mobileUnknown` です。</span><span class="sxs-lookup"><span data-stu-id="a9134-177">Possible values are: `unknown`, `desktop`, `laptop`, `worksWorkstation`, `enterpriseServer`, `phone`, `tablet`, `mobileOther`, `mobileUnknown`.</span></span>|
|<span data-ttu-id="a9134-178">operatingSystem</span><span class="sxs-lookup"><span data-stu-id="a9134-178">operatingSystem</span></span>|<span data-ttu-id="a9134-179">String</span><span class="sxs-lookup"><span data-stu-id="a9134-179">String</span></span>|<span data-ttu-id="a9134-180">デバイスのオペレーティング システム。</span><span class="sxs-lookup"><span data-stu-id="a9134-180">Operating system of the device.</span></span> <span data-ttu-id="a9134-181">Windows では、iOS などです。[ManagedDevice](../resources/intune-devices-manageddevice.md)から継承されました。</span><span class="sxs-lookup"><span data-stu-id="a9134-181">Windows, iOS, etc. Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="a9134-182">deviceType</span><span class="sxs-lookup"><span data-stu-id="a9134-182">deviceType</span></span>|[<span data-ttu-id="a9134-183">deviceType</span><span class="sxs-lookup"><span data-stu-id="a9134-183">deviceType</span></span>](../resources/intune-shared-devicetype.md)|<span data-ttu-id="a9134-184">デバイスのプラットフォームです。</span><span class="sxs-lookup"><span data-stu-id="a9134-184">Platform of the device.</span></span> <span data-ttu-id="a9134-185">[ManagedDevice](../resources/intune-devices-manageddevice.md)から継承されます。</span><span class="sxs-lookup"><span data-stu-id="a9134-185">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="a9134-186">使用可能な値: `desktop`、 `windowsRT`、 `winMO6`、 `nokia`、 `windowsPhone`、 `mac`、 `winCE`、 `winEmbedded`、 `iPhone`、 `iPad`、 `iPod`、 `android`、 `iSocConsumer`、 `unix`、 `macMDM`、 `holoLens`、 `surfaceHub`、 `androidForWork`、 `androidEnterprise`, `blackberry`, `palm`, `unknown`.</span><span class="sxs-lookup"><span data-stu-id="a9134-186">Possible values are: `desktop`, `windowsRT`, `winMO6`, `nokia`, `windowsPhone`, `mac`, `winCE`, `winEmbedded`, `iPhone`, `iPad`, `iPod`, `android`, `iSocConsumer`, `unix`, `macMDM`, `holoLens`, `surfaceHub`, `androidForWork`, `androidEnterprise`, `blackberry`, `palm`, `unknown`.</span></span>|
|<span data-ttu-id="a9134-187">complianceState</span><span class="sxs-lookup"><span data-stu-id="a9134-187">complianceState</span></span>|[<span data-ttu-id="a9134-188">complianceState</span><span class="sxs-lookup"><span data-stu-id="a9134-188">complianceState</span></span>](../resources/intune-devices-compliancestate.md)|<span data-ttu-id="a9134-189">デバイスのコンプライアンス状態。</span><span class="sxs-lookup"><span data-stu-id="a9134-189">Compliance state of the device.</span></span> <span data-ttu-id="a9134-190">[ManagedDevice](../resources/intune-devices-manageddevice.md)から継承されます。</span><span class="sxs-lookup"><span data-stu-id="a9134-190">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="a9134-191">可能な値は、`unknown`、`compliant`、`noncompliant`、`conflict`、`error`、`inGracePeriod`、`configManager` です。</span><span class="sxs-lookup"><span data-stu-id="a9134-191">Possible values are: `unknown`, `compliant`, `noncompliant`, `conflict`, `error`, `inGracePeriod`, `configManager`.</span></span>|
|<span data-ttu-id="a9134-192">jailBroken</span><span class="sxs-lookup"><span data-stu-id="a9134-192">jailBroken</span></span>|<span data-ttu-id="a9134-193">String</span><span class="sxs-lookup"><span data-stu-id="a9134-193">String</span></span>|<span data-ttu-id="a9134-194">デバイスが脱獄またはルート化されているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="a9134-194">whether the device is jail broken or rooted.</span></span> <span data-ttu-id="a9134-195">[ManagedDevice](../resources/intune-devices-manageddevice.md)から継承されました。</span><span class="sxs-lookup"><span data-stu-id="a9134-195">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="a9134-196">managementAgent</span><span class="sxs-lookup"><span data-stu-id="a9134-196">managementAgent</span></span>|[<span data-ttu-id="a9134-197">managementAgentType</span><span class="sxs-lookup"><span data-stu-id="a9134-197">managementAgentType</span></span>](../resources/intune-devices-managementagenttype.md)|<span data-ttu-id="a9134-198">デバイスの管理チャネル。</span><span class="sxs-lookup"><span data-stu-id="a9134-198">Management channel of the device.</span></span> <span data-ttu-id="a9134-199">Intune、EA などです。[ManagedDevice](../resources/intune-devices-manageddevice.md)から継承されます。</span><span class="sxs-lookup"><span data-stu-id="a9134-199">Intune, EAS, etc. Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="a9134-200">可能な値は、`eas`、`mdm`、`easMdm`、`intuneClient`、`easIntuneClient`、`configurationManagerClient`、`configurationManagerClientMdm`、`configurationManagerClientMdmEas`、`unknown`、`jamf`、`googleCloudDevicePolicyController`、`microsoft365ManagedMdm` です。</span><span class="sxs-lookup"><span data-stu-id="a9134-200">Possible values are: `eas`, `mdm`, `easMdm`, `intuneClient`, `easIntuneClient`, `configurationManagerClient`, `configurationManagerClientMdm`, `configurationManagerClientMdmEas`, `unknown`, `jamf`, `googleCloudDevicePolicyController`, `microsoft365ManagedMdm`.</span></span>|
|<span data-ttu-id="a9134-201">osVersion</span><span class="sxs-lookup"><span data-stu-id="a9134-201">osVersion</span></span>|<span data-ttu-id="a9134-202">String</span><span class="sxs-lookup"><span data-stu-id="a9134-202">String</span></span>|<span data-ttu-id="a9134-203">デバイスのオペレーティング システムのバージョン。</span><span class="sxs-lookup"><span data-stu-id="a9134-203">Operating system version of the device.</span></span> <span data-ttu-id="a9134-204">[ManagedDevice](../resources/intune-devices-manageddevice.md)から継承されました。</span><span class="sxs-lookup"><span data-stu-id="a9134-204">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="a9134-205">easActivated</span><span class="sxs-lookup"><span data-stu-id="a9134-205">easActivated</span></span>|<span data-ttu-id="a9134-206">Boolean</span><span class="sxs-lookup"><span data-stu-id="a9134-206">Boolean</span></span>|<span data-ttu-id="a9134-207">Exchange ActiveSync がアクティブになっているデバイスかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="a9134-207">Whether the device is Exchange ActiveSync activated.</span></span> <span data-ttu-id="a9134-208">[ManagedDevice](../resources/intune-devices-manageddevice.md)から継承されました。</span><span class="sxs-lookup"><span data-stu-id="a9134-208">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="a9134-209">easDeviceId</span><span class="sxs-lookup"><span data-stu-id="a9134-209">easDeviceId</span></span>|<span data-ttu-id="a9134-210">String</span><span class="sxs-lookup"><span data-stu-id="a9134-210">String</span></span>|<span data-ttu-id="a9134-211">デバイスの Exchange ActiveSync の ID。</span><span class="sxs-lookup"><span data-stu-id="a9134-211">Exchange ActiveSync Id of the device.</span></span> <span data-ttu-id="a9134-212">[ManagedDevice](../resources/intune-devices-manageddevice.md)から継承されました。</span><span class="sxs-lookup"><span data-stu-id="a9134-212">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="a9134-213">easActivationDateTime</span><span class="sxs-lookup"><span data-stu-id="a9134-213">easActivationDateTime</span></span>|<span data-ttu-id="a9134-214">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a9134-214">DateTimeOffset</span></span>|<span data-ttu-id="a9134-215">デバイスの Exchange ActivationSync のアクティブ化の時刻。</span><span class="sxs-lookup"><span data-stu-id="a9134-215">Exchange ActivationSync activation time of the device.</span></span> <span data-ttu-id="a9134-216">[ManagedDevice](../resources/intune-devices-manageddevice.md)から継承されました。</span><span class="sxs-lookup"><span data-stu-id="a9134-216">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="a9134-217">aadRegistered</span><span class="sxs-lookup"><span data-stu-id="a9134-217">aadRegistered</span></span>|<span data-ttu-id="a9134-218">Boolean</span><span class="sxs-lookup"><span data-stu-id="a9134-218">Boolean</span></span>|<span data-ttu-id="a9134-219">Azure Active Directory が登録されているデバイスかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="a9134-219">Whether the device is Azure Active Directory registered.</span></span> <span data-ttu-id="a9134-220">[ManagedDevice](../resources/intune-devices-manageddevice.md)から継承されました。</span><span class="sxs-lookup"><span data-stu-id="a9134-220">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="a9134-221">azureADRegistered</span><span class="sxs-lookup"><span data-stu-id="a9134-221">azureADRegistered</span></span>|<span data-ttu-id="a9134-222">Boolean</span><span class="sxs-lookup"><span data-stu-id="a9134-222">Boolean</span></span>|<span data-ttu-id="a9134-223">Azure Active Directory が登録されているデバイスかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="a9134-223">Whether the device is Azure Active Directory registered.</span></span> <span data-ttu-id="a9134-224">[ManagedDevice](../resources/intune-devices-manageddevice.md)から継承されました。</span><span class="sxs-lookup"><span data-stu-id="a9134-224">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="a9134-225">deviceEnrollmentType</span><span class="sxs-lookup"><span data-stu-id="a9134-225">deviceEnrollmentType</span></span>|[<span data-ttu-id="a9134-226">deviceEnrollmentType</span><span class="sxs-lookup"><span data-stu-id="a9134-226">deviceEnrollmentType</span></span>](../resources/intune-shared-deviceenrollmenttype.md)|<span data-ttu-id="a9134-227">デバイスの登録の種類。</span><span class="sxs-lookup"><span data-stu-id="a9134-227">Enrollment type of the device.</span></span> <span data-ttu-id="a9134-228">[ManagedDevice](../resources/intune-devices-manageddevice.md)から継承されます。</span><span class="sxs-lookup"><span data-stu-id="a9134-228">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="a9134-229">可能な値は、`unknown`、`userEnrollment`、`deviceEnrollmentManager`、`appleBulkWithUser`、`appleBulkWithoutUser`、`windowsAzureADJoin`、`windowsBulkUserless`、`windowsAutoEnrollment`、`windowsBulkAzureDomainJoin`、`windowsCoManagement` です。</span><span class="sxs-lookup"><span data-stu-id="a9134-229">Possible values are: `unknown`, `userEnrollment`, `deviceEnrollmentManager`, `appleBulkWithUser`, `appleBulkWithoutUser`, `windowsAzureADJoin`, `windowsBulkUserless`, `windowsAutoEnrollment`, `windowsBulkAzureDomainJoin`, `windowsCoManagement`.</span></span>|
|<span data-ttu-id="a9134-230">lostModeState</span><span class="sxs-lookup"><span data-stu-id="a9134-230">lostModeState</span></span>|[<span data-ttu-id="a9134-231">lostModeState</span><span class="sxs-lookup"><span data-stu-id="a9134-231">lostModeState</span></span>](../resources/intune-devices-lostmodestate.md)|<span data-ttu-id="a9134-232">失われたモードが有効になっているか、 [managedDevice](../resources/intune-devices-manageddevice.md)からの継承を無効にかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="a9134-232">Indicates if Lost mode is enabled or disabled Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="a9134-233">使用可能な値は、`disabled`、`enabled` です。</span><span class="sxs-lookup"><span data-stu-id="a9134-233">Possible values are: `disabled`, `enabled`.</span></span>|
|<span data-ttu-id="a9134-234">activationLockBypassCode</span><span class="sxs-lookup"><span data-stu-id="a9134-234">activationLockBypassCode</span></span>|<span data-ttu-id="a9134-235">String</span><span class="sxs-lookup"><span data-stu-id="a9134-235">String</span></span>|<span data-ttu-id="a9134-236">デバイスのアクティベーション ロックをバイパスするためのコード。</span><span class="sxs-lookup"><span data-stu-id="a9134-236">Code that allows the Activation Lock on a device to be bypassed.</span></span> <span data-ttu-id="a9134-237">[ManagedDevice](../resources/intune-devices-manageddevice.md)から継承されました。</span><span class="sxs-lookup"><span data-stu-id="a9134-237">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="a9134-238">emailAddress</span><span class="sxs-lookup"><span data-stu-id="a9134-238">emailAddress</span></span>|<span data-ttu-id="a9134-239">String</span><span class="sxs-lookup"><span data-stu-id="a9134-239">String</span></span>|<span data-ttu-id="a9134-240">[ManagedDevice](../resources/intune-devices-manageddevice.md)から継承される、デバイスに関連付けられているユーザーの email(s)</span><span class="sxs-lookup"><span data-stu-id="a9134-240">Email(s) for the user associated with the device Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="a9134-241">azureActiveDirectoryDeviceId</span><span class="sxs-lookup"><span data-stu-id="a9134-241">azureActiveDirectoryDeviceId</span></span>|<span data-ttu-id="a9134-242">String</span><span class="sxs-lookup"><span data-stu-id="a9134-242">String</span></span>|<span data-ttu-id="a9134-243">Azure Active Directory デバイスの一意識別子。</span><span class="sxs-lookup"><span data-stu-id="a9134-243">The unique identifier for the Azure Active Directory device.</span></span> <span data-ttu-id="a9134-244">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="a9134-244">Read only.</span></span> <span data-ttu-id="a9134-245">[ManagedDevice](../resources/intune-devices-manageddevice.md)から継承されました。</span><span class="sxs-lookup"><span data-stu-id="a9134-245">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="a9134-246">azureADDeviceId</span><span class="sxs-lookup"><span data-stu-id="a9134-246">azureADDeviceId</span></span>|<span data-ttu-id="a9134-247">String</span><span class="sxs-lookup"><span data-stu-id="a9134-247">String</span></span>|<span data-ttu-id="a9134-248">Azure Active Directory デバイスの一意識別子。</span><span class="sxs-lookup"><span data-stu-id="a9134-248">The unique identifier for the Azure Active Directory device.</span></span> <span data-ttu-id="a9134-249">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="a9134-249">Read only.</span></span> <span data-ttu-id="a9134-250">[ManagedDevice](../resources/intune-devices-manageddevice.md)から継承されました。</span><span class="sxs-lookup"><span data-stu-id="a9134-250">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="a9134-251">deviceRegistrationState</span><span class="sxs-lookup"><span data-stu-id="a9134-251">deviceRegistrationState</span></span>|[<span data-ttu-id="a9134-252">deviceRegistrationState</span><span class="sxs-lookup"><span data-stu-id="a9134-252">deviceRegistrationState</span></span>](../resources/intune-devices-deviceregistrationstate.md)|<span data-ttu-id="a9134-253">デバイスの登録状態。</span><span class="sxs-lookup"><span data-stu-id="a9134-253">Device registration state.</span></span> <span data-ttu-id="a9134-254">[ManagedDevice](../resources/intune-devices-manageddevice.md)から継承されます。</span><span class="sxs-lookup"><span data-stu-id="a9134-254">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="a9134-255">可能な値は、`notRegistered`、`registered`、`revoked`、`keyConflict`、`approvalPending`、`certificateReset`、`notRegisteredPendingEnrollment`、`unknown` です。</span><span class="sxs-lookup"><span data-stu-id="a9134-255">Possible values are: `notRegistered`, `registered`, `revoked`, `keyConflict`, `approvalPending`, `certificateReset`, `notRegisteredPendingEnrollment`, `unknown`.</span></span>|
|<span data-ttu-id="a9134-256">deviceCategoryDisplayName</span><span class="sxs-lookup"><span data-stu-id="a9134-256">deviceCategoryDisplayName</span></span>|<span data-ttu-id="a9134-257">String</span><span class="sxs-lookup"><span data-stu-id="a9134-257">String</span></span>|<span data-ttu-id="a9134-258">デバイスのカテゴリ表示名を継承[managedDevice から](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="a9134-258">Device category display name Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="a9134-259">isSupervised</span><span class="sxs-lookup"><span data-stu-id="a9134-259">isSupervised</span></span>|<span data-ttu-id="a9134-260">Boolean</span><span class="sxs-lookup"><span data-stu-id="a9134-260">Boolean</span></span>|<span data-ttu-id="a9134-261">デバイスは、 [managedDevice](../resources/intune-devices-manageddevice.md)からの継承の状態を管理</span><span class="sxs-lookup"><span data-stu-id="a9134-261">Device supervised status Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="a9134-262">exchangeLastSuccessfulSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="a9134-262">exchangeLastSuccessfulSyncDateTime</span></span>|<span data-ttu-id="a9134-263">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a9134-263">DateTimeOffset</span></span>|<span data-ttu-id="a9134-264">最後にデバイスが Exchange に接続した時刻。</span><span class="sxs-lookup"><span data-stu-id="a9134-264">Last time the device contacted Exchange.</span></span> <span data-ttu-id="a9134-265">[ManagedDevice](../resources/intune-devices-manageddevice.md)から継承されました。</span><span class="sxs-lookup"><span data-stu-id="a9134-265">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="a9134-266">exchangeAccessState</span><span class="sxs-lookup"><span data-stu-id="a9134-266">exchangeAccessState</span></span>|[<span data-ttu-id="a9134-267">deviceManagementExchangeAccessState</span><span class="sxs-lookup"><span data-stu-id="a9134-267">deviceManagementExchangeAccessState</span></span>](../resources/intune-devices-devicemanagementexchangeaccessstate.md)|<span data-ttu-id="a9134-268">Exchange でのデバイスのアクセスの状態。</span><span class="sxs-lookup"><span data-stu-id="a9134-268">The Access State of the device in Exchange.</span></span> <span data-ttu-id="a9134-269">[ManagedDevice](../resources/intune-devices-manageddevice.md)から継承されます。</span><span class="sxs-lookup"><span data-stu-id="a9134-269">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="a9134-270">可能な値は、`none`、`unknown`、`allowed`、`blocked`、`quarantined` です。</span><span class="sxs-lookup"><span data-stu-id="a9134-270">Possible values are: `none`, `unknown`, `allowed`, `blocked`, `quarantined`.</span></span>|
|<span data-ttu-id="a9134-271">exchangeAccessStateReason</span><span class="sxs-lookup"><span data-stu-id="a9134-271">exchangeAccessStateReason</span></span>|[<span data-ttu-id="a9134-272">deviceManagementExchangeAccessStateReason</span><span class="sxs-lookup"><span data-stu-id="a9134-272">deviceManagementExchangeAccessStateReason</span></span>](../resources/intune-devices-devicemanagementexchangeaccessstatereason.md)|<span data-ttu-id="a9134-273">Exchange でのデバイスのアクセス状態の理由。
</span><span class="sxs-lookup"><span data-stu-id="a9134-273">The reason for the device's access state in Exchange.</span></span> <span data-ttu-id="a9134-274">[ManagedDevice](../resources/intune-devices-manageddevice.md)から継承されます。</span><span class="sxs-lookup"><span data-stu-id="a9134-274">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="a9134-275">可能な値は、`none`、`unknown`、`exchangeGlobalRule`、`exchangeIndividualRule`、`exchangeDeviceRule`、`exchangeUpgrade`、`exchangeMailboxPolicy`、`other`、`compliant`、`notCompliant`、`notEnrolled`、`unknownLocation`、`mfaRequired`、`azureADBlockDueToAccessPolicy`、`compromisedPassword`、`deviceNotKnownWithManagedApp` です。</span><span class="sxs-lookup"><span data-stu-id="a9134-275">Possible values are: `none`, `unknown`, `exchangeGlobalRule`, `exchangeIndividualRule`, `exchangeDeviceRule`, `exchangeUpgrade`, `exchangeMailboxPolicy`, `other`, `compliant`, `notCompliant`, `notEnrolled`, `unknownLocation`, `mfaRequired`, `azureADBlockDueToAccessPolicy`, `compromisedPassword`, `deviceNotKnownWithManagedApp`.</span></span>|
|<span data-ttu-id="a9134-276">remoteAssistanceSessionUrl</span><span class="sxs-lookup"><span data-stu-id="a9134-276">remoteAssistanceSessionUrl</span></span>|<span data-ttu-id="a9134-277">String</span><span class="sxs-lookup"><span data-stu-id="a9134-277">String</span></span>|<span data-ttu-id="a9134-278">デバイスとのリモート アシスタンス セッションを確立できるようにする URL。</span><span class="sxs-lookup"><span data-stu-id="a9134-278">Url that allows a Remote Assistance session to be established with the device.</span></span> <span data-ttu-id="a9134-279">[ManagedDevice](../resources/intune-devices-manageddevice.md)から継承されました。</span><span class="sxs-lookup"><span data-stu-id="a9134-279">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="a9134-280">remoteAssistanceSessionErrorDetails</span><span class="sxs-lookup"><span data-stu-id="a9134-280">remoteAssistanceSessionErrorDetails</span></span>|<span data-ttu-id="a9134-281">String</span><span class="sxs-lookup"><span data-stu-id="a9134-281">String</span></span>|<span data-ttu-id="a9134-282">リモート アシスタンス セッション オブジェクトの作成時に問題を識別するエラー文字列。</span><span class="sxs-lookup"><span data-stu-id="a9134-282">An error string that identifies issues when creating Remote Assistance session objects.</span></span> <span data-ttu-id="a9134-283">[ManagedDevice](../resources/intune-devices-manageddevice.md)から継承されました。</span><span class="sxs-lookup"><span data-stu-id="a9134-283">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="a9134-284">isEncrypted</span><span class="sxs-lookup"><span data-stu-id="a9134-284">isEncrypted</span></span>|<span data-ttu-id="a9134-285">Boolean</span><span class="sxs-lookup"><span data-stu-id="a9134-285">Boolean</span></span>|<span data-ttu-id="a9134-286">[ManagedDevice](../resources/intune-devices-manageddevice.md)から、デバイスの暗号化状態継承</span><span class="sxs-lookup"><span data-stu-id="a9134-286">Device encryption status Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="a9134-287">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="a9134-287">userPrincipalName</span></span>|<span data-ttu-id="a9134-288">String</span><span class="sxs-lookup"><span data-stu-id="a9134-288">String</span></span>|<span data-ttu-id="a9134-289">デバイス ユーザー プリンシパル名で継承される[managedDevice から](../resources/intune-devices-manageddevice.md)</span><span class="sxs-lookup"><span data-stu-id="a9134-289">Device user principal name Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="a9134-290">model</span><span class="sxs-lookup"><span data-stu-id="a9134-290">model</span></span>|<span data-ttu-id="a9134-291">String</span><span class="sxs-lookup"><span data-stu-id="a9134-291">String</span></span>|<span data-ttu-id="a9134-292">[ManagedDevice](../resources/intune-devices-manageddevice.md)から継承されるデバイスのモデル</span><span class="sxs-lookup"><span data-stu-id="a9134-292">Model of the device Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="a9134-293">manufacturer</span><span class="sxs-lookup"><span data-stu-id="a9134-293">manufacturer</span></span>|<span data-ttu-id="a9134-294">String</span><span class="sxs-lookup"><span data-stu-id="a9134-294">String</span></span>|<span data-ttu-id="a9134-295">[ManagedDevice](../resources/intune-devices-manageddevice.md)から継承される、デバイスの製造元</span><span class="sxs-lookup"><span data-stu-id="a9134-295">Manufacturer of the device Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="a9134-296">imei</span><span class="sxs-lookup"><span data-stu-id="a9134-296">imei</span></span>|<span data-ttu-id="a9134-297">String</span><span class="sxs-lookup"><span data-stu-id="a9134-297">String</span></span>|<span data-ttu-id="a9134-298">IMEI は[managedDevice](../resources/intune-devices-manageddevice.md)から継承</span><span class="sxs-lookup"><span data-stu-id="a9134-298">IMEI Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="a9134-299">complianceGracePeriodExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="a9134-299">complianceGracePeriodExpirationDateTime</span></span>|<span data-ttu-id="a9134-300">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a9134-300">DateTimeOffset</span></span>|<span data-ttu-id="a9134-301">[ManagedDevice](../resources/intune-devices-manageddevice.md)から継承されるがデバイスのコンプライアンスの猶予期間の有効期限が切れると、日付と時刻</span><span class="sxs-lookup"><span data-stu-id="a9134-301">The DateTime when device compliance grace period expires Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="a9134-302">シリアル番号</span><span class="sxs-lookup"><span data-stu-id="a9134-302">serialNumber</span></span>|<span data-ttu-id="a9134-303">String</span><span class="sxs-lookup"><span data-stu-id="a9134-303">String</span></span>|<span data-ttu-id="a9134-304">シリアル番号は[managedDevice](../resources/intune-devices-manageddevice.md)から継承</span><span class="sxs-lookup"><span data-stu-id="a9134-304">SerialNumber Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="a9134-305">phoneNumber</span><span class="sxs-lookup"><span data-stu-id="a9134-305">phoneNumber</span></span>|<span data-ttu-id="a9134-306">String</span><span class="sxs-lookup"><span data-stu-id="a9134-306">String</span></span>|<span data-ttu-id="a9134-307">[ManagedDevice](../resources/intune-devices-manageddevice.md)から継承されるデバイスの電話番号</span><span class="sxs-lookup"><span data-stu-id="a9134-307">Phone number of the device Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="a9134-308">androidSecurityPatchLevel</span><span class="sxs-lookup"><span data-stu-id="a9134-308">androidSecurityPatchLevel</span></span>|<span data-ttu-id="a9134-309">String</span><span class="sxs-lookup"><span data-stu-id="a9134-309">String</span></span>|<span data-ttu-id="a9134-310">[ManagedDevice](../resources/intune-devices-manageddevice.md)から android のセキュリティ ・ パッチ ・ レベル継承</span><span class="sxs-lookup"><span data-stu-id="a9134-310">Android security patch level Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="a9134-311">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="a9134-311">userDisplayName</span></span>|<span data-ttu-id="a9134-312">String</span><span class="sxs-lookup"><span data-stu-id="a9134-312">String</span></span>|<span data-ttu-id="a9134-313">[ManagedDevice](../resources/intune-devices-manageddevice.md)から、ユーザーの表示名継承</span><span class="sxs-lookup"><span data-stu-id="a9134-313">User display name Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="a9134-314">configurationManagerClientEnabledFeatures</span><span class="sxs-lookup"><span data-stu-id="a9134-314">configurationManagerClientEnabledFeatures</span></span>|[<span data-ttu-id="a9134-315">configurationManagerClientEnabledFeatures</span><span class="sxs-lookup"><span data-stu-id="a9134-315">configurationManagerClientEnabledFeatures</span></span>](../resources/intune-devices-configurationmanagerclientenabledfeatures.md)|<span data-ttu-id="a9134-316">ConfigrMgr クライアントには、 [managedDevice](../resources/intune-devices-manageddevice.md)からの継承の機能が有効になっています。</span><span class="sxs-lookup"><span data-stu-id="a9134-316">ConfigrMgr client enabled features Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="a9134-317">wiFiMacAddress</span><span class="sxs-lookup"><span data-stu-id="a9134-317">wiFiMacAddress</span></span>|<span data-ttu-id="a9134-318">String</span><span class="sxs-lookup"><span data-stu-id="a9134-318">String</span></span>|<span data-ttu-id="a9134-319">Wi-fi MAC は、 [managedDevice](../resources/intune-devices-manageddevice.md)から継承されました。</span><span class="sxs-lookup"><span data-stu-id="a9134-319">Wi-Fi MAC Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="a9134-320">deviceHealthAttestationState</span><span class="sxs-lookup"><span data-stu-id="a9134-320">deviceHealthAttestationState</span></span>|[<span data-ttu-id="a9134-321">deviceHealthAttestationState</span><span class="sxs-lookup"><span data-stu-id="a9134-321">deviceHealthAttestationState</span></span>](../resources/intune-devices-devicehealthattestationstate.md)|<span data-ttu-id="a9134-322">デバイスの正常性構成証明の状態。</span><span class="sxs-lookup"><span data-stu-id="a9134-322">The device health attestation state.</span></span> <span data-ttu-id="a9134-323">[ManagedDevice](../resources/intune-devices-manageddevice.md)から継承されました。</span><span class="sxs-lookup"><span data-stu-id="a9134-323">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="a9134-324">subscriberCarrier</span><span class="sxs-lookup"><span data-stu-id="a9134-324">subscriberCarrier</span></span>|<span data-ttu-id="a9134-325">String</span><span class="sxs-lookup"><span data-stu-id="a9134-325">String</span></span>|<span data-ttu-id="a9134-326">サブスクライバーのキャリアは、 [managedDevice](../resources/intune-devices-manageddevice.md)から継承されました。</span><span class="sxs-lookup"><span data-stu-id="a9134-326">Subscriber Carrier Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="a9134-327">meid</span><span class="sxs-lookup"><span data-stu-id="a9134-327">meid</span></span>|<span data-ttu-id="a9134-328">String</span><span class="sxs-lookup"><span data-stu-id="a9134-328">String</span></span>|<span data-ttu-id="a9134-329">MEID は[managedDevice](../resources/intune-devices-manageddevice.md)から継承</span><span class="sxs-lookup"><span data-stu-id="a9134-329">MEID Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="a9134-330">totalStorageSpaceInBytes</span><span class="sxs-lookup"><span data-stu-id="a9134-330">totalStorageSpaceInBytes</span></span>|<span data-ttu-id="a9134-331">Int64</span><span class="sxs-lookup"><span data-stu-id="a9134-331">Int64</span></span>|<span data-ttu-id="a9134-332">バイトが[managedDevice](../resources/intune-devices-manageddevice.md)から継承することでストレージの合計</span><span class="sxs-lookup"><span data-stu-id="a9134-332">Total Storage in Bytes Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="a9134-333">freeStorageSpaceInBytes</span><span class="sxs-lookup"><span data-stu-id="a9134-333">freeStorageSpaceInBytes</span></span>|<span data-ttu-id="a9134-334">Int64</span><span class="sxs-lookup"><span data-stu-id="a9134-334">Int64</span></span>|<span data-ttu-id="a9134-335">空きバイト数は、 [managedDevice](../resources/intune-devices-manageddevice.md)から継承することで</span><span class="sxs-lookup"><span data-stu-id="a9134-335">Free Storage in Bytes Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="a9134-336">managedDeviceName</span><span class="sxs-lookup"><span data-stu-id="a9134-336">managedDeviceName</span></span>|<span data-ttu-id="a9134-337">String</span><span class="sxs-lookup"><span data-stu-id="a9134-337">String</span></span>|<span data-ttu-id="a9134-338">デバイスを識別する名前が自動的に生成されます。</span><span class="sxs-lookup"><span data-stu-id="a9134-338">Automatically generated name to identify a device.</span></span> <span data-ttu-id="a9134-339">ユーザー フレンドリ名に上書きできます。</span><span class="sxs-lookup"><span data-stu-id="a9134-339">Can be overwritten to a user friendly name.</span></span> <span data-ttu-id="a9134-340">[ManagedDevice](../resources/intune-devices-manageddevice.md)から継承されました。</span><span class="sxs-lookup"><span data-stu-id="a9134-340">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="a9134-341">partnerReportedThreatState</span><span class="sxs-lookup"><span data-stu-id="a9134-341">partnerReportedThreatState</span></span>|[<span data-ttu-id="a9134-342">managedDevicePartnerReportedHealthState</span><span class="sxs-lookup"><span data-stu-id="a9134-342">managedDevicePartnerReportedHealthState</span></span>](../resources/intune-devices-manageddevicepartnerreportedhealthstate.md)|<span data-ttu-id="a9134-343">Mobile Threat Defense パートナーがアカウントおよびデバイスで使用されている場合の、デバイスの脅威の状態を示します。</span><span class="sxs-lookup"><span data-stu-id="a9134-343">Indicates the threat state of a device when a Mobile Threat Defense partner is in use by the account and device.</span></span> <span data-ttu-id="a9134-344">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="a9134-344">Read Only.</span></span> <span data-ttu-id="a9134-345">[ManagedDevice](../resources/intune-devices-manageddevice.md)から継承されます。</span><span class="sxs-lookup"><span data-stu-id="a9134-345">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="a9134-346">可能な値は、`unknown`、`activated`、`deactivated`、`secured`、`lowSeverity`、`mediumSeverity`、`highSeverity`、`unresponsive`、`compromised`、`misconfigured` です。</span><span class="sxs-lookup"><span data-stu-id="a9134-346">Possible values are: `unknown`, `activated`, `deactivated`, `secured`, `lowSeverity`, `mediumSeverity`, `highSeverity`, `unresponsive`, `compromised`, `misconfigured`.</span></span>|
|<span data-ttu-id="a9134-347">usersLoggedOn</span><span class="sxs-lookup"><span data-stu-id="a9134-347">usersLoggedOn</span></span>|<span data-ttu-id="a9134-348">[loggedOnUser](../resources/intune-devices-loggedonuser.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="a9134-348">[loggedOnUser](../resources/intune-devices-loggedonuser.md) collection</span></span>|<span data-ttu-id="a9134-349">最後に[managedDevice](../resources/intune-devices-manageddevice.md)から継承される、デバイスのユーザーのログオンを示します</span><span class="sxs-lookup"><span data-stu-id="a9134-349">Indicates the last logged on users of a device Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="a9134-350">preferMdmOverGroupPolicyAppliedDateTime</span><span class="sxs-lookup"><span data-stu-id="a9134-350">preferMdmOverGroupPolicyAppliedDateTime</span></span>|<span data-ttu-id="a9134-351">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a9134-351">DateTimeOffset</span></span>|<span data-ttu-id="a9134-352">レポート preferMdmOverGroupPolicy 設定日付と時刻が設定されています。</span><span class="sxs-lookup"><span data-stu-id="a9134-352">Reports the DateTime the preferMdmOverGroupPolicy setting was set.</span></span>  <span data-ttu-id="a9134-353">設定すると、Intune MDM 設定が優先されますグループ ポリシー設定の競合がある場合。</span><span class="sxs-lookup"><span data-stu-id="a9134-353">When set, the Intune MDM settings will override Group Policy settings if there is a conflict.</span></span> <span data-ttu-id="a9134-354">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="a9134-354">Read Only.</span></span> <span data-ttu-id="a9134-355">[ManagedDevice](../resources/intune-devices-manageddevice.md)から継承されました。</span><span class="sxs-lookup"><span data-stu-id="a9134-355">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="a9134-356">autopilotEnrolled</span><span class="sxs-lookup"><span data-stu-id="a9134-356">autopilotEnrolled</span></span>|<span data-ttu-id="a9134-357">ブール値</span><span class="sxs-lookup"><span data-stu-id="a9134-357">Boolean</span></span>|<span data-ttu-id="a9134-358">自動操縦を使用して管理対象のデバイスが登録されている場合にレポートします。</span><span class="sxs-lookup"><span data-stu-id="a9134-358">Reports if the managed device is enrolled via auto-pilot.</span></span> <span data-ttu-id="a9134-359">[ManagedDevice](../resources/intune-devices-manageddevice.md)から継承されました。</span><span class="sxs-lookup"><span data-stu-id="a9134-359">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="a9134-360">requireUserEnrollmentApproval</span><span class="sxs-lookup"><span data-stu-id="a9134-360">requireUserEnrollmentApproval</span></span>|<span data-ttu-id="a9134-361">ブール値</span><span class="sxs-lookup"><span data-stu-id="a9134-361">Boolean</span></span>|<span data-ttu-id="a9134-362">マネージ iOS デバイスがユーザーの承認登録の場合にレポートします。</span><span class="sxs-lookup"><span data-stu-id="a9134-362">Reports if the managed iOS device is user approval enrollment.</span></span> <span data-ttu-id="a9134-363">[ManagedDevice](../resources/intune-devices-manageddevice.md)から継承されました。</span><span class="sxs-lookup"><span data-stu-id="a9134-363">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="a9134-364">managementCertificateExpirationDate</span><span class="sxs-lookup"><span data-stu-id="a9134-364">managementCertificateExpirationDate</span></span>|<span data-ttu-id="a9134-365">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a9134-365">DateTimeOffset</span></span>|<span data-ttu-id="a9134-366">デバイス管理証明書の有効期限の日付継承[managedDevice](../resources/intune-devices-manageddevice.md)からの報告します。</span><span class="sxs-lookup"><span data-stu-id="a9134-366">Reports device management certificate expiration date Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="a9134-367">iccid</span><span class="sxs-lookup"><span data-stu-id="a9134-367">iccid</span></span>|<span data-ttu-id="a9134-368">String</span><span class="sxs-lookup"><span data-stu-id="a9134-368">String</span></span>|<span data-ttu-id="a9134-369">A SIM カードの一意の識別番号は集積回路カードの識別子です。</span><span class="sxs-lookup"><span data-stu-id="a9134-369">Integrated Circuit Card Identifier, it is A SIM card's unique identification number.</span></span> <span data-ttu-id="a9134-370">[ManagedDevice](../resources/intune-devices-manageddevice.md)から継承されました。</span><span class="sxs-lookup"><span data-stu-id="a9134-370">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="a9134-371">udid</span><span class="sxs-lookup"><span data-stu-id="a9134-371">udid</span></span>|<span data-ttu-id="a9134-372">String</span><span class="sxs-lookup"><span data-stu-id="a9134-372">String</span></span>|<span data-ttu-id="a9134-373">IOS と macOS デバイスに一意のデバイス識別子です。</span><span class="sxs-lookup"><span data-stu-id="a9134-373">Unique Device Identifier for iOS and macOS devices.</span></span> <span data-ttu-id="a9134-374">[ManagedDevice](../resources/intune-devices-manageddevice.md)から継承されました。</span><span class="sxs-lookup"><span data-stu-id="a9134-374">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="a9134-375">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="a9134-375">roleScopeTagIds</span></span>|<span data-ttu-id="a9134-376">String コレクション</span><span class="sxs-lookup"><span data-stu-id="a9134-376">String collection</span></span>|<span data-ttu-id="a9134-377">このデバイス インスタンスのスコープのタグ Id のリストです。</span><span class="sxs-lookup"><span data-stu-id="a9134-377">List of Scope Tag IDs for this Device instance.</span></span> <span data-ttu-id="a9134-378">[ManagedDevice](../resources/intune-devices-manageddevice.md)から継承されました。</span><span class="sxs-lookup"><span data-stu-id="a9134-378">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="a9134-379">windowsActiveMalwareCount</span><span class="sxs-lookup"><span data-stu-id="a9134-379">windowsActiveMalwareCount</span></span>|<span data-ttu-id="a9134-380">Int32</span><span class="sxs-lookup"><span data-stu-id="a9134-380">Int32</span></span>|<span data-ttu-id="a9134-381">[ManagedDevice](../resources/intune-devices-manageddevice.md)から継承される windows デバイスのアクティブなマルウェアの数</span><span class="sxs-lookup"><span data-stu-id="a9134-381">Count of active malware for this windows device Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="a9134-382">windowsRemediatedMalwareCount</span><span class="sxs-lookup"><span data-stu-id="a9134-382">windowsRemediatedMalwareCount</span></span>|<span data-ttu-id="a9134-383">Int32</span><span class="sxs-lookup"><span data-stu-id="a9134-383">Int32</span></span>|<span data-ttu-id="a9134-384">この windows デバイス継承[managedDevice](../resources/intune-devices-manageddevice.md)からの修正されたマルウェアの数</span><span class="sxs-lookup"><span data-stu-id="a9134-384">Count of remediated malware for this windows device Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="a9134-385">notes</span><span class="sxs-lookup"><span data-stu-id="a9134-385">notes</span></span>|<span data-ttu-id="a9134-386">String</span><span class="sxs-lookup"><span data-stu-id="a9134-386">String</span></span>|<span data-ttu-id="a9134-387">[ManagedDevice](../resources/intune-devices-manageddevice.md)から IT 管理者は継承によって作成されたデバイスに関する注意事項</span><span class="sxs-lookup"><span data-stu-id="a9134-387">Notes on the device created by IT Admin Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="a9134-388">configurationManagerClientHealthState</span><span class="sxs-lookup"><span data-stu-id="a9134-388">configurationManagerClientHealthState</span></span>|[<span data-ttu-id="a9134-389">configurationManagerClientHealthState</span><span class="sxs-lookup"><span data-stu-id="a9134-389">configurationManagerClientHealthState</span></span>](../resources/intune-devices-configurationmanagerclienthealthstate.md)|<span data-ttu-id="a9134-390">構成マネージャー クライアント正常性の状態、 [managedDevice](../resources/intune-devices-manageddevice.md)から、MDM と構成マネージャー エージェントの継承によって管理されているデバイスに対してのみ有効です。</span><span class="sxs-lookup"><span data-stu-id="a9134-390">Configuration manager client health state, valid only for devices managed by MDM/ConfigMgr Agent Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|



## <a name="response"></a><span data-ttu-id="a9134-391">応答</span><span class="sxs-lookup"><span data-stu-id="a9134-391">Response</span></span>
<span data-ttu-id="a9134-392">かどうかは成功すると、このメソッドが返されます、`201 Created`応答コードおよび応答の本文に[windowsManagedDevice](../resources/intune-devices-windowsmanageddevice.md)オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="a9134-392">If successful, this method returns a `201 Created` response code and a [windowsManagedDevice](../resources/intune-devices-windowsmanageddevice.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a9134-393">例</span><span class="sxs-lookup"><span data-stu-id="a9134-393">Example</span></span>
### <a name="request"></a><span data-ttu-id="a9134-394">要求</span><span class="sxs-lookup"><span data-stu-id="a9134-394">Request</span></span>
<span data-ttu-id="a9134-395">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="a9134-395">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/users/{usersId}/managedDevices
Content-type: application/json
Content-length: 7173

{
  "@odata.type": "#microsoft.graph.windowsManagedDevice",
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

### <a name="response"></a><span data-ttu-id="a9134-396">応答</span><span class="sxs-lookup"><span data-stu-id="a9134-396">Response</span></span>
<span data-ttu-id="a9134-p142">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="a9134-p142">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 7222

{
  "@odata.type": "#microsoft.graph.windowsManagedDevice",
  "id": "97842b67-2b67-9784-672b-8497672b8497",
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





