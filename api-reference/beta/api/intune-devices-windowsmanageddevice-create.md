---
title: windowsmanageddevice の作成
description: 新しい windowsmanageddevice オブジェクトを作成します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 2d2860a5e982e9079356df81b527a0cf9d02f6f7
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/21/2019
ms.locfileid: "30161146"
---
# <a name="create-windowsmanageddevice"></a><span data-ttu-id="62d59-103">windowsmanageddevice の作成</span><span class="sxs-lookup"><span data-stu-id="62d59-103">Create windowsManagedDevice</span></span>

> <span data-ttu-id="62d59-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="62d59-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="62d59-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="62d59-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="62d59-106">新しい[windowsmanageddevice](../resources/intune-devices-windowsmanageddevice.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="62d59-106">Create a new [windowsManagedDevice](../resources/intune-devices-windowsmanageddevice.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="62d59-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="62d59-107">Prerequisites</span></span>
<span data-ttu-id="62d59-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/concepts/permissions-reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="62d59-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="62d59-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="62d59-110">Permission type</span></span>|<span data-ttu-id="62d59-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="62d59-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="62d59-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="62d59-112">Delegated (work or school account)</span></span>|<span data-ttu-id="62d59-113">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="62d59-113">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="62d59-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="62d59-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="62d59-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="62d59-115">Not supported.</span></span>|
|<span data-ttu-id="62d59-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="62d59-116">Application</span></span>|<span data-ttu-id="62d59-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="62d59-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="62d59-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="62d59-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /users/{usersId}/managedDevices
POST /deviceManagement/managedDevices
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/detectedApps/{detectedAppId}/managedDevices
```

## <a name="request-headers"></a><span data-ttu-id="62d59-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="62d59-119">Request headers</span></span>
|<span data-ttu-id="62d59-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="62d59-120">Header</span></span>|<span data-ttu-id="62d59-121">値</span><span class="sxs-lookup"><span data-stu-id="62d59-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="62d59-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="62d59-122">Authorization</span></span>|<span data-ttu-id="62d59-123">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="62d59-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="62d59-124">承諾</span><span class="sxs-lookup"><span data-stu-id="62d59-124">Accept</span></span>|<span data-ttu-id="62d59-125">application/json</span><span class="sxs-lookup"><span data-stu-id="62d59-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="62d59-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="62d59-126">Request body</span></span>
<span data-ttu-id="62d59-127">要求本文で、windowsmanageddevice オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="62d59-127">In the request body, supply a JSON representation for the windowsManagedDevice object.</span></span>

<span data-ttu-id="62d59-128">次の表に、windowsmanageddevice の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="62d59-128">The following table shows the properties that are required when you create the windowsManagedDevice.</span></span>

|<span data-ttu-id="62d59-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="62d59-129">Property</span></span>|<span data-ttu-id="62d59-130">型</span><span class="sxs-lookup"><span data-stu-id="62d59-130">Type</span></span>|<span data-ttu-id="62d59-131">説明</span><span class="sxs-lookup"><span data-stu-id="62d59-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="62d59-132">id</span><span class="sxs-lookup"><span data-stu-id="62d59-132">id</span></span>|<span data-ttu-id="62d59-133">String</span><span class="sxs-lookup"><span data-stu-id="62d59-133">String</span></span>|<span data-ttu-id="62d59-134">[manageddevice](../resources/intune-devices-manageddevice.md)から継承されたデバイスの一意識別子</span><span class="sxs-lookup"><span data-stu-id="62d59-134">Unique Identifier for the device Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="62d59-135">userId</span><span class="sxs-lookup"><span data-stu-id="62d59-135">userId</span></span>|<span data-ttu-id="62d59-136">String</span><span class="sxs-lookup"><span data-stu-id="62d59-136">String</span></span>|<span data-ttu-id="62d59-137">[manageddevice](../resources/intune-devices-manageddevice.md)から継承したデバイスに関連付けられているユーザーの一意識別子</span><span class="sxs-lookup"><span data-stu-id="62d59-137">Unique Identifier for the user associated with the device Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="62d59-138">deviceName</span><span class="sxs-lookup"><span data-stu-id="62d59-138">deviceName</span></span>|<span data-ttu-id="62d59-139">String</span><span class="sxs-lookup"><span data-stu-id="62d59-139">String</span></span>|<span data-ttu-id="62d59-140">[manageddevice](../resources/intune-devices-manageddevice.md)から継承されたデバイスの名前</span><span class="sxs-lookup"><span data-stu-id="62d59-140">Name of the device Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="62d59-141">hardwareInformation</span><span class="sxs-lookup"><span data-stu-id="62d59-141">hardwareInformation</span></span>|[<span data-ttu-id="62d59-142">hardwareInformation</span><span class="sxs-lookup"><span data-stu-id="62d59-142">hardwareInformation</span></span>](../resources/intune-devices-hardwareinformation.md)|<span data-ttu-id="62d59-143">デバイスのハードワードの詳細。</span><span class="sxs-lookup"><span data-stu-id="62d59-143">The hardward details for the device.</span></span>  <span data-ttu-id="62d59-144">記憶領域、製造元、シリアル番号などの情報が含まれます。[manageddevice](../resources/intune-devices-manageddevice.md)から継承します</span><span class="sxs-lookup"><span data-stu-id="62d59-144">Includes information such as storage space, manufacturer, serial number, etc. Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="62d59-145">ownerType</span><span class="sxs-lookup"><span data-stu-id="62d59-145">ownerType</span></span>|[<span data-ttu-id="62d59-146">ownerType</span><span class="sxs-lookup"><span data-stu-id="62d59-146">ownerType</span></span>](../resources/intune-devices-ownertype.md)|<span data-ttu-id="62d59-147">デバイスの所有権。</span><span class="sxs-lookup"><span data-stu-id="62d59-147">Ownership of the device.</span></span> <span data-ttu-id="62d59-148">' company ' または ' personal ' を[manageddevice](../resources/intune-devices-manageddevice.md)から継承することができます。</span><span class="sxs-lookup"><span data-stu-id="62d59-148">Can be 'company' or 'personal' Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="62d59-149">可能な値は `unknown`、`company`、`personal` です。</span><span class="sxs-lookup"><span data-stu-id="62d59-149">Possible values are: `unknown`, `company`, `personal`.</span></span>|
|<span data-ttu-id="62d59-150">managedDeviceOwnerType</span><span class="sxs-lookup"><span data-stu-id="62d59-150">managedDeviceOwnerType</span></span>|[<span data-ttu-id="62d59-151">managedDeviceOwnerType</span><span class="sxs-lookup"><span data-stu-id="62d59-151">managedDeviceOwnerType</span></span>](../resources/intune-devices-manageddeviceownertype.md)|<span data-ttu-id="62d59-152">デバイスの所有権。</span><span class="sxs-lookup"><span data-stu-id="62d59-152">Ownership of the device.</span></span> <span data-ttu-id="62d59-153">' company ' または ' personal ' を[manageddevice](../resources/intune-devices-manageddevice.md)から継承することができます。</span><span class="sxs-lookup"><span data-stu-id="62d59-153">Can be 'company' or 'personal' Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="62d59-154">可能な値は `unknown`、`company`、`personal` です。</span><span class="sxs-lookup"><span data-stu-id="62d59-154">Possible values are: `unknown`, `company`, `personal`.</span></span>|
|<span data-ttu-id="62d59-155">deviceActionResults</span><span class="sxs-lookup"><span data-stu-id="62d59-155">deviceActionResults</span></span>|<span data-ttu-id="62d59-156">[deviceActionResult](../resources/intune-devices-deviceactionresult.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="62d59-156">[deviceActionResult](../resources/intune-devices-deviceactionresult.md) collection</span></span>|<span data-ttu-id="62d59-157">ComplexType deviceActionResult オブジェクトのリスト。</span><span class="sxs-lookup"><span data-stu-id="62d59-157">List of ComplexType deviceActionResult objects.</span></span> <span data-ttu-id="62d59-158">[manageddevice](../resources/intune-devices-manageddevice.md)から継承します</span><span class="sxs-lookup"><span data-stu-id="62d59-158">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="62d59-159">managementstate</span><span class="sxs-lookup"><span data-stu-id="62d59-159">managementState</span></span>|[<span data-ttu-id="62d59-160">managementstate</span><span class="sxs-lookup"><span data-stu-id="62d59-160">managementState</span></span>](../resources/intune-devices-managementstate.md)|<span data-ttu-id="62d59-161">デバイスの管理状態。</span><span class="sxs-lookup"><span data-stu-id="62d59-161">Management state of the device.</span></span> <span data-ttu-id="62d59-162">[manageddevice](../resources/intune-devices-manageddevice.md)から継承されます。</span><span class="sxs-lookup"><span data-stu-id="62d59-162">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="62d59-163">可能な値は、`managed`、`retirePending`、`retireFailed`、`wipePending`、`wipeFailed`、`unhealthy`、`deletePending`、`retireIssued`、`wipeIssued`、`wipeCanceled`、`retireCanceled`、`discovered` です。</span><span class="sxs-lookup"><span data-stu-id="62d59-163">Possible values are: `managed`, `retirePending`, `retireFailed`, `wipePending`, `wipeFailed`, `unhealthy`, `deletePending`, `retireIssued`, `wipeIssued`, `wipeCanceled`, `retireCanceled`, `discovered`.</span></span>|
|<span data-ttu-id="62d59-164">enrolledDateTime</span><span class="sxs-lookup"><span data-stu-id="62d59-164">enrolledDateTime</span></span>|<span data-ttu-id="62d59-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="62d59-165">DateTimeOffset</span></span>|<span data-ttu-id="62d59-166">デバイスの登録時刻。</span><span class="sxs-lookup"><span data-stu-id="62d59-166">Enrollment time of the device.</span></span> <span data-ttu-id="62d59-167">[manageddevice](../resources/intune-devices-manageddevice.md)から継承します</span><span class="sxs-lookup"><span data-stu-id="62d59-167">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="62d59-168">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="62d59-168">lastSyncDateTime</span></span>|<span data-ttu-id="62d59-169">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="62d59-169">DateTimeOffset</span></span>|<span data-ttu-id="62d59-170">デバイスが Intune との正常な同期を最終的に完了した日時。</span><span class="sxs-lookup"><span data-stu-id="62d59-170">The date and time that the device last completed a successful sync with Intune.</span></span> <span data-ttu-id="62d59-171">[manageddevice](../resources/intune-devices-manageddevice.md)から継承します</span><span class="sxs-lookup"><span data-stu-id="62d59-171">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="62d59-172">chassisType</span><span class="sxs-lookup"><span data-stu-id="62d59-172">chassisType</span></span>|[<span data-ttu-id="62d59-173">chassisType</span><span class="sxs-lookup"><span data-stu-id="62d59-173">chassisType</span></span>](../resources/intune-devices-chassistype.md)|<span data-ttu-id="62d59-174">デバイスのシャーシの種類。</span><span class="sxs-lookup"><span data-stu-id="62d59-174">Chassis type of the device.</span></span> <span data-ttu-id="62d59-175">[manageddevice](../resources/intune-devices-manageddevice.md)から継承されます。</span><span class="sxs-lookup"><span data-stu-id="62d59-175">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="62d59-176">可能な値は、`unknown`、`desktop`、`laptop`、`worksWorkstation`、`enterpriseServer`、`phone`、`tablet`、`mobileOther`、`mobileUnknown` です。</span><span class="sxs-lookup"><span data-stu-id="62d59-176">Possible values are: `unknown`, `desktop`, `laptop`, `worksWorkstation`, `enterpriseServer`, `phone`, `tablet`, `mobileOther`, `mobileUnknown`.</span></span>|
|<span data-ttu-id="62d59-177">operatingSystem</span><span class="sxs-lookup"><span data-stu-id="62d59-177">operatingSystem</span></span>|<span data-ttu-id="62d59-178">文字列</span><span class="sxs-lookup"><span data-stu-id="62d59-178">String</span></span>|<span data-ttu-id="62d59-179">デバイスのオペレーティング システム。</span><span class="sxs-lookup"><span data-stu-id="62d59-179">Operating system of the device.</span></span> <span data-ttu-id="62d59-180">Windows、iOS など[manageddevice](../resources/intune-devices-manageddevice.md)から継承します</span><span class="sxs-lookup"><span data-stu-id="62d59-180">Windows, iOS, etc. Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="62d59-181">deviceType</span><span class="sxs-lookup"><span data-stu-id="62d59-181">deviceType</span></span>|[<span data-ttu-id="62d59-182">deviceType</span><span class="sxs-lookup"><span data-stu-id="62d59-182">deviceType</span></span>](../resources/intune-shared-devicetype.md)|<span data-ttu-id="62d59-183">デバイスのプラットフォーム。</span><span class="sxs-lookup"><span data-stu-id="62d59-183">Platform of the device.</span></span> <span data-ttu-id="62d59-184">[manageddevice](../resources/intune-devices-manageddevice.md)から継承されます。</span><span class="sxs-lookup"><span data-stu-id="62d59-184">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="62d59-185">可能な値: `desktop`、 `windowsRT` `winMO6` `nokia` `windowsPhone` `mac` `winCE` `winEmbedded` `iPhone` `iPad` `iPod` `android`、、、、、、、、、、、、 `iSocConsumer` `unix` `macMDM` `holoLens` `surfaceHub` `androidForWork` `androidEnterprise`, `blackberry`, `palm`, `unknown`.</span><span class="sxs-lookup"><span data-stu-id="62d59-185">Possible values are: `desktop`, `windowsRT`, `winMO6`, `nokia`, `windowsPhone`, `mac`, `winCE`, `winEmbedded`, `iPhone`, `iPad`, `iPod`, `android`, `iSocConsumer`, `unix`, `macMDM`, `holoLens`, `surfaceHub`, `androidForWork`, `androidEnterprise`, `blackberry`, `palm`, `unknown`.</span></span>|
|<span data-ttu-id="62d59-186">complianceState</span><span class="sxs-lookup"><span data-stu-id="62d59-186">complianceState</span></span>|[<span data-ttu-id="62d59-187">complianceState</span><span class="sxs-lookup"><span data-stu-id="62d59-187">complianceState</span></span>](../resources/intune-devices-compliancestate.md)|<span data-ttu-id="62d59-188">デバイスのコンプライアンス状態。</span><span class="sxs-lookup"><span data-stu-id="62d59-188">Compliance state of the device.</span></span> <span data-ttu-id="62d59-189">[manageddevice](../resources/intune-devices-manageddevice.md)から継承されます。</span><span class="sxs-lookup"><span data-stu-id="62d59-189">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="62d59-190">可能な値は、`unknown`、`compliant`、`noncompliant`、`conflict`、`error`、`inGracePeriod`、`configManager` です。</span><span class="sxs-lookup"><span data-stu-id="62d59-190">Possible values are: `unknown`, `compliant`, `noncompliant`, `conflict`, `error`, `inGracePeriod`, `configManager`.</span></span>|
|<span data-ttu-id="62d59-191">jailBroken</span><span class="sxs-lookup"><span data-stu-id="62d59-191">jailBroken</span></span>|<span data-ttu-id="62d59-192">String</span><span class="sxs-lookup"><span data-stu-id="62d59-192">String</span></span>|<span data-ttu-id="62d59-193">デバイスが脱獄またはルート化されているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="62d59-193">whether the device is jail broken or rooted.</span></span> <span data-ttu-id="62d59-194">[manageddevice](../resources/intune-devices-manageddevice.md)から継承します</span><span class="sxs-lookup"><span data-stu-id="62d59-194">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="62d59-195">managementAgent</span><span class="sxs-lookup"><span data-stu-id="62d59-195">managementAgent</span></span>|[<span data-ttu-id="62d59-196">managementagenttype</span><span class="sxs-lookup"><span data-stu-id="62d59-196">managementAgentType</span></span>](../resources/intune-devices-managementagenttype.md)|<span data-ttu-id="62d59-197">デバイスの管理チャネル。</span><span class="sxs-lookup"><span data-stu-id="62d59-197">Management channel of the device.</span></span> <span data-ttu-id="62d59-198">Intune、EAS など。[manageddevice](../resources/intune-devices-manageddevice.md)から継承されます。</span><span class="sxs-lookup"><span data-stu-id="62d59-198">Intune, EAS, etc. Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="62d59-199">可能な値は、`eas`、`mdm`、`easMdm`、`intuneClient`、`easIntuneClient`、`configurationManagerClient`、`configurationManagerClientMdm`、`configurationManagerClientMdmEas`、`unknown`、`jamf`、`googleCloudDevicePolicyController`、`microsoft365ManagedMdm` です。</span><span class="sxs-lookup"><span data-stu-id="62d59-199">Possible values are: `eas`, `mdm`, `easMdm`, `intuneClient`, `easIntuneClient`, `configurationManagerClient`, `configurationManagerClientMdm`, `configurationManagerClientMdmEas`, `unknown`, `jamf`, `googleCloudDevicePolicyController`, `microsoft365ManagedMdm`.</span></span>|
|<span data-ttu-id="62d59-200">osVersion</span><span class="sxs-lookup"><span data-stu-id="62d59-200">osVersion</span></span>|<span data-ttu-id="62d59-201">String</span><span class="sxs-lookup"><span data-stu-id="62d59-201">String</span></span>|<span data-ttu-id="62d59-202">デバイスのオペレーティング システムのバージョン。</span><span class="sxs-lookup"><span data-stu-id="62d59-202">Operating system version of the device.</span></span> <span data-ttu-id="62d59-203">[manageddevice](../resources/intune-devices-manageddevice.md)から継承します</span><span class="sxs-lookup"><span data-stu-id="62d59-203">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="62d59-204">easActivated</span><span class="sxs-lookup"><span data-stu-id="62d59-204">easActivated</span></span>|<span data-ttu-id="62d59-205">ブール値</span><span class="sxs-lookup"><span data-stu-id="62d59-205">Boolean</span></span>|<span data-ttu-id="62d59-206">Exchange ActiveSync がアクティブになっているデバイスかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="62d59-206">Whether the device is Exchange ActiveSync activated.</span></span> <span data-ttu-id="62d59-207">[manageddevice](../resources/intune-devices-manageddevice.md)から継承します</span><span class="sxs-lookup"><span data-stu-id="62d59-207">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="62d59-208">easDeviceId</span><span class="sxs-lookup"><span data-stu-id="62d59-208">easDeviceId</span></span>|<span data-ttu-id="62d59-209">String</span><span class="sxs-lookup"><span data-stu-id="62d59-209">String</span></span>|<span data-ttu-id="62d59-210">デバイスの Exchange ActiveSync の ID。</span><span class="sxs-lookup"><span data-stu-id="62d59-210">Exchange ActiveSync Id of the device.</span></span> <span data-ttu-id="62d59-211">[manageddevice](../resources/intune-devices-manageddevice.md)から継承します</span><span class="sxs-lookup"><span data-stu-id="62d59-211">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="62d59-212">easActivationDateTime</span><span class="sxs-lookup"><span data-stu-id="62d59-212">easActivationDateTime</span></span>|<span data-ttu-id="62d59-213">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="62d59-213">DateTimeOffset</span></span>|<span data-ttu-id="62d59-214">デバイスの Exchange ActivationSync のアクティブ化の時刻。</span><span class="sxs-lookup"><span data-stu-id="62d59-214">Exchange ActivationSync activation time of the device.</span></span> <span data-ttu-id="62d59-215">[manageddevice](../resources/intune-devices-manageddevice.md)から継承します</span><span class="sxs-lookup"><span data-stu-id="62d59-215">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="62d59-216">aadRegistered</span><span class="sxs-lookup"><span data-stu-id="62d59-216">aadRegistered</span></span>|<span data-ttu-id="62d59-217">Boolean</span><span class="sxs-lookup"><span data-stu-id="62d59-217">Boolean</span></span>|<span data-ttu-id="62d59-218">Azure Active Directory が登録されているデバイスかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="62d59-218">Whether the device is Azure Active Directory registered.</span></span> <span data-ttu-id="62d59-219">[manageddevice](../resources/intune-devices-manageddevice.md)から継承します</span><span class="sxs-lookup"><span data-stu-id="62d59-219">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="62d59-220">azureADRegistered</span><span class="sxs-lookup"><span data-stu-id="62d59-220">azureADRegistered</span></span>|<span data-ttu-id="62d59-221">Boolean</span><span class="sxs-lookup"><span data-stu-id="62d59-221">Boolean</span></span>|<span data-ttu-id="62d59-222">Azure Active Directory が登録されているデバイスかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="62d59-222">Whether the device is Azure Active Directory registered.</span></span> <span data-ttu-id="62d59-223">[manageddevice](../resources/intune-devices-manageddevice.md)から継承します</span><span class="sxs-lookup"><span data-stu-id="62d59-223">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="62d59-224">deviceEnrollmentType</span><span class="sxs-lookup"><span data-stu-id="62d59-224">deviceEnrollmentType</span></span>|[<span data-ttu-id="62d59-225">deviceEnrollmentType</span><span class="sxs-lookup"><span data-stu-id="62d59-225">deviceEnrollmentType</span></span>](../resources/intune-shared-deviceenrollmenttype.md)|<span data-ttu-id="62d59-226">デバイスの登録の種類。</span><span class="sxs-lookup"><span data-stu-id="62d59-226">Enrollment type of the device.</span></span> <span data-ttu-id="62d59-227">[manageddevice](../resources/intune-devices-manageddevice.md)から継承されます。</span><span class="sxs-lookup"><span data-stu-id="62d59-227">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="62d59-228">可能な値は、`unknown`、`userEnrollment`、`deviceEnrollmentManager`、`appleBulkWithUser`、`appleBulkWithoutUser`、`windowsAzureADJoin`、`windowsBulkUserless`、`windowsAutoEnrollment`、`windowsBulkAzureDomainJoin`、`windowsCoManagement` です。</span><span class="sxs-lookup"><span data-stu-id="62d59-228">Possible values are: `unknown`, `userEnrollment`, `deviceEnrollmentManager`, `appleBulkWithUser`, `appleBulkWithoutUser`, `windowsAzureADJoin`, `windowsBulkUserless`, `windowsAutoEnrollment`, `windowsBulkAzureDomainJoin`, `windowsCoManagement`.</span></span>|
|<span data-ttu-id="62d59-229">lostModeState</span><span class="sxs-lookup"><span data-stu-id="62d59-229">lostModeState</span></span>|[<span data-ttu-id="62d59-230">lostModeState</span><span class="sxs-lookup"><span data-stu-id="62d59-230">lostModeState</span></span>](../resources/intune-devices-lostmodestate.md)|<span data-ttu-id="62d59-231">失われたモードが有効になっているか、 [manageddevice](../resources/intune-devices-manageddevice.md)から継承が無効かどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="62d59-231">Indicates if Lost mode is enabled or disabled Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="62d59-232">使用可能な値は、`disabled`、`enabled` です。</span><span class="sxs-lookup"><span data-stu-id="62d59-232">Possible values are: `disabled`, `enabled`.</span></span>|
|<span data-ttu-id="62d59-233">activationLockBypassCode</span><span class="sxs-lookup"><span data-stu-id="62d59-233">activationLockBypassCode</span></span>|<span data-ttu-id="62d59-234">String</span><span class="sxs-lookup"><span data-stu-id="62d59-234">String</span></span>|<span data-ttu-id="62d59-235">デバイスのアクティベーション ロックをバイパスするためのコード。</span><span class="sxs-lookup"><span data-stu-id="62d59-235">Code that allows the Activation Lock on a device to be bypassed.</span></span> <span data-ttu-id="62d59-236">[manageddevice](../resources/intune-devices-manageddevice.md)から継承します</span><span class="sxs-lookup"><span data-stu-id="62d59-236">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="62d59-237">emailAddress</span><span class="sxs-lookup"><span data-stu-id="62d59-237">emailAddress</span></span>|<span data-ttu-id="62d59-238">String</span><span class="sxs-lookup"><span data-stu-id="62d59-238">String</span></span>|<span data-ttu-id="62d59-239">[manageddevice](../resources/intune-devices-manageddevice.md)から継承したデバイスに関連付けられているユーザーの電子メール</span><span class="sxs-lookup"><span data-stu-id="62d59-239">Email(s) for the user associated with the device Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="62d59-240">azureActiveDirectoryDeviceId</span><span class="sxs-lookup"><span data-stu-id="62d59-240">azureActiveDirectoryDeviceId</span></span>|<span data-ttu-id="62d59-241">String</span><span class="sxs-lookup"><span data-stu-id="62d59-241">String</span></span>|<span data-ttu-id="62d59-242">Azure Active Directory デバイスの一意識別子。</span><span class="sxs-lookup"><span data-stu-id="62d59-242">The unique identifier for the Azure Active Directory device.</span></span> <span data-ttu-id="62d59-243">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="62d59-243">Read only.</span></span> <span data-ttu-id="62d59-244">[manageddevice](../resources/intune-devices-manageddevice.md)から継承します</span><span class="sxs-lookup"><span data-stu-id="62d59-244">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="62d59-245">azureADDeviceId</span><span class="sxs-lookup"><span data-stu-id="62d59-245">azureADDeviceId</span></span>|<span data-ttu-id="62d59-246">String</span><span class="sxs-lookup"><span data-stu-id="62d59-246">String</span></span>|<span data-ttu-id="62d59-247">Azure Active Directory デバイスの一意識別子。</span><span class="sxs-lookup"><span data-stu-id="62d59-247">The unique identifier for the Azure Active Directory device.</span></span> <span data-ttu-id="62d59-248">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="62d59-248">Read only.</span></span> <span data-ttu-id="62d59-249">[manageddevice](../resources/intune-devices-manageddevice.md)から継承します</span><span class="sxs-lookup"><span data-stu-id="62d59-249">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="62d59-250">deviceRegistrationState</span><span class="sxs-lookup"><span data-stu-id="62d59-250">deviceRegistrationState</span></span>|[<span data-ttu-id="62d59-251">deviceRegistrationState</span><span class="sxs-lookup"><span data-stu-id="62d59-251">deviceRegistrationState</span></span>](../resources/intune-devices-deviceregistrationstate.md)|<span data-ttu-id="62d59-252">デバイスの登録状態。</span><span class="sxs-lookup"><span data-stu-id="62d59-252">Device registration state.</span></span> <span data-ttu-id="62d59-253">[manageddevice](../resources/intune-devices-manageddevice.md)から継承されます。</span><span class="sxs-lookup"><span data-stu-id="62d59-253">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="62d59-254">可能な値は、`notRegistered`、`registered`、`revoked`、`keyConflict`、`approvalPending`、`certificateReset`、`notRegisteredPendingEnrollment`、`unknown` です。</span><span class="sxs-lookup"><span data-stu-id="62d59-254">Possible values are: `notRegistered`, `registered`, `revoked`, `keyConflict`, `approvalPending`, `certificateReset`, `notRegisteredPendingEnrollment`, `unknown`.</span></span>|
|<span data-ttu-id="62d59-255">deviceCategoryDisplayName</span><span class="sxs-lookup"><span data-stu-id="62d59-255">deviceCategoryDisplayName</span></span>|<span data-ttu-id="62d59-256">String</span><span class="sxs-lookup"><span data-stu-id="62d59-256">String</span></span>|<span data-ttu-id="62d59-257">[manageddevice](../resources/intune-devices-manageddevice.md)から継承されたデバイスカテゴリの表示名</span><span class="sxs-lookup"><span data-stu-id="62d59-257">Device category display name Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="62d59-258">isSupervised</span><span class="sxs-lookup"><span data-stu-id="62d59-258">isSupervised</span></span>|<span data-ttu-id="62d59-259">ブール値</span><span class="sxs-lookup"><span data-stu-id="62d59-259">Boolean</span></span>|<span data-ttu-id="62d59-260">[manageddevice](../resources/intune-devices-manageddevice.md)から継承されたデバイスの監視状態</span><span class="sxs-lookup"><span data-stu-id="62d59-260">Device supervised status Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="62d59-261">exchangeLastSuccessfulSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="62d59-261">exchangeLastSuccessfulSyncDateTime</span></span>|<span data-ttu-id="62d59-262">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="62d59-262">DateTimeOffset</span></span>|<span data-ttu-id="62d59-263">最後にデバイスが Exchange に接続した時刻。</span><span class="sxs-lookup"><span data-stu-id="62d59-263">Last time the device contacted Exchange.</span></span> <span data-ttu-id="62d59-264">[manageddevice](../resources/intune-devices-manageddevice.md)から継承します</span><span class="sxs-lookup"><span data-stu-id="62d59-264">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="62d59-265">exchangeAccessState</span><span class="sxs-lookup"><span data-stu-id="62d59-265">exchangeAccessState</span></span>|[<span data-ttu-id="62d59-266">devicemanagementexchangeaccessstate</span><span class="sxs-lookup"><span data-stu-id="62d59-266">deviceManagementExchangeAccessState</span></span>](../resources/intune-devices-devicemanagementexchangeaccessstate.md)|<span data-ttu-id="62d59-267">Exchange でのデバイスのアクセスの状態。</span><span class="sxs-lookup"><span data-stu-id="62d59-267">The Access State of the device in Exchange.</span></span> <span data-ttu-id="62d59-268">[manageddevice](../resources/intune-devices-manageddevice.md)から継承されます。</span><span class="sxs-lookup"><span data-stu-id="62d59-268">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="62d59-269">可能な値は、`none`、`unknown`、`allowed`、`blocked`、`quarantined` です。</span><span class="sxs-lookup"><span data-stu-id="62d59-269">Possible values are: `none`, `unknown`, `allowed`, `blocked`, `quarantined`.</span></span>|
|<span data-ttu-id="62d59-270">exchangeAccessStateReason</span><span class="sxs-lookup"><span data-stu-id="62d59-270">exchangeAccessStateReason</span></span>|[<span data-ttu-id="62d59-271">deviceManagementExchangeAccessStateReason</span><span class="sxs-lookup"><span data-stu-id="62d59-271">deviceManagementExchangeAccessStateReason</span></span>](../resources/intune-devices-devicemanagementexchangeaccessstatereason.md)|<span data-ttu-id="62d59-272">Exchange でのデバイスのアクセス状態の理由。
</span><span class="sxs-lookup"><span data-stu-id="62d59-272">The reason for the device's access state in Exchange.</span></span> <span data-ttu-id="62d59-273">[manageddevice](../resources/intune-devices-manageddevice.md)から継承されます。</span><span class="sxs-lookup"><span data-stu-id="62d59-273">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="62d59-274">可能な値は、`none`、`unknown`、`exchangeGlobalRule`、`exchangeIndividualRule`、`exchangeDeviceRule`、`exchangeUpgrade`、`exchangeMailboxPolicy`、`other`、`compliant`、`notCompliant`、`notEnrolled`、`unknownLocation`、`mfaRequired`、`azureADBlockDueToAccessPolicy`、`compromisedPassword`、`deviceNotKnownWithManagedApp` です。</span><span class="sxs-lookup"><span data-stu-id="62d59-274">Possible values are: `none`, `unknown`, `exchangeGlobalRule`, `exchangeIndividualRule`, `exchangeDeviceRule`, `exchangeUpgrade`, `exchangeMailboxPolicy`, `other`, `compliant`, `notCompliant`, `notEnrolled`, `unknownLocation`, `mfaRequired`, `azureADBlockDueToAccessPolicy`, `compromisedPassword`, `deviceNotKnownWithManagedApp`.</span></span>|
|<span data-ttu-id="62d59-275">remoteAssistanceSessionUrl</span><span class="sxs-lookup"><span data-stu-id="62d59-275">remoteAssistanceSessionUrl</span></span>|<span data-ttu-id="62d59-276">String</span><span class="sxs-lookup"><span data-stu-id="62d59-276">String</span></span>|<span data-ttu-id="62d59-277">デバイスとのリモート アシスタンス セッションを確立できるようにする URL。</span><span class="sxs-lookup"><span data-stu-id="62d59-277">Url that allows a Remote Assistance session to be established with the device.</span></span> <span data-ttu-id="62d59-278">[manageddevice](../resources/intune-devices-manageddevice.md)から継承します</span><span class="sxs-lookup"><span data-stu-id="62d59-278">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="62d59-279">remoteAssistanceSessionErrorDetails</span><span class="sxs-lookup"><span data-stu-id="62d59-279">remoteAssistanceSessionErrorDetails</span></span>|<span data-ttu-id="62d59-280">String</span><span class="sxs-lookup"><span data-stu-id="62d59-280">String</span></span>|<span data-ttu-id="62d59-281">リモート アシスタンス セッション オブジェクトの作成時に問題を識別するエラー文字列。</span><span class="sxs-lookup"><span data-stu-id="62d59-281">An error string that identifies issues when creating Remote Assistance session objects.</span></span> <span data-ttu-id="62d59-282">[manageddevice](../resources/intune-devices-manageddevice.md)から継承します</span><span class="sxs-lookup"><span data-stu-id="62d59-282">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="62d59-283">isEncrypted</span><span class="sxs-lookup"><span data-stu-id="62d59-283">isEncrypted</span></span>|<span data-ttu-id="62d59-284">Boolean</span><span class="sxs-lookup"><span data-stu-id="62d59-284">Boolean</span></span>|<span data-ttu-id="62d59-285">[manageddevice](../resources/intune-devices-manageddevice.md)から継承されたデバイスの暗号化状態</span><span class="sxs-lookup"><span data-stu-id="62d59-285">Device encryption status Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="62d59-286">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="62d59-286">userPrincipalName</span></span>|<span data-ttu-id="62d59-287">文字列</span><span class="sxs-lookup"><span data-stu-id="62d59-287">String</span></span>|<span data-ttu-id="62d59-288">[manageddevice](../resources/intune-devices-manageddevice.md)から継承されたデバイスユーザープリンシパル名</span><span class="sxs-lookup"><span data-stu-id="62d59-288">Device user principal name Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="62d59-289">model</span><span class="sxs-lookup"><span data-stu-id="62d59-289">model</span></span>|<span data-ttu-id="62d59-290">String</span><span class="sxs-lookup"><span data-stu-id="62d59-290">String</span></span>|<span data-ttu-id="62d59-291">[manageddevice](../resources/intune-devices-manageddevice.md)から継承されたデバイスのモデル</span><span class="sxs-lookup"><span data-stu-id="62d59-291">Model of the device Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="62d59-292">manufacturer</span><span class="sxs-lookup"><span data-stu-id="62d59-292">manufacturer</span></span>|<span data-ttu-id="62d59-293">String</span><span class="sxs-lookup"><span data-stu-id="62d59-293">String</span></span>|<span data-ttu-id="62d59-294">[manageddevice](../resources/intune-devices-manageddevice.md)から継承されたデバイスの製造元</span><span class="sxs-lookup"><span data-stu-id="62d59-294">Manufacturer of the device Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="62d59-295">imei</span><span class="sxs-lookup"><span data-stu-id="62d59-295">imei</span></span>|<span data-ttu-id="62d59-296">String</span><span class="sxs-lookup"><span data-stu-id="62d59-296">String</span></span>|<span data-ttu-id="62d59-297">[manageddevice](../resources/intune-devices-manageddevice.md)から継承された IMEI</span><span class="sxs-lookup"><span data-stu-id="62d59-297">IMEI Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="62d59-298">complianceGracePeriodExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="62d59-298">complianceGracePeriodExpirationDateTime</span></span>|<span data-ttu-id="62d59-299">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="62d59-299">DateTimeOffset</span></span>|<span data-ttu-id="62d59-300">デバイスコンプライアンスの猶予期間が[manageddevice](../resources/intune-devices-manageddevice.md)から継承される日時</span><span class="sxs-lookup"><span data-stu-id="62d59-300">The DateTime when device compliance grace period expires Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="62d59-301">シリアル番号</span><span class="sxs-lookup"><span data-stu-id="62d59-301">serialNumber</span></span>|<span data-ttu-id="62d59-302">String</span><span class="sxs-lookup"><span data-stu-id="62d59-302">String</span></span>|<span data-ttu-id="62d59-303">[manageddevice](../resources/intune-devices-manageddevice.md)から継承されたシリアル</span><span class="sxs-lookup"><span data-stu-id="62d59-303">SerialNumber Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="62d59-304">phoneNumber</span><span class="sxs-lookup"><span data-stu-id="62d59-304">phoneNumber</span></span>|<span data-ttu-id="62d59-305">String</span><span class="sxs-lookup"><span data-stu-id="62d59-305">String</span></span>|<span data-ttu-id="62d59-306">[manageddevice](../resources/intune-devices-manageddevice.md)から継承されたデバイスの電話番号</span><span class="sxs-lookup"><span data-stu-id="62d59-306">Phone number of the device Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="62d59-307">androidSecurityPatchLevel</span><span class="sxs-lookup"><span data-stu-id="62d59-307">androidSecurityPatchLevel</span></span>|<span data-ttu-id="62d59-308">String</span><span class="sxs-lookup"><span data-stu-id="62d59-308">String</span></span>|<span data-ttu-id="62d59-309">[manageddevice](../resources/intune-devices-manageddevice.md)から継承された Android セキュリティパッチレベル</span><span class="sxs-lookup"><span data-stu-id="62d59-309">Android security patch level Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="62d59-310">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="62d59-310">userDisplayName</span></span>|<span data-ttu-id="62d59-311">String</span><span class="sxs-lookup"><span data-stu-id="62d59-311">String</span></span>|<span data-ttu-id="62d59-312">[manageddevice](../resources/intune-devices-manageddevice.md)から継承されたユーザーの表示名</span><span class="sxs-lookup"><span data-stu-id="62d59-312">User display name Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="62d59-313">configurationManagerClientEnabledFeatures</span><span class="sxs-lookup"><span data-stu-id="62d59-313">configurationManagerClientEnabledFeatures</span></span>|[<span data-ttu-id="62d59-314">configurationManagerClientEnabledFeatures</span><span class="sxs-lookup"><span data-stu-id="62d59-314">configurationManagerClientEnabledFeatures</span></span>](../resources/intune-devices-configurationmanagerclientenabledfeatures.md)|<span data-ttu-id="62d59-315">[manageddevice](../resources/intune-devices-manageddevice.md)から継承された grmgr クライアントの有効な機能の設定</span><span class="sxs-lookup"><span data-stu-id="62d59-315">ConfigrMgr client enabled features Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="62d59-316">wiFiMacAddress</span><span class="sxs-lookup"><span data-stu-id="62d59-316">wiFiMacAddress</span></span>|<span data-ttu-id="62d59-317">String</span><span class="sxs-lookup"><span data-stu-id="62d59-317">String</span></span>|<span data-ttu-id="62d59-318">[manageddevice](../resources/intune-devices-manageddevice.md)から継承された wi-fi MAC</span><span class="sxs-lookup"><span data-stu-id="62d59-318">Wi-Fi MAC Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="62d59-319">deviceHealthAttestationState</span><span class="sxs-lookup"><span data-stu-id="62d59-319">deviceHealthAttestationState</span></span>|[<span data-ttu-id="62d59-320">deviceHealthAttestationState</span><span class="sxs-lookup"><span data-stu-id="62d59-320">deviceHealthAttestationState</span></span>](../resources/intune-devices-devicehealthattestationstate.md)|<span data-ttu-id="62d59-321">デバイスの正常性構成証明の状態。</span><span class="sxs-lookup"><span data-stu-id="62d59-321">The device health attestation state.</span></span> <span data-ttu-id="62d59-322">[manageddevice](../resources/intune-devices-manageddevice.md)から継承します</span><span class="sxs-lookup"><span data-stu-id="62d59-322">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="62d59-323">subscriberCarrier</span><span class="sxs-lookup"><span data-stu-id="62d59-323">subscriberCarrier</span></span>|<span data-ttu-id="62d59-324">String</span><span class="sxs-lookup"><span data-stu-id="62d59-324">String</span></span>|<span data-ttu-id="62d59-325">[manageddevice](../resources/intune-devices-manageddevice.md)から継承されたサブスクライバーキャリア</span><span class="sxs-lookup"><span data-stu-id="62d59-325">Subscriber Carrier Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="62d59-326">meid</span><span class="sxs-lookup"><span data-stu-id="62d59-326">meid</span></span>|<span data-ttu-id="62d59-327">String</span><span class="sxs-lookup"><span data-stu-id="62d59-327">String</span></span>|<span data-ttu-id="62d59-328">[manageddevice](../resources/intune-devices-manageddevice.md)から継承された meid</span><span class="sxs-lookup"><span data-stu-id="62d59-328">MEID Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="62d59-329">totalStorageSpaceInBytes</span><span class="sxs-lookup"><span data-stu-id="62d59-329">totalStorageSpaceInBytes</span></span>|<span data-ttu-id="62d59-330">Int64</span><span class="sxs-lookup"><span data-stu-id="62d59-330">Int64</span></span>|<span data-ttu-id="62d59-331">[manageddevice](../resources/intune-devices-manageddevice.md)から継承された合計記憶域 (バイト)</span><span class="sxs-lookup"><span data-stu-id="62d59-331">Total Storage in Bytes Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="62d59-332">freeStorageSpaceInBytes</span><span class="sxs-lookup"><span data-stu-id="62d59-332">freeStorageSpaceInBytes</span></span>|<span data-ttu-id="62d59-333">Int64</span><span class="sxs-lookup"><span data-stu-id="62d59-333">Int64</span></span>|<span data-ttu-id="62d59-334">[manageddevice](../resources/intune-devices-manageddevice.md)から継承された空き記憶域 (バイト単位)</span><span class="sxs-lookup"><span data-stu-id="62d59-334">Free Storage in Bytes Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="62d59-335">managedDeviceName</span><span class="sxs-lookup"><span data-stu-id="62d59-335">managedDeviceName</span></span>|<span data-ttu-id="62d59-336">String</span><span class="sxs-lookup"><span data-stu-id="62d59-336">String</span></span>|<span data-ttu-id="62d59-337">デバイスを識別する名前が自動的に生成されます。</span><span class="sxs-lookup"><span data-stu-id="62d59-337">Automatically generated name to identify a device.</span></span> <span data-ttu-id="62d59-338">ユーザー フレンドリ名に上書きできます。</span><span class="sxs-lookup"><span data-stu-id="62d59-338">Can be overwritten to a user friendly name.</span></span> <span data-ttu-id="62d59-339">[manageddevice](../resources/intune-devices-manageddevice.md)から継承します</span><span class="sxs-lookup"><span data-stu-id="62d59-339">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="62d59-340">partnerReportedThreatState</span><span class="sxs-lookup"><span data-stu-id="62d59-340">partnerReportedThreatState</span></span>|[<span data-ttu-id="62d59-341">manageddevicepartnerreportedhealthstate</span><span class="sxs-lookup"><span data-stu-id="62d59-341">managedDevicePartnerReportedHealthState</span></span>](../resources/intune-devices-manageddevicepartnerreportedhealthstate.md)|<span data-ttu-id="62d59-342">Mobile Threat Defense パートナーがアカウントおよびデバイスで使用されている場合の、デバイスの脅威の状態を示します。</span><span class="sxs-lookup"><span data-stu-id="62d59-342">Indicates the threat state of a device when a Mobile Threat Defense partner is in use by the account and device.</span></span> <span data-ttu-id="62d59-343">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="62d59-343">Read Only.</span></span> <span data-ttu-id="62d59-344">[manageddevice](../resources/intune-devices-manageddevice.md)から継承されます。</span><span class="sxs-lookup"><span data-stu-id="62d59-344">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md).</span></span> <span data-ttu-id="62d59-345">可能な値は、`unknown`、`activated`、`deactivated`、`secured`、`lowSeverity`、`mediumSeverity`、`highSeverity`、`unresponsive`、`compromised`、`misconfigured` です。</span><span class="sxs-lookup"><span data-stu-id="62d59-345">Possible values are: `unknown`, `activated`, `deactivated`, `secured`, `lowSeverity`, `mediumSeverity`, `highSeverity`, `unresponsive`, `compromised`, `misconfigured`.</span></span>|
|<span data-ttu-id="62d59-346">usersLoggedOn</span><span class="sxs-lookup"><span data-stu-id="62d59-346">usersLoggedOn</span></span>|<span data-ttu-id="62d59-347">[loggedOnUser](../resources/intune-devices-loggedonuser.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="62d59-347">[loggedOnUser](../resources/intune-devices-loggedonuser.md) collection</span></span>|<span data-ttu-id="62d59-348">[manageddevice](../resources/intune-devices-manageddevice.md)から継承されたデバイスの最後にログオンしたユーザーを示します</span><span class="sxs-lookup"><span data-stu-id="62d59-348">Indicates the last logged on users of a device Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="62d59-349">preferMdmOverGroupPolicyAppliedDateTime</span><span class="sxs-lookup"><span data-stu-id="62d59-349">preferMdmOverGroupPolicyAppliedDateTime</span></span>|<span data-ttu-id="62d59-350">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="62d59-350">DateTimeOffset</span></span>|<span data-ttu-id="62d59-351">preferMdmOverGroupPolicy の設定が設定された DateTime を報告します。</span><span class="sxs-lookup"><span data-stu-id="62d59-351">Reports the DateTime the preferMdmOverGroupPolicy setting was set.</span></span>  <span data-ttu-id="62d59-352">設定すると、競合がある場合に Intune MDM 設定がグループポリシー設定を上書きします。</span><span class="sxs-lookup"><span data-stu-id="62d59-352">When set, the Intune MDM settings will override Group Policy settings if there is a conflict.</span></span> <span data-ttu-id="62d59-353">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="62d59-353">Read Only.</span></span> <span data-ttu-id="62d59-354">[manageddevice](../resources/intune-devices-manageddevice.md)から継承します</span><span class="sxs-lookup"><span data-stu-id="62d59-354">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="62d59-355">autopilotEnrolled</span><span class="sxs-lookup"><span data-stu-id="62d59-355">autopilotEnrolled</span></span>|<span data-ttu-id="62d59-356">ブール値</span><span class="sxs-lookup"><span data-stu-id="62d59-356">Boolean</span></span>|<span data-ttu-id="62d59-357">管理対象デバイスが自動パイロットで登録されているかどうかを報告します。</span><span class="sxs-lookup"><span data-stu-id="62d59-357">Reports if the managed device is enrolled via auto-pilot.</span></span> <span data-ttu-id="62d59-358">[manageddevice](../resources/intune-devices-manageddevice.md)から継承します</span><span class="sxs-lookup"><span data-stu-id="62d59-358">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="62d59-359">requireUserEnrollmentApproval</span><span class="sxs-lookup"><span data-stu-id="62d59-359">requireUserEnrollmentApproval</span></span>|<span data-ttu-id="62d59-360">ブール値</span><span class="sxs-lookup"><span data-stu-id="62d59-360">Boolean</span></span>|<span data-ttu-id="62d59-361">管理対象 iOS デバイスがユーザー承認登録であるかどうかを報告します。</span><span class="sxs-lookup"><span data-stu-id="62d59-361">Reports if the managed iOS device is user approval enrollment.</span></span> <span data-ttu-id="62d59-362">[manageddevice](../resources/intune-devices-manageddevice.md)から継承します</span><span class="sxs-lookup"><span data-stu-id="62d59-362">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="62d59-363">managementCertificateExpirationDate</span><span class="sxs-lookup"><span data-stu-id="62d59-363">managementCertificateExpirationDate</span></span>|<span data-ttu-id="62d59-364">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="62d59-364">DateTimeOffset</span></span>|<span data-ttu-id="62d59-365">[manageddevice](../resources/intune-devices-manageddevice.md)から継承されたデバイス管理証明書の有効期限日を報告します</span><span class="sxs-lookup"><span data-stu-id="62d59-365">Reports device management certificate expiration date Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="62d59-366">iccid</span><span class="sxs-lookup"><span data-stu-id="62d59-366">iccid</span></span>|<span data-ttu-id="62d59-367">String</span><span class="sxs-lookup"><span data-stu-id="62d59-367">String</span></span>|<span data-ttu-id="62d59-368">ic カード識別子。 SIM カードの一意の識別番号です。</span><span class="sxs-lookup"><span data-stu-id="62d59-368">Integrated Circuit Card Identifier, it is A SIM card's unique identification number.</span></span> <span data-ttu-id="62d59-369">[manageddevice](../resources/intune-devices-manageddevice.md)から継承します</span><span class="sxs-lookup"><span data-stu-id="62d59-369">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="62d59-370">udid</span><span class="sxs-lookup"><span data-stu-id="62d59-370">udid</span></span>|<span data-ttu-id="62d59-371">String</span><span class="sxs-lookup"><span data-stu-id="62d59-371">String</span></span>|<span data-ttu-id="62d59-372">iOS および macOS デバイスの一意のデバイス識別子。</span><span class="sxs-lookup"><span data-stu-id="62d59-372">Unique Device Identifier for iOS and macOS devices.</span></span> <span data-ttu-id="62d59-373">[manageddevice](../resources/intune-devices-manageddevice.md)から継承します</span><span class="sxs-lookup"><span data-stu-id="62d59-373">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="62d59-374">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="62d59-374">roleScopeTagIds</span></span>|<span data-ttu-id="62d59-375">String collection</span><span class="sxs-lookup"><span data-stu-id="62d59-375">String collection</span></span>|<span data-ttu-id="62d59-376">このデバイスインスタンスの範囲タグ id のリスト。</span><span class="sxs-lookup"><span data-stu-id="62d59-376">List of Scope Tag IDs for this Device instance.</span></span> <span data-ttu-id="62d59-377">[manageddevice](../resources/intune-devices-manageddevice.md)から継承します</span><span class="sxs-lookup"><span data-stu-id="62d59-377">Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="62d59-378">windowsactivemalwarecount 再計算</span><span class="sxs-lookup"><span data-stu-id="62d59-378">windowsActiveMalwareCount</span></span>|<span data-ttu-id="62d59-379">Int32</span><span class="sxs-lookup"><span data-stu-id="62d59-379">Int32</span></span>|<span data-ttu-id="62d59-380">[manageddevice](../resources/intune-devices-manageddevice.md)から継承された、この windows デバイスのアクティブなマルウェアの数</span><span class="sxs-lookup"><span data-stu-id="62d59-380">Count of active malware for this windows device Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="62d59-381">windowsRemediatedMalwareCount</span><span class="sxs-lookup"><span data-stu-id="62d59-381">windowsRemediatedMalwareCount</span></span>|<span data-ttu-id="62d59-382">Int32</span><span class="sxs-lookup"><span data-stu-id="62d59-382">Int32</span></span>|<span data-ttu-id="62d59-383">[manageddevice](../resources/intune-devices-manageddevice.md)から継承された、この windows デバイスの修復されたマルウェアの数</span><span class="sxs-lookup"><span data-stu-id="62d59-383">Count of remediated malware for this windows device Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="62d59-384">notes</span><span class="sxs-lookup"><span data-stu-id="62d59-384">notes</span></span>|<span data-ttu-id="62d59-385">String</span><span class="sxs-lookup"><span data-stu-id="62d59-385">String</span></span>|<span data-ttu-id="62d59-386">IT 管理者によって作成された、 [manageddevice](../resources/intune-devices-manageddevice.md)から継承したデバイス上のメモ</span><span class="sxs-lookup"><span data-stu-id="62d59-386">Notes on the device created by IT Admin Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|
|<span data-ttu-id="62d59-387">configurationManagerClientHealthState</span><span class="sxs-lookup"><span data-stu-id="62d59-387">configurationManagerClientHealthState</span></span>|[<span data-ttu-id="62d59-388">configurationManagerClientHealthState</span><span class="sxs-lookup"><span data-stu-id="62d59-388">configurationManagerClientHealthState</span></span>](../resources/intune-devices-configurationmanagerclienthealthstate.md)|<span data-ttu-id="62d59-389">構成マネージャークライアントの正常性状態。 MDM/ConfigMgr エージェントによって管理されているデバイスに対してのみ有効。 [manageddevice](../resources/intune-devices-manageddevice.md)から継承されます。</span><span class="sxs-lookup"><span data-stu-id="62d59-389">Configuration manager client health state, valid only for devices managed by MDM/ConfigMgr Agent Inherited from [managedDevice](../resources/intune-devices-manageddevice.md)</span></span>|



## <a name="response"></a><span data-ttu-id="62d59-390">応答</span><span class="sxs-lookup"><span data-stu-id="62d59-390">Response</span></span>
<span data-ttu-id="62d59-391">成功した場合、このメソッド`201 Created`は応答コードと、応答本文で[windowsmanageddevice](../resources/intune-devices-windowsmanageddevice.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="62d59-391">If successful, this method returns a `201 Created` response code and a [windowsManagedDevice](../resources/intune-devices-windowsmanageddevice.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="62d59-392">例</span><span class="sxs-lookup"><span data-stu-id="62d59-392">Example</span></span>

### <a name="request"></a><span data-ttu-id="62d59-393">要求</span><span class="sxs-lookup"><span data-stu-id="62d59-393">Request</span></span>
<span data-ttu-id="62d59-394">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="62d59-394">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/users/{usersId}/managedDevices
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

### <a name="response"></a><span data-ttu-id="62d59-395">応答</span><span class="sxs-lookup"><span data-stu-id="62d59-395">Response</span></span>
<span data-ttu-id="62d59-p141">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="62d59-p141">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




