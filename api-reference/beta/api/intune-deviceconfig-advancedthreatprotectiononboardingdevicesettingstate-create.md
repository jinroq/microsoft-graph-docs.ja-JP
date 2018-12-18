---
title: AdvancedThreatProtectionOnboardingDeviceSettingState を作成します。
description: 新しい advancedThreatProtectionOnboardingDeviceSettingState オブジェクトを作成します。
author: tfitzmac
ms.openlocfilehash: 221ecef8a9aebdd7a04ec889ff2a04d524ac05d7
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27342953"
---
# <a name="create-advancedthreatprotectiononboardingdevicesettingstate"></a><span data-ttu-id="c8bd0-103">AdvancedThreatProtectionOnboardingDeviceSettingState を作成します。</span><span class="sxs-lookup"><span data-stu-id="c8bd0-103">Create advancedThreatProtectionOnboardingDeviceSettingState</span></span>

> <span data-ttu-id="c8bd0-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="c8bd0-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c8bd0-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c8bd0-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="c8bd0-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="c8bd0-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="c8bd0-107">新しい[advancedThreatProtectionOnboardingDeviceSettingState](../resources/intune-deviceconfig-advancedthreatprotectiononboardingdevicesettingstate.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="c8bd0-107">Create a new [advancedThreatProtectionOnboardingDeviceSettingState](../resources/intune-deviceconfig-advancedthreatprotectiononboardingdevicesettingstate.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="c8bd0-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="c8bd0-108">Prerequisites</span></span>
<span data-ttu-id="c8bd0-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="c8bd0-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c8bd0-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="c8bd0-111">Permission type</span></span>|<span data-ttu-id="c8bd0-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="c8bd0-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c8bd0-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="c8bd0-113">Delegated (work or school account)</span></span>|<span data-ttu-id="c8bd0-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c8bd0-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="c8bd0-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="c8bd0-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c8bd0-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c8bd0-116">Not supported.</span></span>|
|<span data-ttu-id="c8bd0-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="c8bd0-117">Application</span></span>|<span data-ttu-id="c8bd0-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c8bd0-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c8bd0-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="c8bd0-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/advancedThreatProtectionOnboardingStateSummary/advancedThreatProtectionOnboardingDeviceSettingStates
```

## <a name="request-headers"></a><span data-ttu-id="c8bd0-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="c8bd0-120">Request headers</span></span>
|<span data-ttu-id="c8bd0-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="c8bd0-121">Header</span></span>|<span data-ttu-id="c8bd0-122">値</span><span class="sxs-lookup"><span data-stu-id="c8bd0-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c8bd0-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="c8bd0-123">Authorization</span></span>|<span data-ttu-id="c8bd0-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="c8bd0-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c8bd0-125">Accept</span><span class="sxs-lookup"><span data-stu-id="c8bd0-125">Accept</span></span>|<span data-ttu-id="c8bd0-126">application/json</span><span class="sxs-lookup"><span data-stu-id="c8bd0-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c8bd0-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="c8bd0-127">Request body</span></span>
<span data-ttu-id="c8bd0-128">要求の本文に advancedThreatProtectionOnboardingDeviceSettingState オブジェクトの JSON の形式を指定します。</span><span class="sxs-lookup"><span data-stu-id="c8bd0-128">In the request body, supply a JSON representation for the advancedThreatProtectionOnboardingDeviceSettingState object.</span></span>

<span data-ttu-id="c8bd0-129">次の表は、advancedThreatProtectionOnboardingDeviceSettingState を作成するときに必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="c8bd0-129">The following table shows the properties that are required when you create the advancedThreatProtectionOnboardingDeviceSettingState.</span></span>

|<span data-ttu-id="c8bd0-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="c8bd0-130">Property</span></span>|<span data-ttu-id="c8bd0-131">種類</span><span class="sxs-lookup"><span data-stu-id="c8bd0-131">Type</span></span>|<span data-ttu-id="c8bd0-132">説明</span><span class="sxs-lookup"><span data-stu-id="c8bd0-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c8bd0-133">ID</span><span class="sxs-lookup"><span data-stu-id="c8bd0-133">id</span></span>|<span data-ttu-id="c8bd0-134">String</span><span class="sxs-lookup"><span data-stu-id="c8bd0-134">String</span></span>|<span data-ttu-id="c8bd0-135">エンティティのキー</span><span class="sxs-lookup"><span data-stu-id="c8bd0-135">Key of the entity</span></span>|
|<span data-ttu-id="c8bd0-136">platformType</span><span class="sxs-lookup"><span data-stu-id="c8bd0-136">platformType</span></span>|[<span data-ttu-id="c8bd0-137">deviceType</span><span class="sxs-lookup"><span data-stu-id="c8bd0-137">deviceType</span></span>](../resources/intune-shared-devicetype.md)|<span data-ttu-id="c8bd0-138">デバイス プラットフォームのタイプです。</span><span class="sxs-lookup"><span data-stu-id="c8bd0-138">Device platform type.</span></span> <span data-ttu-id="c8bd0-139">使用可能な値: `desktop`、 `windowsRT`、 `winMO6`、 `nokia`、 `windowsPhone`、 `mac`、 `winCE`、 `winEmbedded`、 `iPhone`、 `iPad`、 `iPod`、 `android`、 `iSocConsumer`、 `unix`、 `macMDM`、 `holoLens`、 `surfaceHub`、 `androidForWork`、 `androidEnterprise`, `blackberry`, `palm`, `unknown`.</span><span class="sxs-lookup"><span data-stu-id="c8bd0-139">Possible values are: `desktop`, `windowsRT`, `winMO6`, `nokia`, `windowsPhone`, `mac`, `winCE`, `winEmbedded`, `iPhone`, `iPad`, `iPod`, `android`, `iSocConsumer`, `unix`, `macMDM`, `holoLens`, `surfaceHub`, `androidForWork`, `androidEnterprise`, `blackberry`, `palm`, `unknown`.</span></span>|
|<span data-ttu-id="c8bd0-140">setting</span><span class="sxs-lookup"><span data-stu-id="c8bd0-140">setting</span></span>|<span data-ttu-id="c8bd0-141">String</span><span class="sxs-lookup"><span data-stu-id="c8bd0-141">String</span></span>|<span data-ttu-id="c8bd0-142">設定のクラス名とプロパティ名。</span><span class="sxs-lookup"><span data-stu-id="c8bd0-142">The setting class name and property name.</span></span>|
|<span data-ttu-id="c8bd0-143">settingName</span><span class="sxs-lookup"><span data-stu-id="c8bd0-143">settingName</span></span>|<span data-ttu-id="c8bd0-144">String</span><span class="sxs-lookup"><span data-stu-id="c8bd0-144">String</span></span>|<span data-ttu-id="c8bd0-145">レポートされている設定名。</span><span class="sxs-lookup"><span data-stu-id="c8bd0-145">The Setting Name that is being reported</span></span>|
|<span data-ttu-id="c8bd0-146">deviceId</span><span class="sxs-lookup"><span data-stu-id="c8bd0-146">deviceId</span></span>|<span data-ttu-id="c8bd0-147">String</span><span class="sxs-lookup"><span data-stu-id="c8bd0-147">String</span></span>|<span data-ttu-id="c8bd0-148">レポートされているデバイス ID。</span><span class="sxs-lookup"><span data-stu-id="c8bd0-148">The Device Id that is being reported</span></span>|
|<span data-ttu-id="c8bd0-149">deviceName</span><span class="sxs-lookup"><span data-stu-id="c8bd0-149">deviceName</span></span>|<span data-ttu-id="c8bd0-150">String</span><span class="sxs-lookup"><span data-stu-id="c8bd0-150">String</span></span>|<span data-ttu-id="c8bd0-151">レポートされているデバイス名。</span><span class="sxs-lookup"><span data-stu-id="c8bd0-151">The Device Name that is being reported</span></span>|
|<span data-ttu-id="c8bd0-152">userId</span><span class="sxs-lookup"><span data-stu-id="c8bd0-152">userId</span></span>|<span data-ttu-id="c8bd0-153">String</span><span class="sxs-lookup"><span data-stu-id="c8bd0-153">String</span></span>|<span data-ttu-id="c8bd0-154">レポートされているユーザー ID</span><span class="sxs-lookup"><span data-stu-id="c8bd0-154">The user Id that is being reported</span></span>|
|<span data-ttu-id="c8bd0-155">userEmail</span><span class="sxs-lookup"><span data-stu-id="c8bd0-155">userEmail</span></span>|<span data-ttu-id="c8bd0-156">String</span><span class="sxs-lookup"><span data-stu-id="c8bd0-156">String</span></span>|<span data-ttu-id="c8bd0-157">レポートされているユーザーのメール アドレス。</span><span class="sxs-lookup"><span data-stu-id="c8bd0-157">The User email address that is being reported</span></span>|
|<span data-ttu-id="c8bd0-158">userName</span><span class="sxs-lookup"><span data-stu-id="c8bd0-158">userName</span></span>|<span data-ttu-id="c8bd0-159">String</span><span class="sxs-lookup"><span data-stu-id="c8bd0-159">String</span></span>|<span data-ttu-id="c8bd0-160">レポートされているユーザー名</span><span class="sxs-lookup"><span data-stu-id="c8bd0-160">The User Name that is being reported</span></span>|
|<span data-ttu-id="c8bd0-161">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="c8bd0-161">userPrincipalName</span></span>|<span data-ttu-id="c8bd0-162">String</span><span class="sxs-lookup"><span data-stu-id="c8bd0-162">String</span></span>|<span data-ttu-id="c8bd0-163">レポートされているユーザーの PrincipalName</span><span class="sxs-lookup"><span data-stu-id="c8bd0-163">The User PrincipalName that is being reported</span></span>|
|<span data-ttu-id="c8bd0-164">deviceModel</span><span class="sxs-lookup"><span data-stu-id="c8bd0-164">deviceModel</span></span>|<span data-ttu-id="c8bd0-165">String</span><span class="sxs-lookup"><span data-stu-id="c8bd0-165">String</span></span>|<span data-ttu-id="c8bd0-166">レポートされているデバイス モデル</span><span class="sxs-lookup"><span data-stu-id="c8bd0-166">The device model that is being reported</span></span>|
|<span data-ttu-id="c8bd0-167">state</span><span class="sxs-lookup"><span data-stu-id="c8bd0-167">state</span></span>|[<span data-ttu-id="c8bd0-168">complianceStatus</span><span class="sxs-lookup"><span data-stu-id="c8bd0-168">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="c8bd0-169">設定のコンプライアンスの状態です。</span><span class="sxs-lookup"><span data-stu-id="c8bd0-169">The compliance state of the setting.</span></span> <span data-ttu-id="c8bd0-170">可能な値は、`unknown`、`notApplicable`、`compliant`、`remediated`、`nonCompliant`、`error`、`conflict`、`notAssigned` です。</span><span class="sxs-lookup"><span data-stu-id="c8bd0-170">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="c8bd0-171">complianceGracePeriodExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="c8bd0-171">complianceGracePeriodExpirationDateTime</span></span>|<span data-ttu-id="c8bd0-172">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c8bd0-172">DateTimeOffset</span></span>|<span data-ttu-id="c8bd0-173">デバイス コンプライアンスの猶予期間が過ぎる DateTime</span><span class="sxs-lookup"><span data-stu-id="c8bd0-173">The DateTime when device compliance grace period expires</span></span>|



## <a name="response"></a><span data-ttu-id="c8bd0-174">応答</span><span class="sxs-lookup"><span data-stu-id="c8bd0-174">Response</span></span>
<span data-ttu-id="c8bd0-175">かどうかは成功すると、このメソッドが返されます、`201 Created`応答コードおよび応答の本文に[advancedThreatProtectionOnboardingDeviceSettingState](../resources/intune-deviceconfig-advancedthreatprotectiononboardingdevicesettingstate.md)オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="c8bd0-175">If successful, this method returns a `201 Created` response code and a [advancedThreatProtectionOnboardingDeviceSettingState](../resources/intune-deviceconfig-advancedthreatprotectiononboardingdevicesettingstate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c8bd0-176">例</span><span class="sxs-lookup"><span data-stu-id="c8bd0-176">Example</span></span>
### <a name="request"></a><span data-ttu-id="c8bd0-177">要求</span><span class="sxs-lookup"><span data-stu-id="c8bd0-177">Request</span></span>
<span data-ttu-id="c8bd0-178">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="c8bd0-178">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="c8bd0-179">応答</span><span class="sxs-lookup"><span data-stu-id="c8bd0-179">Response</span></span>
<span data-ttu-id="c8bd0-p105">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="c8bd0-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





