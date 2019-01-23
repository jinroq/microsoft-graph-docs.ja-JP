---
title: AdvancedThreatProtectionOnboardingDeviceSettingState を更新します。
description: AdvancedThreatProtectionOnboardingDeviceSettingState オブジェクトのプロパティを更新します。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 2fe6b59f27a6041456096551fbfb0ca66f48329f
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29408636"
---
# <a name="update-advancedthreatprotectiononboardingdevicesettingstate"></a><span data-ttu-id="0b71d-103">AdvancedThreatProtectionOnboardingDeviceSettingState を更新します。</span><span class="sxs-lookup"><span data-stu-id="0b71d-103">Update advancedThreatProtectionOnboardingDeviceSettingState</span></span>

> <span data-ttu-id="0b71d-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="0b71d-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="0b71d-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="0b71d-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="0b71d-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="0b71d-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0b71d-107">[AdvancedThreatProtectionOnboardingDeviceSettingState](../resources/intune-deviceconfig-advancedthreatprotectiononboardingdevicesettingstate.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="0b71d-107">Update the properties of a [advancedThreatProtectionOnboardingDeviceSettingState](../resources/intune-deviceconfig-advancedthreatprotectiononboardingdevicesettingstate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="0b71d-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="0b71d-108">Prerequisites</span></span>
<span data-ttu-id="0b71d-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/concepts/permissions-reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="0b71d-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="0b71d-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="0b71d-111">Permission type</span></span>|<span data-ttu-id="0b71d-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="0b71d-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0b71d-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="0b71d-113">Delegated (work or school account)</span></span>|<span data-ttu-id="0b71d-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0b71d-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="0b71d-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="0b71d-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0b71d-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="0b71d-116">Not supported.</span></span>|
|<span data-ttu-id="0b71d-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="0b71d-117">Application</span></span>|<span data-ttu-id="0b71d-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="0b71d-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="0b71d-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="0b71d-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/advancedThreatProtectionOnboardingStateSummary/advancedThreatProtectionOnboardingDeviceSettingStates/{advancedThreatProtectionOnboardingDeviceSettingStateId}
```

## <a name="request-headers"></a><span data-ttu-id="0b71d-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="0b71d-120">Request headers</span></span>
|<span data-ttu-id="0b71d-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="0b71d-121">Header</span></span>|<span data-ttu-id="0b71d-122">値</span><span class="sxs-lookup"><span data-stu-id="0b71d-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0b71d-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="0b71d-123">Authorization</span></span>|<span data-ttu-id="0b71d-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="0b71d-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0b71d-125">Accept</span><span class="sxs-lookup"><span data-stu-id="0b71d-125">Accept</span></span>|<span data-ttu-id="0b71d-126">application/json</span><span class="sxs-lookup"><span data-stu-id="0b71d-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0b71d-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="0b71d-127">Request body</span></span>
<span data-ttu-id="0b71d-128">要求の本文に[advancedThreatProtectionOnboardingDeviceSettingState](../resources/intune-deviceconfig-advancedthreatprotectiononboardingdevicesettingstate.md)オブジェクトの JSON の形式を指定します。</span><span class="sxs-lookup"><span data-stu-id="0b71d-128">In the request body, supply a JSON representation for the [advancedThreatProtectionOnboardingDeviceSettingState](../resources/intune-deviceconfig-advancedthreatprotectiononboardingdevicesettingstate.md) object.</span></span>

<span data-ttu-id="0b71d-129">[AdvancedThreatProtectionOnboardingDeviceSettingState](../resources/intune-deviceconfig-advancedthreatprotectiononboardingdevicesettingstate.md)を作成するときに必要なプロパティを次の表に示します。</span><span class="sxs-lookup"><span data-stu-id="0b71d-129">The following table shows the properties that are required when you create the [advancedThreatProtectionOnboardingDeviceSettingState](../resources/intune-deviceconfig-advancedthreatprotectiononboardingdevicesettingstate.md).</span></span>

|<span data-ttu-id="0b71d-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="0b71d-130">Property</span></span>|<span data-ttu-id="0b71d-131">型</span><span class="sxs-lookup"><span data-stu-id="0b71d-131">Type</span></span>|<span data-ttu-id="0b71d-132">説明</span><span class="sxs-lookup"><span data-stu-id="0b71d-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0b71d-133">id</span><span class="sxs-lookup"><span data-stu-id="0b71d-133">id</span></span>|<span data-ttu-id="0b71d-134">String</span><span class="sxs-lookup"><span data-stu-id="0b71d-134">String</span></span>|<span data-ttu-id="0b71d-135">エンティティのキー</span><span class="sxs-lookup"><span data-stu-id="0b71d-135">Key of the entity</span></span>|
|<span data-ttu-id="0b71d-136">platformType</span><span class="sxs-lookup"><span data-stu-id="0b71d-136">platformType</span></span>|[<span data-ttu-id="0b71d-137">deviceType</span><span class="sxs-lookup"><span data-stu-id="0b71d-137">deviceType</span></span>](../resources/intune-shared-devicetype.md)|<span data-ttu-id="0b71d-138">デバイス プラットフォームのタイプです。</span><span class="sxs-lookup"><span data-stu-id="0b71d-138">Device platform type.</span></span> <span data-ttu-id="0b71d-139">使用可能な値: `desktop`、 `windowsRT`、 `winMO6`、 `nokia`、 `windowsPhone`、 `mac`、 `winCE`、 `winEmbedded`、 `iPhone`、 `iPad`、 `iPod`、 `android`、 `iSocConsumer`、 `unix`、 `macMDM`、 `holoLens`、 `surfaceHub`、 `androidForWork`、 `androidEnterprise`, `blackberry`, `palm`, `unknown`.</span><span class="sxs-lookup"><span data-stu-id="0b71d-139">Possible values are: `desktop`, `windowsRT`, `winMO6`, `nokia`, `windowsPhone`, `mac`, `winCE`, `winEmbedded`, `iPhone`, `iPad`, `iPod`, `android`, `iSocConsumer`, `unix`, `macMDM`, `holoLens`, `surfaceHub`, `androidForWork`, `androidEnterprise`, `blackberry`, `palm`, `unknown`.</span></span>|
|<span data-ttu-id="0b71d-140">setting</span><span class="sxs-lookup"><span data-stu-id="0b71d-140">setting</span></span>|<span data-ttu-id="0b71d-141">String</span><span class="sxs-lookup"><span data-stu-id="0b71d-141">String</span></span>|<span data-ttu-id="0b71d-142">設定のクラス名とプロパティ名。</span><span class="sxs-lookup"><span data-stu-id="0b71d-142">The setting class name and property name.</span></span>|
|<span data-ttu-id="0b71d-143">settingName</span><span class="sxs-lookup"><span data-stu-id="0b71d-143">settingName</span></span>|<span data-ttu-id="0b71d-144">String</span><span class="sxs-lookup"><span data-stu-id="0b71d-144">String</span></span>|<span data-ttu-id="0b71d-145">レポートされている設定名。</span><span class="sxs-lookup"><span data-stu-id="0b71d-145">The Setting Name that is being reported</span></span>|
|<span data-ttu-id="0b71d-146">deviceId</span><span class="sxs-lookup"><span data-stu-id="0b71d-146">deviceId</span></span>|<span data-ttu-id="0b71d-147">String</span><span class="sxs-lookup"><span data-stu-id="0b71d-147">String</span></span>|<span data-ttu-id="0b71d-148">レポートされているデバイス ID。</span><span class="sxs-lookup"><span data-stu-id="0b71d-148">The Device Id that is being reported</span></span>|
|<span data-ttu-id="0b71d-149">deviceName</span><span class="sxs-lookup"><span data-stu-id="0b71d-149">deviceName</span></span>|<span data-ttu-id="0b71d-150">String</span><span class="sxs-lookup"><span data-stu-id="0b71d-150">String</span></span>|<span data-ttu-id="0b71d-151">レポートされているデバイス名。</span><span class="sxs-lookup"><span data-stu-id="0b71d-151">The Device Name that is being reported</span></span>|
|<span data-ttu-id="0b71d-152">userId</span><span class="sxs-lookup"><span data-stu-id="0b71d-152">userId</span></span>|<span data-ttu-id="0b71d-153">String</span><span class="sxs-lookup"><span data-stu-id="0b71d-153">String</span></span>|<span data-ttu-id="0b71d-154">レポートされているユーザー ID</span><span class="sxs-lookup"><span data-stu-id="0b71d-154">The user Id that is being reported</span></span>|
|<span data-ttu-id="0b71d-155">userEmail</span><span class="sxs-lookup"><span data-stu-id="0b71d-155">userEmail</span></span>|<span data-ttu-id="0b71d-156">String</span><span class="sxs-lookup"><span data-stu-id="0b71d-156">String</span></span>|<span data-ttu-id="0b71d-157">レポートされているユーザーのメール アドレス。</span><span class="sxs-lookup"><span data-stu-id="0b71d-157">The User email address that is being reported</span></span>|
|<span data-ttu-id="0b71d-158">userName</span><span class="sxs-lookup"><span data-stu-id="0b71d-158">userName</span></span>|<span data-ttu-id="0b71d-159">String</span><span class="sxs-lookup"><span data-stu-id="0b71d-159">String</span></span>|<span data-ttu-id="0b71d-160">レポートされているユーザー名</span><span class="sxs-lookup"><span data-stu-id="0b71d-160">The User Name that is being reported</span></span>|
|<span data-ttu-id="0b71d-161">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="0b71d-161">userPrincipalName</span></span>|<span data-ttu-id="0b71d-162">String</span><span class="sxs-lookup"><span data-stu-id="0b71d-162">String</span></span>|<span data-ttu-id="0b71d-163">レポートされているユーザーの PrincipalName</span><span class="sxs-lookup"><span data-stu-id="0b71d-163">The User PrincipalName that is being reported</span></span>|
|<span data-ttu-id="0b71d-164">deviceModel</span><span class="sxs-lookup"><span data-stu-id="0b71d-164">deviceModel</span></span>|<span data-ttu-id="0b71d-165">String</span><span class="sxs-lookup"><span data-stu-id="0b71d-165">String</span></span>|<span data-ttu-id="0b71d-166">レポートされているデバイス モデル</span><span class="sxs-lookup"><span data-stu-id="0b71d-166">The device model that is being reported</span></span>|
|<span data-ttu-id="0b71d-167">state</span><span class="sxs-lookup"><span data-stu-id="0b71d-167">state</span></span>|[<span data-ttu-id="0b71d-168">complianceStatus</span><span class="sxs-lookup"><span data-stu-id="0b71d-168">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="0b71d-169">設定のコンプライアンスの状態です。</span><span class="sxs-lookup"><span data-stu-id="0b71d-169">The compliance state of the setting.</span></span> <span data-ttu-id="0b71d-170">可能な値は、`unknown`、`notApplicable`、`compliant`、`remediated`、`nonCompliant`、`error`、`conflict`、`notAssigned` です。</span><span class="sxs-lookup"><span data-stu-id="0b71d-170">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="0b71d-171">complianceGracePeriodExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="0b71d-171">complianceGracePeriodExpirationDateTime</span></span>|<span data-ttu-id="0b71d-172">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0b71d-172">DateTimeOffset</span></span>|<span data-ttu-id="0b71d-173">デバイス コンプライアンスの猶予期間が過ぎる DateTime</span><span class="sxs-lookup"><span data-stu-id="0b71d-173">The DateTime when device compliance grace period expires</span></span>|



## <a name="response"></a><span data-ttu-id="0b71d-174">応答</span><span class="sxs-lookup"><span data-stu-id="0b71d-174">Response</span></span>
<span data-ttu-id="0b71d-175">かどうかは成功すると、このメソッドが返されます、`200 OK`応答コードおよび応答の本文に更新された[advancedThreatProtectionOnboardingDeviceSettingState](../resources/intune-deviceconfig-advancedthreatprotectiononboardingdevicesettingstate.md)オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="0b71d-175">If successful, this method returns a `200 OK` response code and an updated [advancedThreatProtectionOnboardingDeviceSettingState](../resources/intune-deviceconfig-advancedthreatprotectiononboardingdevicesettingstate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0b71d-176">例</span><span class="sxs-lookup"><span data-stu-id="0b71d-176">Example</span></span>

### <a name="request"></a><span data-ttu-id="0b71d-177">要求</span><span class="sxs-lookup"><span data-stu-id="0b71d-177">Request</span></span>
<span data-ttu-id="0b71d-178">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="0b71d-178">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="0b71d-179">応答</span><span class="sxs-lookup"><span data-stu-id="0b71d-179">Response</span></span>
<span data-ttu-id="0b71d-p105">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="0b71d-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




