---
title: deviceCompliancePolicySettingStateSummary の更新
description: deviceCompliancePolicySettingStateSummary オブジェクトのプロパティを更新します。
author: tfitzmac
ms.openlocfilehash: d85aa50045c3378a2a4da7826dcaa3fb968664ce
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27345074"
---
# <a name="update-devicecompliancepolicysettingstatesummary"></a><span data-ttu-id="8eed3-103">deviceCompliancePolicySettingStateSummary の更新</span><span class="sxs-lookup"><span data-stu-id="8eed3-103">Update deviceCompliancePolicySettingStateSummary</span></span>

> <span data-ttu-id="8eed3-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="8eed3-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="8eed3-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="8eed3-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="8eed3-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="8eed3-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="8eed3-107">[deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="8eed3-107">Update the properties of a [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="8eed3-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="8eed3-108">Prerequisites</span></span>
<span data-ttu-id="8eed3-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="8eed3-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8eed3-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="8eed3-111">Permission type</span></span>|<span data-ttu-id="8eed3-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="8eed3-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8eed3-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="8eed3-113">Delegated (work or school account)</span></span>|<span data-ttu-id="8eed3-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8eed3-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="8eed3-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="8eed3-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8eed3-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="8eed3-116">Not supported.</span></span>|
|<span data-ttu-id="8eed3-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="8eed3-117">Application</span></span>|<span data-ttu-id="8eed3-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="8eed3-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="8eed3-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="8eed3-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicySettingStateSummaries/{deviceCompliancePolicySettingStateSummaryId}
```

## <a name="request-headers"></a><span data-ttu-id="8eed3-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="8eed3-120">Request headers</span></span>
|<span data-ttu-id="8eed3-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="8eed3-121">Header</span></span>|<span data-ttu-id="8eed3-122">値</span><span class="sxs-lookup"><span data-stu-id="8eed3-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8eed3-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="8eed3-123">Authorization</span></span>|<span data-ttu-id="8eed3-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="8eed3-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8eed3-125">Accept</span><span class="sxs-lookup"><span data-stu-id="8eed3-125">Accept</span></span>|<span data-ttu-id="8eed3-126">application/json</span><span class="sxs-lookup"><span data-stu-id="8eed3-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8eed3-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="8eed3-127">Request body</span></span>
<span data-ttu-id="8eed3-128">要求本文で、[deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="8eed3-128">In the request body, supply a JSON representation for the [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md) object.</span></span>

<span data-ttu-id="8eed3-129">次の表に、[deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md) の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="8eed3-129">The following table shows the properties that are required when you create the [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md).</span></span>

|<span data-ttu-id="8eed3-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="8eed3-130">Property</span></span>|<span data-ttu-id="8eed3-131">種類</span><span class="sxs-lookup"><span data-stu-id="8eed3-131">Type</span></span>|<span data-ttu-id="8eed3-132">説明</span><span class="sxs-lookup"><span data-stu-id="8eed3-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8eed3-133">ID</span><span class="sxs-lookup"><span data-stu-id="8eed3-133">id</span></span>|<span data-ttu-id="8eed3-134">String</span><span class="sxs-lookup"><span data-stu-id="8eed3-134">String</span></span>|<span data-ttu-id="8eed3-135">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="8eed3-135">Key of the entity.</span></span>|
|<span data-ttu-id="8eed3-136">setting</span><span class="sxs-lookup"><span data-stu-id="8eed3-136">setting</span></span>|<span data-ttu-id="8eed3-137">String</span><span class="sxs-lookup"><span data-stu-id="8eed3-137">String</span></span>|<span data-ttu-id="8eed3-138">設定のクラス名とプロパティ名。</span><span class="sxs-lookup"><span data-stu-id="8eed3-138">The setting class name and property name.</span></span>|
|<span data-ttu-id="8eed3-139">settingName</span><span class="sxs-lookup"><span data-stu-id="8eed3-139">settingName</span></span>|<span data-ttu-id="8eed3-140">String</span><span class="sxs-lookup"><span data-stu-id="8eed3-140">String</span></span>|<span data-ttu-id="8eed3-141">設定の名前。</span><span class="sxs-lookup"><span data-stu-id="8eed3-141">Name of the setting.</span></span>|
|<span data-ttu-id="8eed3-142">platformType</span><span class="sxs-lookup"><span data-stu-id="8eed3-142">platformType</span></span>|[<span data-ttu-id="8eed3-143">policyPlatformType</span><span class="sxs-lookup"><span data-stu-id="8eed3-143">policyPlatformType</span></span>](../resources/intune-deviceconfig-policyplatformtype.md)|<span data-ttu-id="8eed3-144">設定のプラットフォームです。</span><span class="sxs-lookup"><span data-stu-id="8eed3-144">Setting platform.</span></span> <span data-ttu-id="8eed3-145">可能な値は、`android`、`androidForWork`、`iOS`、`macOS`、`windowsPhone81`、`windows81AndLater`、`windows10AndLater`、`androidWorkProfile`、`all` です。</span><span class="sxs-lookup"><span data-stu-id="8eed3-145">Possible values are: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `all`.</span></span>|
|<span data-ttu-id="8eed3-146">unknownDeviceCount</span><span class="sxs-lookup"><span data-stu-id="8eed3-146">unknownDeviceCount</span></span>|<span data-ttu-id="8eed3-147">Int32</span><span class="sxs-lookup"><span data-stu-id="8eed3-147">Int32</span></span>|<span data-ttu-id="8eed3-148">不明なデバイスの数</span><span class="sxs-lookup"><span data-stu-id="8eed3-148">Number of unknown devices</span></span>|
|<span data-ttu-id="8eed3-149">notApplicableDeviceCount</span><span class="sxs-lookup"><span data-stu-id="8eed3-149">notApplicableDeviceCount</span></span>|<span data-ttu-id="8eed3-150">Int32</span><span class="sxs-lookup"><span data-stu-id="8eed3-150">Int32</span></span>|<span data-ttu-id="8eed3-151">該当しないデバイスの数</span><span class="sxs-lookup"><span data-stu-id="8eed3-151">Number of not applicable devices</span></span>|
|<span data-ttu-id="8eed3-152">compliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="8eed3-152">compliantDeviceCount</span></span>|<span data-ttu-id="8eed3-153">Int32</span><span class="sxs-lookup"><span data-stu-id="8eed3-153">Int32</span></span>|<span data-ttu-id="8eed3-154">準拠デバイスの数</span><span class="sxs-lookup"><span data-stu-id="8eed3-154">Number of compliant devices</span></span>|
|<span data-ttu-id="8eed3-155">remediatedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="8eed3-155">remediatedDeviceCount</span></span>|<span data-ttu-id="8eed3-156">Int32</span><span class="sxs-lookup"><span data-stu-id="8eed3-156">Int32</span></span>|<span data-ttu-id="8eed3-157">修復済みデバイスの数</span><span class="sxs-lookup"><span data-stu-id="8eed3-157">Number of remediated devices</span></span>|
|<span data-ttu-id="8eed3-158">nonCompliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="8eed3-158">nonCompliantDeviceCount</span></span>|<span data-ttu-id="8eed3-159">Int32</span><span class="sxs-lookup"><span data-stu-id="8eed3-159">Int32</span></span>|<span data-ttu-id="8eed3-160">準拠していないデバイスの数</span><span class="sxs-lookup"><span data-stu-id="8eed3-160">Number of NonCompliant devices</span></span>|
|<span data-ttu-id="8eed3-161">errorDeviceCount</span><span class="sxs-lookup"><span data-stu-id="8eed3-161">errorDeviceCount</span></span>|<span data-ttu-id="8eed3-162">Int32</span><span class="sxs-lookup"><span data-stu-id="8eed3-162">Int32</span></span>|<span data-ttu-id="8eed3-163">エラー デバイスの数</span><span class="sxs-lookup"><span data-stu-id="8eed3-163">Number of error devices</span></span>|
|<span data-ttu-id="8eed3-164">conflictDeviceCount</span><span class="sxs-lookup"><span data-stu-id="8eed3-164">conflictDeviceCount</span></span>|<span data-ttu-id="8eed3-165">Int32</span><span class="sxs-lookup"><span data-stu-id="8eed3-165">Int32</span></span>|<span data-ttu-id="8eed3-166">競合デバイスの数</span><span class="sxs-lookup"><span data-stu-id="8eed3-166">Number of conflict devices</span></span>|



## <a name="response"></a><span data-ttu-id="8eed3-167">応答</span><span class="sxs-lookup"><span data-stu-id="8eed3-167">Response</span></span>
<span data-ttu-id="8eed3-168">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で更新された [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="8eed3-168">If successful, this method returns a `200 OK` response code and an updated [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8eed3-169">例</span><span class="sxs-lookup"><span data-stu-id="8eed3-169">Example</span></span>
### <a name="request"></a><span data-ttu-id="8eed3-170">要求</span><span class="sxs-lookup"><span data-stu-id="8eed3-170">Request</span></span>
<span data-ttu-id="8eed3-171">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="8eed3-171">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicySettingStateSummaries/{deviceCompliancePolicySettingStateSummaryId}
Content-type: application/json
Content-length: 322

{
  "setting": "Setting value",
  "settingName": "Setting Name value",
  "platformType": "androidForWork",
  "unknownDeviceCount": 2,
  "notApplicableDeviceCount": 8,
  "compliantDeviceCount": 4,
  "remediatedDeviceCount": 5,
  "nonCompliantDeviceCount": 7,
  "errorDeviceCount": 0,
  "conflictDeviceCount": 3
}
```

### <a name="response"></a><span data-ttu-id="8eed3-172">応答</span><span class="sxs-lookup"><span data-stu-id="8eed3-172">Response</span></span>
<span data-ttu-id="8eed3-p104">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="8eed3-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 451

{
  "@odata.type": "#microsoft.graph.deviceCompliancePolicySettingStateSummary",
  "id": "7474d6d5-d6d5-7474-d5d6-7474d5d67474",
  "setting": "Setting value",
  "settingName": "Setting Name value",
  "platformType": "androidForWork",
  "unknownDeviceCount": 2,
  "notApplicableDeviceCount": 8,
  "compliantDeviceCount": 4,
  "remediatedDeviceCount": 5,
  "nonCompliantDeviceCount": 7,
  "errorDeviceCount": 0,
  "conflictDeviceCount": 3
}
```




