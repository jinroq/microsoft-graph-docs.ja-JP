---
title: deviceComplianceSettingState の更新
description: deviceComplianceSettingState オブジェクトのプロパティを更新します。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: ce9dbae6f3b0ffe3b84323018ff37036a554518f
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29398255"
---
# <a name="update-devicecompliancesettingstate"></a><span data-ttu-id="98065-103">deviceComplianceSettingState の更新</span><span class="sxs-lookup"><span data-stu-id="98065-103">Update deviceComplianceSettingState</span></span>

> <span data-ttu-id="98065-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="98065-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="98065-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="98065-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="98065-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="98065-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="98065-107">[deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="98065-107">Update the properties of a [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="98065-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="98065-108">Prerequisites</span></span>
<span data-ttu-id="98065-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/concepts/permissions-reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="98065-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="98065-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="98065-111">Permission type</span></span>|<span data-ttu-id="98065-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="98065-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="98065-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="98065-113">Delegated (work or school account)</span></span>|<span data-ttu-id="98065-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="98065-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="98065-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="98065-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="98065-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="98065-116">Not supported.</span></span>|
|<span data-ttu-id="98065-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="98065-117">Application</span></span>|<span data-ttu-id="98065-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="98065-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="98065-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="98065-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicySettingStateSummaries/{deviceCompliancePolicySettingStateSummaryId}/deviceComplianceSettingStates/{deviceComplianceSettingStateId}
```

## <a name="request-headers"></a><span data-ttu-id="98065-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="98065-120">Request headers</span></span>
|<span data-ttu-id="98065-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="98065-121">Header</span></span>|<span data-ttu-id="98065-122">値</span><span class="sxs-lookup"><span data-stu-id="98065-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="98065-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="98065-123">Authorization</span></span>|<span data-ttu-id="98065-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="98065-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="98065-125">Accept</span><span class="sxs-lookup"><span data-stu-id="98065-125">Accept</span></span>|<span data-ttu-id="98065-126">application/json</span><span class="sxs-lookup"><span data-stu-id="98065-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="98065-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="98065-127">Request body</span></span>
<span data-ttu-id="98065-128">要求本文で、[deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="98065-128">In the request body, supply a JSON representation for the [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) object.</span></span>

<span data-ttu-id="98065-129">次の表に、[deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="98065-129">The following table shows the properties that are required when you create the [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md).</span></span>

|<span data-ttu-id="98065-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="98065-130">Property</span></span>|<span data-ttu-id="98065-131">型</span><span class="sxs-lookup"><span data-stu-id="98065-131">Type</span></span>|<span data-ttu-id="98065-132">説明</span><span class="sxs-lookup"><span data-stu-id="98065-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="98065-133">id</span><span class="sxs-lookup"><span data-stu-id="98065-133">id</span></span>|<span data-ttu-id="98065-134">String</span><span class="sxs-lookup"><span data-stu-id="98065-134">String</span></span>|<span data-ttu-id="98065-135">エンティティのキー</span><span class="sxs-lookup"><span data-stu-id="98065-135">Key of the entity</span></span>|
|<span data-ttu-id="98065-136">platformType</span><span class="sxs-lookup"><span data-stu-id="98065-136">platformType</span></span>|[<span data-ttu-id="98065-137">deviceType</span><span class="sxs-lookup"><span data-stu-id="98065-137">deviceType</span></span>](../resources/intune-shared-devicetype.md)|<span data-ttu-id="98065-138">デバイス プラットフォームのタイプです。</span><span class="sxs-lookup"><span data-stu-id="98065-138">Device platform type.</span></span> <span data-ttu-id="98065-139">使用可能な値: `desktop`、 `windowsRT`、 `winMO6`、 `nokia`、 `windowsPhone`、 `mac`、 `winCE`、 `winEmbedded`、 `iPhone`、 `iPad`、 `iPod`、 `android`、 `iSocConsumer`、 `unix`、 `macMDM`、 `holoLens`、 `surfaceHub`、 `androidForWork`、 `androidEnterprise`, `blackberry`, `palm`, `unknown`.</span><span class="sxs-lookup"><span data-stu-id="98065-139">Possible values are: `desktop`, `windowsRT`, `winMO6`, `nokia`, `windowsPhone`, `mac`, `winCE`, `winEmbedded`, `iPhone`, `iPad`, `iPod`, `android`, `iSocConsumer`, `unix`, `macMDM`, `holoLens`, `surfaceHub`, `androidForWork`, `androidEnterprise`, `blackberry`, `palm`, `unknown`.</span></span>|
|<span data-ttu-id="98065-140">setting</span><span class="sxs-lookup"><span data-stu-id="98065-140">setting</span></span>|<span data-ttu-id="98065-141">String</span><span class="sxs-lookup"><span data-stu-id="98065-141">String</span></span>|<span data-ttu-id="98065-142">設定のクラス名とプロパティ名。</span><span class="sxs-lookup"><span data-stu-id="98065-142">The setting class name and property name.</span></span>|
|<span data-ttu-id="98065-143">settingName</span><span class="sxs-lookup"><span data-stu-id="98065-143">settingName</span></span>|<span data-ttu-id="98065-144">String</span><span class="sxs-lookup"><span data-stu-id="98065-144">String</span></span>|<span data-ttu-id="98065-145">レポートされている設定名。</span><span class="sxs-lookup"><span data-stu-id="98065-145">The Setting Name that is being reported</span></span>|
|<span data-ttu-id="98065-146">deviceId</span><span class="sxs-lookup"><span data-stu-id="98065-146">deviceId</span></span>|<span data-ttu-id="98065-147">String</span><span class="sxs-lookup"><span data-stu-id="98065-147">String</span></span>|<span data-ttu-id="98065-148">レポートされているデバイス ID。</span><span class="sxs-lookup"><span data-stu-id="98065-148">The Device Id that is being reported</span></span>|
|<span data-ttu-id="98065-149">deviceName</span><span class="sxs-lookup"><span data-stu-id="98065-149">deviceName</span></span>|<span data-ttu-id="98065-150">String</span><span class="sxs-lookup"><span data-stu-id="98065-150">String</span></span>|<span data-ttu-id="98065-151">レポートされているデバイス名。</span><span class="sxs-lookup"><span data-stu-id="98065-151">The Device Name that is being reported</span></span>|
|<span data-ttu-id="98065-152">userId</span><span class="sxs-lookup"><span data-stu-id="98065-152">userId</span></span>|<span data-ttu-id="98065-153">String</span><span class="sxs-lookup"><span data-stu-id="98065-153">String</span></span>|<span data-ttu-id="98065-154">レポートされているユーザー ID</span><span class="sxs-lookup"><span data-stu-id="98065-154">The user Id that is being reported</span></span>|
|<span data-ttu-id="98065-155">userEmail</span><span class="sxs-lookup"><span data-stu-id="98065-155">userEmail</span></span>|<span data-ttu-id="98065-156">String</span><span class="sxs-lookup"><span data-stu-id="98065-156">String</span></span>|<span data-ttu-id="98065-157">レポートされているユーザーのメール アドレス。</span><span class="sxs-lookup"><span data-stu-id="98065-157">The User email address that is being reported</span></span>|
|<span data-ttu-id="98065-158">userName</span><span class="sxs-lookup"><span data-stu-id="98065-158">userName</span></span>|<span data-ttu-id="98065-159">String</span><span class="sxs-lookup"><span data-stu-id="98065-159">String</span></span>|<span data-ttu-id="98065-160">レポートされているユーザー名</span><span class="sxs-lookup"><span data-stu-id="98065-160">The User Name that is being reported</span></span>|
|<span data-ttu-id="98065-161">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="98065-161">userPrincipalName</span></span>|<span data-ttu-id="98065-162">String</span><span class="sxs-lookup"><span data-stu-id="98065-162">String</span></span>|<span data-ttu-id="98065-163">レポートされているユーザーの PrincipalName</span><span class="sxs-lookup"><span data-stu-id="98065-163">The User PrincipalName that is being reported</span></span>|
|<span data-ttu-id="98065-164">deviceModel</span><span class="sxs-lookup"><span data-stu-id="98065-164">deviceModel</span></span>|<span data-ttu-id="98065-165">String</span><span class="sxs-lookup"><span data-stu-id="98065-165">String</span></span>|<span data-ttu-id="98065-166">レポートされているデバイス モデル</span><span class="sxs-lookup"><span data-stu-id="98065-166">The device model that is being reported</span></span>|
|<span data-ttu-id="98065-167">state</span><span class="sxs-lookup"><span data-stu-id="98065-167">state</span></span>|[<span data-ttu-id="98065-168">complianceStatus</span><span class="sxs-lookup"><span data-stu-id="98065-168">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="98065-169">設定のコンプライアンスの状態です。</span><span class="sxs-lookup"><span data-stu-id="98065-169">The compliance state of the setting.</span></span> <span data-ttu-id="98065-170">可能な値は、`unknown`、`notApplicable`、`compliant`、`remediated`、`nonCompliant`、`error`、`conflict`、`notAssigned` です。</span><span class="sxs-lookup"><span data-stu-id="98065-170">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="98065-171">complianceGracePeriodExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="98065-171">complianceGracePeriodExpirationDateTime</span></span>|<span data-ttu-id="98065-172">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="98065-172">DateTimeOffset</span></span>|<span data-ttu-id="98065-173">デバイス コンプライアンスの猶予期間が過ぎる DateTime</span><span class="sxs-lookup"><span data-stu-id="98065-173">The DateTime when device compliance grace period expires</span></span>|



## <a name="response"></a><span data-ttu-id="98065-174">応答</span><span class="sxs-lookup"><span data-stu-id="98065-174">Response</span></span>
<span data-ttu-id="98065-175">成功した場合、このメソッドは `200 OK` 応答コードと、更新された [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) オブジェクトを応答本文で返します。</span><span class="sxs-lookup"><span data-stu-id="98065-175">If successful, this method returns a `200 OK` response code and an updated [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="98065-176">例</span><span class="sxs-lookup"><span data-stu-id="98065-176">Example</span></span>

### <a name="request"></a><span data-ttu-id="98065-177">要求</span><span class="sxs-lookup"><span data-stu-id="98065-177">Request</span></span>
<span data-ttu-id="98065-178">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="98065-178">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="98065-179">応答</span><span class="sxs-lookup"><span data-stu-id="98065-179">Response</span></span>
<span data-ttu-id="98065-p105">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="98065-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




