---
title: windowsmanageddevice を更新する
description: windowsmanageddevice オブジェクトのプロパティを更新します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: e1fd03350e06b467713ee1338e62f58cab45b44a
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/29/2019
ms.locfileid: "30962555"
---
# <a name="update-windowsmanageddevice"></a><span data-ttu-id="13f86-103">windowsmanageddevice を更新する</span><span class="sxs-lookup"><span data-stu-id="13f86-103">Update windowsManagedDevice</span></span>

> <span data-ttu-id="13f86-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="13f86-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="13f86-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="13f86-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="13f86-106">[windowsmanageddevice](../resources/intune-devices-windowsmanageddevice.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="13f86-106">Update the properties of a [windowsManagedDevice](../resources/intune-devices-windowsmanageddevice.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="13f86-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="13f86-107">Prerequisites</span></span>
<span data-ttu-id="13f86-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="13f86-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="13f86-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="13f86-110">Permission type</span></span>|<span data-ttu-id="13f86-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="13f86-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="13f86-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="13f86-112">Delegated (work or school account)</span></span>|<span data-ttu-id="13f86-113">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="13f86-113">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="13f86-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="13f86-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="13f86-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="13f86-115">Not supported.</span></span>|
|<span data-ttu-id="13f86-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="13f86-116">Application</span></span>|<span data-ttu-id="13f86-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="13f86-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="13f86-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="13f86-118">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="13f86-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="13f86-119">Request headers</span></span>
|<span data-ttu-id="13f86-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="13f86-120">Header</span></span>|<span data-ttu-id="13f86-121">値</span><span class="sxs-lookup"><span data-stu-id="13f86-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="13f86-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="13f86-122">Authorization</span></span>|<span data-ttu-id="13f86-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="13f86-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="13f86-124">承諾</span><span class="sxs-lookup"><span data-stu-id="13f86-124">Accept</span></span>|<span data-ttu-id="13f86-125">application/json</span><span class="sxs-lookup"><span data-stu-id="13f86-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="13f86-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="13f86-126">Request body</span></span>
<span data-ttu-id="13f86-127">要求本文で、 [windowsmanageddevice](../resources/intune-devices-windowsmanageddevice.md)オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="13f86-127">In the request body, supply a JSON representation for the [windowsManagedDevice](../resources/intune-devices-windowsmanageddevice.md) object.</span></span>

<span data-ttu-id="13f86-128">次の表に、 [windowsmanageddevice](../resources/intune-devices-windowsmanageddevice.md)の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="13f86-128">The following table shows the properties that are required when you create the [windowsManagedDevice](../resources/intune-devices-windowsmanageddevice.md).</span></span>

|<span data-ttu-id="13f86-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="13f86-129">Property</span></span>|<span data-ttu-id="13f86-130">型</span><span class="sxs-lookup"><span data-stu-id="13f86-130">Type</span></span>|<span data-ttu-id="13f86-131">説明</span><span class="sxs-lookup"><span data-stu-id="13f86-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="13f86-132">id</span><span class="sxs-lookup"><span data-stu-id="13f86-132">id</span></span>|<span data-ttu-id="13f86-133">String</span><span class="sxs-lookup"><span data-stu-id="13f86-133">String</span></span>|<span data-ttu-id="13f86-134">[manageddevice](../resources/intune-devices-manageddevice.md)から継承されたデバイスの一意識別子</span><span class="sxs-lookup"><span data-stu-id="13f86-134">Unique Identifier for the device Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="13f86-135">userId</span><span class="sxs-lookup"><span data-stu-id="13f86-135">userId</span></span>|<span data-ttu-id="13f86-136">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="13f86-136">String</span></span>|<span data-ttu-id="13f86-137">[manageddevice](../resources/intune-devices-manageddevice.md)から継承したデバイスに関連付けられているユーザーの一意識別子</span><span class="sxs-lookup"><span data-stu-id="13f86-137">Unique Identifier for the user associated with the device Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="13f86-138">deviceName</span><span class="sxs-lookup"><span data-stu-id="13f86-138">deviceName</span></span>|<span data-ttu-id="13f86-139">String</span><span class="sxs-lookup"><span data-stu-id="13f86-139">String</span></span>|<span data-ttu-id="13f86-140">[manageddevice](../resources/intune-devices-manageddevice.md)から継承されたデバイスの名前</span><span class="sxs-lookup"><span data-stu-id="13f86-140">Name of the device Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="13f86-141">hardwareInformation</span><span class="sxs-lookup"><span data-stu-id="13f86-141">hardwareInformation</span></span>|[<span data-ttu-id="13f86-142">hardwareInformation</span><span class="sxs-lookup"><span data-stu-id="13f86-142">hardwareInformation</span></span>](../resources/intune-devices-hardwareinformation.md)|<span data-ttu-id="13f86-143">デバイスのハードワードの詳細。</span><span class="sxs-lookup"><span data-stu-id="13f86-143">The hardward details for the device.</span></span>  <span data-ttu-id="13f86-144">記憶領域、製造元、シリアル番号などの情報が含まれます。[manageddevice](../resources/intune-devices-manageddevice.md)から継承します</span><span class="sxs-lookup"><span data-stu-id="13f86-144">Includes information such as storage space, manufacturer, serial number, etc. Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="13f86-145">ownerType</span><span class="sxs-lookup"><span data-stu-id="13f86-145">ownerType</span></span>|[<span data-ttu-id="13f86-146">ownerType</span><span class="sxs-lookup"><span data-stu-id="13f86-146">ownerType</span></span>](../resources/intune-devices-ownertype.md)|<span data-ttu-id="13f86-147">デバイスの所有権。</span><span class="sxs-lookup"><span data-stu-id="13f86-147">Ownership of the device.</span></span> <span data-ttu-id="13f86-148">' company ' または ' personal ' を[manageddevice](../resources/intune-devices-manageddevice.md)から継承することができます。</span><span class="sxs-lookup"><span data-stu-id="13f86-148">Can be 'company' or 'personal' Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="13f86-149">使用可能な値は、`unknown`、`company`、`personal` です。</span><span class="sxs-lookup"><span data-stu-id="13f86-149">Possible values are: `unknown`, `company`, `personal`.</span></span>|
|<span data-ttu-id="13f86-150">managedDeviceOwnerType</span><span class="sxs-lookup"><span data-stu-id="13f86-150">managedDeviceOwnerType</span></span>|[<span data-ttu-id="13f86-151">managedDeviceOwnerType</span><span class="sxs-lookup"><span data-stu-id="13f86-151">managedDeviceOwnerType</span></span>](../resources/intune-devices-manageddeviceownertype.md)|<span data-ttu-id="13f86-152">デバイスの所有権。</span><span class="sxs-lookup"><span data-stu-id="13f86-152">Ownership of the device.</span></span> <span data-ttu-id="13f86-153">' company ' または ' personal ' を[manageddevice](../resources/intune-devices-manageddevice.md)から継承することができます。</span><span class="sxs-lookup"><span data-stu-id="13f86-153">Can be 'company' or 'personal' Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="13f86-154">使用可能な値は、`unknown`、`company`、`personal` です。</span><span class="sxs-lookup"><span data-stu-id="13f86-154">Possible values are: `unknown`, `company`, `personal`.</span></span>|
|<span data-ttu-id="13f86-155">deviceActionResults</span><span class="sxs-lookup"><span data-stu-id="13f86-155">deviceActionResults</span></span>|<span data-ttu-id="13f86-156">[deviceActionResult](../resources/intune-devices-deviceactionresult.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="13f86-156">[deviceActionResult](../resources/intune-devices-deviceactionresult.md) collection</span></span>|<span data-ttu-id="13f86-157">ComplexType deviceActionResult オブジェクトのリスト。</span><span class="sxs-lookup"><span data-stu-id="13f86-157">List of ComplexType deviceActionResult objects.</span></span> <span data-ttu-id="13f86-158">[manageddevice](../resources/intune-devices-manageddevice.md)から継承します</span><span class="sxs-lookup"><span data-stu-id="13f86-158">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="13f86-159">managementstate</span><span class="sxs-lookup"><span data-stu-id="13f86-159">managementState</span></span>|[<span data-ttu-id="13f86-160">managementstate</span><span class="sxs-lookup"><span data-stu-id="13f86-160">managementState</span></span>](../resources/intune-devices-managementstate.md)|<span data-ttu-id="13f86-161">デバイスの管理状態。</span><span class="sxs-lookup"><span data-stu-id="13f86-161">Management state of the device.</span></span> <span data-ttu-id="13f86-162">[manageddevice](../resources/intune-devices-manageddevice.md)から継承されます。</span><span class="sxs-lookup"><span data-stu-id="13f86-162">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="13f86-163">可能な値は、`managed`、`retirePending`、`retireFailed`、`wipePending`、`wipeFailed`、`unhealthy`、`deletePending`、`retireIssued`、`wipeIssued`、`wipeCanceled`、`retireCanceled`、`discovered` です。</span><span class="sxs-lookup"><span data-stu-id="13f86-163">Possible values are: `managed`, `retirePending`, `retireFailed`, `wipePending`, `wipeFailed`, `unhealthy`, `deletePending`, `retireIssued`, `wipeIssued`, `wipeCanceled`, `retireCanceled`, `discovered`.</span></span>|
|<span data-ttu-id="13f86-164">enrolledDateTime</span><span class="sxs-lookup"><span data-stu-id="13f86-164">enrolledDateTime</span></span>|<span data-ttu-id="13f86-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="13f86-165">DateTimeOffset</span></span>|<span data-ttu-id="13f86-166">デバイスの登録時刻。</span><span class="sxs-lookup"><span data-stu-id="13f86-166">Enrollment time of the device.</span></span> <span data-ttu-id="13f86-167">[manageddevice](../resources/intune-devices-manageddevice.md)から継承します</span><span class="sxs-lookup"><span data-stu-id="13f86-167">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="13f86-168">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="13f86-168">lastSyncDateTime</span></span>|<span data-ttu-id="13f86-169">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="13f86-169">DateTimeOffset</span></span>|<span data-ttu-id="13f86-170">デバイスが Intune との正常な同期を最終的に完了した日時。</span><span class="sxs-lookup"><span data-stu-id="13f86-170">The date and time that the device last completed a successful sync with Intune.</span></span> <span data-ttu-id="13f86-171">[manageddevice](../resources/intune-devices-manageddevice.md)から継承します</span><span class="sxs-lookup"><span data-stu-id="13f86-171">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="13f86-172">chassisType</span><span class="sxs-lookup"><span data-stu-id="13f86-172">chassisType</span></span>|[<span data-ttu-id="13f86-173">chassisType</span><span class="sxs-lookup"><span data-stu-id="13f86-173">chassisType</span></span>](../resources/intune-devices-chassistype.md)|<span data-ttu-id="13f86-174">デバイスのシャーシの種類。</span><span class="sxs-lookup"><span data-stu-id="13f86-174">Chassis type of the device.</span></span> <span data-ttu-id="13f86-175">[manageddevice](../resources/intune-devices-manageddevice.md)から継承されます。</span><span class="sxs-lookup"><span data-stu-id="13f86-175">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="13f86-176">可能な値は、`unknown`、`desktop`、`laptop`、`worksWorkstation`、`enterpriseServer`、`phone`、`tablet`、`mobileOther`、`mobileUnknown` です。</span><span class="sxs-lookup"><span data-stu-id="13f86-176">Possible values are: `unknown`, `desktop`, `laptop`, `worksWorkstation`, `enterpriseServer`, `phone`, `tablet`, `mobileOther`, `mobileUnknown`.</span></span>|
|<span data-ttu-id="13f86-177">operatingSystem</span><span class="sxs-lookup"><span data-stu-id="13f86-177">operatingSystem</span></span>|<span data-ttu-id="13f86-178">文字列</span><span class="sxs-lookup"><span data-stu-id="13f86-178">String</span></span>|<span data-ttu-id="13f86-179">デバイスのオペレーティング システム。</span><span class="sxs-lookup"><span data-stu-id="13f86-179">Operating system of the device.</span></span> <span data-ttu-id="13f86-180">Windows、iOS など[manageddevice](../resources/intune-devices-manageddevice.md)から継承します</span><span class="sxs-lookup"><span data-stu-id="13f86-180">Windows, iOS, etc. Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="13f86-181">deviceType</span><span class="sxs-lookup"><span data-stu-id="13f86-181">deviceType</span></span>|[<span data-ttu-id="13f86-182">deviceType</span><span class="sxs-lookup"><span data-stu-id="13f86-182">deviceType</span></span>](../resources/intune-shared-devicetype.md)|<span data-ttu-id="13f86-183">デバイスのプラットフォーム。</span><span class="sxs-lookup"><span data-stu-id="13f86-183">Platform of the device.</span></span> <span data-ttu-id="13f86-184">[manageddevice](../resources/intune-devices-manageddevice.md)から継承されます。</span><span class="sxs-lookup"><span data-stu-id="13f86-184">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="13f86-185">可能な値: `desktop`、 `windowsRT` `winMO6` `nokia` `windowsPhone` `mac` `winCE` `winEmbedded` `iPhone` `iPad` `iPod` `android`、、、、、、、、、、、、 `iSocConsumer` `unix` `macMDM` `holoLens` `surfaceHub` `androidForWork` `androidEnterprise`, `blackberry`, `palm`, `unknown`.</span><span class="sxs-lookup"><span data-stu-id="13f86-185">Possible values are: `desktop`, `windowsRT`, `winMO6`, `nokia`, `windowsPhone`, `mac`, `winCE`, `winEmbedded`, `iPhone`, `iPad`, `iPod`, `android`, `iSocConsumer`, `unix`, `macMDM`, `holoLens`, `surfaceHub`, `androidForWork`, `androidEnterprise`, `blackberry`, `palm`, `unknown`.</span></span>|
|<span data-ttu-id="13f86-186">complianceState</span><span class="sxs-lookup"><span data-stu-id="13f86-186">complianceState</span></span>|[<span data-ttu-id="13f86-187">complianceState</span><span class="sxs-lookup"><span data-stu-id="13f86-187">complianceState</span></span>](../resources/intune-devices-compliancestate.md)|<span data-ttu-id="13f86-188">デバイスのコンプライアンス状態。</span><span class="sxs-lookup"><span data-stu-id="13f86-188">Compliance state of the device.</span></span> <span data-ttu-id="13f86-189">[manageddevice](../resources/intune-devices-manageddevice.md)から継承されます。</span><span class="sxs-lookup"><span data-stu-id="13f86-189">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="13f86-190">可能な値は、`unknown`、`compliant`、`noncompliant`、`conflict`、`error`、`inGracePeriod`、`configManager` です。</span><span class="sxs-lookup"><span data-stu-id="13f86-190">Possible values are: `unknown`, `compliant`, `noncompliant`, `conflict`, `error`, `inGracePeriod`, `configManager`.</span></span>|
|<span data-ttu-id="13f86-191">jailBroken</span><span class="sxs-lookup"><span data-stu-id="13f86-191">jailBroken</span></span>|<span data-ttu-id="13f86-192">String</span><span class="sxs-lookup"><span data-stu-id="13f86-192">String</span></span>|<span data-ttu-id="13f86-193">デバイスが脱獄またはルート化されているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="13f86-193">whether the device is jail broken or rooted.</span></span> <span data-ttu-id="13f86-194">[manageddevice](../resources/intune-devices-manageddevice.md)から継承します</span><span class="sxs-lookup"><span data-stu-id="13f86-194">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="13f86-195">managementAgent</span><span class="sxs-lookup"><span data-stu-id="13f86-195">managementAgent</span></span>|[<span data-ttu-id="13f86-196">managementagenttype</span><span class="sxs-lookup"><span data-stu-id="13f86-196">managementAgentType</span></span>](../resources/intune-devices-managementagenttype.md)|<span data-ttu-id="13f86-197">デバイスの管理チャネル。</span><span class="sxs-lookup"><span data-stu-id="13f86-197">Management channel of the device.</span></span> <span data-ttu-id="13f86-198">Intune、EAS など。[manageddevice](../resources/intune-devices-manageddevice.md)から継承されます。</span><span class="sxs-lookup"><span data-stu-id="13f86-198">Intune, EAS, etc. Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="13f86-199">可能な値は、`eas`、`mdm`、`easMdm`、`intuneClient`、`easIntuneClient`、`configurationManagerClient`、`configurationManagerClientMdm`、`configurationManagerClientMdmEas`、`unknown`、`jamf`、`googleCloudDevicePolicyController`、`microsoft365ManagedMdm` です。</span><span class="sxs-lookup"><span data-stu-id="13f86-199">Possible values are: `eas`, `mdm`, `easMdm`, `intuneClient`, `easIntuneClient`, `configurationManagerClient`, `configurationManagerClientMdm`, `configurationManagerClientMdmEas`, `unknown`, `jamf`, `googleCloudDevicePolicyController`, `microsoft365ManagedMdm`.</span></span>|
|<span data-ttu-id="13f86-200">osVersion</span><span class="sxs-lookup"><span data-stu-id="13f86-200">osVersion</span></span>|<span data-ttu-id="13f86-201">String</span><span class="sxs-lookup"><span data-stu-id="13f86-201">String</span></span>|<span data-ttu-id="13f86-202">デバイスのオペレーティング システムのバージョン。</span><span class="sxs-lookup"><span data-stu-id="13f86-202">Operating system version of the device.</span></span> <span data-ttu-id="13f86-203">[manageddevice](../resources/intune-devices-manageddevice.md)から継承します</span><span class="sxs-lookup"><span data-stu-id="13f86-203">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="13f86-204">easActivated</span><span class="sxs-lookup"><span data-stu-id="13f86-204">easActivated</span></span>|<span data-ttu-id="13f86-205">Boolean</span><span class="sxs-lookup"><span data-stu-id="13f86-205">Boolean</span></span>|<span data-ttu-id="13f86-206">Exchange ActiveSync がアクティブになっているデバイスかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="13f86-206">Whether the device is Exchange ActiveSync activated.</span></span> <span data-ttu-id="13f86-207">[manageddevice](../resources/intune-devices-manageddevice.md)から継承します</span><span class="sxs-lookup"><span data-stu-id="13f86-207">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="13f86-208">easDeviceId</span><span class="sxs-lookup"><span data-stu-id="13f86-208">easDeviceId</span></span>|<span data-ttu-id="13f86-209">String</span><span class="sxs-lookup"><span data-stu-id="13f86-209">String</span></span>|<span data-ttu-id="13f86-210">デバイスの Exchange ActiveSync の ID。</span><span class="sxs-lookup"><span data-stu-id="13f86-210">Exchange ActiveSync Id of the device.</span></span> <span data-ttu-id="13f86-211">[manageddevice](../resources/intune-devices-manageddevice.md)から継承します</span><span class="sxs-lookup"><span data-stu-id="13f86-211">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="13f86-212">easActivationDateTime</span><span class="sxs-lookup"><span data-stu-id="13f86-212">easActivationDateTime</span></span>|<span data-ttu-id="13f86-213">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="13f86-213">DateTimeOffset</span></span>|<span data-ttu-id="13f86-214">デバイスの Exchange ActivationSync のアクティブ化の時刻。</span><span class="sxs-lookup"><span data-stu-id="13f86-214">Exchange ActivationSync activation time of the device.</span></span> <span data-ttu-id="13f86-215">[manageddevice](../resources/intune-devices-manageddevice.md)から継承します</span><span class="sxs-lookup"><span data-stu-id="13f86-215">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="13f86-216">aadRegistered</span><span class="sxs-lookup"><span data-stu-id="13f86-216">aadRegistered</span></span>|<span data-ttu-id="13f86-217">Boolean</span><span class="sxs-lookup"><span data-stu-id="13f86-217">Boolean</span></span>|<span data-ttu-id="13f86-218">Azure Active Directory が登録されているデバイスかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="13f86-218">Whether the device is Azure Active Directory registered.</span></span> <span data-ttu-id="13f86-219">[manageddevice](../resources/intune-devices-manageddevice.md)から継承します</span><span class="sxs-lookup"><span data-stu-id="13f86-219">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="13f86-220">azureADRegistered</span><span class="sxs-lookup"><span data-stu-id="13f86-220">azureADRegistered</span></span>|<span data-ttu-id="13f86-221">Boolean</span><span class="sxs-lookup"><span data-stu-id="13f86-221">Boolean</span></span>|<span data-ttu-id="13f86-222">Azure Active Directory が登録されているデバイスかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="13f86-222">Whether the device is Azure Active Directory registered.</span></span> <span data-ttu-id="13f86-223">[manageddevice](../resources/intune-devices-manageddevice.md)から継承します</span><span class="sxs-lookup"><span data-stu-id="13f86-223">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="13f86-224">deviceEnrollmentType</span><span class="sxs-lookup"><span data-stu-id="13f86-224">deviceEnrollmentType</span></span>|[<span data-ttu-id="13f86-225">deviceEnrollmentType</span><span class="sxs-lookup"><span data-stu-id="13f86-225">deviceEnrollmentType</span></span>](../resources/intune-shared-deviceenrollmenttype.md)|<span data-ttu-id="13f86-226">デバイスの登録の種類。</span><span class="sxs-lookup"><span data-stu-id="13f86-226">Enrollment type of the device.</span></span> <span data-ttu-id="13f86-227">[manageddevice](../resources/intune-devices-manageddevice.md)から継承されます。</span><span class="sxs-lookup"><span data-stu-id="13f86-227">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="13f86-228">可能な値は、`unknown`、`userEnrollment`、`deviceEnrollmentManager`、`appleBulkWithUser`、`appleBulkWithoutUser`、`windowsAzureADJoin`、`windowsBulkUserless`、`windowsAutoEnrollment`、`windowsBulkAzureDomainJoin`、`windowsCoManagement` です。</span><span class="sxs-lookup"><span data-stu-id="13f86-228">Possible values are: `unknown`, `userEnrollment`, `deviceEnrollmentManager`, `appleBulkWithUser`, `appleBulkWithoutUser`, `windowsAzureADJoin`, `windowsBulkUserless`, `windowsAutoEnrollment`, `windowsBulkAzureDomainJoin`, `windowsCoManagement`.</span></span>|
|<span data-ttu-id="13f86-229">lostModeState</span><span class="sxs-lookup"><span data-stu-id="13f86-229">lostModeState</span></span>|[<span data-ttu-id="13f86-230">lostModeState</span><span class="sxs-lookup"><span data-stu-id="13f86-230">lostModeState</span></span>](../resources/intune-devices-lostmodestate.md)|<span data-ttu-id="13f86-231">失われたモードが有効になっているか、 [manageddevice](../resources/intune-devices-manageddevice.md)から継承が無効かどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="13f86-231">Indicates if Lost mode is enabled or disabled Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="13f86-232">可能な値は、`disabled`、`enabled` です。</span><span class="sxs-lookup"><span data-stu-id="13f86-232">Possible values are: `disabled`, `enabled`.</span></span>|
|<span data-ttu-id="13f86-233">activationLockBypassCode</span><span class="sxs-lookup"><span data-stu-id="13f86-233">activationLockBypassCode</span></span>|<span data-ttu-id="13f86-234">String</span><span class="sxs-lookup"><span data-stu-id="13f86-234">String</span></span>|<span data-ttu-id="13f86-235">デバイスのアクティベーション ロックをバイパスするためのコード。</span><span class="sxs-lookup"><span data-stu-id="13f86-235">Code that allows the Activation Lock on a device to be bypassed.</span></span> <span data-ttu-id="13f86-236">[manageddevice](../resources/intune-devices-manageddevice.md)から継承します</span><span class="sxs-lookup"><span data-stu-id="13f86-236">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="13f86-237">emailAddress</span><span class="sxs-lookup"><span data-stu-id="13f86-237">emailAddress</span></span>|<span data-ttu-id="13f86-238">String</span><span class="sxs-lookup"><span data-stu-id="13f86-238">String</span></span>|<span data-ttu-id="13f86-239">[manageddevice](../resources/intune-devices-manageddevice.md)から継承したデバイスに関連付けられているユーザーの電子メール</span><span class="sxs-lookup"><span data-stu-id="13f86-239">Email(s) for the user associated with the device Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="13f86-240">azureActiveDirectoryDeviceId</span><span class="sxs-lookup"><span data-stu-id="13f86-240">azureActiveDirectoryDeviceId</span></span>|<span data-ttu-id="13f86-241">String</span><span class="sxs-lookup"><span data-stu-id="13f86-241">String</span></span>|<span data-ttu-id="13f86-242">Azure Active Directory デバイスの一意識別子。</span><span class="sxs-lookup"><span data-stu-id="13f86-242">The unique identifier for the Azure Active Directory device.</span></span> <span data-ttu-id="13f86-243">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="13f86-243">Read only.</span></span> <span data-ttu-id="13f86-244">[manageddevice](../resources/intune-devices-manageddevice.md)から継承します</span><span class="sxs-lookup"><span data-stu-id="13f86-244">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="13f86-245">azureADDeviceId</span><span class="sxs-lookup"><span data-stu-id="13f86-245">azureADDeviceId</span></span>|<span data-ttu-id="13f86-246">String</span><span class="sxs-lookup"><span data-stu-id="13f86-246">String</span></span>|<span data-ttu-id="13f86-247">Azure Active Directory デバイスの一意識別子。</span><span class="sxs-lookup"><span data-stu-id="13f86-247">The unique identifier for the Azure Active Directory device.</span></span> <span data-ttu-id="13f86-248">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="13f86-248">Read only.</span></span> <span data-ttu-id="13f86-249">[manageddevice](../resources/intune-devices-manageddevice.md)から継承します</span><span class="sxs-lookup"><span data-stu-id="13f86-249">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="13f86-250">deviceRegistrationState</span><span class="sxs-lookup"><span data-stu-id="13f86-250">deviceRegistrationState</span></span>|[<span data-ttu-id="13f86-251">deviceRegistrationState</span><span class="sxs-lookup"><span data-stu-id="13f86-251">deviceRegistrationState</span></span>](../resources/intune-devices-deviceregistrationstate.md)|<span data-ttu-id="13f86-252">デバイスの登録状態。</span><span class="sxs-lookup"><span data-stu-id="13f86-252">Device registration state.</span></span> <span data-ttu-id="13f86-253">[manageddevice](../resources/intune-devices-manageddevice.md)から継承されます。</span><span class="sxs-lookup"><span data-stu-id="13f86-253">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="13f86-254">可能な値は、`notRegistered`、`registered`、`revoked`、`keyConflict`、`approvalPending`、`certificateReset`、`notRegisteredPendingEnrollment`、`unknown` です。</span><span class="sxs-lookup"><span data-stu-id="13f86-254">Possible values are: `notRegistered`, `registered`, `revoked`, `keyConflict`, `approvalPending`, `certificateReset`, `notRegisteredPendingEnrollment`, `unknown`.</span></span>|
|<span data-ttu-id="13f86-255">deviceCategoryDisplayName</span><span class="sxs-lookup"><span data-stu-id="13f86-255">deviceCategoryDisplayName</span></span>|<span data-ttu-id="13f86-256">String</span><span class="sxs-lookup"><span data-stu-id="13f86-256">String</span></span>|<span data-ttu-id="13f86-257">[manageddevice](../resources/intune-devices-manageddevice.md)から継承されたデバイスカテゴリの表示名</span><span class="sxs-lookup"><span data-stu-id="13f86-257">Device category display name Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="13f86-258">isSupervised</span><span class="sxs-lookup"><span data-stu-id="13f86-258">isSupervised</span></span>|<span data-ttu-id="13f86-259">Boolean</span><span class="sxs-lookup"><span data-stu-id="13f86-259">Boolean</span></span>|<span data-ttu-id="13f86-260">[manageddevice](../resources/intune-devices-manageddevice.md)から継承されたデバイスの監視状態</span><span class="sxs-lookup"><span data-stu-id="13f86-260">Device supervised status Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="13f86-261">exchangeLastSuccessfulSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="13f86-261">exchangeLastSuccessfulSyncDateTime</span></span>|<span data-ttu-id="13f86-262">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="13f86-262">DateTimeOffset</span></span>|<span data-ttu-id="13f86-263">最後にデバイスが Exchange に接続した時刻。</span><span class="sxs-lookup"><span data-stu-id="13f86-263">Last time the device contacted Exchange.</span></span> <span data-ttu-id="13f86-264">[manageddevice](../resources/intune-devices-manageddevice.md)から継承します</span><span class="sxs-lookup"><span data-stu-id="13f86-264">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="13f86-265">exchangeAccessState</span><span class="sxs-lookup"><span data-stu-id="13f86-265">exchangeAccessState</span></span>|[<span data-ttu-id="13f86-266">devicemanagementexchangeaccessstate</span><span class="sxs-lookup"><span data-stu-id="13f86-266">deviceManagementExchangeAccessState</span></span>](../resources/intune-devices-devicemanagementexchangeaccessstate.md)|<span data-ttu-id="13f86-267">Exchange でのデバイスのアクセスの状態。</span><span class="sxs-lookup"><span data-stu-id="13f86-267">The Access State of the device in Exchange.</span></span> <span data-ttu-id="13f86-268">[manageddevice](../resources/intune-devices-manageddevice.md)から継承されます。</span><span class="sxs-lookup"><span data-stu-id="13f86-268">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="13f86-269">可能な値は、`none`、`unknown`、`allowed`、`blocked`、`quarantined` です。</span><span class="sxs-lookup"><span data-stu-id="13f86-269">Possible values are: `none`, `unknown`, `allowed`, `blocked`, `quarantined`.</span></span>|
|<span data-ttu-id="13f86-270">exchangeAccessStateReason</span><span class="sxs-lookup"><span data-stu-id="13f86-270">exchangeAccessStateReason</span></span>|[<span data-ttu-id="13f86-271">deviceManagementExchangeAccessStateReason</span><span class="sxs-lookup"><span data-stu-id="13f86-271">deviceManagementExchangeAccessStateReason</span></span>](../resources/intune-devices-devicemanagementexchangeaccessstatereason.md)|<span data-ttu-id="13f86-272">Exchange でのデバイスのアクセス状態の理由。
</span><span class="sxs-lookup"><span data-stu-id="13f86-272">The reason for the device's access state in Exchange.</span></span> <span data-ttu-id="13f86-273">[manageddevice](../resources/intune-devices-manageddevice.md)から継承されます。</span><span class="sxs-lookup"><span data-stu-id="13f86-273">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="13f86-274">可能な値は、`none`、`unknown`、`exchangeGlobalRule`、`exchangeIndividualRule`、`exchangeDeviceRule`、`exchangeUpgrade`、`exchangeMailboxPolicy`、`other`、`compliant`、`notCompliant`、`notEnrolled`、`unknownLocation`、`mfaRequired`、`azureADBlockDueToAccessPolicy`、`compromisedPassword`、`deviceNotKnownWithManagedApp` です。</span><span class="sxs-lookup"><span data-stu-id="13f86-274">Possible values are: `none`, `unknown`, `exchangeGlobalRule`, `exchangeIndividualRule`, `exchangeDeviceRule`, `exchangeUpgrade`, `exchangeMailboxPolicy`, `other`, `compliant`, `notCompliant`, `notEnrolled`, `unknownLocation`, `mfaRequired`, `azureADBlockDueToAccessPolicy`, `compromisedPassword`, `deviceNotKnownWithManagedApp`.</span></span>|
|<span data-ttu-id="13f86-275">remoteAssistanceSessionUrl</span><span class="sxs-lookup"><span data-stu-id="13f86-275">remoteAssistanceSessionUrl</span></span>|<span data-ttu-id="13f86-276">String</span><span class="sxs-lookup"><span data-stu-id="13f86-276">String</span></span>|<span data-ttu-id="13f86-277">デバイスとのリモート アシスタンス セッションを確立できるようにする URL。</span><span class="sxs-lookup"><span data-stu-id="13f86-277">Url that allows a Remote Assistance session to be established with the device.</span></span> <span data-ttu-id="13f86-278">[manageddevice](../resources/intune-devices-manageddevice.md)から継承します</span><span class="sxs-lookup"><span data-stu-id="13f86-278">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="13f86-279">remoteAssistanceSessionErrorDetails</span><span class="sxs-lookup"><span data-stu-id="13f86-279">remoteAssistanceSessionErrorDetails</span></span>|<span data-ttu-id="13f86-280">String</span><span class="sxs-lookup"><span data-stu-id="13f86-280">String</span></span>|<span data-ttu-id="13f86-281">リモート アシスタンス セッション オブジェクトの作成時に問題を識別するエラー文字列。</span><span class="sxs-lookup"><span data-stu-id="13f86-281">An error string that identifies issues when creating Remote Assistance session objects.</span></span> <span data-ttu-id="13f86-282">[manageddevice](../resources/intune-devices-manageddevice.md)から継承します</span><span class="sxs-lookup"><span data-stu-id="13f86-282">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="13f86-283">isEncrypted</span><span class="sxs-lookup"><span data-stu-id="13f86-283">isEncrypted</span></span>|<span data-ttu-id="13f86-284">Boolean</span><span class="sxs-lookup"><span data-stu-id="13f86-284">Boolean</span></span>|<span data-ttu-id="13f86-285">[manageddevice](../resources/intune-devices-manageddevice.md)から継承されたデバイスの暗号化状態</span><span class="sxs-lookup"><span data-stu-id="13f86-285">Device encryption status Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="13f86-286">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="13f86-286">userPrincipalName</span></span>|<span data-ttu-id="13f86-287">String</span><span class="sxs-lookup"><span data-stu-id="13f86-287">String</span></span>|<span data-ttu-id="13f86-288">[manageddevice](../resources/intune-devices-manageddevice.md)から継承されたデバイスユーザープリンシパル名</span><span class="sxs-lookup"><span data-stu-id="13f86-288">Device user principal name Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="13f86-289">model</span><span class="sxs-lookup"><span data-stu-id="13f86-289">model</span></span>|<span data-ttu-id="13f86-290">String</span><span class="sxs-lookup"><span data-stu-id="13f86-290">String</span></span>|<span data-ttu-id="13f86-291">[manageddevice](../resources/intune-devices-manageddevice.md)から継承されたデバイスのモデル</span><span class="sxs-lookup"><span data-stu-id="13f86-291">Model of the device Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="13f86-292">manufacturer</span><span class="sxs-lookup"><span data-stu-id="13f86-292">manufacturer</span></span>|<span data-ttu-id="13f86-293">String</span><span class="sxs-lookup"><span data-stu-id="13f86-293">String</span></span>|<span data-ttu-id="13f86-294">[manageddevice](../resources/intune-devices-manageddevice.md)から継承されたデバイスの製造元</span><span class="sxs-lookup"><span data-stu-id="13f86-294">Manufacturer of the device Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="13f86-295">imei</span><span class="sxs-lookup"><span data-stu-id="13f86-295">imei</span></span>|<span data-ttu-id="13f86-296">String</span><span class="sxs-lookup"><span data-stu-id="13f86-296">String</span></span>|<span data-ttu-id="13f86-297">[manageddevice](../resources/intune-devices-manageddevice.md)から継承された IMEI</span><span class="sxs-lookup"><span data-stu-id="13f86-297">IMEI Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="13f86-298">complianceGracePeriodExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="13f86-298">complianceGracePeriodExpirationDateTime</span></span>|<span data-ttu-id="13f86-299">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="13f86-299">DateTimeOffset</span></span>|<span data-ttu-id="13f86-300">デバイスコンプライアンスの猶予期間が[manageddevice](../resources/intune-devices-manageddevice.md)から継承される日時</span><span class="sxs-lookup"><span data-stu-id="13f86-300">The DateTime when device compliance grace period expires Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="13f86-301">シリアル番号</span><span class="sxs-lookup"><span data-stu-id="13f86-301">serialNumber</span></span>|<span data-ttu-id="13f86-302">String</span><span class="sxs-lookup"><span data-stu-id="13f86-302">String</span></span>|<span data-ttu-id="13f86-303">[manageddevice](../resources/intune-devices-manageddevice.md)から継承されたシリアル</span><span class="sxs-lookup"><span data-stu-id="13f86-303">SerialNumber Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="13f86-304">phoneNumber</span><span class="sxs-lookup"><span data-stu-id="13f86-304">phoneNumber</span></span>|<span data-ttu-id="13f86-305">String</span><span class="sxs-lookup"><span data-stu-id="13f86-305">String</span></span>|<span data-ttu-id="13f86-306">[manageddevice](../resources/intune-devices-manageddevice.md)から継承されたデバイスの電話番号</span><span class="sxs-lookup"><span data-stu-id="13f86-306">Phone number of the device Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="13f86-307">androidSecurityPatchLevel</span><span class="sxs-lookup"><span data-stu-id="13f86-307">androidSecurityPatchLevel</span></span>|<span data-ttu-id="13f86-308">String</span><span class="sxs-lookup"><span data-stu-id="13f86-308">String</span></span>|<span data-ttu-id="13f86-309">[manageddevice](../resources/intune-devices-manageddevice.md)から継承された Android セキュリティパッチレベル</span><span class="sxs-lookup"><span data-stu-id="13f86-309">Android security patch level Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="13f86-310">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="13f86-310">userDisplayName</span></span>|<span data-ttu-id="13f86-311">String</span><span class="sxs-lookup"><span data-stu-id="13f86-311">String</span></span>|<span data-ttu-id="13f86-312">[manageddevice](../resources/intune-devices-manageddevice.md)から継承されたユーザーの表示名</span><span class="sxs-lookup"><span data-stu-id="13f86-312">User display name Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="13f86-313">configurationManagerClientEnabledFeatures</span><span class="sxs-lookup"><span data-stu-id="13f86-313">configurationManagerClientEnabledFeatures</span></span>|[<span data-ttu-id="13f86-314">configurationManagerClientEnabledFeatures</span><span class="sxs-lookup"><span data-stu-id="13f86-314">configurationManagerClientEnabledFeatures</span></span>](../resources/intune-devices-configurationmanagerclientenabledfeatures.md)|<span data-ttu-id="13f86-315">[manageddevice](../resources/intune-devices-manageddevice.md)から継承された grmgr クライアントの有効な機能の設定</span><span class="sxs-lookup"><span data-stu-id="13f86-315">ConfigrMgr client enabled features Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="13f86-316">wiFiMacAddress</span><span class="sxs-lookup"><span data-stu-id="13f86-316">wiFiMacAddress</span></span>|<span data-ttu-id="13f86-317">String</span><span class="sxs-lookup"><span data-stu-id="13f86-317">String</span></span>|<span data-ttu-id="13f86-318">[manageddevice](../resources/intune-devices-manageddevice.md)から継承された wi-fi MAC</span><span class="sxs-lookup"><span data-stu-id="13f86-318">Wi-Fi MAC Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="13f86-319">deviceHealthAttestationState</span><span class="sxs-lookup"><span data-stu-id="13f86-319">deviceHealthAttestationState</span></span>|[<span data-ttu-id="13f86-320">deviceHealthAttestationState</span><span class="sxs-lookup"><span data-stu-id="13f86-320">deviceHealthAttestationState</span></span>](../resources/intune-devices-devicehealthattestationstate.md)|<span data-ttu-id="13f86-321">デバイスの正常性構成証明の状態。</span><span class="sxs-lookup"><span data-stu-id="13f86-321">The device health attestation state.</span></span> <span data-ttu-id="13f86-322">[manageddevice](../resources/intune-devices-manageddevice.md)から継承します</span><span class="sxs-lookup"><span data-stu-id="13f86-322">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="13f86-323">subscriberCarrier</span><span class="sxs-lookup"><span data-stu-id="13f86-323">subscriberCarrier</span></span>|<span data-ttu-id="13f86-324">String</span><span class="sxs-lookup"><span data-stu-id="13f86-324">String</span></span>|<span data-ttu-id="13f86-325">[manageddevice](../resources/intune-devices-manageddevice.md)から継承されたサブスクライバーキャリア</span><span class="sxs-lookup"><span data-stu-id="13f86-325">Subscriber Carrier Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="13f86-326">meid</span><span class="sxs-lookup"><span data-stu-id="13f86-326">meid</span></span>|<span data-ttu-id="13f86-327">String</span><span class="sxs-lookup"><span data-stu-id="13f86-327">String</span></span>|<span data-ttu-id="13f86-328">[manageddevice](../resources/intune-devices-manageddevice.md)から継承された meid</span><span class="sxs-lookup"><span data-stu-id="13f86-328">MEID Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="13f86-329">totalStorageSpaceInBytes</span><span class="sxs-lookup"><span data-stu-id="13f86-329">totalStorageSpaceInBytes</span></span>|<span data-ttu-id="13f86-330">Int64</span><span class="sxs-lookup"><span data-stu-id="13f86-330">Int64</span></span>|<span data-ttu-id="13f86-331">[manageddevice](../resources/intune-devices-manageddevice.md)から継承された合計記憶域 (バイト)</span><span class="sxs-lookup"><span data-stu-id="13f86-331">Total Storage in Bytes Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="13f86-332">freeStorageSpaceInBytes</span><span class="sxs-lookup"><span data-stu-id="13f86-332">freeStorageSpaceInBytes</span></span>|<span data-ttu-id="13f86-333">Int64</span><span class="sxs-lookup"><span data-stu-id="13f86-333">Int64</span></span>|<span data-ttu-id="13f86-334">[manageddevice](../resources/intune-devices-manageddevice.md)から継承された空き記憶域 (バイト単位)</span><span class="sxs-lookup"><span data-stu-id="13f86-334">Free Storage in Bytes Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="13f86-335">managedDeviceName</span><span class="sxs-lookup"><span data-stu-id="13f86-335">managedDeviceName</span></span>|<span data-ttu-id="13f86-336">String</span><span class="sxs-lookup"><span data-stu-id="13f86-336">String</span></span>|<span data-ttu-id="13f86-337">デバイスを識別する名前が自動的に生成されます。</span><span class="sxs-lookup"><span data-stu-id="13f86-337">Automatically generated name to identify a device.</span></span> <span data-ttu-id="13f86-338">ユーザー フレンドリ名に上書きできます。</span><span class="sxs-lookup"><span data-stu-id="13f86-338">Can be overwritten to a user friendly name.</span></span> <span data-ttu-id="13f86-339">[manageddevice](../resources/intune-devices-manageddevice.md)から継承します</span><span class="sxs-lookup"><span data-stu-id="13f86-339">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="13f86-340">partnerReportedThreatState</span><span class="sxs-lookup"><span data-stu-id="13f86-340">partnerReportedThreatState</span></span>|[<span data-ttu-id="13f86-341">manageddevicepartnerreportedhealthstate</span><span class="sxs-lookup"><span data-stu-id="13f86-341">managedDevicePartnerReportedHealthState</span></span>](../resources/intune-devices-manageddevicepartnerreportedhealthstate.md)|<span data-ttu-id="13f86-342">Mobile Threat Defense パートナーがアカウントおよびデバイスで使用されている場合の、デバイスの脅威の状態を示します。</span><span class="sxs-lookup"><span data-stu-id="13f86-342">Indicates the threat state of a device when a Mobile Threat Defense partner is in use by the account and device.</span></span> <span data-ttu-id="13f86-343">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="13f86-343">Read Only.</span></span> <span data-ttu-id="13f86-344">[manageddevice](../resources/intune-devices-manageddevice.md)から継承されます。</span><span class="sxs-lookup"><span data-stu-id="13f86-344">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="13f86-345">可能な値は、`unknown`、`activated`、`deactivated`、`secured`、`lowSeverity`、`mediumSeverity`、`highSeverity`、`unresponsive`、`compromised`、`misconfigured` です。</span><span class="sxs-lookup"><span data-stu-id="13f86-345">Possible values are: `unknown`, `activated`, `deactivated`, `secured`, `lowSeverity`, `mediumSeverity`, `highSeverity`, `unresponsive`, `compromised`, `misconfigured`.</span></span>|
|<span data-ttu-id="13f86-346">usersLoggedOn</span><span class="sxs-lookup"><span data-stu-id="13f86-346">usersLoggedOn</span></span>|<span data-ttu-id="13f86-347">[loggedOnUser](../resources/intune-devices-loggedonuser.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="13f86-347">[loggedOnUser](../resources/intune-devices-loggedonuser.md) collection</span></span>|<span data-ttu-id="13f86-348">[manageddevice](../resources/intune-devices-manageddevice.md)から継承されたデバイスの最後にログオンしたユーザーを示します</span><span class="sxs-lookup"><span data-stu-id="13f86-348">Indicates the last logged on users of a device Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="13f86-349">preferMdmOverGroupPolicyAppliedDateTime</span><span class="sxs-lookup"><span data-stu-id="13f86-349">preferMdmOverGroupPolicyAppliedDateTime</span></span>|<span data-ttu-id="13f86-350">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="13f86-350">DateTimeOffset</span></span>|<span data-ttu-id="13f86-351">preferMdmOverGroupPolicy の設定が設定された DateTime を報告します。</span><span class="sxs-lookup"><span data-stu-id="13f86-351">Reports the DateTime the preferMdmOverGroupPolicy setting was set.</span></span>  <span data-ttu-id="13f86-352">設定すると、競合がある場合に Intune MDM 設定がグループポリシー設定を上書きします。</span><span class="sxs-lookup"><span data-stu-id="13f86-352">When set, the Intune MDM settings will override Group Policy settings if there is a conflict.</span></span> <span data-ttu-id="13f86-353">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="13f86-353">Read Only.</span></span> <span data-ttu-id="13f86-354">[manageddevice](../resources/intune-devices-manageddevice.md)から継承します</span><span class="sxs-lookup"><span data-stu-id="13f86-354">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="13f86-355">autopilotEnrolled</span><span class="sxs-lookup"><span data-stu-id="13f86-355">autopilotEnrolled</span></span>|<span data-ttu-id="13f86-356">Boolean</span><span class="sxs-lookup"><span data-stu-id="13f86-356">Boolean</span></span>|<span data-ttu-id="13f86-357">管理対象デバイスが自動パイロットで登録されているかどうかを報告します。</span><span class="sxs-lookup"><span data-stu-id="13f86-357">Reports if the managed device is enrolled via auto-pilot.</span></span> <span data-ttu-id="13f86-358">[manageddevice](../resources/intune-devices-manageddevice.md)から継承します</span><span class="sxs-lookup"><span data-stu-id="13f86-358">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="13f86-359">requireUserEnrollmentApproval</span><span class="sxs-lookup"><span data-stu-id="13f86-359">requireUserEnrollmentApproval</span></span>|<span data-ttu-id="13f86-360">Boolean</span><span class="sxs-lookup"><span data-stu-id="13f86-360">Boolean</span></span>|<span data-ttu-id="13f86-361">管理対象 iOS デバイスがユーザー承認登録であるかどうかを報告します。</span><span class="sxs-lookup"><span data-stu-id="13f86-361">Reports if the managed iOS device is user approval enrollment.</span></span> <span data-ttu-id="13f86-362">[manageddevice](../resources/intune-devices-manageddevice.md)から継承します</span><span class="sxs-lookup"><span data-stu-id="13f86-362">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="13f86-363">managementCertificateExpirationDate</span><span class="sxs-lookup"><span data-stu-id="13f86-363">managementCertificateExpirationDate</span></span>|<span data-ttu-id="13f86-364">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="13f86-364">DateTimeOffset</span></span>|<span data-ttu-id="13f86-365">[manageddevice](../resources/intune-devices-manageddevice.md)から継承されたデバイス管理証明書の有効期限日を報告します</span><span class="sxs-lookup"><span data-stu-id="13f86-365">Reports device management certificate expiration date Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="13f86-366">iccid</span><span class="sxs-lookup"><span data-stu-id="13f86-366">iccid</span></span>|<span data-ttu-id="13f86-367">String</span><span class="sxs-lookup"><span data-stu-id="13f86-367">String</span></span>|<span data-ttu-id="13f86-368">ic カード識別子。 SIM カードの一意の識別番号です。</span><span class="sxs-lookup"><span data-stu-id="13f86-368">Integrated Circuit Card Identifier, it is A SIM card's unique identification number.</span></span> <span data-ttu-id="13f86-369">[manageddevice](../resources/intune-devices-manageddevice.md)から継承します</span><span class="sxs-lookup"><span data-stu-id="13f86-369">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="13f86-370">udid</span><span class="sxs-lookup"><span data-stu-id="13f86-370">udid</span></span>|<span data-ttu-id="13f86-371">String</span><span class="sxs-lookup"><span data-stu-id="13f86-371">String</span></span>|<span data-ttu-id="13f86-372">iOS および macOS デバイスの一意のデバイス識別子。</span><span class="sxs-lookup"><span data-stu-id="13f86-372">Unique Device Identifier for iOS and macOS devices.</span></span> <span data-ttu-id="13f86-373">[manageddevice](../resources/intune-devices-manageddevice.md)から継承します</span><span class="sxs-lookup"><span data-stu-id="13f86-373">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="13f86-374">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="13f86-374">roleScopeTagIds</span></span>|<span data-ttu-id="13f86-375">String collection</span><span class="sxs-lookup"><span data-stu-id="13f86-375">String collection</span></span>|<span data-ttu-id="13f86-376">このデバイスインスタンスの範囲タグ id のリスト。</span><span class="sxs-lookup"><span data-stu-id="13f86-376">List of Scope Tag IDs for this Device instance.</span></span> <span data-ttu-id="13f86-377">[manageddevice](../resources/intune-devices-manageddevice.md)から継承します</span><span class="sxs-lookup"><span data-stu-id="13f86-377">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="13f86-378">windowsactivemalwarecount 再計算</span><span class="sxs-lookup"><span data-stu-id="13f86-378">windowsActiveMalwareCount</span></span>|<span data-ttu-id="13f86-379">Int32</span><span class="sxs-lookup"><span data-stu-id="13f86-379">Int32</span></span>|<span data-ttu-id="13f86-380">[manageddevice](../resources/intune-devices-manageddevice.md)から継承された、この windows デバイスのアクティブなマルウェアの数</span><span class="sxs-lookup"><span data-stu-id="13f86-380">Count of active malware for this windows device Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="13f86-381">windowsRemediatedMalwareCount</span><span class="sxs-lookup"><span data-stu-id="13f86-381">windowsRemediatedMalwareCount</span></span>|<span data-ttu-id="13f86-382">Int32</span><span class="sxs-lookup"><span data-stu-id="13f86-382">Int32</span></span>|<span data-ttu-id="13f86-383">[manageddevice](../resources/intune-devices-manageddevice.md)から継承された、この windows デバイスの修復されたマルウェアの数</span><span class="sxs-lookup"><span data-stu-id="13f86-383">Count of remediated malware for this windows device Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="13f86-384">notes</span><span class="sxs-lookup"><span data-stu-id="13f86-384">notes</span></span>|<span data-ttu-id="13f86-385">String</span><span class="sxs-lookup"><span data-stu-id="13f86-385">String</span></span>|<span data-ttu-id="13f86-386">IT 管理者によって作成された、 [manageddevice](../resources/intune-devices-manageddevice.md)から継承したデバイス上のメモ</span><span class="sxs-lookup"><span data-stu-id="13f86-386">Notes on the device created by IT Admin Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="13f86-387">configurationManagerClientHealthState</span><span class="sxs-lookup"><span data-stu-id="13f86-387">configurationManagerClientHealthState</span></span>|[<span data-ttu-id="13f86-388">configurationManagerClientHealthState</span><span class="sxs-lookup"><span data-stu-id="13f86-388">configurationManagerClientHealthState</span></span>](../resources/intune-devices-configurationmanagerclienthealthstate.md)|<span data-ttu-id="13f86-389">構成マネージャークライアントの正常性状態。 MDM/ConfigMgr エージェントによって管理されているデバイスに対してのみ有効。 [manageddevice](../resources/intune-devices-manageddevice.md)から継承されます。</span><span class="sxs-lookup"><span data-stu-id="13f86-389">Configuration manager client health state, valid only for devices managed by MDM/ConfigMgr Agent Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|



## <a name="response"></a><span data-ttu-id="13f86-390">応答</span><span class="sxs-lookup"><span data-stu-id="13f86-390">Response</span></span>
<span data-ttu-id="13f86-391">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で更新された[windowsmanageddevice](../resources/intune-devices-windowsmanageddevice.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="13f86-391">If successful, this method returns a `200 OK` response code and an updated [windowsManagedDevice](../resources/intune-devices-windowsmanageddevice.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="13f86-392">例</span><span class="sxs-lookup"><span data-stu-id="13f86-392">Example</span></span>

### <a name="request"></a><span data-ttu-id="13f86-393">要求</span><span class="sxs-lookup"><span data-stu-id="13f86-393">Request</span></span>
<span data-ttu-id="13f86-394">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="13f86-394">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/users/{usersId}/managedDevices/{managedDeviceId}
Content-type: application/json
Content-length: 7231

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

### <a name="response"></a><span data-ttu-id="13f86-395">応答</span><span class="sxs-lookup"><span data-stu-id="13f86-395">Response</span></span>
<span data-ttu-id="13f86-p141">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="13f86-p141">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 7280

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




