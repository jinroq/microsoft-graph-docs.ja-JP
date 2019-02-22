---
title: advancedThreatProtectionOnboardingDeviceSettingState を作成する
description: 新しい advancedThreatProtectionOnboardingDeviceSettingState オブジェクトを作成します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: d0d37c00522a5f27db84e180035c38cc7d45db48
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/21/2019
ms.locfileid: "30155903"
---
# <a name="create-advancedthreatprotectiononboardingdevicesettingstate"></a><span data-ttu-id="4fbae-103">advancedThreatProtectionOnboardingDeviceSettingState を作成する</span><span class="sxs-lookup"><span data-stu-id="4fbae-103">Create advancedThreatProtectionOnboardingDeviceSettingState</span></span>

> <span data-ttu-id="4fbae-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="4fbae-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4fbae-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="4fbae-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4fbae-106">新しい[advancedThreatProtectionOnboardingDeviceSettingState](../resources/intune-deviceconfig-advancedthreatprotectiononboardingdevicesettingstate.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="4fbae-106">Create a new [advancedThreatProtectionOnboardingDeviceSettingState](../resources/intune-deviceconfig-advancedthreatprotectiononboardingdevicesettingstate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="4fbae-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="4fbae-107">Prerequisites</span></span>
<span data-ttu-id="4fbae-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/concepts/permissions-reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="4fbae-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="4fbae-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="4fbae-110">Permission type</span></span>|<span data-ttu-id="4fbae-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="4fbae-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4fbae-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="4fbae-112">Delegated (work or school account)</span></span>|<span data-ttu-id="4fbae-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4fbae-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="4fbae-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="4fbae-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4fbae-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="4fbae-115">Not supported.</span></span>|
|<span data-ttu-id="4fbae-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="4fbae-116">Application</span></span>|<span data-ttu-id="4fbae-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="4fbae-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="4fbae-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="4fbae-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/advancedThreatProtectionOnboardingStateSummary/advancedThreatProtectionOnboardingDeviceSettingStates
```

## <a name="request-headers"></a><span data-ttu-id="4fbae-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="4fbae-119">Request headers</span></span>
|<span data-ttu-id="4fbae-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="4fbae-120">Header</span></span>|<span data-ttu-id="4fbae-121">値</span><span class="sxs-lookup"><span data-stu-id="4fbae-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4fbae-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="4fbae-122">Authorization</span></span>|<span data-ttu-id="4fbae-123">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="4fbae-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4fbae-124">承諾</span><span class="sxs-lookup"><span data-stu-id="4fbae-124">Accept</span></span>|<span data-ttu-id="4fbae-125">application/json</span><span class="sxs-lookup"><span data-stu-id="4fbae-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4fbae-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="4fbae-126">Request body</span></span>
<span data-ttu-id="4fbae-127">要求本文で、advancedThreatProtectionOnboardingDeviceSettingState オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="4fbae-127">In the request body, supply a JSON representation for the advancedThreatProtectionOnboardingDeviceSettingState object.</span></span>

<span data-ttu-id="4fbae-128">次の表に、advancedThreatProtectionOnboardingDeviceSettingState の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="4fbae-128">The following table shows the properties that are required when you create the advancedThreatProtectionOnboardingDeviceSettingState.</span></span>

|<span data-ttu-id="4fbae-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="4fbae-129">Property</span></span>|<span data-ttu-id="4fbae-130">型</span><span class="sxs-lookup"><span data-stu-id="4fbae-130">Type</span></span>|<span data-ttu-id="4fbae-131">説明</span><span class="sxs-lookup"><span data-stu-id="4fbae-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4fbae-132">id</span><span class="sxs-lookup"><span data-stu-id="4fbae-132">id</span></span>|<span data-ttu-id="4fbae-133">String</span><span class="sxs-lookup"><span data-stu-id="4fbae-133">String</span></span>|<span data-ttu-id="4fbae-134">エンティティのキー</span><span class="sxs-lookup"><span data-stu-id="4fbae-134">Key of the entity</span></span>|
|<span data-ttu-id="4fbae-135">platformType</span><span class="sxs-lookup"><span data-stu-id="4fbae-135">platformType</span></span>|[<span data-ttu-id="4fbae-136">deviceType</span><span class="sxs-lookup"><span data-stu-id="4fbae-136">deviceType</span></span>](../resources/intune-shared-devicetype.md)|<span data-ttu-id="4fbae-137">デバイスプラットフォームの種類。</span><span class="sxs-lookup"><span data-stu-id="4fbae-137">Device platform type.</span></span> <span data-ttu-id="4fbae-138">可能な値: `desktop`、 `windowsRT` `winMO6` `nokia` `windowsPhone` `mac` `winCE` `winEmbedded` `iPhone` `iPad` `iPod` `android`、、、、、、、、、、、、 `iSocConsumer` `unix` `macMDM` `holoLens` `surfaceHub` `androidForWork` `androidEnterprise`, `blackberry`, `palm`, `unknown`.</span><span class="sxs-lookup"><span data-stu-id="4fbae-138">Possible values are: `desktop`, `windowsRT`, `winMO6`, `nokia`, `windowsPhone`, `mac`, `winCE`, `winEmbedded`, `iPhone`, `iPad`, `iPod`, `android`, `iSocConsumer`, `unix`, `macMDM`, `holoLens`, `surfaceHub`, `androidForWork`, `androidEnterprise`, `blackberry`, `palm`, `unknown`.</span></span>|
|<span data-ttu-id="4fbae-139">setting</span><span class="sxs-lookup"><span data-stu-id="4fbae-139">setting</span></span>|<span data-ttu-id="4fbae-140">String</span><span class="sxs-lookup"><span data-stu-id="4fbae-140">String</span></span>|<span data-ttu-id="4fbae-141">設定のクラス名とプロパティ名。</span><span class="sxs-lookup"><span data-stu-id="4fbae-141">The setting class name and property name.</span></span>|
|<span data-ttu-id="4fbae-142">settingName</span><span class="sxs-lookup"><span data-stu-id="4fbae-142">settingName</span></span>|<span data-ttu-id="4fbae-143">String</span><span class="sxs-lookup"><span data-stu-id="4fbae-143">String</span></span>|<span data-ttu-id="4fbae-144">レポートされている設定名。</span><span class="sxs-lookup"><span data-stu-id="4fbae-144">The Setting Name that is being reported</span></span>|
|<span data-ttu-id="4fbae-145">deviceId</span><span class="sxs-lookup"><span data-stu-id="4fbae-145">deviceId</span></span>|<span data-ttu-id="4fbae-146">String</span><span class="sxs-lookup"><span data-stu-id="4fbae-146">String</span></span>|<span data-ttu-id="4fbae-147">レポートされているデバイス ID。</span><span class="sxs-lookup"><span data-stu-id="4fbae-147">The Device Id that is being reported</span></span>|
|<span data-ttu-id="4fbae-148">deviceName</span><span class="sxs-lookup"><span data-stu-id="4fbae-148">deviceName</span></span>|<span data-ttu-id="4fbae-149">String</span><span class="sxs-lookup"><span data-stu-id="4fbae-149">String</span></span>|<span data-ttu-id="4fbae-150">レポートされているデバイス名。</span><span class="sxs-lookup"><span data-stu-id="4fbae-150">The Device Name that is being reported</span></span>|
|<span data-ttu-id="4fbae-151">userId</span><span class="sxs-lookup"><span data-stu-id="4fbae-151">userId</span></span>|<span data-ttu-id="4fbae-152">String</span><span class="sxs-lookup"><span data-stu-id="4fbae-152">String</span></span>|<span data-ttu-id="4fbae-153">レポートされているユーザー ID</span><span class="sxs-lookup"><span data-stu-id="4fbae-153">The user Id that is being reported</span></span>|
|<span data-ttu-id="4fbae-154">userEmail</span><span class="sxs-lookup"><span data-stu-id="4fbae-154">userEmail</span></span>|<span data-ttu-id="4fbae-155">String</span><span class="sxs-lookup"><span data-stu-id="4fbae-155">String</span></span>|<span data-ttu-id="4fbae-156">レポートされているユーザーのメール アドレス。</span><span class="sxs-lookup"><span data-stu-id="4fbae-156">The User email address that is being reported</span></span>|
|<span data-ttu-id="4fbae-157">userName</span><span class="sxs-lookup"><span data-stu-id="4fbae-157">userName</span></span>|<span data-ttu-id="4fbae-158">String</span><span class="sxs-lookup"><span data-stu-id="4fbae-158">String</span></span>|<span data-ttu-id="4fbae-159">レポートされているユーザー名</span><span class="sxs-lookup"><span data-stu-id="4fbae-159">The User Name that is being reported</span></span>|
|<span data-ttu-id="4fbae-160">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="4fbae-160">userPrincipalName</span></span>|<span data-ttu-id="4fbae-161">String</span><span class="sxs-lookup"><span data-stu-id="4fbae-161">String</span></span>|<span data-ttu-id="4fbae-162">レポートされているユーザーの PrincipalName</span><span class="sxs-lookup"><span data-stu-id="4fbae-162">The User PrincipalName that is being reported</span></span>|
|<span data-ttu-id="4fbae-163">deviceModel</span><span class="sxs-lookup"><span data-stu-id="4fbae-163">deviceModel</span></span>|<span data-ttu-id="4fbae-164">String</span><span class="sxs-lookup"><span data-stu-id="4fbae-164">String</span></span>|<span data-ttu-id="4fbae-165">レポートされているデバイス モデル</span><span class="sxs-lookup"><span data-stu-id="4fbae-165">The device model that is being reported</span></span>|
|<span data-ttu-id="4fbae-166">state</span><span class="sxs-lookup"><span data-stu-id="4fbae-166">state</span></span>|[<span data-ttu-id="4fbae-167">complianceStatus</span><span class="sxs-lookup"><span data-stu-id="4fbae-167">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="4fbae-168">設定のコンプライアンス状態。</span><span class="sxs-lookup"><span data-stu-id="4fbae-168">The compliance state of the setting.</span></span> <span data-ttu-id="4fbae-169">可能な値は、`unknown`、`notApplicable`、`compliant`、`remediated`、`nonCompliant`、`error`、`conflict`、`notAssigned` です。</span><span class="sxs-lookup"><span data-stu-id="4fbae-169">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="4fbae-170">complianceGracePeriodExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="4fbae-170">complianceGracePeriodExpirationDateTime</span></span>|<span data-ttu-id="4fbae-171">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4fbae-171">DateTimeOffset</span></span>|<span data-ttu-id="4fbae-172">デバイス コンプライアンスの猶予期間が過ぎる DateTime</span><span class="sxs-lookup"><span data-stu-id="4fbae-172">The DateTime when device compliance grace period expires</span></span>|



## <a name="response"></a><span data-ttu-id="4fbae-173">応答</span><span class="sxs-lookup"><span data-stu-id="4fbae-173">Response</span></span>
<span data-ttu-id="4fbae-174">成功した場合、このメソッド`201 Created`は応答コードと、応答本文で[advancedThreatProtectionOnboardingDeviceSettingState](../resources/intune-deviceconfig-advancedthreatprotectiononboardingdevicesettingstate.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="4fbae-174">If successful, this method returns a `201 Created` response code and a [advancedThreatProtectionOnboardingDeviceSettingState](../resources/intune-deviceconfig-advancedthreatprotectiononboardingdevicesettingstate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4fbae-175">例</span><span class="sxs-lookup"><span data-stu-id="4fbae-175">Example</span></span>

### <a name="request"></a><span data-ttu-id="4fbae-176">要求</span><span class="sxs-lookup"><span data-stu-id="4fbae-176">Request</span></span>
<span data-ttu-id="4fbae-177">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="4fbae-177">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/advancedThreatProtectionOnboardingStateSummary/advancedThreatProtectionOnboardingDeviceSettingStates
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

### <a name="response"></a><span data-ttu-id="4fbae-178">応答</span><span class="sxs-lookup"><span data-stu-id="4fbae-178">Response</span></span>
<span data-ttu-id="4fbae-p104">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="4fbae-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




