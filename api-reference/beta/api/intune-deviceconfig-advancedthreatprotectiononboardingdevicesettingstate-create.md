---
title: advancedThreatProtectionOnboardingDeviceSettingState を作成する
description: 新しい advancedThreatProtectionOnboardingDeviceSettingState オブジェクトを作成します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: d877edcdc82cee35c7fc75c556ca5ac0035221ad
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/29/2019
ms.locfileid: "30980664"
---
# <a name="create-advancedthreatprotectiononboardingdevicesettingstate"></a><span data-ttu-id="c7c02-103">advancedThreatProtectionOnboardingDeviceSettingState を作成する</span><span class="sxs-lookup"><span data-stu-id="c7c02-103">Create advancedThreatProtectionOnboardingDeviceSettingState</span></span>

> <span data-ttu-id="c7c02-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c7c02-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c7c02-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="c7c02-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c7c02-106">新しい[advancedThreatProtectionOnboardingDeviceSettingState](../resources/intune-deviceconfig-advancedthreatprotectiononboardingdevicesettingstate.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="c7c02-106">Create a new [advancedThreatProtectionOnboardingDeviceSettingState](../resources/intune-deviceconfig-advancedthreatprotectiononboardingdevicesettingstate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c7c02-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="c7c02-107">Prerequisites</span></span>
<span data-ttu-id="c7c02-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="c7c02-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c7c02-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="c7c02-110">Permission type</span></span>|<span data-ttu-id="c7c02-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="c7c02-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c7c02-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="c7c02-112">Delegated (work or school account)</span></span>|<span data-ttu-id="c7c02-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c7c02-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="c7c02-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="c7c02-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c7c02-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c7c02-115">Not supported.</span></span>|
|<span data-ttu-id="c7c02-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="c7c02-116">Application</span></span>|<span data-ttu-id="c7c02-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c7c02-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c7c02-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="c7c02-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/advancedThreatProtectionOnboardingStateSummary/advancedThreatProtectionOnboardingDeviceSettingStates
```

## <a name="request-headers"></a><span data-ttu-id="c7c02-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="c7c02-119">Request headers</span></span>
|<span data-ttu-id="c7c02-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="c7c02-120">Header</span></span>|<span data-ttu-id="c7c02-121">値</span><span class="sxs-lookup"><span data-stu-id="c7c02-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c7c02-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="c7c02-122">Authorization</span></span>|<span data-ttu-id="c7c02-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="c7c02-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c7c02-124">承諾</span><span class="sxs-lookup"><span data-stu-id="c7c02-124">Accept</span></span>|<span data-ttu-id="c7c02-125">application/json</span><span class="sxs-lookup"><span data-stu-id="c7c02-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c7c02-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="c7c02-126">Request body</span></span>
<span data-ttu-id="c7c02-127">要求本文で、advancedThreatProtectionOnboardingDeviceSettingState オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="c7c02-127">In the request body, supply a JSON representation for the advancedThreatProtectionOnboardingDeviceSettingState object.</span></span>

<span data-ttu-id="c7c02-128">次の表に、advancedThreatProtectionOnboardingDeviceSettingState の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="c7c02-128">The following table shows the properties that are required when you create the advancedThreatProtectionOnboardingDeviceSettingState.</span></span>

|<span data-ttu-id="c7c02-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="c7c02-129">Property</span></span>|<span data-ttu-id="c7c02-130">型</span><span class="sxs-lookup"><span data-stu-id="c7c02-130">Type</span></span>|<span data-ttu-id="c7c02-131">説明</span><span class="sxs-lookup"><span data-stu-id="c7c02-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c7c02-132">id</span><span class="sxs-lookup"><span data-stu-id="c7c02-132">id</span></span>|<span data-ttu-id="c7c02-133">String</span><span class="sxs-lookup"><span data-stu-id="c7c02-133">String</span></span>|<span data-ttu-id="c7c02-134">エンティティのキー</span><span class="sxs-lookup"><span data-stu-id="c7c02-134">Key of the entity</span></span>|
|<span data-ttu-id="c7c02-135">platformType</span><span class="sxs-lookup"><span data-stu-id="c7c02-135">platformType</span></span>|[<span data-ttu-id="c7c02-136">deviceType</span><span class="sxs-lookup"><span data-stu-id="c7c02-136">deviceType</span></span>](../resources/intune-shared-devicetype.md)|<span data-ttu-id="c7c02-137">デバイスプラットフォームの種類。</span><span class="sxs-lookup"><span data-stu-id="c7c02-137">Device platform type.</span></span> <span data-ttu-id="c7c02-138">可能な値: `desktop`、 `windowsRT` `winMO6` `nokia` `windowsPhone` `mac` `winCE` `winEmbedded` `iPhone` `iPad` `iPod` `android`、、、、、、、、、、、、 `iSocConsumer` `unix` `macMDM` `holoLens` `surfaceHub` `androidForWork` `androidEnterprise`, `blackberry`, `palm`, `unknown`.</span><span class="sxs-lookup"><span data-stu-id="c7c02-138">Possible values are: `desktop`, `windowsRT`, `winMO6`, `nokia`, `windowsPhone`, `mac`, `winCE`, `winEmbedded`, `iPhone`, `iPad`, `iPod`, `android`, `iSocConsumer`, `unix`, `macMDM`, `holoLens`, `surfaceHub`, `androidForWork`, `androidEnterprise`, `blackberry`, `palm`, `unknown`.</span></span>|
|<span data-ttu-id="c7c02-139">setting</span><span class="sxs-lookup"><span data-stu-id="c7c02-139">setting</span></span>|<span data-ttu-id="c7c02-140">String</span><span class="sxs-lookup"><span data-stu-id="c7c02-140">String</span></span>|<span data-ttu-id="c7c02-141">設定のクラス名とプロパティ名。</span><span class="sxs-lookup"><span data-stu-id="c7c02-141">The setting class name and property name.</span></span>|
|<span data-ttu-id="c7c02-142">settingName</span><span class="sxs-lookup"><span data-stu-id="c7c02-142">settingName</span></span>|<span data-ttu-id="c7c02-143">String</span><span class="sxs-lookup"><span data-stu-id="c7c02-143">String</span></span>|<span data-ttu-id="c7c02-144">レポートされている設定名。</span><span class="sxs-lookup"><span data-stu-id="c7c02-144">The Setting Name that is being reported</span></span>|
|<span data-ttu-id="c7c02-145">deviceId</span><span class="sxs-lookup"><span data-stu-id="c7c02-145">deviceId</span></span>|<span data-ttu-id="c7c02-146">String</span><span class="sxs-lookup"><span data-stu-id="c7c02-146">String</span></span>|<span data-ttu-id="c7c02-147">レポートされているデバイス ID。</span><span class="sxs-lookup"><span data-stu-id="c7c02-147">The Device Id that is being reported</span></span>|
|<span data-ttu-id="c7c02-148">deviceName</span><span class="sxs-lookup"><span data-stu-id="c7c02-148">deviceName</span></span>|<span data-ttu-id="c7c02-149">String</span><span class="sxs-lookup"><span data-stu-id="c7c02-149">String</span></span>|<span data-ttu-id="c7c02-150">レポートされているデバイス名。</span><span class="sxs-lookup"><span data-stu-id="c7c02-150">The Device Name that is being reported</span></span>|
|<span data-ttu-id="c7c02-151">userId</span><span class="sxs-lookup"><span data-stu-id="c7c02-151">userId</span></span>|<span data-ttu-id="c7c02-152">String</span><span class="sxs-lookup"><span data-stu-id="c7c02-152">String</span></span>|<span data-ttu-id="c7c02-153">レポートされているユーザー ID</span><span class="sxs-lookup"><span data-stu-id="c7c02-153">The user Id that is being reported</span></span>|
|<span data-ttu-id="c7c02-154">userEmail</span><span class="sxs-lookup"><span data-stu-id="c7c02-154">userEmail</span></span>|<span data-ttu-id="c7c02-155">String</span><span class="sxs-lookup"><span data-stu-id="c7c02-155">String</span></span>|<span data-ttu-id="c7c02-156">レポートされているユーザーのメール アドレス。</span><span class="sxs-lookup"><span data-stu-id="c7c02-156">The User email address that is being reported</span></span>|
|<span data-ttu-id="c7c02-157">userName</span><span class="sxs-lookup"><span data-stu-id="c7c02-157">userName</span></span>|<span data-ttu-id="c7c02-158">String</span><span class="sxs-lookup"><span data-stu-id="c7c02-158">String</span></span>|<span data-ttu-id="c7c02-159">レポートされているユーザー名</span><span class="sxs-lookup"><span data-stu-id="c7c02-159">The User Name that is being reported</span></span>|
|<span data-ttu-id="c7c02-160">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="c7c02-160">userPrincipalName</span></span>|<span data-ttu-id="c7c02-161">String</span><span class="sxs-lookup"><span data-stu-id="c7c02-161">String</span></span>|<span data-ttu-id="c7c02-162">レポートされているユーザーの PrincipalName</span><span class="sxs-lookup"><span data-stu-id="c7c02-162">The User PrincipalName that is being reported</span></span>|
|<span data-ttu-id="c7c02-163">deviceModel</span><span class="sxs-lookup"><span data-stu-id="c7c02-163">deviceModel</span></span>|<span data-ttu-id="c7c02-164">String</span><span class="sxs-lookup"><span data-stu-id="c7c02-164">String</span></span>|<span data-ttu-id="c7c02-165">レポートされているデバイス モデル</span><span class="sxs-lookup"><span data-stu-id="c7c02-165">The device model that is being reported</span></span>|
|<span data-ttu-id="c7c02-166">state</span><span class="sxs-lookup"><span data-stu-id="c7c02-166">state</span></span>|[<span data-ttu-id="c7c02-167">complianceStatus</span><span class="sxs-lookup"><span data-stu-id="c7c02-167">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="c7c02-168">設定のコンプライアンス状態。</span><span class="sxs-lookup"><span data-stu-id="c7c02-168">The compliance state of the setting.</span></span> <span data-ttu-id="c7c02-169">可能な値は、`unknown`、`notApplicable`、`compliant`、`remediated`、`nonCompliant`、`error`、`conflict`、`notAssigned` です。</span><span class="sxs-lookup"><span data-stu-id="c7c02-169">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="c7c02-170">complianceGracePeriodExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="c7c02-170">complianceGracePeriodExpirationDateTime</span></span>|<span data-ttu-id="c7c02-171">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c7c02-171">DateTimeOffset</span></span>|<span data-ttu-id="c7c02-172">デバイス コンプライアンスの猶予期間が過ぎる DateTime</span><span class="sxs-lookup"><span data-stu-id="c7c02-172">The DateTime when device compliance grace period expires</span></span>|



## <a name="response"></a><span data-ttu-id="c7c02-173">応答</span><span class="sxs-lookup"><span data-stu-id="c7c02-173">Response</span></span>
<span data-ttu-id="c7c02-174">成功した場合、このメソッド`201 Created`は応答コードと、応答本文で[advancedThreatProtectionOnboardingDeviceSettingState](../resources/intune-deviceconfig-advancedthreatprotectiononboardingdevicesettingstate.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="c7c02-174">If successful, this method returns a `201 Created` response code and a [advancedThreatProtectionOnboardingDeviceSettingState](../resources/intune-deviceconfig-advancedthreatprotectiononboardingdevicesettingstate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c7c02-175">例</span><span class="sxs-lookup"><span data-stu-id="c7c02-175">Example</span></span>

### <a name="request"></a><span data-ttu-id="c7c02-176">要求</span><span class="sxs-lookup"><span data-stu-id="c7c02-176">Request</span></span>
<span data-ttu-id="c7c02-177">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="c7c02-177">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="c7c02-178">応答</span><span class="sxs-lookup"><span data-stu-id="c7c02-178">Response</span></span>
<span data-ttu-id="c7c02-p104">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="c7c02-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




