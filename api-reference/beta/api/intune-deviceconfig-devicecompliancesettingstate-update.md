---
title: deviceComplianceSettingState の更新
description: deviceComplianceSettingState オブジェクトのプロパティを更新します。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 8b5fba82013fa555f584ad86e29dd31b6ce1118a
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/11/2019
ms.locfileid: "33927630"
---
# <a name="update-devicecompliancesettingstate"></a><span data-ttu-id="d0ebd-103">deviceComplianceSettingState の更新</span><span class="sxs-lookup"><span data-stu-id="d0ebd-103">Update deviceComplianceSettingState</span></span>

> <span data-ttu-id="d0ebd-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d0ebd-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d0ebd-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="d0ebd-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d0ebd-106">[deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="d0ebd-106">Update the properties of a [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d0ebd-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="d0ebd-107">Prerequisites</span></span>
<span data-ttu-id="d0ebd-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="d0ebd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d0ebd-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="d0ebd-110">Permission type</span></span>|<span data-ttu-id="d0ebd-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="d0ebd-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d0ebd-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="d0ebd-112">Delegated (work or school account)</span></span>|<span data-ttu-id="d0ebd-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d0ebd-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="d0ebd-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="d0ebd-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d0ebd-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d0ebd-115">Not supported.</span></span>|
|<span data-ttu-id="d0ebd-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="d0ebd-116">Application</span></span>|<span data-ttu-id="d0ebd-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d0ebd-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d0ebd-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="d0ebd-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicySettingStateSummaries/{deviceCompliancePolicySettingStateSummaryId}/deviceComplianceSettingStates/{deviceComplianceSettingStateId}
```

## <a name="request-headers"></a><span data-ttu-id="d0ebd-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="d0ebd-119">Request headers</span></span>
|<span data-ttu-id="d0ebd-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="d0ebd-120">Header</span></span>|<span data-ttu-id="d0ebd-121">値</span><span class="sxs-lookup"><span data-stu-id="d0ebd-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d0ebd-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="d0ebd-122">Authorization</span></span>|<span data-ttu-id="d0ebd-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="d0ebd-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d0ebd-124">承諾</span><span class="sxs-lookup"><span data-stu-id="d0ebd-124">Accept</span></span>|<span data-ttu-id="d0ebd-125">application/json</span><span class="sxs-lookup"><span data-stu-id="d0ebd-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d0ebd-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="d0ebd-126">Request body</span></span>
<span data-ttu-id="d0ebd-127">要求本文で、[deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="d0ebd-127">In the request body, supply a JSON representation for the [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) object.</span></span>

<span data-ttu-id="d0ebd-128">次の表に、[deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="d0ebd-128">The following table shows the properties that are required when you create the [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md).</span></span>

|<span data-ttu-id="d0ebd-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="d0ebd-129">Property</span></span>|<span data-ttu-id="d0ebd-130">型</span><span class="sxs-lookup"><span data-stu-id="d0ebd-130">Type</span></span>|<span data-ttu-id="d0ebd-131">説明</span><span class="sxs-lookup"><span data-stu-id="d0ebd-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d0ebd-132">id</span><span class="sxs-lookup"><span data-stu-id="d0ebd-132">id</span></span>|<span data-ttu-id="d0ebd-133">文字列</span><span class="sxs-lookup"><span data-stu-id="d0ebd-133">String</span></span>|<span data-ttu-id="d0ebd-134">エンティティのキー</span><span class="sxs-lookup"><span data-stu-id="d0ebd-134">Key of the entity</span></span>|
|<span data-ttu-id="d0ebd-135">platformType</span><span class="sxs-lookup"><span data-stu-id="d0ebd-135">platformType</span></span>|[<span data-ttu-id="d0ebd-136">deviceType</span><span class="sxs-lookup"><span data-stu-id="d0ebd-136">deviceType</span></span>](../resources/intune-shared-devicetype.md)|<span data-ttu-id="d0ebd-137">デバイスプラットフォームの種類。</span><span class="sxs-lookup"><span data-stu-id="d0ebd-137">Device platform type.</span></span> <span data-ttu-id="d0ebd-138">可能な値: `desktop`、 `windowsRT` `winMO6` `nokia` `windowsPhone` `mac` `winCE` `winEmbedded` `iPhone` `iPad` `iPod` `android`、、、、、、、、、、、、 `iSocConsumer` `unix` `macMDM` `holoLens` `surfaceHub` `androidForWork` `androidEnterprise`, `blackberry`, `palm`, `unknown`.</span><span class="sxs-lookup"><span data-stu-id="d0ebd-138">Possible values are: `desktop`, `windowsRT`, `winMO6`, `nokia`, `windowsPhone`, `mac`, `winCE`, `winEmbedded`, `iPhone`, `iPad`, `iPod`, `android`, `iSocConsumer`, `unix`, `macMDM`, `holoLens`, `surfaceHub`, `androidForWork`, `androidEnterprise`, `blackberry`, `palm`, `unknown`.</span></span>|
|<span data-ttu-id="d0ebd-139">setting</span><span class="sxs-lookup"><span data-stu-id="d0ebd-139">setting</span></span>|<span data-ttu-id="d0ebd-140">String</span><span class="sxs-lookup"><span data-stu-id="d0ebd-140">String</span></span>|<span data-ttu-id="d0ebd-141">設定のクラス名とプロパティ名。</span><span class="sxs-lookup"><span data-stu-id="d0ebd-141">The setting class name and property name.</span></span>|
|<span data-ttu-id="d0ebd-142">settingName</span><span class="sxs-lookup"><span data-stu-id="d0ebd-142">settingName</span></span>|<span data-ttu-id="d0ebd-143">String</span><span class="sxs-lookup"><span data-stu-id="d0ebd-143">String</span></span>|<span data-ttu-id="d0ebd-144">レポートされている設定名。</span><span class="sxs-lookup"><span data-stu-id="d0ebd-144">The Setting Name that is being reported</span></span>|
|<span data-ttu-id="d0ebd-145">deviceId</span><span class="sxs-lookup"><span data-stu-id="d0ebd-145">deviceId</span></span>|<span data-ttu-id="d0ebd-146">String</span><span class="sxs-lookup"><span data-stu-id="d0ebd-146">String</span></span>|<span data-ttu-id="d0ebd-147">レポートされているデバイス ID。</span><span class="sxs-lookup"><span data-stu-id="d0ebd-147">The Device Id that is being reported</span></span>|
|<span data-ttu-id="d0ebd-148">deviceName</span><span class="sxs-lookup"><span data-stu-id="d0ebd-148">deviceName</span></span>|<span data-ttu-id="d0ebd-149">String</span><span class="sxs-lookup"><span data-stu-id="d0ebd-149">String</span></span>|<span data-ttu-id="d0ebd-150">レポートされているデバイス名。</span><span class="sxs-lookup"><span data-stu-id="d0ebd-150">The Device Name that is being reported</span></span>|
|<span data-ttu-id="d0ebd-151">userId</span><span class="sxs-lookup"><span data-stu-id="d0ebd-151">userId</span></span>|<span data-ttu-id="d0ebd-152">String</span><span class="sxs-lookup"><span data-stu-id="d0ebd-152">String</span></span>|<span data-ttu-id="d0ebd-153">レポートされているユーザー ID</span><span class="sxs-lookup"><span data-stu-id="d0ebd-153">The user Id that is being reported</span></span>|
|<span data-ttu-id="d0ebd-154">userEmail</span><span class="sxs-lookup"><span data-stu-id="d0ebd-154">userEmail</span></span>|<span data-ttu-id="d0ebd-155">String</span><span class="sxs-lookup"><span data-stu-id="d0ebd-155">String</span></span>|<span data-ttu-id="d0ebd-156">レポートされているユーザーのメール アドレス。</span><span class="sxs-lookup"><span data-stu-id="d0ebd-156">The User email address that is being reported</span></span>|
|<span data-ttu-id="d0ebd-157">userName</span><span class="sxs-lookup"><span data-stu-id="d0ebd-157">userName</span></span>|<span data-ttu-id="d0ebd-158">String</span><span class="sxs-lookup"><span data-stu-id="d0ebd-158">String</span></span>|<span data-ttu-id="d0ebd-159">レポートされているユーザー名</span><span class="sxs-lookup"><span data-stu-id="d0ebd-159">The User Name that is being reported</span></span>|
|<span data-ttu-id="d0ebd-160">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="d0ebd-160">userPrincipalName</span></span>|<span data-ttu-id="d0ebd-161">String</span><span class="sxs-lookup"><span data-stu-id="d0ebd-161">String</span></span>|<span data-ttu-id="d0ebd-162">レポートされているユーザーの PrincipalName</span><span class="sxs-lookup"><span data-stu-id="d0ebd-162">The User PrincipalName that is being reported</span></span>|
|<span data-ttu-id="d0ebd-163">deviceModel</span><span class="sxs-lookup"><span data-stu-id="d0ebd-163">deviceModel</span></span>|<span data-ttu-id="d0ebd-164">String</span><span class="sxs-lookup"><span data-stu-id="d0ebd-164">String</span></span>|<span data-ttu-id="d0ebd-165">レポートされているデバイス モデル</span><span class="sxs-lookup"><span data-stu-id="d0ebd-165">The device model that is being reported</span></span>|
|<span data-ttu-id="d0ebd-166">state</span><span class="sxs-lookup"><span data-stu-id="d0ebd-166">state</span></span>|[<span data-ttu-id="d0ebd-167">complianceStatus</span><span class="sxs-lookup"><span data-stu-id="d0ebd-167">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="d0ebd-168">設定のコンプライアンス状態。</span><span class="sxs-lookup"><span data-stu-id="d0ebd-168">The compliance state of the setting.</span></span> <span data-ttu-id="d0ebd-169">可能な値は、`unknown`、`notApplicable`、`compliant`、`remediated`、`nonCompliant`、`error`、`conflict`、`notAssigned` です。</span><span class="sxs-lookup"><span data-stu-id="d0ebd-169">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="d0ebd-170">complianceGracePeriodExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="d0ebd-170">complianceGracePeriodExpirationDateTime</span></span>|<span data-ttu-id="d0ebd-171">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d0ebd-171">DateTimeOffset</span></span>|<span data-ttu-id="d0ebd-172">デバイス コンプライアンスの猶予期間が過ぎる DateTime</span><span class="sxs-lookup"><span data-stu-id="d0ebd-172">The DateTime when device compliance grace period expires</span></span>|



## <a name="response"></a><span data-ttu-id="d0ebd-173">応答</span><span class="sxs-lookup"><span data-stu-id="d0ebd-173">Response</span></span>
<span data-ttu-id="d0ebd-174">成功した場合、このメソッドは `200 OK` 応答コードと、更新された [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) オブジェクトを応答本文で返します。</span><span class="sxs-lookup"><span data-stu-id="d0ebd-174">If successful, this method returns a `200 OK` response code and an updated [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d0ebd-175">例</span><span class="sxs-lookup"><span data-stu-id="d0ebd-175">Example</span></span>

### <a name="request"></a><span data-ttu-id="d0ebd-176">要求</span><span class="sxs-lookup"><span data-stu-id="d0ebd-176">Request</span></span>
<span data-ttu-id="d0ebd-177">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="d0ebd-177">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicySettingStateSummaries/{deviceCompliancePolicySettingStateSummaryId}/deviceComplianceSettingStates/{deviceComplianceSettingStateId}
Content-type: application/json
Content-length: 549

{
  "@odata.type": "#microsoft.graph.deviceComplianceSettingState",
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

### <a name="response"></a><span data-ttu-id="d0ebd-178">応答</span><span class="sxs-lookup"><span data-stu-id="d0ebd-178">Response</span></span>
<span data-ttu-id="d0ebd-p104">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="d0ebd-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 598

{
  "@odata.type": "#microsoft.graph.deviceComplianceSettingState",
  "id": "9905f955-f955-9905-55f9-059955f90599",
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




