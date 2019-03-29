---
title: deviceCompliancePolicyDeviceStateSummary の更新
description: deviceCompliancePolicyDeviceStateSummary オブジェクトのプロパティを更新します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: bd58291b1f9dbec8c18449202aa10f461c645b6f
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/29/2019
ms.locfileid: "30959517"
---
# <a name="update-devicecompliancepolicydevicestatesummary"></a><span data-ttu-id="80c3e-103">deviceCompliancePolicyDeviceStateSummary の更新</span><span class="sxs-lookup"><span data-stu-id="80c3e-103">Update deviceCompliancePolicyDeviceStateSummary</span></span>

> <span data-ttu-id="80c3e-104">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="80c3e-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="80c3e-105">[deviceCompliancePolicyDeviceStateSummary](../resources/intune-deviceconfig-devicecompliancepolicydevicestatesummary.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="80c3e-105">Update the properties of a [deviceCompliancePolicyDeviceStateSummary](../resources/intune-deviceconfig-devicecompliancepolicydevicestatesummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="80c3e-106">前提条件</span><span class="sxs-lookup"><span data-stu-id="80c3e-106">Prerequisites</span></span>
<span data-ttu-id="80c3e-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="80c3e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="80c3e-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="80c3e-109">Permission type</span></span>|<span data-ttu-id="80c3e-110">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="80c3e-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="80c3e-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="80c3e-111">Delegated (work or school account)</span></span>|<span data-ttu-id="80c3e-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="80c3e-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="80c3e-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="80c3e-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="80c3e-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="80c3e-114">Not supported.</span></span>|
|<span data-ttu-id="80c3e-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="80c3e-115">Application</span></span>|<span data-ttu-id="80c3e-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="80c3e-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="80c3e-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="80c3e-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicyDeviceStateSummary
```

## <a name="request-headers"></a><span data-ttu-id="80c3e-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="80c3e-118">Request headers</span></span>
|<span data-ttu-id="80c3e-119">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="80c3e-119">Header</span></span>|<span data-ttu-id="80c3e-120">値</span><span class="sxs-lookup"><span data-stu-id="80c3e-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="80c3e-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="80c3e-121">Authorization</span></span>|<span data-ttu-id="80c3e-122">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="80c3e-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="80c3e-123">承諾</span><span class="sxs-lookup"><span data-stu-id="80c3e-123">Accept</span></span>|<span data-ttu-id="80c3e-124">application/json</span><span class="sxs-lookup"><span data-stu-id="80c3e-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="80c3e-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="80c3e-125">Request body</span></span>
<span data-ttu-id="80c3e-126">要求本文で、[deviceCompliancePolicyDeviceStateSummary](../resources/intune-deviceconfig-devicecompliancepolicydevicestatesummary.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="80c3e-126">In the request body, supply a JSON representation for the [deviceCompliancePolicyDeviceStateSummary](../resources/intune-deviceconfig-devicecompliancepolicydevicestatesummary.md) object.</span></span>

<span data-ttu-id="80c3e-127">次の表に、[deviceCompliancePolicyDeviceStateSummary](../resources/intune-deviceconfig-devicecompliancepolicydevicestatesummary.md) の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="80c3e-127">The following table shows the properties that are required when you create the [deviceCompliancePolicyDeviceStateSummary](../resources/intune-deviceconfig-devicecompliancepolicydevicestatesummary.md).</span></span>

|<span data-ttu-id="80c3e-128">プロパティ</span><span class="sxs-lookup"><span data-stu-id="80c3e-128">Property</span></span>|<span data-ttu-id="80c3e-129">型</span><span class="sxs-lookup"><span data-stu-id="80c3e-129">Type</span></span>|<span data-ttu-id="80c3e-130">説明</span><span class="sxs-lookup"><span data-stu-id="80c3e-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="80c3e-131">inGracePeriodCount</span><span class="sxs-lookup"><span data-stu-id="80c3e-131">inGracePeriodCount</span></span>|<span data-ttu-id="80c3e-132">Int32</span><span class="sxs-lookup"><span data-stu-id="80c3e-132">Int32</span></span>|<span data-ttu-id="80c3e-133">解約猶予期間内のデバイスの数</span><span class="sxs-lookup"><span data-stu-id="80c3e-133">Number of devices that are in grace period</span></span>|
|<span data-ttu-id="80c3e-134">configManagerCount</span><span class="sxs-lookup"><span data-stu-id="80c3e-134">configManagerCount</span></span>|<span data-ttu-id="80c3e-135">Int32</span><span class="sxs-lookup"><span data-stu-id="80c3e-135">Int32</span></span>|<span data-ttu-id="80c3e-136">System Center Configuration Manager によってコンプライアンスが管理されているデバイスの数</span><span class="sxs-lookup"><span data-stu-id="80c3e-136">Number of devices that have compliance managed by System Center Configuration Manager</span></span>|
|<span data-ttu-id="80c3e-137">id</span><span class="sxs-lookup"><span data-stu-id="80c3e-137">id</span></span>|<span data-ttu-id="80c3e-138">String</span><span class="sxs-lookup"><span data-stu-id="80c3e-138">String</span></span>|<span data-ttu-id="80c3e-139">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="80c3e-139">Key of the entity.</span></span>|
|<span data-ttu-id="80c3e-140">unknownDeviceCount</span><span class="sxs-lookup"><span data-stu-id="80c3e-140">unknownDeviceCount</span></span>|<span data-ttu-id="80c3e-141">Int32</span><span class="sxs-lookup"><span data-stu-id="80c3e-141">Int32</span></span>|<span data-ttu-id="80c3e-142">不明なデバイスの数</span><span class="sxs-lookup"><span data-stu-id="80c3e-142">Number of unknown devices</span></span>|
|<span data-ttu-id="80c3e-143">notApplicableDeviceCount</span><span class="sxs-lookup"><span data-stu-id="80c3e-143">notApplicableDeviceCount</span></span>|<span data-ttu-id="80c3e-144">Int32</span><span class="sxs-lookup"><span data-stu-id="80c3e-144">Int32</span></span>|<span data-ttu-id="80c3e-145">該当しないデバイスの数</span><span class="sxs-lookup"><span data-stu-id="80c3e-145">Number of not applicable devices</span></span>|
|<span data-ttu-id="80c3e-146">compliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="80c3e-146">compliantDeviceCount</span></span>|<span data-ttu-id="80c3e-147">Int32</span><span class="sxs-lookup"><span data-stu-id="80c3e-147">Int32</span></span>|<span data-ttu-id="80c3e-148">準拠デバイスの数</span><span class="sxs-lookup"><span data-stu-id="80c3e-148">Number of compliant devices</span></span>|
|<span data-ttu-id="80c3e-149">remediatedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="80c3e-149">remediatedDeviceCount</span></span>|<span data-ttu-id="80c3e-150">Int32</span><span class="sxs-lookup"><span data-stu-id="80c3e-150">Int32</span></span>|<span data-ttu-id="80c3e-151">修復済みデバイスの数</span><span class="sxs-lookup"><span data-stu-id="80c3e-151">Number of remediated devices</span></span>|
|<span data-ttu-id="80c3e-152">nonCompliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="80c3e-152">nonCompliantDeviceCount</span></span>|<span data-ttu-id="80c3e-153">Int32</span><span class="sxs-lookup"><span data-stu-id="80c3e-153">Int32</span></span>|<span data-ttu-id="80c3e-154">準拠していないデバイスの数</span><span class="sxs-lookup"><span data-stu-id="80c3e-154">Number of NonCompliant devices</span></span>|
|<span data-ttu-id="80c3e-155">errorDeviceCount</span><span class="sxs-lookup"><span data-stu-id="80c3e-155">errorDeviceCount</span></span>|<span data-ttu-id="80c3e-156">Int32</span><span class="sxs-lookup"><span data-stu-id="80c3e-156">Int32</span></span>|<span data-ttu-id="80c3e-157">エラー デバイスの数</span><span class="sxs-lookup"><span data-stu-id="80c3e-157">Number of error devices</span></span>|
|<span data-ttu-id="80c3e-158">conflictDeviceCount</span><span class="sxs-lookup"><span data-stu-id="80c3e-158">conflictDeviceCount</span></span>|<span data-ttu-id="80c3e-159">Int32</span><span class="sxs-lookup"><span data-stu-id="80c3e-159">Int32</span></span>|<span data-ttu-id="80c3e-160">競合デバイスの数</span><span class="sxs-lookup"><span data-stu-id="80c3e-160">Number of conflict devices</span></span>|



## <a name="response"></a><span data-ttu-id="80c3e-161">応答</span><span class="sxs-lookup"><span data-stu-id="80c3e-161">Response</span></span>
<span data-ttu-id="80c3e-162">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で更新された [deviceCompliancePolicyDeviceStateSummary](../resources/intune-deviceconfig-devicecompliancepolicydevicestatesummary.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="80c3e-162">If successful, this method returns a `200 OK` response code and an updated [deviceCompliancePolicyDeviceStateSummary](../resources/intune-deviceconfig-devicecompliancepolicydevicestatesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="80c3e-163">例</span><span class="sxs-lookup"><span data-stu-id="80c3e-163">Example</span></span>

### <a name="request"></a><span data-ttu-id="80c3e-164">要求</span><span class="sxs-lookup"><span data-stu-id="80c3e-164">Request</span></span>
<span data-ttu-id="80c3e-165">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="80c3e-165">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/deviceCompliancePolicyDeviceStateSummary
Content-type: application/json
Content-length: 349

{
  "@odata.type": "#microsoft.graph.deviceCompliancePolicyDeviceStateSummary",
  "inGracePeriodCount": 2,
  "configManagerCount": 2,
  "unknownDeviceCount": 2,
  "notApplicableDeviceCount": 8,
  "compliantDeviceCount": 4,
  "remediatedDeviceCount": 5,
  "nonCompliantDeviceCount": 7,
  "errorDeviceCount": 0,
  "conflictDeviceCount": 3
}
```

### <a name="response"></a><span data-ttu-id="80c3e-166">応答</span><span class="sxs-lookup"><span data-stu-id="80c3e-166">Response</span></span>
<span data-ttu-id="80c3e-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="80c3e-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 398

{
  "@odata.type": "#microsoft.graph.deviceCompliancePolicyDeviceStateSummary",
  "inGracePeriodCount": 2,
  "configManagerCount": 2,
  "id": "8c4de8a7-e8a7-8c4d-a7e8-4d8ca7e84d8c",
  "unknownDeviceCount": 2,
  "notApplicableDeviceCount": 8,
  "compliantDeviceCount": 4,
  "remediatedDeviceCount": 5,
  "nonCompliantDeviceCount": 7,
  "errorDeviceCount": 0,
  "conflictDeviceCount": 3
}
```



