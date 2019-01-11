---
title: deviceComplianceSettingState の更新
description: deviceComplianceSettingState オブジェクトのプロパティを更新します。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 0f607b699f4a89d925f099724851d92800ed9ddc
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27807136"
---
# <a name="update-devicecompliancesettingstate"></a><span data-ttu-id="78e2a-103">deviceComplianceSettingState の更新</span><span class="sxs-lookup"><span data-stu-id="78e2a-103">Update deviceComplianceSettingState</span></span>

> <span data-ttu-id="78e2a-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="78e2a-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="78e2a-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="78e2a-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="78e2a-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="78e2a-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="78e2a-107">[deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="78e2a-107">Update the properties of a [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="78e2a-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="78e2a-108">Prerequisites</span></span>
<span data-ttu-id="78e2a-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="78e2a-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="78e2a-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="78e2a-111">Permission type</span></span>|<span data-ttu-id="78e2a-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="78e2a-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="78e2a-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="78e2a-113">Delegated (work or school account)</span></span>|<span data-ttu-id="78e2a-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="78e2a-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="78e2a-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="78e2a-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="78e2a-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="78e2a-116">Not supported.</span></span>|
|<span data-ttu-id="78e2a-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="78e2a-117">Application</span></span>|<span data-ttu-id="78e2a-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="78e2a-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="78e2a-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="78e2a-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicySettingStateSummaries/{deviceCompliancePolicySettingStateSummaryId}/deviceComplianceSettingStates/{deviceComplianceSettingStateId}
```

## <a name="request-headers"></a><span data-ttu-id="78e2a-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="78e2a-120">Request headers</span></span>
|<span data-ttu-id="78e2a-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="78e2a-121">Header</span></span>|<span data-ttu-id="78e2a-122">値</span><span class="sxs-lookup"><span data-stu-id="78e2a-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="78e2a-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="78e2a-123">Authorization</span></span>|<span data-ttu-id="78e2a-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="78e2a-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="78e2a-125">Accept</span><span class="sxs-lookup"><span data-stu-id="78e2a-125">Accept</span></span>|<span data-ttu-id="78e2a-126">application/json</span><span class="sxs-lookup"><span data-stu-id="78e2a-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="78e2a-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="78e2a-127">Request body</span></span>
<span data-ttu-id="78e2a-128">要求本文で、[deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="78e2a-128">In the request body, supply a JSON representation for the [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) object.</span></span>

<span data-ttu-id="78e2a-129">次の表に、[deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="78e2a-129">The following table shows the properties that are required when you create the [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md).</span></span>

|<span data-ttu-id="78e2a-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="78e2a-130">Property</span></span>|<span data-ttu-id="78e2a-131">種類</span><span class="sxs-lookup"><span data-stu-id="78e2a-131">Type</span></span>|<span data-ttu-id="78e2a-132">説明</span><span class="sxs-lookup"><span data-stu-id="78e2a-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="78e2a-133">ID</span><span class="sxs-lookup"><span data-stu-id="78e2a-133">id</span></span>|<span data-ttu-id="78e2a-134">String</span><span class="sxs-lookup"><span data-stu-id="78e2a-134">String</span></span>|<span data-ttu-id="78e2a-135">エンティティのキー</span><span class="sxs-lookup"><span data-stu-id="78e2a-135">Key of the entity</span></span>|
|<span data-ttu-id="78e2a-136">platformType</span><span class="sxs-lookup"><span data-stu-id="78e2a-136">platformType</span></span>|[<span data-ttu-id="78e2a-137">deviceType</span><span class="sxs-lookup"><span data-stu-id="78e2a-137">deviceType</span></span>](../resources/intune-shared-devicetype.md)|<span data-ttu-id="78e2a-138">デバイス プラットフォームのタイプです。</span><span class="sxs-lookup"><span data-stu-id="78e2a-138">Device platform type.</span></span> <span data-ttu-id="78e2a-139">使用可能な値: `desktop`、 `windowsRT`、 `winMO6`、 `nokia`、 `windowsPhone`、 `mac`、 `winCE`、 `winEmbedded`、 `iPhone`、 `iPad`、 `iPod`、 `android`、 `iSocConsumer`、 `unix`、 `macMDM`、 `holoLens`、 `surfaceHub`、 `androidForWork`、 `androidEnterprise`, `blackberry`, `palm`, `unknown`.</span><span class="sxs-lookup"><span data-stu-id="78e2a-139">Possible values are: `desktop`, `windowsRT`, `winMO6`, `nokia`, `windowsPhone`, `mac`, `winCE`, `winEmbedded`, `iPhone`, `iPad`, `iPod`, `android`, `iSocConsumer`, `unix`, `macMDM`, `holoLens`, `surfaceHub`, `androidForWork`, `androidEnterprise`, `blackberry`, `palm`, `unknown`.</span></span>|
|<span data-ttu-id="78e2a-140">setting</span><span class="sxs-lookup"><span data-stu-id="78e2a-140">setting</span></span>|<span data-ttu-id="78e2a-141">String</span><span class="sxs-lookup"><span data-stu-id="78e2a-141">String</span></span>|<span data-ttu-id="78e2a-142">設定のクラス名とプロパティ名。</span><span class="sxs-lookup"><span data-stu-id="78e2a-142">The setting class name and property name.</span></span>|
|<span data-ttu-id="78e2a-143">settingName</span><span class="sxs-lookup"><span data-stu-id="78e2a-143">settingName</span></span>|<span data-ttu-id="78e2a-144">String</span><span class="sxs-lookup"><span data-stu-id="78e2a-144">String</span></span>|<span data-ttu-id="78e2a-145">レポートされている設定名。</span><span class="sxs-lookup"><span data-stu-id="78e2a-145">The Setting Name that is being reported</span></span>|
|<span data-ttu-id="78e2a-146">deviceId</span><span class="sxs-lookup"><span data-stu-id="78e2a-146">deviceId</span></span>|<span data-ttu-id="78e2a-147">String</span><span class="sxs-lookup"><span data-stu-id="78e2a-147">String</span></span>|<span data-ttu-id="78e2a-148">レポートされているデバイス ID。</span><span class="sxs-lookup"><span data-stu-id="78e2a-148">The Device Id that is being reported</span></span>|
|<span data-ttu-id="78e2a-149">deviceName</span><span class="sxs-lookup"><span data-stu-id="78e2a-149">deviceName</span></span>|<span data-ttu-id="78e2a-150">String</span><span class="sxs-lookup"><span data-stu-id="78e2a-150">String</span></span>|<span data-ttu-id="78e2a-151">レポートされているデバイス名。</span><span class="sxs-lookup"><span data-stu-id="78e2a-151">The Device Name that is being reported</span></span>|
|<span data-ttu-id="78e2a-152">userId</span><span class="sxs-lookup"><span data-stu-id="78e2a-152">userId</span></span>|<span data-ttu-id="78e2a-153">String</span><span class="sxs-lookup"><span data-stu-id="78e2a-153">String</span></span>|<span data-ttu-id="78e2a-154">レポートされているユーザー ID</span><span class="sxs-lookup"><span data-stu-id="78e2a-154">The user Id that is being reported</span></span>|
|<span data-ttu-id="78e2a-155">userEmail</span><span class="sxs-lookup"><span data-stu-id="78e2a-155">userEmail</span></span>|<span data-ttu-id="78e2a-156">String</span><span class="sxs-lookup"><span data-stu-id="78e2a-156">String</span></span>|<span data-ttu-id="78e2a-157">レポートされているユーザーのメール アドレス。</span><span class="sxs-lookup"><span data-stu-id="78e2a-157">The User email address that is being reported</span></span>|
|<span data-ttu-id="78e2a-158">userName</span><span class="sxs-lookup"><span data-stu-id="78e2a-158">userName</span></span>|<span data-ttu-id="78e2a-159">String</span><span class="sxs-lookup"><span data-stu-id="78e2a-159">String</span></span>|<span data-ttu-id="78e2a-160">レポートされているユーザー名</span><span class="sxs-lookup"><span data-stu-id="78e2a-160">The User Name that is being reported</span></span>|
|<span data-ttu-id="78e2a-161">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="78e2a-161">userPrincipalName</span></span>|<span data-ttu-id="78e2a-162">String</span><span class="sxs-lookup"><span data-stu-id="78e2a-162">String</span></span>|<span data-ttu-id="78e2a-163">レポートされているユーザーの PrincipalName</span><span class="sxs-lookup"><span data-stu-id="78e2a-163">The User PrincipalName that is being reported</span></span>|
|<span data-ttu-id="78e2a-164">deviceModel</span><span class="sxs-lookup"><span data-stu-id="78e2a-164">deviceModel</span></span>|<span data-ttu-id="78e2a-165">String</span><span class="sxs-lookup"><span data-stu-id="78e2a-165">String</span></span>|<span data-ttu-id="78e2a-166">レポートされているデバイス モデル</span><span class="sxs-lookup"><span data-stu-id="78e2a-166">The device model that is being reported</span></span>|
|<span data-ttu-id="78e2a-167">state</span><span class="sxs-lookup"><span data-stu-id="78e2a-167">state</span></span>|[<span data-ttu-id="78e2a-168">complianceStatus</span><span class="sxs-lookup"><span data-stu-id="78e2a-168">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="78e2a-169">設定のコンプライアンスの状態です。</span><span class="sxs-lookup"><span data-stu-id="78e2a-169">The compliance state of the setting.</span></span> <span data-ttu-id="78e2a-170">可能な値は、`unknown`、`notApplicable`、`compliant`、`remediated`、`nonCompliant`、`error`、`conflict`、`notAssigned` です。</span><span class="sxs-lookup"><span data-stu-id="78e2a-170">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="78e2a-171">complianceGracePeriodExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="78e2a-171">complianceGracePeriodExpirationDateTime</span></span>|<span data-ttu-id="78e2a-172">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="78e2a-172">DateTimeOffset</span></span>|<span data-ttu-id="78e2a-173">デバイス コンプライアンスの猶予期間が過ぎる DateTime</span><span class="sxs-lookup"><span data-stu-id="78e2a-173">The DateTime when device compliance grace period expires</span></span>|



## <a name="response"></a><span data-ttu-id="78e2a-174">応答</span><span class="sxs-lookup"><span data-stu-id="78e2a-174">Response</span></span>
<span data-ttu-id="78e2a-175">成功した場合、このメソッドは `200 OK` 応答コードと、更新された [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) オブジェクトを応答本文で返します。</span><span class="sxs-lookup"><span data-stu-id="78e2a-175">If successful, this method returns a `200 OK` response code and an updated [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="78e2a-176">例</span><span class="sxs-lookup"><span data-stu-id="78e2a-176">Example</span></span>
### <a name="request"></a><span data-ttu-id="78e2a-177">要求</span><span class="sxs-lookup"><span data-stu-id="78e2a-177">Request</span></span>
<span data-ttu-id="78e2a-178">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="78e2a-178">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="78e2a-179">応答</span><span class="sxs-lookup"><span data-stu-id="78e2a-179">Response</span></span>
<span data-ttu-id="78e2a-p105">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="78e2a-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





