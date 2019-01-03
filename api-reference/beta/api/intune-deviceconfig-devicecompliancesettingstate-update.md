---
title: deviceComplianceSettingState の更新
description: deviceComplianceSettingState オブジェクトのプロパティを更新します。
author: tfitzmac
ms.openlocfilehash: 699ddfebe1e333c97d6fc186e4d65e40c4f367aa
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27348210"
---
# <a name="update-devicecompliancesettingstate"></a><span data-ttu-id="95263-103">deviceComplianceSettingState の更新</span><span class="sxs-lookup"><span data-stu-id="95263-103">Update deviceComplianceSettingState</span></span>

> <span data-ttu-id="95263-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="95263-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="95263-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="95263-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="95263-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="95263-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="95263-107">[deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="95263-107">Update the properties of a [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="95263-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="95263-108">Prerequisites</span></span>
<span data-ttu-id="95263-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="95263-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="95263-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="95263-111">Permission type</span></span>|<span data-ttu-id="95263-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="95263-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="95263-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="95263-113">Delegated (work or school account)</span></span>|<span data-ttu-id="95263-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="95263-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="95263-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="95263-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="95263-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="95263-116">Not supported.</span></span>|
|<span data-ttu-id="95263-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="95263-117">Application</span></span>|<span data-ttu-id="95263-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="95263-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="95263-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="95263-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicySettingStateSummaries/{deviceCompliancePolicySettingStateSummaryId}/deviceComplianceSettingStates/{deviceComplianceSettingStateId}
```

## <a name="request-headers"></a><span data-ttu-id="95263-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="95263-120">Request headers</span></span>
|<span data-ttu-id="95263-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="95263-121">Header</span></span>|<span data-ttu-id="95263-122">値</span><span class="sxs-lookup"><span data-stu-id="95263-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="95263-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="95263-123">Authorization</span></span>|<span data-ttu-id="95263-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="95263-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="95263-125">Accept</span><span class="sxs-lookup"><span data-stu-id="95263-125">Accept</span></span>|<span data-ttu-id="95263-126">application/json</span><span class="sxs-lookup"><span data-stu-id="95263-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="95263-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="95263-127">Request body</span></span>
<span data-ttu-id="95263-128">要求本文で、[deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="95263-128">In the request body, supply a JSON representation for the [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) object.</span></span>

<span data-ttu-id="95263-129">次の表に、[deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="95263-129">The following table shows the properties that are required when you create the [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md).</span></span>

|<span data-ttu-id="95263-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="95263-130">Property</span></span>|<span data-ttu-id="95263-131">種類</span><span class="sxs-lookup"><span data-stu-id="95263-131">Type</span></span>|<span data-ttu-id="95263-132">説明</span><span class="sxs-lookup"><span data-stu-id="95263-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="95263-133">ID</span><span class="sxs-lookup"><span data-stu-id="95263-133">id</span></span>|<span data-ttu-id="95263-134">String</span><span class="sxs-lookup"><span data-stu-id="95263-134">String</span></span>|<span data-ttu-id="95263-135">エンティティのキー</span><span class="sxs-lookup"><span data-stu-id="95263-135">Key of the entity</span></span>|
|<span data-ttu-id="95263-136">platformType</span><span class="sxs-lookup"><span data-stu-id="95263-136">platformType</span></span>|[<span data-ttu-id="95263-137">deviceType</span><span class="sxs-lookup"><span data-stu-id="95263-137">deviceType</span></span>](../resources/intune-shared-devicetype.md)|<span data-ttu-id="95263-138">デバイス プラットフォームのタイプです。</span><span class="sxs-lookup"><span data-stu-id="95263-138">Device platform type.</span></span> <span data-ttu-id="95263-139">使用可能な値: `desktop`、 `windowsRT`、 `winMO6`、 `nokia`、 `windowsPhone`、 `mac`、 `winCE`、 `winEmbedded`、 `iPhone`、 `iPad`、 `iPod`、 `android`、 `iSocConsumer`、 `unix`、 `macMDM`、 `holoLens`、 `surfaceHub`、 `androidForWork`、 `androidEnterprise`, `blackberry`, `palm`, `unknown`.</span><span class="sxs-lookup"><span data-stu-id="95263-139">Possible values are: `desktop`, `windowsRT`, `winMO6`, `nokia`, `windowsPhone`, `mac`, `winCE`, `winEmbedded`, `iPhone`, `iPad`, `iPod`, `android`, `iSocConsumer`, `unix`, `macMDM`, `holoLens`, `surfaceHub`, `androidForWork`, `androidEnterprise`, `blackberry`, `palm`, `unknown`.</span></span>|
|<span data-ttu-id="95263-140">setting</span><span class="sxs-lookup"><span data-stu-id="95263-140">setting</span></span>|<span data-ttu-id="95263-141">String</span><span class="sxs-lookup"><span data-stu-id="95263-141">String</span></span>|<span data-ttu-id="95263-142">設定のクラス名とプロパティ名。</span><span class="sxs-lookup"><span data-stu-id="95263-142">The setting class name and property name.</span></span>|
|<span data-ttu-id="95263-143">settingName</span><span class="sxs-lookup"><span data-stu-id="95263-143">settingName</span></span>|<span data-ttu-id="95263-144">String</span><span class="sxs-lookup"><span data-stu-id="95263-144">String</span></span>|<span data-ttu-id="95263-145">レポートされている設定名。</span><span class="sxs-lookup"><span data-stu-id="95263-145">The Setting Name that is being reported</span></span>|
|<span data-ttu-id="95263-146">deviceId</span><span class="sxs-lookup"><span data-stu-id="95263-146">deviceId</span></span>|<span data-ttu-id="95263-147">String</span><span class="sxs-lookup"><span data-stu-id="95263-147">String</span></span>|<span data-ttu-id="95263-148">レポートされているデバイス ID。</span><span class="sxs-lookup"><span data-stu-id="95263-148">The Device Id that is being reported</span></span>|
|<span data-ttu-id="95263-149">deviceName</span><span class="sxs-lookup"><span data-stu-id="95263-149">deviceName</span></span>|<span data-ttu-id="95263-150">String</span><span class="sxs-lookup"><span data-stu-id="95263-150">String</span></span>|<span data-ttu-id="95263-151">レポートされているデバイス名。</span><span class="sxs-lookup"><span data-stu-id="95263-151">The Device Name that is being reported</span></span>|
|<span data-ttu-id="95263-152">userId</span><span class="sxs-lookup"><span data-stu-id="95263-152">userId</span></span>|<span data-ttu-id="95263-153">String</span><span class="sxs-lookup"><span data-stu-id="95263-153">String</span></span>|<span data-ttu-id="95263-154">レポートされているユーザー ID</span><span class="sxs-lookup"><span data-stu-id="95263-154">The user Id that is being reported</span></span>|
|<span data-ttu-id="95263-155">userEmail</span><span class="sxs-lookup"><span data-stu-id="95263-155">userEmail</span></span>|<span data-ttu-id="95263-156">String</span><span class="sxs-lookup"><span data-stu-id="95263-156">String</span></span>|<span data-ttu-id="95263-157">レポートされているユーザーのメール アドレス。</span><span class="sxs-lookup"><span data-stu-id="95263-157">The User email address that is being reported</span></span>|
|<span data-ttu-id="95263-158">userName</span><span class="sxs-lookup"><span data-stu-id="95263-158">userName</span></span>|<span data-ttu-id="95263-159">String</span><span class="sxs-lookup"><span data-stu-id="95263-159">String</span></span>|<span data-ttu-id="95263-160">レポートされているユーザー名</span><span class="sxs-lookup"><span data-stu-id="95263-160">The User Name that is being reported</span></span>|
|<span data-ttu-id="95263-161">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="95263-161">userPrincipalName</span></span>|<span data-ttu-id="95263-162">String</span><span class="sxs-lookup"><span data-stu-id="95263-162">String</span></span>|<span data-ttu-id="95263-163">レポートされているユーザーの PrincipalName</span><span class="sxs-lookup"><span data-stu-id="95263-163">The User PrincipalName that is being reported</span></span>|
|<span data-ttu-id="95263-164">deviceModel</span><span class="sxs-lookup"><span data-stu-id="95263-164">deviceModel</span></span>|<span data-ttu-id="95263-165">String</span><span class="sxs-lookup"><span data-stu-id="95263-165">String</span></span>|<span data-ttu-id="95263-166">レポートされているデバイス モデル</span><span class="sxs-lookup"><span data-stu-id="95263-166">The device model that is being reported</span></span>|
|<span data-ttu-id="95263-167">state</span><span class="sxs-lookup"><span data-stu-id="95263-167">state</span></span>|[<span data-ttu-id="95263-168">complianceStatus</span><span class="sxs-lookup"><span data-stu-id="95263-168">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="95263-169">設定のコンプライアンスの状態です。</span><span class="sxs-lookup"><span data-stu-id="95263-169">The compliance state of the setting.</span></span> <span data-ttu-id="95263-170">可能な値は、`unknown`、`notApplicable`、`compliant`、`remediated`、`nonCompliant`、`error`、`conflict`、`notAssigned` です。</span><span class="sxs-lookup"><span data-stu-id="95263-170">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="95263-171">complianceGracePeriodExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="95263-171">complianceGracePeriodExpirationDateTime</span></span>|<span data-ttu-id="95263-172">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="95263-172">DateTimeOffset</span></span>|<span data-ttu-id="95263-173">デバイス コンプライアンスの猶予期間が過ぎる DateTime</span><span class="sxs-lookup"><span data-stu-id="95263-173">The DateTime when device compliance grace period expires</span></span>|



## <a name="response"></a><span data-ttu-id="95263-174">応答</span><span class="sxs-lookup"><span data-stu-id="95263-174">Response</span></span>
<span data-ttu-id="95263-175">成功した場合、このメソッドは `200 OK` 応答コードと、更新された [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) オブジェクトを応答本文で返します。</span><span class="sxs-lookup"><span data-stu-id="95263-175">If successful, this method returns a `200 OK` response code and an updated [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="95263-176">例</span><span class="sxs-lookup"><span data-stu-id="95263-176">Example</span></span>
### <a name="request"></a><span data-ttu-id="95263-177">要求</span><span class="sxs-lookup"><span data-stu-id="95263-177">Request</span></span>
<span data-ttu-id="95263-178">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="95263-178">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicySettingStateSummaries/{deviceCompliancePolicySettingStateSummaryId}/deviceComplianceSettingStates/{deviceComplianceSettingStateId}
Content-type: application/json
Content-length: 482

{
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

### <a name="response"></a><span data-ttu-id="95263-179">応答</span><span class="sxs-lookup"><span data-stu-id="95263-179">Response</span></span>
<span data-ttu-id="95263-p105">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="95263-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




