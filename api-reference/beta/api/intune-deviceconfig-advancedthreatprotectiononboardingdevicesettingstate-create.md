---
title: AdvancedThreatProtectionOnboardingDeviceSettingState を作成します。
description: 新しい advancedThreatProtectionOnboardingDeviceSettingState オブジェクトを作成します。
ms.openlocfilehash: 623db746a44792f80255b1f76d3d92fca0ab30cb
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27070607"
---
# <a name="create-advancedthreatprotectiononboardingdevicesettingstate"></a><span data-ttu-id="1ada3-103">AdvancedThreatProtectionOnboardingDeviceSettingState を作成します。</span><span class="sxs-lookup"><span data-stu-id="1ada3-103">Create advancedThreatProtectionOnboardingDeviceSettingState</span></span>

> <span data-ttu-id="1ada3-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="1ada3-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="1ada3-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="1ada3-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="1ada3-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="1ada3-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="1ada3-107">新しい[advancedThreatProtectionOnboardingDeviceSettingState](../resources/intune-deviceconfig-advancedthreatprotectiononboardingdevicesettingstate.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="1ada3-107">Create a new [advancedThreatProtectionOnboardingDeviceSettingState](../resources/intune-deviceconfig-advancedthreatprotectiononboardingdevicesettingstate.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="1ada3-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="1ada3-108">Prerequisites</span></span>
<span data-ttu-id="1ada3-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="1ada3-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1ada3-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="1ada3-111">Permission type</span></span>|<span data-ttu-id="1ada3-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="1ada3-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1ada3-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="1ada3-113">Delegated (work or school account)</span></span>|<span data-ttu-id="1ada3-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1ada3-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="1ada3-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="1ada3-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1ada3-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="1ada3-116">Not supported.</span></span>|
|<span data-ttu-id="1ada3-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="1ada3-117">Application</span></span>|<span data-ttu-id="1ada3-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="1ada3-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="1ada3-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="1ada3-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/advancedThreatProtectionOnboardingStateSummary/advancedThreatProtectionOnboardingDeviceSettingStates
```

## <a name="request-headers"></a><span data-ttu-id="1ada3-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="1ada3-120">Request headers</span></span>
|<span data-ttu-id="1ada3-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="1ada3-121">Header</span></span>|<span data-ttu-id="1ada3-122">値</span><span class="sxs-lookup"><span data-stu-id="1ada3-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1ada3-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="1ada3-123">Authorization</span></span>|<span data-ttu-id="1ada3-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="1ada3-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1ada3-125">Accept</span><span class="sxs-lookup"><span data-stu-id="1ada3-125">Accept</span></span>|<span data-ttu-id="1ada3-126">application/json</span><span class="sxs-lookup"><span data-stu-id="1ada3-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1ada3-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="1ada3-127">Request body</span></span>
<span data-ttu-id="1ada3-128">要求の本文に advancedThreatProtectionOnboardingDeviceSettingState オブジェクトの JSON の形式を指定します。</span><span class="sxs-lookup"><span data-stu-id="1ada3-128">In the request body, supply a JSON representation for the advancedThreatProtectionOnboardingDeviceSettingState object.</span></span>

<span data-ttu-id="1ada3-129">次の表は、advancedThreatProtectionOnboardingDeviceSettingState を作成するときに必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="1ada3-129">The following table shows the properties that are required when you create the advancedThreatProtectionOnboardingDeviceSettingState.</span></span>

|<span data-ttu-id="1ada3-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="1ada3-130">Property</span></span>|<span data-ttu-id="1ada3-131">型</span><span class="sxs-lookup"><span data-stu-id="1ada3-131">Type</span></span>|<span data-ttu-id="1ada3-132">説明</span><span class="sxs-lookup"><span data-stu-id="1ada3-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1ada3-133">id</span><span class="sxs-lookup"><span data-stu-id="1ada3-133">id</span></span>|<span data-ttu-id="1ada3-134">String</span><span class="sxs-lookup"><span data-stu-id="1ada3-134">String</span></span>|<span data-ttu-id="1ada3-135">エンティティのキー</span><span class="sxs-lookup"><span data-stu-id="1ada3-135">Key of the entity</span></span>|
|<span data-ttu-id="1ada3-136">platformType</span><span class="sxs-lookup"><span data-stu-id="1ada3-136">platformType</span></span>|[<span data-ttu-id="1ada3-137">deviceType</span><span class="sxs-lookup"><span data-stu-id="1ada3-137">deviceType</span></span>](../resources/intune-shared-devicetype.md)|<span data-ttu-id="1ada3-138">デバイス プラットフォームのタイプです。</span><span class="sxs-lookup"><span data-stu-id="1ada3-138">Device platform type.</span></span> <span data-ttu-id="1ada3-139">使用可能な値: `desktop`、 `windowsRT`、 `winMO6`、 `nokia`、 `windowsPhone`、 `mac`、 `winCE`、 `winEmbedded`、 `iPhone`、 `iPad`、 `iPod`、 `android`、 `iSocConsumer`、 `unix`、 `macMDM`、 `holoLens`、 `surfaceHub`、 `androidForWork`、 `androidEnterprise`, `blackberry`, `palm`, `unknown`.</span><span class="sxs-lookup"><span data-stu-id="1ada3-139">Possible values are: `desktop`, `windowsRT`, `winMO6`, `nokia`, `windowsPhone`, `mac`, `winCE`, `winEmbedded`, `iPhone`, `iPad`, `iPod`, `android`, `iSocConsumer`, `unix`, `macMDM`, `holoLens`, `surfaceHub`, `androidForWork`, `androidEnterprise`, `blackberry`, `palm`, `unknown`.</span></span>|
|<span data-ttu-id="1ada3-140">setting</span><span class="sxs-lookup"><span data-stu-id="1ada3-140">setting</span></span>|<span data-ttu-id="1ada3-141">String</span><span class="sxs-lookup"><span data-stu-id="1ada3-141">String</span></span>|<span data-ttu-id="1ada3-142">設定のクラス名とプロパティ名。</span><span class="sxs-lookup"><span data-stu-id="1ada3-142">The setting class name and property name.</span></span>|
|<span data-ttu-id="1ada3-143">settingName</span><span class="sxs-lookup"><span data-stu-id="1ada3-143">settingName</span></span>|<span data-ttu-id="1ada3-144">String</span><span class="sxs-lookup"><span data-stu-id="1ada3-144">String</span></span>|<span data-ttu-id="1ada3-145">レポートされている設定名。</span><span class="sxs-lookup"><span data-stu-id="1ada3-145">The Setting Name that is being reported</span></span>|
|<span data-ttu-id="1ada3-146">deviceId</span><span class="sxs-lookup"><span data-stu-id="1ada3-146">deviceId</span></span>|<span data-ttu-id="1ada3-147">String</span><span class="sxs-lookup"><span data-stu-id="1ada3-147">String</span></span>|<span data-ttu-id="1ada3-148">レポートされているデバイス ID。</span><span class="sxs-lookup"><span data-stu-id="1ada3-148">The Device Id that is being reported</span></span>|
|<span data-ttu-id="1ada3-149">deviceName</span><span class="sxs-lookup"><span data-stu-id="1ada3-149">deviceName</span></span>|<span data-ttu-id="1ada3-150">String</span><span class="sxs-lookup"><span data-stu-id="1ada3-150">String</span></span>|<span data-ttu-id="1ada3-151">レポートされているデバイス名。</span><span class="sxs-lookup"><span data-stu-id="1ada3-151">The Device Name that is being reported</span></span>|
|<span data-ttu-id="1ada3-152">userId</span><span class="sxs-lookup"><span data-stu-id="1ada3-152">userId</span></span>|<span data-ttu-id="1ada3-153">String</span><span class="sxs-lookup"><span data-stu-id="1ada3-153">String</span></span>|<span data-ttu-id="1ada3-154">レポートされているユーザー ID</span><span class="sxs-lookup"><span data-stu-id="1ada3-154">The user Id that is being reported</span></span>|
|<span data-ttu-id="1ada3-155">userEmail</span><span class="sxs-lookup"><span data-stu-id="1ada3-155">userEmail</span></span>|<span data-ttu-id="1ada3-156">String</span><span class="sxs-lookup"><span data-stu-id="1ada3-156">String</span></span>|<span data-ttu-id="1ada3-157">レポートされているユーザーのメール アドレス。</span><span class="sxs-lookup"><span data-stu-id="1ada3-157">The User email address that is being reported</span></span>|
|<span data-ttu-id="1ada3-158">userName</span><span class="sxs-lookup"><span data-stu-id="1ada3-158">userName</span></span>|<span data-ttu-id="1ada3-159">String</span><span class="sxs-lookup"><span data-stu-id="1ada3-159">String</span></span>|<span data-ttu-id="1ada3-160">レポートされているユーザー名</span><span class="sxs-lookup"><span data-stu-id="1ada3-160">The User Name that is being reported</span></span>|
|<span data-ttu-id="1ada3-161">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="1ada3-161">userPrincipalName</span></span>|<span data-ttu-id="1ada3-162">String</span><span class="sxs-lookup"><span data-stu-id="1ada3-162">String</span></span>|<span data-ttu-id="1ada3-163">レポートされているユーザーの PrincipalName</span><span class="sxs-lookup"><span data-stu-id="1ada3-163">The User PrincipalName that is being reported</span></span>|
|<span data-ttu-id="1ada3-164">deviceModel</span><span class="sxs-lookup"><span data-stu-id="1ada3-164">deviceModel</span></span>|<span data-ttu-id="1ada3-165">String</span><span class="sxs-lookup"><span data-stu-id="1ada3-165">String</span></span>|<span data-ttu-id="1ada3-166">レポートされているデバイス モデル</span><span class="sxs-lookup"><span data-stu-id="1ada3-166">The device model that is being reported</span></span>|
|<span data-ttu-id="1ada3-167">state</span><span class="sxs-lookup"><span data-stu-id="1ada3-167">state</span></span>|[<span data-ttu-id="1ada3-168">complianceStatus</span><span class="sxs-lookup"><span data-stu-id="1ada3-168">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="1ada3-169">設定のコンプライアンスの状態です。</span><span class="sxs-lookup"><span data-stu-id="1ada3-169">The compliance state of the setting.</span></span> <span data-ttu-id="1ada3-170">可能な値は、`unknown`、`notApplicable`、`compliant`、`remediated`、`nonCompliant`、`error`、`conflict`、`notAssigned` です。</span><span class="sxs-lookup"><span data-stu-id="1ada3-170">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="1ada3-171">complianceGracePeriodExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="1ada3-171">complianceGracePeriodExpirationDateTime</span></span>|<span data-ttu-id="1ada3-172">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1ada3-172">DateTimeOffset</span></span>|<span data-ttu-id="1ada3-173">デバイス コンプライアンスの猶予期間が過ぎる DateTime</span><span class="sxs-lookup"><span data-stu-id="1ada3-173">The DateTime when device compliance grace period expires</span></span>|



## <a name="response"></a><span data-ttu-id="1ada3-174">応答</span><span class="sxs-lookup"><span data-stu-id="1ada3-174">Response</span></span>
<span data-ttu-id="1ada3-175">かどうかは成功すると、このメソッドが返されます、`201 Created`応答コードおよび応答の本文に[advancedThreatProtectionOnboardingDeviceSettingState](../resources/intune-deviceconfig-advancedthreatprotectiononboardingdevicesettingstate.md)オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="1ada3-175">If successful, this method returns a `201 Created` response code and a [advancedThreatProtectionOnboardingDeviceSettingState](../resources/intune-deviceconfig-advancedthreatprotectiononboardingdevicesettingstate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1ada3-176">例</span><span class="sxs-lookup"><span data-stu-id="1ada3-176">Example</span></span>
### <a name="request"></a><span data-ttu-id="1ada3-177">要求</span><span class="sxs-lookup"><span data-stu-id="1ada3-177">Request</span></span>
<span data-ttu-id="1ada3-178">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="1ada3-178">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="1ada3-179">応答</span><span class="sxs-lookup"><span data-stu-id="1ada3-179">Response</span></span>
<span data-ttu-id="1ada3-p105">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="1ada3-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





