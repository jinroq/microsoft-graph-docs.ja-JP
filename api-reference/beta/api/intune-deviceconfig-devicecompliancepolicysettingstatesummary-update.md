---
title: deviceCompliancePolicySettingStateSummary の更新
description: deviceCompliancePolicySettingStateSummary オブジェクトのプロパティを更新します。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: b2861d37c6e742689af2cf2d480f0961b9ccd9a5
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/14/2019
ms.locfileid: "34968274"
---
# <a name="update-devicecompliancepolicysettingstatesummary"></a><span data-ttu-id="d39e5-103">deviceCompliancePolicySettingStateSummary の更新</span><span class="sxs-lookup"><span data-stu-id="d39e5-103">Update deviceCompliancePolicySettingStateSummary</span></span>

> <span data-ttu-id="d39e5-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d39e5-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d39e5-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="d39e5-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d39e5-106">[deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="d39e5-106">Update the properties of a [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d39e5-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="d39e5-107">Prerequisites</span></span>
<span data-ttu-id="d39e5-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="d39e5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d39e5-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="d39e5-110">Permission type</span></span>|<span data-ttu-id="d39e5-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="d39e5-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d39e5-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="d39e5-112">Delegated (work or school account)</span></span>|<span data-ttu-id="d39e5-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d39e5-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="d39e5-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="d39e5-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d39e5-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d39e5-115">Not supported.</span></span>|
|<span data-ttu-id="d39e5-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="d39e5-116">Application</span></span>|<span data-ttu-id="d39e5-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d39e5-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d39e5-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="d39e5-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicySettingStateSummaries/{deviceCompliancePolicySettingStateSummaryId}
```

## <a name="request-headers"></a><span data-ttu-id="d39e5-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="d39e5-119">Request headers</span></span>
|<span data-ttu-id="d39e5-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="d39e5-120">Header</span></span>|<span data-ttu-id="d39e5-121">値</span><span class="sxs-lookup"><span data-stu-id="d39e5-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d39e5-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="d39e5-122">Authorization</span></span>|<span data-ttu-id="d39e5-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="d39e5-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d39e5-124">承諾</span><span class="sxs-lookup"><span data-stu-id="d39e5-124">Accept</span></span>|<span data-ttu-id="d39e5-125">application/json</span><span class="sxs-lookup"><span data-stu-id="d39e5-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d39e5-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="d39e5-126">Request body</span></span>
<span data-ttu-id="d39e5-127">要求本文で、[deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="d39e5-127">In the request body, supply a JSON representation for the [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md) object.</span></span>

<span data-ttu-id="d39e5-128">次の表に、[deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md) の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="d39e5-128">The following table shows the properties that are required when you create the [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md).</span></span>

|<span data-ttu-id="d39e5-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="d39e5-129">Property</span></span>|<span data-ttu-id="d39e5-130">型</span><span class="sxs-lookup"><span data-stu-id="d39e5-130">Type</span></span>|<span data-ttu-id="d39e5-131">説明</span><span class="sxs-lookup"><span data-stu-id="d39e5-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d39e5-132">id</span><span class="sxs-lookup"><span data-stu-id="d39e5-132">id</span></span>|<span data-ttu-id="d39e5-133">String</span><span class="sxs-lookup"><span data-stu-id="d39e5-133">String</span></span>|<span data-ttu-id="d39e5-134">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="d39e5-134">Key of the entity.</span></span>|
|<span data-ttu-id="d39e5-135">setting</span><span class="sxs-lookup"><span data-stu-id="d39e5-135">setting</span></span>|<span data-ttu-id="d39e5-136">String</span><span class="sxs-lookup"><span data-stu-id="d39e5-136">String</span></span>|<span data-ttu-id="d39e5-137">設定のクラス名とプロパティ名。</span><span class="sxs-lookup"><span data-stu-id="d39e5-137">The setting class name and property name.</span></span>|
|<span data-ttu-id="d39e5-138">settingName</span><span class="sxs-lookup"><span data-stu-id="d39e5-138">settingName</span></span>|<span data-ttu-id="d39e5-139">String</span><span class="sxs-lookup"><span data-stu-id="d39e5-139">String</span></span>|<span data-ttu-id="d39e5-140">設定の名前。</span><span class="sxs-lookup"><span data-stu-id="d39e5-140">Name of the setting.</span></span>|
|<span data-ttu-id="d39e5-141">platformType</span><span class="sxs-lookup"><span data-stu-id="d39e5-141">platformType</span></span>|[<span data-ttu-id="d39e5-142">policyPlatformType</span><span class="sxs-lookup"><span data-stu-id="d39e5-142">policyPlatformType</span></span>](../resources/intune-deviceconfig-policyplatformtype.md)|<span data-ttu-id="d39e5-143">プラットフォームを設定します。</span><span class="sxs-lookup"><span data-stu-id="d39e5-143">Setting platform.</span></span> <span data-ttu-id="d39e5-144">可能な値は、`android`、`androidForWork`、`iOS`、`macOS`、`windowsPhone81`、`windows81AndLater`、`windows10AndLater`、`androidWorkProfile`、`all` です。</span><span class="sxs-lookup"><span data-stu-id="d39e5-144">Possible values are: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `all`.</span></span>|
|<span data-ttu-id="d39e5-145">unknownDeviceCount</span><span class="sxs-lookup"><span data-stu-id="d39e5-145">unknownDeviceCount</span></span>|<span data-ttu-id="d39e5-146">Int32</span><span class="sxs-lookup"><span data-stu-id="d39e5-146">Int32</span></span>|<span data-ttu-id="d39e5-147">不明なデバイスの数</span><span class="sxs-lookup"><span data-stu-id="d39e5-147">Number of unknown devices</span></span>|
|<span data-ttu-id="d39e5-148">notApplicableDeviceCount</span><span class="sxs-lookup"><span data-stu-id="d39e5-148">notApplicableDeviceCount</span></span>|<span data-ttu-id="d39e5-149">Int32</span><span class="sxs-lookup"><span data-stu-id="d39e5-149">Int32</span></span>|<span data-ttu-id="d39e5-150">該当しないデバイスの数</span><span class="sxs-lookup"><span data-stu-id="d39e5-150">Number of not applicable devices</span></span>|
|<span data-ttu-id="d39e5-151">compliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="d39e5-151">compliantDeviceCount</span></span>|<span data-ttu-id="d39e5-152">Int32</span><span class="sxs-lookup"><span data-stu-id="d39e5-152">Int32</span></span>|<span data-ttu-id="d39e5-153">準拠デバイスの数</span><span class="sxs-lookup"><span data-stu-id="d39e5-153">Number of compliant devices</span></span>|
|<span data-ttu-id="d39e5-154">remediatedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="d39e5-154">remediatedDeviceCount</span></span>|<span data-ttu-id="d39e5-155">Int32</span><span class="sxs-lookup"><span data-stu-id="d39e5-155">Int32</span></span>|<span data-ttu-id="d39e5-156">修復済みデバイスの数</span><span class="sxs-lookup"><span data-stu-id="d39e5-156">Number of remediated devices</span></span>|
|<span data-ttu-id="d39e5-157">nonCompliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="d39e5-157">nonCompliantDeviceCount</span></span>|<span data-ttu-id="d39e5-158">Int32</span><span class="sxs-lookup"><span data-stu-id="d39e5-158">Int32</span></span>|<span data-ttu-id="d39e5-159">準拠していないデバイスの数</span><span class="sxs-lookup"><span data-stu-id="d39e5-159">Number of NonCompliant devices</span></span>|
|<span data-ttu-id="d39e5-160">errorDeviceCount</span><span class="sxs-lookup"><span data-stu-id="d39e5-160">errorDeviceCount</span></span>|<span data-ttu-id="d39e5-161">Int32</span><span class="sxs-lookup"><span data-stu-id="d39e5-161">Int32</span></span>|<span data-ttu-id="d39e5-162">エラー デバイスの数</span><span class="sxs-lookup"><span data-stu-id="d39e5-162">Number of error devices</span></span>|
|<span data-ttu-id="d39e5-163">conflictDeviceCount</span><span class="sxs-lookup"><span data-stu-id="d39e5-163">conflictDeviceCount</span></span>|<span data-ttu-id="d39e5-164">Int32</span><span class="sxs-lookup"><span data-stu-id="d39e5-164">Int32</span></span>|<span data-ttu-id="d39e5-165">競合デバイスの数</span><span class="sxs-lookup"><span data-stu-id="d39e5-165">Number of conflict devices</span></span>|



## <a name="response"></a><span data-ttu-id="d39e5-166">応答</span><span class="sxs-lookup"><span data-stu-id="d39e5-166">Response</span></span>
<span data-ttu-id="d39e5-167">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で更新された [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="d39e5-167">If successful, this method returns a `200 OK` response code and an updated [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d39e5-168">例</span><span class="sxs-lookup"><span data-stu-id="d39e5-168">Example</span></span>

### <a name="request"></a><span data-ttu-id="d39e5-169">要求</span><span class="sxs-lookup"><span data-stu-id="d39e5-169">Request</span></span>
<span data-ttu-id="d39e5-170">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="d39e5-170">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicySettingStateSummaries/{deviceCompliancePolicySettingStateSummaryId}
Content-type: application/json
Content-length: 402

{
  "@odata.type": "#microsoft.graph.deviceCompliancePolicySettingStateSummary",
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

### <a name="response"></a><span data-ttu-id="d39e5-171">応答</span><span class="sxs-lookup"><span data-stu-id="d39e5-171">Response</span></span>
<span data-ttu-id="d39e5-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="d39e5-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





