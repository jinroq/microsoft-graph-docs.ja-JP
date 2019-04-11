---
title: deviceCompliancePolicySettingStateSummary の更新
description: deviceCompliancePolicySettingStateSummary オブジェクトのプロパティを更新します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 3c37cf5b3f63e65b9efdffb76a7203202a8d2fdf
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/11/2019
ms.locfileid: "31799833"
---
# <a name="update-devicecompliancepolicysettingstatesummary"></a><span data-ttu-id="12692-103">deviceCompliancePolicySettingStateSummary の更新</span><span class="sxs-lookup"><span data-stu-id="12692-103">Update deviceCompliancePolicySettingStateSummary</span></span>

> <span data-ttu-id="12692-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="12692-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="12692-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="12692-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="12692-106">[deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="12692-106">Update the properties of a [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="12692-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="12692-107">Prerequisites</span></span>
<span data-ttu-id="12692-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="12692-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="12692-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="12692-110">Permission type</span></span>|<span data-ttu-id="12692-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="12692-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="12692-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="12692-112">Delegated (work or school account)</span></span>|<span data-ttu-id="12692-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="12692-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="12692-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="12692-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="12692-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="12692-115">Not supported.</span></span>|
|<span data-ttu-id="12692-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="12692-116">Application</span></span>|<span data-ttu-id="12692-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="12692-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="12692-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="12692-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicySettingStateSummaries/{deviceCompliancePolicySettingStateSummaryId}
```

## <a name="request-headers"></a><span data-ttu-id="12692-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="12692-119">Request headers</span></span>
|<span data-ttu-id="12692-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="12692-120">Header</span></span>|<span data-ttu-id="12692-121">値</span><span class="sxs-lookup"><span data-stu-id="12692-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="12692-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="12692-122">Authorization</span></span>|<span data-ttu-id="12692-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="12692-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="12692-124">承諾</span><span class="sxs-lookup"><span data-stu-id="12692-124">Accept</span></span>|<span data-ttu-id="12692-125">application/json</span><span class="sxs-lookup"><span data-stu-id="12692-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="12692-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="12692-126">Request body</span></span>
<span data-ttu-id="12692-127">要求本文で、[deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="12692-127">In the request body, supply a JSON representation for the [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md) object.</span></span>

<span data-ttu-id="12692-128">次の表に、[deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md) の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="12692-128">The following table shows the properties that are required when you create the [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md).</span></span>

|<span data-ttu-id="12692-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="12692-129">Property</span></span>|<span data-ttu-id="12692-130">型</span><span class="sxs-lookup"><span data-stu-id="12692-130">Type</span></span>|<span data-ttu-id="12692-131">説明</span><span class="sxs-lookup"><span data-stu-id="12692-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="12692-132">id</span><span class="sxs-lookup"><span data-stu-id="12692-132">id</span></span>|<span data-ttu-id="12692-133">String</span><span class="sxs-lookup"><span data-stu-id="12692-133">String</span></span>|<span data-ttu-id="12692-134">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="12692-134">Key of the entity.</span></span>|
|<span data-ttu-id="12692-135">setting</span><span class="sxs-lookup"><span data-stu-id="12692-135">setting</span></span>|<span data-ttu-id="12692-136">文字列</span><span class="sxs-lookup"><span data-stu-id="12692-136">String</span></span>|<span data-ttu-id="12692-137">設定のクラス名とプロパティ名。</span><span class="sxs-lookup"><span data-stu-id="12692-137">The setting class name and property name.</span></span>|
|<span data-ttu-id="12692-138">settingName</span><span class="sxs-lookup"><span data-stu-id="12692-138">settingName</span></span>|<span data-ttu-id="12692-139">String</span><span class="sxs-lookup"><span data-stu-id="12692-139">String</span></span>|<span data-ttu-id="12692-140">設定の名前。</span><span class="sxs-lookup"><span data-stu-id="12692-140">Name of the setting.</span></span>|
|<span data-ttu-id="12692-141">platformType</span><span class="sxs-lookup"><span data-stu-id="12692-141">platformType</span></span>|[<span data-ttu-id="12692-142">policyPlatformType</span><span class="sxs-lookup"><span data-stu-id="12692-142">policyPlatformType</span></span>](../resources/intune-deviceconfig-policyplatformtype.md)|<span data-ttu-id="12692-143">プラットフォームを設定します。</span><span class="sxs-lookup"><span data-stu-id="12692-143">Setting platform.</span></span> <span data-ttu-id="12692-144">可能な値は、`android`、`androidForWork`、`iOS`、`macOS`、`windowsPhone81`、`windows81AndLater`、`windows10AndLater`、`androidWorkProfile`、`all` です。</span><span class="sxs-lookup"><span data-stu-id="12692-144">Possible values are: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `all`.</span></span>|
|<span data-ttu-id="12692-145">unknownDeviceCount</span><span class="sxs-lookup"><span data-stu-id="12692-145">unknownDeviceCount</span></span>|<span data-ttu-id="12692-146">Int32</span><span class="sxs-lookup"><span data-stu-id="12692-146">Int32</span></span>|<span data-ttu-id="12692-147">不明なデバイスの数</span><span class="sxs-lookup"><span data-stu-id="12692-147">Number of unknown devices</span></span>|
|<span data-ttu-id="12692-148">notApplicableDeviceCount</span><span class="sxs-lookup"><span data-stu-id="12692-148">notApplicableDeviceCount</span></span>|<span data-ttu-id="12692-149">Int32</span><span class="sxs-lookup"><span data-stu-id="12692-149">Int32</span></span>|<span data-ttu-id="12692-150">該当しないデバイスの数</span><span class="sxs-lookup"><span data-stu-id="12692-150">Number of not applicable devices</span></span>|
|<span data-ttu-id="12692-151">compliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="12692-151">compliantDeviceCount</span></span>|<span data-ttu-id="12692-152">Int32</span><span class="sxs-lookup"><span data-stu-id="12692-152">Int32</span></span>|<span data-ttu-id="12692-153">準拠デバイスの数</span><span class="sxs-lookup"><span data-stu-id="12692-153">Number of compliant devices</span></span>|
|<span data-ttu-id="12692-154">remediatedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="12692-154">remediatedDeviceCount</span></span>|<span data-ttu-id="12692-155">Int32</span><span class="sxs-lookup"><span data-stu-id="12692-155">Int32</span></span>|<span data-ttu-id="12692-156">修復済みデバイスの数</span><span class="sxs-lookup"><span data-stu-id="12692-156">Number of remediated devices</span></span>|
|<span data-ttu-id="12692-157">nonCompliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="12692-157">nonCompliantDeviceCount</span></span>|<span data-ttu-id="12692-158">Int32</span><span class="sxs-lookup"><span data-stu-id="12692-158">Int32</span></span>|<span data-ttu-id="12692-159">準拠していないデバイスの数</span><span class="sxs-lookup"><span data-stu-id="12692-159">Number of NonCompliant devices</span></span>|
|<span data-ttu-id="12692-160">errorDeviceCount</span><span class="sxs-lookup"><span data-stu-id="12692-160">errorDeviceCount</span></span>|<span data-ttu-id="12692-161">Int32</span><span class="sxs-lookup"><span data-stu-id="12692-161">Int32</span></span>|<span data-ttu-id="12692-162">エラー デバイスの数</span><span class="sxs-lookup"><span data-stu-id="12692-162">Number of error devices</span></span>|
|<span data-ttu-id="12692-163">conflictDeviceCount</span><span class="sxs-lookup"><span data-stu-id="12692-163">conflictDeviceCount</span></span>|<span data-ttu-id="12692-164">Int32</span><span class="sxs-lookup"><span data-stu-id="12692-164">Int32</span></span>|<span data-ttu-id="12692-165">競合デバイスの数</span><span class="sxs-lookup"><span data-stu-id="12692-165">Number of conflict devices</span></span>|



## <a name="response"></a><span data-ttu-id="12692-166">応答</span><span class="sxs-lookup"><span data-stu-id="12692-166">Response</span></span>
<span data-ttu-id="12692-167">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で更新された [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="12692-167">If successful, this method returns a `200 OK` response code and an updated [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="12692-168">例</span><span class="sxs-lookup"><span data-stu-id="12692-168">Example</span></span>

### <a name="request"></a><span data-ttu-id="12692-169">要求</span><span class="sxs-lookup"><span data-stu-id="12692-169">Request</span></span>
<span data-ttu-id="12692-170">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="12692-170">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="12692-171">応答</span><span class="sxs-lookup"><span data-stu-id="12692-171">Response</span></span>
<span data-ttu-id="12692-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="12692-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





