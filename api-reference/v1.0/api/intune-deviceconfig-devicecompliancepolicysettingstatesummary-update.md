---
title: deviceCompliancePolicySettingStateSummary の更新
description: deviceCompliancePolicySettingStateSummary オブジェクトのプロパティを更新します。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 97eec7bba67552c21c208ed087aab40a096d47b7
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27830024"
---
# <a name="update-devicecompliancepolicysettingstatesummary"></a><span data-ttu-id="1557c-103">deviceCompliancePolicySettingStateSummary の更新</span><span class="sxs-lookup"><span data-stu-id="1557c-103">Update deviceCompliancePolicySettingStateSummary</span></span>

> <span data-ttu-id="1557c-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="1557c-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="1557c-105">[deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="1557c-105">Update the properties of a [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="1557c-106">前提条件</span><span class="sxs-lookup"><span data-stu-id="1557c-106">Prerequisites</span></span>
<span data-ttu-id="1557c-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="1557c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1557c-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="1557c-109">Permission type</span></span>|<span data-ttu-id="1557c-110">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="1557c-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1557c-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="1557c-111">Delegated (work or school account)</span></span>|<span data-ttu-id="1557c-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1557c-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="1557c-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="1557c-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1557c-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="1557c-114">Not supported.</span></span>|
|<span data-ttu-id="1557c-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="1557c-115">Application</span></span>|<span data-ttu-id="1557c-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="1557c-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="1557c-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="1557c-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicySettingStateSummaries/{deviceCompliancePolicySettingStateSummaryId}
```

## <a name="request-headers"></a><span data-ttu-id="1557c-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="1557c-118">Request headers</span></span>
|<span data-ttu-id="1557c-119">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="1557c-119">Header</span></span>|<span data-ttu-id="1557c-120">値</span><span class="sxs-lookup"><span data-stu-id="1557c-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1557c-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="1557c-121">Authorization</span></span>|<span data-ttu-id="1557c-122">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="1557c-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1557c-123">Accept</span><span class="sxs-lookup"><span data-stu-id="1557c-123">Accept</span></span>|<span data-ttu-id="1557c-124">application/json</span><span class="sxs-lookup"><span data-stu-id="1557c-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1557c-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="1557c-125">Request body</span></span>
<span data-ttu-id="1557c-126">要求本文で、[deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="1557c-126">In the request body, supply a JSON representation for the [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md) object.</span></span>

<span data-ttu-id="1557c-127">次の表に、[deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md) の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="1557c-127">The following table shows the properties that are required when you create the [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md).</span></span>

|<span data-ttu-id="1557c-128">プロパティ</span><span class="sxs-lookup"><span data-stu-id="1557c-128">Property</span></span>|<span data-ttu-id="1557c-129">種類</span><span class="sxs-lookup"><span data-stu-id="1557c-129">Type</span></span>|<span data-ttu-id="1557c-130">説明</span><span class="sxs-lookup"><span data-stu-id="1557c-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1557c-131">ID</span><span class="sxs-lookup"><span data-stu-id="1557c-131">id</span></span>|<span data-ttu-id="1557c-132">String</span><span class="sxs-lookup"><span data-stu-id="1557c-132">String</span></span>|<span data-ttu-id="1557c-133">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="1557c-133">Key of the entity.</span></span>|
|<span data-ttu-id="1557c-134">setting</span><span class="sxs-lookup"><span data-stu-id="1557c-134">setting</span></span>|<span data-ttu-id="1557c-135">String</span><span class="sxs-lookup"><span data-stu-id="1557c-135">String</span></span>|<span data-ttu-id="1557c-136">設定のクラス名とプロパティ名。</span><span class="sxs-lookup"><span data-stu-id="1557c-136">The setting class name and property name.</span></span>|
|<span data-ttu-id="1557c-137">settingName</span><span class="sxs-lookup"><span data-stu-id="1557c-137">settingName</span></span>|<span data-ttu-id="1557c-138">String</span><span class="sxs-lookup"><span data-stu-id="1557c-138">String</span></span>|<span data-ttu-id="1557c-139">設定の名前。</span><span class="sxs-lookup"><span data-stu-id="1557c-139">Name of the setting.</span></span>|
|<span data-ttu-id="1557c-140">platformType</span><span class="sxs-lookup"><span data-stu-id="1557c-140">platformType</span></span>|[<span data-ttu-id="1557c-141">policyPlatformType</span><span class="sxs-lookup"><span data-stu-id="1557c-141">policyPlatformType</span></span>](../resources/intune-deviceconfig-policyplatformtype.md)|<span data-ttu-id="1557c-142">設定のプラットフォームです。</span><span class="sxs-lookup"><span data-stu-id="1557c-142">Setting platform.</span></span> <span data-ttu-id="1557c-143">可能な値は、`android`、`iOS`、`macOS`、`windowsPhone81`、`windows81AndLater`、`windows10AndLater`、`androidWorkProfile`、`all` です。</span><span class="sxs-lookup"><span data-stu-id="1557c-143">Possible values are: `android`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `all`.</span></span>|
|<span data-ttu-id="1557c-144">unknownDeviceCount</span><span class="sxs-lookup"><span data-stu-id="1557c-144">unknownDeviceCount</span></span>|<span data-ttu-id="1557c-145">Int32</span><span class="sxs-lookup"><span data-stu-id="1557c-145">Int32</span></span>|<span data-ttu-id="1557c-146">不明なデバイスの数</span><span class="sxs-lookup"><span data-stu-id="1557c-146">Number of unknown devices</span></span>|
|<span data-ttu-id="1557c-147">notApplicableDeviceCount</span><span class="sxs-lookup"><span data-stu-id="1557c-147">notApplicableDeviceCount</span></span>|<span data-ttu-id="1557c-148">Int32</span><span class="sxs-lookup"><span data-stu-id="1557c-148">Int32</span></span>|<span data-ttu-id="1557c-149">該当しないデバイスの数</span><span class="sxs-lookup"><span data-stu-id="1557c-149">Number of not applicable devices</span></span>|
|<span data-ttu-id="1557c-150">compliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="1557c-150">compliantDeviceCount</span></span>|<span data-ttu-id="1557c-151">Int32</span><span class="sxs-lookup"><span data-stu-id="1557c-151">Int32</span></span>|<span data-ttu-id="1557c-152">準拠デバイスの数</span><span class="sxs-lookup"><span data-stu-id="1557c-152">Number of compliant devices</span></span>|
|<span data-ttu-id="1557c-153">remediatedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="1557c-153">remediatedDeviceCount</span></span>|<span data-ttu-id="1557c-154">Int32</span><span class="sxs-lookup"><span data-stu-id="1557c-154">Int32</span></span>|<span data-ttu-id="1557c-155">修復済みデバイスの数</span><span class="sxs-lookup"><span data-stu-id="1557c-155">Number of remediated devices</span></span>|
|<span data-ttu-id="1557c-156">nonCompliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="1557c-156">nonCompliantDeviceCount</span></span>|<span data-ttu-id="1557c-157">Int32</span><span class="sxs-lookup"><span data-stu-id="1557c-157">Int32</span></span>|<span data-ttu-id="1557c-158">準拠していないデバイスの数</span><span class="sxs-lookup"><span data-stu-id="1557c-158">Number of NonCompliant devices</span></span>|
|<span data-ttu-id="1557c-159">errorDeviceCount</span><span class="sxs-lookup"><span data-stu-id="1557c-159">errorDeviceCount</span></span>|<span data-ttu-id="1557c-160">Int32</span><span class="sxs-lookup"><span data-stu-id="1557c-160">Int32</span></span>|<span data-ttu-id="1557c-161">エラー デバイスの数</span><span class="sxs-lookup"><span data-stu-id="1557c-161">Number of error devices</span></span>|
|<span data-ttu-id="1557c-162">conflictDeviceCount</span><span class="sxs-lookup"><span data-stu-id="1557c-162">conflictDeviceCount</span></span>|<span data-ttu-id="1557c-163">Int32</span><span class="sxs-lookup"><span data-stu-id="1557c-163">Int32</span></span>|<span data-ttu-id="1557c-164">競合デバイスの数</span><span class="sxs-lookup"><span data-stu-id="1557c-164">Number of conflict devices</span></span>|



## <a name="response"></a><span data-ttu-id="1557c-165">応答</span><span class="sxs-lookup"><span data-stu-id="1557c-165">Response</span></span>
<span data-ttu-id="1557c-166">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で更新された [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="1557c-166">If successful, this method returns a `200 OK` response code and an updated [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1557c-167">例</span><span class="sxs-lookup"><span data-stu-id="1557c-167">Example</span></span>
### <a name="request"></a><span data-ttu-id="1557c-168">要求</span><span class="sxs-lookup"><span data-stu-id="1557c-168">Request</span></span>
<span data-ttu-id="1557c-169">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="1557c-169">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/deviceCompliancePolicySettingStateSummaries/{deviceCompliancePolicySettingStateSummaryId}
Content-type: application/json
Content-length: 391

{
  "@odata.type": "#microsoft.graph.deviceCompliancePolicySettingStateSummary",
  "setting": "Setting value",
  "settingName": "Setting Name value",
  "platformType": "iOS",
  "unknownDeviceCount": 2,
  "notApplicableDeviceCount": 8,
  "compliantDeviceCount": 4,
  "remediatedDeviceCount": 5,
  "nonCompliantDeviceCount": 7,
  "errorDeviceCount": 0,
  "conflictDeviceCount": 3
}
```

### <a name="response"></a><span data-ttu-id="1557c-170">応答</span><span class="sxs-lookup"><span data-stu-id="1557c-170">Response</span></span>
<span data-ttu-id="1557c-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="1557c-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 440

{
  "@odata.type": "#microsoft.graph.deviceCompliancePolicySettingStateSummary",
  "id": "7474d6d5-d6d5-7474-d5d6-7474d5d67474",
  "setting": "Setting value",
  "settingName": "Setting Name value",
  "platformType": "iOS",
  "unknownDeviceCount": 2,
  "notApplicableDeviceCount": 8,
  "compliantDeviceCount": 4,
  "remediatedDeviceCount": 5,
  "nonCompliantDeviceCount": 7,
  "errorDeviceCount": 0,
  "conflictDeviceCount": 3
}
```



