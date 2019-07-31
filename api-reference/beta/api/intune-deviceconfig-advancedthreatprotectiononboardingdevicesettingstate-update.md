---
title: AdvancedThreatProtectionOnboardingDeviceSettingState の更新
description: AdvancedThreatProtectionOnboardingDeviceSettingState オブジェクトのプロパティを更新します。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 8a7f5bde5d046c5d994b9dafc28a09364f3e616b
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35958473"
---
# <a name="update-advancedthreatprotectiononboardingdevicesettingstate"></a><span data-ttu-id="92e26-103">AdvancedThreatProtectionOnboardingDeviceSettingState の更新</span><span class="sxs-lookup"><span data-stu-id="92e26-103">Update advancedThreatProtectionOnboardingDeviceSettingState</span></span>

> <span data-ttu-id="92e26-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="92e26-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="92e26-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="92e26-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="92e26-106">[AdvancedThreatProtectionOnboardingDeviceSettingState](../resources/intune-deviceconfig-advancedthreatprotectiononboardingdevicesettingstate.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="92e26-106">Update the properties of a [advancedThreatProtectionOnboardingDeviceSettingState](../resources/intune-deviceconfig-advancedthreatprotectiononboardingdevicesettingstate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="92e26-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="92e26-107">Prerequisites</span></span>
<span data-ttu-id="92e26-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="92e26-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="92e26-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="92e26-110">Permission type</span></span>|<span data-ttu-id="92e26-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="92e26-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="92e26-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="92e26-112">Delegated (work or school account)</span></span>|<span data-ttu-id="92e26-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="92e26-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="92e26-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="92e26-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="92e26-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="92e26-115">Not supported.</span></span>|
|<span data-ttu-id="92e26-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="92e26-116">Application</span></span>|<span data-ttu-id="92e26-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="92e26-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="92e26-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="92e26-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/advancedThreatProtectionOnboardingStateSummary/advancedThreatProtectionOnboardingDeviceSettingStates/{advancedThreatProtectionOnboardingDeviceSettingStateId}
```

## <a name="request-headers"></a><span data-ttu-id="92e26-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="92e26-119">Request headers</span></span>
|<span data-ttu-id="92e26-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="92e26-120">Header</span></span>|<span data-ttu-id="92e26-121">値</span><span class="sxs-lookup"><span data-stu-id="92e26-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="92e26-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="92e26-122">Authorization</span></span>|<span data-ttu-id="92e26-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="92e26-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="92e26-124">承諾</span><span class="sxs-lookup"><span data-stu-id="92e26-124">Accept</span></span>|<span data-ttu-id="92e26-125">application/json</span><span class="sxs-lookup"><span data-stu-id="92e26-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="92e26-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="92e26-126">Request body</span></span>
<span data-ttu-id="92e26-127">要求本文で、 [advancedThreatProtectionOnboardingDeviceSettingState](../resources/intune-deviceconfig-advancedthreatprotectiononboardingdevicesettingstate.md)オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="92e26-127">In the request body, supply a JSON representation for the [advancedThreatProtectionOnboardingDeviceSettingState](../resources/intune-deviceconfig-advancedthreatprotectiononboardingdevicesettingstate.md) object.</span></span>

<span data-ttu-id="92e26-128">次の表に、 [advancedThreatProtectionOnboardingDeviceSettingState](../resources/intune-deviceconfig-advancedthreatprotectiononboardingdevicesettingstate.md)の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="92e26-128">The following table shows the properties that are required when you create the [advancedThreatProtectionOnboardingDeviceSettingState](../resources/intune-deviceconfig-advancedthreatprotectiononboardingdevicesettingstate.md).</span></span>

|<span data-ttu-id="92e26-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="92e26-129">Property</span></span>|<span data-ttu-id="92e26-130">型</span><span class="sxs-lookup"><span data-stu-id="92e26-130">Type</span></span>|<span data-ttu-id="92e26-131">説明</span><span class="sxs-lookup"><span data-stu-id="92e26-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="92e26-132">id</span><span class="sxs-lookup"><span data-stu-id="92e26-132">id</span></span>|<span data-ttu-id="92e26-133">文字列</span><span class="sxs-lookup"><span data-stu-id="92e26-133">String</span></span>|<span data-ttu-id="92e26-134">エンティティのキー</span><span class="sxs-lookup"><span data-stu-id="92e26-134">Key of the entity</span></span>|
|<span data-ttu-id="92e26-135">platformType</span><span class="sxs-lookup"><span data-stu-id="92e26-135">platformType</span></span>|[<span data-ttu-id="92e26-136">deviceType</span><span class="sxs-lookup"><span data-stu-id="92e26-136">deviceType</span></span>](../resources/intune-shared-devicetype.md)|<span data-ttu-id="92e26-137">デバイスプラットフォームの種類。</span><span class="sxs-lookup"><span data-stu-id="92e26-137">Device platform type.</span></span> <span data-ttu-id="92e26-138">可能な値: `desktop`、 `windowsRT` `winMO6` `nokia` `windowsPhone` `mac` `winCE` `winEmbedded` `iPhone` `iPad` `iPod` `android`、、、、、、、、、、、、 `iSocConsumer` `unix` `macMDM` `holoLens` `surfaceHub` `androidForWork` `androidEnterprise`, `blackberry`, `palm`, `unknown`.</span><span class="sxs-lookup"><span data-stu-id="92e26-138">Possible values are: `desktop`, `windowsRT`, `winMO6`, `nokia`, `windowsPhone`, `mac`, `winCE`, `winEmbedded`, `iPhone`, `iPad`, `iPod`, `android`, `iSocConsumer`, `unix`, `macMDM`, `holoLens`, `surfaceHub`, `androidForWork`, `androidEnterprise`, `blackberry`, `palm`, `unknown`.</span></span>|
|<span data-ttu-id="92e26-139">setting</span><span class="sxs-lookup"><span data-stu-id="92e26-139">setting</span></span>|<span data-ttu-id="92e26-140">String</span><span class="sxs-lookup"><span data-stu-id="92e26-140">String</span></span>|<span data-ttu-id="92e26-141">設定のクラス名とプロパティ名。</span><span class="sxs-lookup"><span data-stu-id="92e26-141">The setting class name and property name.</span></span>|
|<span data-ttu-id="92e26-142">settingName</span><span class="sxs-lookup"><span data-stu-id="92e26-142">settingName</span></span>|<span data-ttu-id="92e26-143">String</span><span class="sxs-lookup"><span data-stu-id="92e26-143">String</span></span>|<span data-ttu-id="92e26-144">レポートされている設定名。</span><span class="sxs-lookup"><span data-stu-id="92e26-144">The Setting Name that is being reported</span></span>|
|<span data-ttu-id="92e26-145">deviceId</span><span class="sxs-lookup"><span data-stu-id="92e26-145">deviceId</span></span>|<span data-ttu-id="92e26-146">String</span><span class="sxs-lookup"><span data-stu-id="92e26-146">String</span></span>|<span data-ttu-id="92e26-147">レポートされているデバイス ID。</span><span class="sxs-lookup"><span data-stu-id="92e26-147">The Device Id that is being reported</span></span>|
|<span data-ttu-id="92e26-148">deviceName</span><span class="sxs-lookup"><span data-stu-id="92e26-148">deviceName</span></span>|<span data-ttu-id="92e26-149">String</span><span class="sxs-lookup"><span data-stu-id="92e26-149">String</span></span>|<span data-ttu-id="92e26-150">レポートされているデバイス名。</span><span class="sxs-lookup"><span data-stu-id="92e26-150">The Device Name that is being reported</span></span>|
|<span data-ttu-id="92e26-151">userId</span><span class="sxs-lookup"><span data-stu-id="92e26-151">userId</span></span>|<span data-ttu-id="92e26-152">String</span><span class="sxs-lookup"><span data-stu-id="92e26-152">String</span></span>|<span data-ttu-id="92e26-153">レポートされているユーザー ID</span><span class="sxs-lookup"><span data-stu-id="92e26-153">The user Id that is being reported</span></span>|
|<span data-ttu-id="92e26-154">userEmail</span><span class="sxs-lookup"><span data-stu-id="92e26-154">userEmail</span></span>|<span data-ttu-id="92e26-155">String</span><span class="sxs-lookup"><span data-stu-id="92e26-155">String</span></span>|<span data-ttu-id="92e26-156">レポートされているユーザーのメール アドレス。</span><span class="sxs-lookup"><span data-stu-id="92e26-156">The User email address that is being reported</span></span>|
|<span data-ttu-id="92e26-157">userName</span><span class="sxs-lookup"><span data-stu-id="92e26-157">userName</span></span>|<span data-ttu-id="92e26-158">String</span><span class="sxs-lookup"><span data-stu-id="92e26-158">String</span></span>|<span data-ttu-id="92e26-159">レポートされているユーザー名</span><span class="sxs-lookup"><span data-stu-id="92e26-159">The User Name that is being reported</span></span>|
|<span data-ttu-id="92e26-160">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="92e26-160">userPrincipalName</span></span>|<span data-ttu-id="92e26-161">String</span><span class="sxs-lookup"><span data-stu-id="92e26-161">String</span></span>|<span data-ttu-id="92e26-162">レポートされているユーザーの PrincipalName</span><span class="sxs-lookup"><span data-stu-id="92e26-162">The User PrincipalName that is being reported</span></span>|
|<span data-ttu-id="92e26-163">deviceModel</span><span class="sxs-lookup"><span data-stu-id="92e26-163">deviceModel</span></span>|<span data-ttu-id="92e26-164">String</span><span class="sxs-lookup"><span data-stu-id="92e26-164">String</span></span>|<span data-ttu-id="92e26-165">レポートされているデバイス モデル</span><span class="sxs-lookup"><span data-stu-id="92e26-165">The device model that is being reported</span></span>|
|<span data-ttu-id="92e26-166">state</span><span class="sxs-lookup"><span data-stu-id="92e26-166">state</span></span>|[<span data-ttu-id="92e26-167">complianceStatus</span><span class="sxs-lookup"><span data-stu-id="92e26-167">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="92e26-168">設定のコンプライアンス状態。</span><span class="sxs-lookup"><span data-stu-id="92e26-168">The compliance state of the setting.</span></span> <span data-ttu-id="92e26-169">可能な値は、`unknown`、`notApplicable`、`compliant`、`remediated`、`nonCompliant`、`error`、`conflict`、`notAssigned` です。</span><span class="sxs-lookup"><span data-stu-id="92e26-169">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="92e26-170">complianceGracePeriodExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="92e26-170">complianceGracePeriodExpirationDateTime</span></span>|<span data-ttu-id="92e26-171">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="92e26-171">DateTimeOffset</span></span>|<span data-ttu-id="92e26-172">デバイス コンプライアンスの猶予期間が過ぎる DateTime</span><span class="sxs-lookup"><span data-stu-id="92e26-172">The DateTime when device compliance grace period expires</span></span>|



## <a name="response"></a><span data-ttu-id="92e26-173">応答</span><span class="sxs-lookup"><span data-stu-id="92e26-173">Response</span></span>
<span data-ttu-id="92e26-174">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で更新された[advancedThreatProtectionOnboardingDeviceSettingState](../resources/intune-deviceconfig-advancedthreatprotectiononboardingdevicesettingstate.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="92e26-174">If successful, this method returns a `200 OK` response code and an updated [advancedThreatProtectionOnboardingDeviceSettingState](../resources/intune-deviceconfig-advancedthreatprotectiononboardingdevicesettingstate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="92e26-175">例</span><span class="sxs-lookup"><span data-stu-id="92e26-175">Example</span></span>

### <a name="request"></a><span data-ttu-id="92e26-176">要求</span><span class="sxs-lookup"><span data-stu-id="92e26-176">Request</span></span>
<span data-ttu-id="92e26-177">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="92e26-177">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/advancedThreatProtectionOnboardingStateSummary/advancedThreatProtectionOnboardingDeviceSettingStates/{advancedThreatProtectionOnboardingDeviceSettingStateId}
Content-type: application/json
Content-length: 573

{
  "@odata.type": "#microsoft.graph.advancedThreatProtectionOnboardingDeviceSettingState",
  "platformType": "windowsRT",
  "setting": "Setting value",
  "settingName": "Setting Name value",
  "deviceId": "Device Id value",
  "deviceName": "Device Name value",
  "userId": "User Id value",
  "userEmail": "User Email value",
  "userName": "User Name value",
  "userPrincipalName": "User Principal Name value",
  "deviceModel": "Device Model value",
  "state": "notApplicable",
  "complianceGracePeriodExpirationDateTime": "2016-12-31T23:56:44.951111-08:00"
}
```

### <a name="response"></a><span data-ttu-id="92e26-178">応答</span><span class="sxs-lookup"><span data-stu-id="92e26-178">Response</span></span>
<span data-ttu-id="92e26-p104">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="92e26-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 622

{
  "@odata.type": "#microsoft.graph.advancedThreatProtectionOnboardingDeviceSettingState",
  "id": "63593fc6-3fc6-6359-c63f-5963c63f5963",
  "platformType": "windowsRT",
  "setting": "Setting value",
  "settingName": "Setting Name value",
  "deviceId": "Device Id value",
  "deviceName": "Device Name value",
  "userId": "User Id value",
  "userEmail": "User Email value",
  "userName": "User Name value",
  "userPrincipalName": "User Principal Name value",
  "deviceModel": "Device Model value",
  "state": "notApplicable",
  "complianceGracePeriodExpirationDateTime": "2016-12-31T23:56:44.951111-08:00"
}
```





