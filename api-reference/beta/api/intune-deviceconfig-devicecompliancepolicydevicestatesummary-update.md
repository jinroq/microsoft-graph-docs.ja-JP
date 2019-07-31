---
title: deviceCompliancePolicyDeviceStateSummary の更新
description: deviceCompliancePolicyDeviceStateSummary オブジェクトのプロパティを更新します。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 913eef32303ac03f167b4cde23b078dd81a5dfe7
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35949749"
---
# <a name="update-devicecompliancepolicydevicestatesummary"></a><span data-ttu-id="5ae53-103">deviceCompliancePolicyDeviceStateSummary の更新</span><span class="sxs-lookup"><span data-stu-id="5ae53-103">Update deviceCompliancePolicyDeviceStateSummary</span></span>

> <span data-ttu-id="5ae53-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="5ae53-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5ae53-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="5ae53-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5ae53-106">[deviceCompliancePolicyDeviceStateSummary](../resources/intune-deviceconfig-devicecompliancepolicydevicestatesummary.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="5ae53-106">Update the properties of a [deviceCompliancePolicyDeviceStateSummary](../resources/intune-deviceconfig-devicecompliancepolicydevicestatesummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="5ae53-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="5ae53-107">Prerequisites</span></span>
<span data-ttu-id="5ae53-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="5ae53-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5ae53-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="5ae53-110">Permission type</span></span>|<span data-ttu-id="5ae53-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="5ae53-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5ae53-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="5ae53-112">Delegated (work or school account)</span></span>|<span data-ttu-id="5ae53-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5ae53-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="5ae53-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="5ae53-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5ae53-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="5ae53-115">Not supported.</span></span>|
|<span data-ttu-id="5ae53-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="5ae53-116">Application</span></span>|<span data-ttu-id="5ae53-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="5ae53-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="5ae53-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="5ae53-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicyDeviceStateSummary
```

## <a name="request-headers"></a><span data-ttu-id="5ae53-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="5ae53-119">Request headers</span></span>
|<span data-ttu-id="5ae53-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="5ae53-120">Header</span></span>|<span data-ttu-id="5ae53-121">値</span><span class="sxs-lookup"><span data-stu-id="5ae53-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5ae53-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="5ae53-122">Authorization</span></span>|<span data-ttu-id="5ae53-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="5ae53-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5ae53-124">承諾</span><span class="sxs-lookup"><span data-stu-id="5ae53-124">Accept</span></span>|<span data-ttu-id="5ae53-125">application/json</span><span class="sxs-lookup"><span data-stu-id="5ae53-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5ae53-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="5ae53-126">Request body</span></span>
<span data-ttu-id="5ae53-127">要求本文で、[deviceCompliancePolicyDeviceStateSummary](../resources/intune-deviceconfig-devicecompliancepolicydevicestatesummary.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="5ae53-127">In the request body, supply a JSON representation for the [deviceCompliancePolicyDeviceStateSummary](../resources/intune-deviceconfig-devicecompliancepolicydevicestatesummary.md) object.</span></span>

<span data-ttu-id="5ae53-128">次の表に、[deviceCompliancePolicyDeviceStateSummary](../resources/intune-deviceconfig-devicecompliancepolicydevicestatesummary.md) の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="5ae53-128">The following table shows the properties that are required when you create the [deviceCompliancePolicyDeviceStateSummary](../resources/intune-deviceconfig-devicecompliancepolicydevicestatesummary.md).</span></span>

|<span data-ttu-id="5ae53-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="5ae53-129">Property</span></span>|<span data-ttu-id="5ae53-130">型</span><span class="sxs-lookup"><span data-stu-id="5ae53-130">Type</span></span>|<span data-ttu-id="5ae53-131">説明</span><span class="sxs-lookup"><span data-stu-id="5ae53-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5ae53-132">inGracePeriodCount</span><span class="sxs-lookup"><span data-stu-id="5ae53-132">inGracePeriodCount</span></span>|<span data-ttu-id="5ae53-133">Int32</span><span class="sxs-lookup"><span data-stu-id="5ae53-133">Int32</span></span>|<span data-ttu-id="5ae53-134">解約猶予期間内のデバイスの数</span><span class="sxs-lookup"><span data-stu-id="5ae53-134">Number of devices that are in grace period</span></span>|
|<span data-ttu-id="5ae53-135">configManagerCount</span><span class="sxs-lookup"><span data-stu-id="5ae53-135">configManagerCount</span></span>|<span data-ttu-id="5ae53-136">Int32</span><span class="sxs-lookup"><span data-stu-id="5ae53-136">Int32</span></span>|<span data-ttu-id="5ae53-137">System Center Configuration Manager によってコンプライアンスが管理されているデバイスの数</span><span class="sxs-lookup"><span data-stu-id="5ae53-137">Number of devices that have compliance managed by System Center Configuration Manager</span></span>|
|<span data-ttu-id="5ae53-138">id</span><span class="sxs-lookup"><span data-stu-id="5ae53-138">id</span></span>|<span data-ttu-id="5ae53-139">String</span><span class="sxs-lookup"><span data-stu-id="5ae53-139">String</span></span>|<span data-ttu-id="5ae53-140">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="5ae53-140">Key of the entity.</span></span>|
|<span data-ttu-id="5ae53-141">unknownDeviceCount</span><span class="sxs-lookup"><span data-stu-id="5ae53-141">unknownDeviceCount</span></span>|<span data-ttu-id="5ae53-142">Int32</span><span class="sxs-lookup"><span data-stu-id="5ae53-142">Int32</span></span>|<span data-ttu-id="5ae53-143">不明なデバイスの数</span><span class="sxs-lookup"><span data-stu-id="5ae53-143">Number of unknown devices</span></span>|
|<span data-ttu-id="5ae53-144">notApplicableDeviceCount</span><span class="sxs-lookup"><span data-stu-id="5ae53-144">notApplicableDeviceCount</span></span>|<span data-ttu-id="5ae53-145">Int32</span><span class="sxs-lookup"><span data-stu-id="5ae53-145">Int32</span></span>|<span data-ttu-id="5ae53-146">該当しないデバイスの数</span><span class="sxs-lookup"><span data-stu-id="5ae53-146">Number of not applicable devices</span></span>|
|<span data-ttu-id="5ae53-147">compliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="5ae53-147">compliantDeviceCount</span></span>|<span data-ttu-id="5ae53-148">Int32</span><span class="sxs-lookup"><span data-stu-id="5ae53-148">Int32</span></span>|<span data-ttu-id="5ae53-149">準拠デバイスの数</span><span class="sxs-lookup"><span data-stu-id="5ae53-149">Number of compliant devices</span></span>|
|<span data-ttu-id="5ae53-150">remediatedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="5ae53-150">remediatedDeviceCount</span></span>|<span data-ttu-id="5ae53-151">Int32</span><span class="sxs-lookup"><span data-stu-id="5ae53-151">Int32</span></span>|<span data-ttu-id="5ae53-152">修復済みデバイスの数</span><span class="sxs-lookup"><span data-stu-id="5ae53-152">Number of remediated devices</span></span>|
|<span data-ttu-id="5ae53-153">nonCompliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="5ae53-153">nonCompliantDeviceCount</span></span>|<span data-ttu-id="5ae53-154">Int32</span><span class="sxs-lookup"><span data-stu-id="5ae53-154">Int32</span></span>|<span data-ttu-id="5ae53-155">準拠していないデバイスの数</span><span class="sxs-lookup"><span data-stu-id="5ae53-155">Number of NonCompliant devices</span></span>|
|<span data-ttu-id="5ae53-156">errorDeviceCount</span><span class="sxs-lookup"><span data-stu-id="5ae53-156">errorDeviceCount</span></span>|<span data-ttu-id="5ae53-157">Int32</span><span class="sxs-lookup"><span data-stu-id="5ae53-157">Int32</span></span>|<span data-ttu-id="5ae53-158">エラー デバイスの数</span><span class="sxs-lookup"><span data-stu-id="5ae53-158">Number of error devices</span></span>|
|<span data-ttu-id="5ae53-159">conflictDeviceCount</span><span class="sxs-lookup"><span data-stu-id="5ae53-159">conflictDeviceCount</span></span>|<span data-ttu-id="5ae53-160">Int32</span><span class="sxs-lookup"><span data-stu-id="5ae53-160">Int32</span></span>|<span data-ttu-id="5ae53-161">競合デバイスの数</span><span class="sxs-lookup"><span data-stu-id="5ae53-161">Number of conflict devices</span></span>|



## <a name="response"></a><span data-ttu-id="5ae53-162">応答</span><span class="sxs-lookup"><span data-stu-id="5ae53-162">Response</span></span>
<span data-ttu-id="5ae53-163">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で更新された [deviceCompliancePolicyDeviceStateSummary](../resources/intune-deviceconfig-devicecompliancepolicydevicestatesummary.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="5ae53-163">If successful, this method returns a `200 OK` response code and an updated [deviceCompliancePolicyDeviceStateSummary](../resources/intune-deviceconfig-devicecompliancepolicydevicestatesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5ae53-164">例</span><span class="sxs-lookup"><span data-stu-id="5ae53-164">Example</span></span>

### <a name="request"></a><span data-ttu-id="5ae53-165">要求</span><span class="sxs-lookup"><span data-stu-id="5ae53-165">Request</span></span>
<span data-ttu-id="5ae53-166">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="5ae53-166">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicyDeviceStateSummary
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

### <a name="response"></a><span data-ttu-id="5ae53-167">応答</span><span class="sxs-lookup"><span data-stu-id="5ae53-167">Response</span></span>
<span data-ttu-id="5ae53-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="5ae53-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





