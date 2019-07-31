---
title: deviceCompliancePolicySettingStateSummary の更新
description: deviceCompliancePolicySettingStateSummary オブジェクトのプロパティを更新します。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: d5664a348e26cb5bb30bc049e0170403fae84350
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35949679"
---
# <a name="update-devicecompliancepolicysettingstatesummary"></a><span data-ttu-id="abebb-103">deviceCompliancePolicySettingStateSummary の更新</span><span class="sxs-lookup"><span data-stu-id="abebb-103">Update deviceCompliancePolicySettingStateSummary</span></span>

> <span data-ttu-id="abebb-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="abebb-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="abebb-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="abebb-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="abebb-106">[deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="abebb-106">Update the properties of a [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="abebb-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="abebb-107">Prerequisites</span></span>
<span data-ttu-id="abebb-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="abebb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="abebb-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="abebb-110">Permission type</span></span>|<span data-ttu-id="abebb-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="abebb-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="abebb-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="abebb-112">Delegated (work or school account)</span></span>|<span data-ttu-id="abebb-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="abebb-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="abebb-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="abebb-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="abebb-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="abebb-115">Not supported.</span></span>|
|<span data-ttu-id="abebb-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="abebb-116">Application</span></span>|<span data-ttu-id="abebb-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="abebb-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="abebb-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="abebb-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicySettingStateSummaries/{deviceCompliancePolicySettingStateSummaryId}
```

## <a name="request-headers"></a><span data-ttu-id="abebb-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="abebb-119">Request headers</span></span>
|<span data-ttu-id="abebb-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="abebb-120">Header</span></span>|<span data-ttu-id="abebb-121">値</span><span class="sxs-lookup"><span data-stu-id="abebb-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="abebb-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="abebb-122">Authorization</span></span>|<span data-ttu-id="abebb-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="abebb-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="abebb-124">承諾</span><span class="sxs-lookup"><span data-stu-id="abebb-124">Accept</span></span>|<span data-ttu-id="abebb-125">application/json</span><span class="sxs-lookup"><span data-stu-id="abebb-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="abebb-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="abebb-126">Request body</span></span>
<span data-ttu-id="abebb-127">要求本文で、[deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="abebb-127">In the request body, supply a JSON representation for the [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md) object.</span></span>

<span data-ttu-id="abebb-128">次の表に、[deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md) の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="abebb-128">The following table shows the properties that are required when you create the [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md).</span></span>

|<span data-ttu-id="abebb-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="abebb-129">Property</span></span>|<span data-ttu-id="abebb-130">型</span><span class="sxs-lookup"><span data-stu-id="abebb-130">Type</span></span>|<span data-ttu-id="abebb-131">説明</span><span class="sxs-lookup"><span data-stu-id="abebb-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="abebb-132">id</span><span class="sxs-lookup"><span data-stu-id="abebb-132">id</span></span>|<span data-ttu-id="abebb-133">String</span><span class="sxs-lookup"><span data-stu-id="abebb-133">String</span></span>|<span data-ttu-id="abebb-134">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="abebb-134">Key of the entity.</span></span>|
|<span data-ttu-id="abebb-135">setting</span><span class="sxs-lookup"><span data-stu-id="abebb-135">setting</span></span>|<span data-ttu-id="abebb-136">String</span><span class="sxs-lookup"><span data-stu-id="abebb-136">String</span></span>|<span data-ttu-id="abebb-137">設定のクラス名とプロパティ名。</span><span class="sxs-lookup"><span data-stu-id="abebb-137">The setting class name and property name.</span></span>|
|<span data-ttu-id="abebb-138">settingName</span><span class="sxs-lookup"><span data-stu-id="abebb-138">settingName</span></span>|<span data-ttu-id="abebb-139">String</span><span class="sxs-lookup"><span data-stu-id="abebb-139">String</span></span>|<span data-ttu-id="abebb-140">設定の名前。</span><span class="sxs-lookup"><span data-stu-id="abebb-140">Name of the setting.</span></span>|
|<span data-ttu-id="abebb-141">platformType</span><span class="sxs-lookup"><span data-stu-id="abebb-141">platformType</span></span>|[<span data-ttu-id="abebb-142">policyPlatformType</span><span class="sxs-lookup"><span data-stu-id="abebb-142">policyPlatformType</span></span>](../resources/intune-deviceconfig-policyplatformtype.md)|<span data-ttu-id="abebb-143">プラットフォームを設定します。</span><span class="sxs-lookup"><span data-stu-id="abebb-143">Setting platform.</span></span> <span data-ttu-id="abebb-144">可能な値は、`android`、`androidForWork`、`iOS`、`macOS`、`windowsPhone81`、`windows81AndLater`、`windows10AndLater`、`androidWorkProfile`、`all` です。</span><span class="sxs-lookup"><span data-stu-id="abebb-144">Possible values are: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `all`.</span></span>|
|<span data-ttu-id="abebb-145">unknownDeviceCount</span><span class="sxs-lookup"><span data-stu-id="abebb-145">unknownDeviceCount</span></span>|<span data-ttu-id="abebb-146">Int32</span><span class="sxs-lookup"><span data-stu-id="abebb-146">Int32</span></span>|<span data-ttu-id="abebb-147">不明なデバイスの数</span><span class="sxs-lookup"><span data-stu-id="abebb-147">Number of unknown devices</span></span>|
|<span data-ttu-id="abebb-148">notApplicableDeviceCount</span><span class="sxs-lookup"><span data-stu-id="abebb-148">notApplicableDeviceCount</span></span>|<span data-ttu-id="abebb-149">Int32</span><span class="sxs-lookup"><span data-stu-id="abebb-149">Int32</span></span>|<span data-ttu-id="abebb-150">該当しないデバイスの数</span><span class="sxs-lookup"><span data-stu-id="abebb-150">Number of not applicable devices</span></span>|
|<span data-ttu-id="abebb-151">compliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="abebb-151">compliantDeviceCount</span></span>|<span data-ttu-id="abebb-152">Int32</span><span class="sxs-lookup"><span data-stu-id="abebb-152">Int32</span></span>|<span data-ttu-id="abebb-153">準拠デバイスの数</span><span class="sxs-lookup"><span data-stu-id="abebb-153">Number of compliant devices</span></span>|
|<span data-ttu-id="abebb-154">remediatedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="abebb-154">remediatedDeviceCount</span></span>|<span data-ttu-id="abebb-155">Int32</span><span class="sxs-lookup"><span data-stu-id="abebb-155">Int32</span></span>|<span data-ttu-id="abebb-156">修復済みデバイスの数</span><span class="sxs-lookup"><span data-stu-id="abebb-156">Number of remediated devices</span></span>|
|<span data-ttu-id="abebb-157">nonCompliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="abebb-157">nonCompliantDeviceCount</span></span>|<span data-ttu-id="abebb-158">Int32</span><span class="sxs-lookup"><span data-stu-id="abebb-158">Int32</span></span>|<span data-ttu-id="abebb-159">準拠していないデバイスの数</span><span class="sxs-lookup"><span data-stu-id="abebb-159">Number of NonCompliant devices</span></span>|
|<span data-ttu-id="abebb-160">errorDeviceCount</span><span class="sxs-lookup"><span data-stu-id="abebb-160">errorDeviceCount</span></span>|<span data-ttu-id="abebb-161">Int32</span><span class="sxs-lookup"><span data-stu-id="abebb-161">Int32</span></span>|<span data-ttu-id="abebb-162">エラー デバイスの数</span><span class="sxs-lookup"><span data-stu-id="abebb-162">Number of error devices</span></span>|
|<span data-ttu-id="abebb-163">conflictDeviceCount</span><span class="sxs-lookup"><span data-stu-id="abebb-163">conflictDeviceCount</span></span>|<span data-ttu-id="abebb-164">Int32</span><span class="sxs-lookup"><span data-stu-id="abebb-164">Int32</span></span>|<span data-ttu-id="abebb-165">競合デバイスの数</span><span class="sxs-lookup"><span data-stu-id="abebb-165">Number of conflict devices</span></span>|



## <a name="response"></a><span data-ttu-id="abebb-166">応答</span><span class="sxs-lookup"><span data-stu-id="abebb-166">Response</span></span>
<span data-ttu-id="abebb-167">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で更新された [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="abebb-167">If successful, this method returns a `200 OK` response code and an updated [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="abebb-168">例</span><span class="sxs-lookup"><span data-stu-id="abebb-168">Example</span></span>

### <a name="request"></a><span data-ttu-id="abebb-169">要求</span><span class="sxs-lookup"><span data-stu-id="abebb-169">Request</span></span>
<span data-ttu-id="abebb-170">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="abebb-170">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="abebb-171">応答</span><span class="sxs-lookup"><span data-stu-id="abebb-171">Response</span></span>
<span data-ttu-id="abebb-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="abebb-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





