---
title: deviceComplianceSettingState の更新
description: deviceComplianceSettingState オブジェクトのプロパティを更新します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: c22c97d8e15e79419066392d3a984ee0899589b7
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/26/2019
ms.locfileid: "30258668"
---
# <a name="update-devicecompliancesettingstate"></a><span data-ttu-id="28ba9-103">deviceComplianceSettingState の更新</span><span class="sxs-lookup"><span data-stu-id="28ba9-103">Update deviceComplianceSettingState</span></span>

> <span data-ttu-id="28ba9-104">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="28ba9-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="28ba9-105">[deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="28ba9-105">Update the properties of a [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="28ba9-106">前提条件</span><span class="sxs-lookup"><span data-stu-id="28ba9-106">Prerequisites</span></span>
<span data-ttu-id="28ba9-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/concepts/permissions-reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="28ba9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="28ba9-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="28ba9-109">Permission type</span></span>|<span data-ttu-id="28ba9-110">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="28ba9-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="28ba9-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="28ba9-111">Delegated (work or school account)</span></span>|<span data-ttu-id="28ba9-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="28ba9-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="28ba9-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="28ba9-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="28ba9-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="28ba9-114">Not supported.</span></span>|
|<span data-ttu-id="28ba9-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="28ba9-115">Application</span></span>|<span data-ttu-id="28ba9-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="28ba9-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="28ba9-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="28ba9-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicySettingStateSummaries/{deviceCompliancePolicySettingStateSummaryId}/deviceComplianceSettingStates/{deviceComplianceSettingStateId}
```

## <a name="request-headers"></a><span data-ttu-id="28ba9-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="28ba9-118">Request headers</span></span>
|<span data-ttu-id="28ba9-119">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="28ba9-119">Header</span></span>|<span data-ttu-id="28ba9-120">値</span><span class="sxs-lookup"><span data-stu-id="28ba9-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="28ba9-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="28ba9-121">Authorization</span></span>|<span data-ttu-id="28ba9-122">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="28ba9-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="28ba9-123">承諾</span><span class="sxs-lookup"><span data-stu-id="28ba9-123">Accept</span></span>|<span data-ttu-id="28ba9-124">application/json</span><span class="sxs-lookup"><span data-stu-id="28ba9-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="28ba9-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="28ba9-125">Request body</span></span>
<span data-ttu-id="28ba9-126">要求本文で、[deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="28ba9-126">In the request body, supply a JSON representation for the [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) object.</span></span>

<span data-ttu-id="28ba9-127">次の表に、[deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="28ba9-127">The following table shows the properties that are required when you create the [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md).</span></span>

|<span data-ttu-id="28ba9-128">プロパティ</span><span class="sxs-lookup"><span data-stu-id="28ba9-128">Property</span></span>|<span data-ttu-id="28ba9-129">型</span><span class="sxs-lookup"><span data-stu-id="28ba9-129">Type</span></span>|<span data-ttu-id="28ba9-130">説明</span><span class="sxs-lookup"><span data-stu-id="28ba9-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="28ba9-131">id</span><span class="sxs-lookup"><span data-stu-id="28ba9-131">id</span></span>|<span data-ttu-id="28ba9-132">String</span><span class="sxs-lookup"><span data-stu-id="28ba9-132">String</span></span>|<span data-ttu-id="28ba9-133">エンティティのキー</span><span class="sxs-lookup"><span data-stu-id="28ba9-133">Key of the entity</span></span>|
|<span data-ttu-id="28ba9-134">setting</span><span class="sxs-lookup"><span data-stu-id="28ba9-134">setting</span></span>|<span data-ttu-id="28ba9-135">String</span><span class="sxs-lookup"><span data-stu-id="28ba9-135">String</span></span>|<span data-ttu-id="28ba9-136">設定のクラス名とプロパティ名。</span><span class="sxs-lookup"><span data-stu-id="28ba9-136">The setting class name and property name.</span></span>|
|<span data-ttu-id="28ba9-137">settingName</span><span class="sxs-lookup"><span data-stu-id="28ba9-137">settingName</span></span>|<span data-ttu-id="28ba9-138">String</span><span class="sxs-lookup"><span data-stu-id="28ba9-138">String</span></span>|<span data-ttu-id="28ba9-139">レポートされている設定名。</span><span class="sxs-lookup"><span data-stu-id="28ba9-139">The Setting Name that is being reported</span></span>|
|<span data-ttu-id="28ba9-140">deviceId</span><span class="sxs-lookup"><span data-stu-id="28ba9-140">deviceId</span></span>|<span data-ttu-id="28ba9-141">String</span><span class="sxs-lookup"><span data-stu-id="28ba9-141">String</span></span>|<span data-ttu-id="28ba9-142">レポートされているデバイス ID。</span><span class="sxs-lookup"><span data-stu-id="28ba9-142">The Device Id that is being reported</span></span>|
|<span data-ttu-id="28ba9-143">deviceName</span><span class="sxs-lookup"><span data-stu-id="28ba9-143">deviceName</span></span>|<span data-ttu-id="28ba9-144">String</span><span class="sxs-lookup"><span data-stu-id="28ba9-144">String</span></span>|<span data-ttu-id="28ba9-145">レポートされているデバイス名。</span><span class="sxs-lookup"><span data-stu-id="28ba9-145">The Device Name that is being reported</span></span>|
|<span data-ttu-id="28ba9-146">userId</span><span class="sxs-lookup"><span data-stu-id="28ba9-146">userId</span></span>|<span data-ttu-id="28ba9-147">String</span><span class="sxs-lookup"><span data-stu-id="28ba9-147">String</span></span>|<span data-ttu-id="28ba9-148">レポートされているユーザー ID</span><span class="sxs-lookup"><span data-stu-id="28ba9-148">The user Id that is being reported</span></span>|
|<span data-ttu-id="28ba9-149">userEmail</span><span class="sxs-lookup"><span data-stu-id="28ba9-149">userEmail</span></span>|<span data-ttu-id="28ba9-150">String</span><span class="sxs-lookup"><span data-stu-id="28ba9-150">String</span></span>|<span data-ttu-id="28ba9-151">レポートされているユーザーのメール アドレス。</span><span class="sxs-lookup"><span data-stu-id="28ba9-151">The User email address that is being reported</span></span>|
|<span data-ttu-id="28ba9-152">userName</span><span class="sxs-lookup"><span data-stu-id="28ba9-152">userName</span></span>|<span data-ttu-id="28ba9-153">String</span><span class="sxs-lookup"><span data-stu-id="28ba9-153">String</span></span>|<span data-ttu-id="28ba9-154">レポートされているユーザー名</span><span class="sxs-lookup"><span data-stu-id="28ba9-154">The User Name that is being reported</span></span>|
|<span data-ttu-id="28ba9-155">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="28ba9-155">userPrincipalName</span></span>|<span data-ttu-id="28ba9-156">String</span><span class="sxs-lookup"><span data-stu-id="28ba9-156">String</span></span>|<span data-ttu-id="28ba9-157">レポートされているユーザーの PrincipalName</span><span class="sxs-lookup"><span data-stu-id="28ba9-157">The User PrincipalName that is being reported</span></span>|
|<span data-ttu-id="28ba9-158">deviceModel</span><span class="sxs-lookup"><span data-stu-id="28ba9-158">deviceModel</span></span>|<span data-ttu-id="28ba9-159">String</span><span class="sxs-lookup"><span data-stu-id="28ba9-159">String</span></span>|<span data-ttu-id="28ba9-160">レポートされているデバイス モデル</span><span class="sxs-lookup"><span data-stu-id="28ba9-160">The device model that is being reported</span></span>|
|<span data-ttu-id="28ba9-161">state</span><span class="sxs-lookup"><span data-stu-id="28ba9-161">state</span></span>|[<span data-ttu-id="28ba9-162">complianceStatus</span><span class="sxs-lookup"><span data-stu-id="28ba9-162">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="28ba9-163">設定のコンプライアンス状態。</span><span class="sxs-lookup"><span data-stu-id="28ba9-163">The compliance state of the setting.</span></span> <span data-ttu-id="28ba9-164">可能な値は、`unknown`、`notApplicable`、`compliant`、`remediated`、`nonCompliant`、`error`、`conflict`、`notAssigned` です。</span><span class="sxs-lookup"><span data-stu-id="28ba9-164">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="28ba9-165">complianceGracePeriodExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="28ba9-165">complianceGracePeriodExpirationDateTime</span></span>|<span data-ttu-id="28ba9-166">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="28ba9-166">DateTimeOffset</span></span>|<span data-ttu-id="28ba9-167">デバイス コンプライアンスの猶予期間が過ぎる DateTime</span><span class="sxs-lookup"><span data-stu-id="28ba9-167">The DateTime when device compliance grace period expires</span></span>|



## <a name="response"></a><span data-ttu-id="28ba9-168">応答</span><span class="sxs-lookup"><span data-stu-id="28ba9-168">Response</span></span>
<span data-ttu-id="28ba9-169">成功した場合、このメソッドは `200 OK` 応答コードと、更新された [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) オブジェクトを応答本文で返します。</span><span class="sxs-lookup"><span data-stu-id="28ba9-169">If successful, this method returns a `200 OK` response code and an updated [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="28ba9-170">例</span><span class="sxs-lookup"><span data-stu-id="28ba9-170">Example</span></span>

### <a name="request"></a><span data-ttu-id="28ba9-171">要求</span><span class="sxs-lookup"><span data-stu-id="28ba9-171">Request</span></span>
<span data-ttu-id="28ba9-172">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="28ba9-172">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/deviceCompliancePolicySettingStateSummaries/{deviceCompliancePolicySettingStateSummaryId}/deviceComplianceSettingStates/{deviceComplianceSettingStateId}
Content-type: application/json
Content-length: 517

{
  "@odata.type": "#microsoft.graph.deviceComplianceSettingState",
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

### <a name="response"></a><span data-ttu-id="28ba9-173">応答</span><span class="sxs-lookup"><span data-stu-id="28ba9-173">Response</span></span>
<span data-ttu-id="28ba9-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="28ba9-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 566

{
  "@odata.type": "#microsoft.graph.deviceComplianceSettingState",
  "id": "9905f955-f955-9905-55f9-059955f90599",
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



