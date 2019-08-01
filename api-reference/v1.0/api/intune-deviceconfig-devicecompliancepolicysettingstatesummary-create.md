---
title: deviceCompliancePolicySettingStateSummary の作成
description: 新しい deviceCompliancePolicySettingStateSummary オブジェクトを作成します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: ccd9ce498af34ec2f0f3640572a336cb5f82c874
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36017785"
---
# <a name="create-devicecompliancepolicysettingstatesummary"></a><span data-ttu-id="817e5-103">deviceCompliancePolicySettingStateSummary の作成</span><span class="sxs-lookup"><span data-stu-id="817e5-103">Create deviceCompliancePolicySettingStateSummary</span></span>

> <span data-ttu-id="817e5-104">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="817e5-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="817e5-105">新しい [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="817e5-105">Create a new [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="817e5-106">前提条件</span><span class="sxs-lookup"><span data-stu-id="817e5-106">Prerequisites</span></span>
<span data-ttu-id="817e5-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="817e5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="817e5-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="817e5-109">Permission type</span></span>|<span data-ttu-id="817e5-110">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="817e5-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="817e5-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="817e5-111">Delegated (work or school account)</span></span>|<span data-ttu-id="817e5-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="817e5-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="817e5-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="817e5-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="817e5-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="817e5-114">Not supported.</span></span>|
|<span data-ttu-id="817e5-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="817e5-115">Application</span></span>|<span data-ttu-id="817e5-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="817e5-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="817e5-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="817e5-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicySettingStateSummaries
```

## <a name="request-headers"></a><span data-ttu-id="817e5-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="817e5-118">Request headers</span></span>
|<span data-ttu-id="817e5-119">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="817e5-119">Header</span></span>|<span data-ttu-id="817e5-120">値</span><span class="sxs-lookup"><span data-stu-id="817e5-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="817e5-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="817e5-121">Authorization</span></span>|<span data-ttu-id="817e5-122">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="817e5-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="817e5-123">承諾</span><span class="sxs-lookup"><span data-stu-id="817e5-123">Accept</span></span>|<span data-ttu-id="817e5-124">application/json</span><span class="sxs-lookup"><span data-stu-id="817e5-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="817e5-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="817e5-125">Request body</span></span>
<span data-ttu-id="817e5-126">要求本文で、deviceCompliancePolicySettingStateSummary オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="817e5-126">In the request body, supply a JSON representation for the deviceCompliancePolicySettingStateSummary object.</span></span>

<span data-ttu-id="817e5-127">次の表に、deviceCompliancePolicySettingStateSummary の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="817e5-127">The following table shows the properties that are required when you create the deviceCompliancePolicySettingStateSummary.</span></span>

|<span data-ttu-id="817e5-128">プロパティ</span><span class="sxs-lookup"><span data-stu-id="817e5-128">Property</span></span>|<span data-ttu-id="817e5-129">型</span><span class="sxs-lookup"><span data-stu-id="817e5-129">Type</span></span>|<span data-ttu-id="817e5-130">説明</span><span class="sxs-lookup"><span data-stu-id="817e5-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="817e5-131">id</span><span class="sxs-lookup"><span data-stu-id="817e5-131">id</span></span>|<span data-ttu-id="817e5-132">String</span><span class="sxs-lookup"><span data-stu-id="817e5-132">String</span></span>|<span data-ttu-id="817e5-133">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="817e5-133">Key of the entity.</span></span>|
|<span data-ttu-id="817e5-134">setting</span><span class="sxs-lookup"><span data-stu-id="817e5-134">setting</span></span>|<span data-ttu-id="817e5-135">String</span><span class="sxs-lookup"><span data-stu-id="817e5-135">String</span></span>|<span data-ttu-id="817e5-136">設定のクラス名とプロパティ名。</span><span class="sxs-lookup"><span data-stu-id="817e5-136">The setting class name and property name.</span></span>|
|<span data-ttu-id="817e5-137">settingName</span><span class="sxs-lookup"><span data-stu-id="817e5-137">settingName</span></span>|<span data-ttu-id="817e5-138">String</span><span class="sxs-lookup"><span data-stu-id="817e5-138">String</span></span>|<span data-ttu-id="817e5-139">設定の名前。</span><span class="sxs-lookup"><span data-stu-id="817e5-139">Name of the setting.</span></span>|
|<span data-ttu-id="817e5-140">platformType</span><span class="sxs-lookup"><span data-stu-id="817e5-140">platformType</span></span>|[<span data-ttu-id="817e5-141">policyPlatformType</span><span class="sxs-lookup"><span data-stu-id="817e5-141">policyPlatformType</span></span>](../resources/intune-deviceconfig-policyplatformtype.md)|<span data-ttu-id="817e5-142">プラットフォームを設定します。</span><span class="sxs-lookup"><span data-stu-id="817e5-142">Setting platform.</span></span> <span data-ttu-id="817e5-143">可能な値は、`android`、`iOS`、`macOS`、`windowsPhone81`、`windows81AndLater`、`windows10AndLater`、`androidWorkProfile`、`all` です。</span><span class="sxs-lookup"><span data-stu-id="817e5-143">Possible values are: `android`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `all`.</span></span>|
|<span data-ttu-id="817e5-144">unknownDeviceCount</span><span class="sxs-lookup"><span data-stu-id="817e5-144">unknownDeviceCount</span></span>|<span data-ttu-id="817e5-145">Int32</span><span class="sxs-lookup"><span data-stu-id="817e5-145">Int32</span></span>|<span data-ttu-id="817e5-146">不明なデバイスの数</span><span class="sxs-lookup"><span data-stu-id="817e5-146">Number of unknown devices</span></span>|
|<span data-ttu-id="817e5-147">notApplicableDeviceCount</span><span class="sxs-lookup"><span data-stu-id="817e5-147">notApplicableDeviceCount</span></span>|<span data-ttu-id="817e5-148">Int32</span><span class="sxs-lookup"><span data-stu-id="817e5-148">Int32</span></span>|<span data-ttu-id="817e5-149">該当しないデバイスの数</span><span class="sxs-lookup"><span data-stu-id="817e5-149">Number of not applicable devices</span></span>|
|<span data-ttu-id="817e5-150">compliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="817e5-150">compliantDeviceCount</span></span>|<span data-ttu-id="817e5-151">Int32</span><span class="sxs-lookup"><span data-stu-id="817e5-151">Int32</span></span>|<span data-ttu-id="817e5-152">準拠デバイスの数</span><span class="sxs-lookup"><span data-stu-id="817e5-152">Number of compliant devices</span></span>|
|<span data-ttu-id="817e5-153">remediatedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="817e5-153">remediatedDeviceCount</span></span>|<span data-ttu-id="817e5-154">Int32</span><span class="sxs-lookup"><span data-stu-id="817e5-154">Int32</span></span>|<span data-ttu-id="817e5-155">修復済みデバイスの数</span><span class="sxs-lookup"><span data-stu-id="817e5-155">Number of remediated devices</span></span>|
|<span data-ttu-id="817e5-156">nonCompliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="817e5-156">nonCompliantDeviceCount</span></span>|<span data-ttu-id="817e5-157">Int32</span><span class="sxs-lookup"><span data-stu-id="817e5-157">Int32</span></span>|<span data-ttu-id="817e5-158">準拠していないデバイスの数</span><span class="sxs-lookup"><span data-stu-id="817e5-158">Number of NonCompliant devices</span></span>|
|<span data-ttu-id="817e5-159">errorDeviceCount</span><span class="sxs-lookup"><span data-stu-id="817e5-159">errorDeviceCount</span></span>|<span data-ttu-id="817e5-160">Int32</span><span class="sxs-lookup"><span data-stu-id="817e5-160">Int32</span></span>|<span data-ttu-id="817e5-161">エラー デバイスの数</span><span class="sxs-lookup"><span data-stu-id="817e5-161">Number of error devices</span></span>|
|<span data-ttu-id="817e5-162">conflictDeviceCount</span><span class="sxs-lookup"><span data-stu-id="817e5-162">conflictDeviceCount</span></span>|<span data-ttu-id="817e5-163">Int32</span><span class="sxs-lookup"><span data-stu-id="817e5-163">Int32</span></span>|<span data-ttu-id="817e5-164">競合デバイスの数</span><span class="sxs-lookup"><span data-stu-id="817e5-164">Number of conflict devices</span></span>|



## <a name="response"></a><span data-ttu-id="817e5-165">応答</span><span class="sxs-lookup"><span data-stu-id="817e5-165">Response</span></span>
<span data-ttu-id="817e5-166">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="817e5-166">If successful, this method returns a `201 Created` response code and a [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="817e5-167">例</span><span class="sxs-lookup"><span data-stu-id="817e5-167">Example</span></span>

### <a name="request"></a><span data-ttu-id="817e5-168">要求</span><span class="sxs-lookup"><span data-stu-id="817e5-168">Request</span></span>
<span data-ttu-id="817e5-169">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="817e5-169">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/deviceCompliancePolicySettingStateSummaries
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

### <a name="response"></a><span data-ttu-id="817e5-170">応答</span><span class="sxs-lookup"><span data-stu-id="817e5-170">Response</span></span>
<span data-ttu-id="817e5-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="817e5-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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



