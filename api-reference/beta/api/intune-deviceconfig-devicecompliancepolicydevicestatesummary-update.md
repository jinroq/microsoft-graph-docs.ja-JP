---
title: deviceCompliancePolicyDeviceStateSummary の更新
description: deviceCompliancePolicyDeviceStateSummary オブジェクトのプロパティを更新します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: e09bf9e326a0d422b1b6ff23e2927141a6f32e41
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/11/2019
ms.locfileid: "31807638"
---
# <a name="update-devicecompliancepolicydevicestatesummary"></a><span data-ttu-id="e0c6b-103">deviceCompliancePolicyDeviceStateSummary の更新</span><span class="sxs-lookup"><span data-stu-id="e0c6b-103">Update deviceCompliancePolicyDeviceStateSummary</span></span>

> <span data-ttu-id="e0c6b-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e0c6b-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e0c6b-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="e0c6b-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e0c6b-106">[deviceCompliancePolicyDeviceStateSummary](../resources/intune-deviceconfig-devicecompliancepolicydevicestatesummary.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="e0c6b-106">Update the properties of a [deviceCompliancePolicyDeviceStateSummary](../resources/intune-deviceconfig-devicecompliancepolicydevicestatesummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e0c6b-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="e0c6b-107">Prerequisites</span></span>
<span data-ttu-id="e0c6b-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="e0c6b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e0c6b-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="e0c6b-110">Permission type</span></span>|<span data-ttu-id="e0c6b-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="e0c6b-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e0c6b-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="e0c6b-112">Delegated (work or school account)</span></span>|<span data-ttu-id="e0c6b-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e0c6b-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="e0c6b-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="e0c6b-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e0c6b-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e0c6b-115">Not supported.</span></span>|
|<span data-ttu-id="e0c6b-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="e0c6b-116">Application</span></span>|<span data-ttu-id="e0c6b-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e0c6b-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e0c6b-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="e0c6b-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicyDeviceStateSummary
```

## <a name="request-headers"></a><span data-ttu-id="e0c6b-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="e0c6b-119">Request headers</span></span>
|<span data-ttu-id="e0c6b-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="e0c6b-120">Header</span></span>|<span data-ttu-id="e0c6b-121">値</span><span class="sxs-lookup"><span data-stu-id="e0c6b-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e0c6b-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="e0c6b-122">Authorization</span></span>|<span data-ttu-id="e0c6b-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="e0c6b-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e0c6b-124">承諾</span><span class="sxs-lookup"><span data-stu-id="e0c6b-124">Accept</span></span>|<span data-ttu-id="e0c6b-125">application/json</span><span class="sxs-lookup"><span data-stu-id="e0c6b-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e0c6b-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="e0c6b-126">Request body</span></span>
<span data-ttu-id="e0c6b-127">要求本文で、[deviceCompliancePolicyDeviceStateSummary](../resources/intune-deviceconfig-devicecompliancepolicydevicestatesummary.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="e0c6b-127">In the request body, supply a JSON representation for the [deviceCompliancePolicyDeviceStateSummary](../resources/intune-deviceconfig-devicecompliancepolicydevicestatesummary.md) object.</span></span>

<span data-ttu-id="e0c6b-128">次の表に、[deviceCompliancePolicyDeviceStateSummary](../resources/intune-deviceconfig-devicecompliancepolicydevicestatesummary.md) の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="e0c6b-128">The following table shows the properties that are required when you create the [deviceCompliancePolicyDeviceStateSummary](../resources/intune-deviceconfig-devicecompliancepolicydevicestatesummary.md).</span></span>

|<span data-ttu-id="e0c6b-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="e0c6b-129">Property</span></span>|<span data-ttu-id="e0c6b-130">型</span><span class="sxs-lookup"><span data-stu-id="e0c6b-130">Type</span></span>|<span data-ttu-id="e0c6b-131">説明</span><span class="sxs-lookup"><span data-stu-id="e0c6b-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e0c6b-132">inGracePeriodCount</span><span class="sxs-lookup"><span data-stu-id="e0c6b-132">inGracePeriodCount</span></span>|<span data-ttu-id="e0c6b-133">Int32</span><span class="sxs-lookup"><span data-stu-id="e0c6b-133">Int32</span></span>|<span data-ttu-id="e0c6b-134">解約猶予期間内のデバイスの数</span><span class="sxs-lookup"><span data-stu-id="e0c6b-134">Number of devices that are in grace period</span></span>|
|<span data-ttu-id="e0c6b-135">configManagerCount</span><span class="sxs-lookup"><span data-stu-id="e0c6b-135">configManagerCount</span></span>|<span data-ttu-id="e0c6b-136">Int32</span><span class="sxs-lookup"><span data-stu-id="e0c6b-136">Int32</span></span>|<span data-ttu-id="e0c6b-137">System Center Configuration Manager によってコンプライアンスが管理されているデバイスの数</span><span class="sxs-lookup"><span data-stu-id="e0c6b-137">Number of devices that have compliance managed by System Center Configuration Manager</span></span>|
|<span data-ttu-id="e0c6b-138">id</span><span class="sxs-lookup"><span data-stu-id="e0c6b-138">id</span></span>|<span data-ttu-id="e0c6b-139">String</span><span class="sxs-lookup"><span data-stu-id="e0c6b-139">String</span></span>|<span data-ttu-id="e0c6b-140">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="e0c6b-140">Key of the entity.</span></span>|
|<span data-ttu-id="e0c6b-141">unknownDeviceCount</span><span class="sxs-lookup"><span data-stu-id="e0c6b-141">unknownDeviceCount</span></span>|<span data-ttu-id="e0c6b-142">Int32</span><span class="sxs-lookup"><span data-stu-id="e0c6b-142">Int32</span></span>|<span data-ttu-id="e0c6b-143">不明なデバイスの数</span><span class="sxs-lookup"><span data-stu-id="e0c6b-143">Number of unknown devices</span></span>|
|<span data-ttu-id="e0c6b-144">notApplicableDeviceCount</span><span class="sxs-lookup"><span data-stu-id="e0c6b-144">notApplicableDeviceCount</span></span>|<span data-ttu-id="e0c6b-145">Int32</span><span class="sxs-lookup"><span data-stu-id="e0c6b-145">Int32</span></span>|<span data-ttu-id="e0c6b-146">該当しないデバイスの数</span><span class="sxs-lookup"><span data-stu-id="e0c6b-146">Number of not applicable devices</span></span>|
|<span data-ttu-id="e0c6b-147">compliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="e0c6b-147">compliantDeviceCount</span></span>|<span data-ttu-id="e0c6b-148">Int32</span><span class="sxs-lookup"><span data-stu-id="e0c6b-148">Int32</span></span>|<span data-ttu-id="e0c6b-149">準拠デバイスの数</span><span class="sxs-lookup"><span data-stu-id="e0c6b-149">Number of compliant devices</span></span>|
|<span data-ttu-id="e0c6b-150">remediatedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="e0c6b-150">remediatedDeviceCount</span></span>|<span data-ttu-id="e0c6b-151">Int32</span><span class="sxs-lookup"><span data-stu-id="e0c6b-151">Int32</span></span>|<span data-ttu-id="e0c6b-152">修復済みデバイスの数</span><span class="sxs-lookup"><span data-stu-id="e0c6b-152">Number of remediated devices</span></span>|
|<span data-ttu-id="e0c6b-153">nonCompliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="e0c6b-153">nonCompliantDeviceCount</span></span>|<span data-ttu-id="e0c6b-154">Int32</span><span class="sxs-lookup"><span data-stu-id="e0c6b-154">Int32</span></span>|<span data-ttu-id="e0c6b-155">準拠していないデバイスの数</span><span class="sxs-lookup"><span data-stu-id="e0c6b-155">Number of NonCompliant devices</span></span>|
|<span data-ttu-id="e0c6b-156">errorDeviceCount</span><span class="sxs-lookup"><span data-stu-id="e0c6b-156">errorDeviceCount</span></span>|<span data-ttu-id="e0c6b-157">Int32</span><span class="sxs-lookup"><span data-stu-id="e0c6b-157">Int32</span></span>|<span data-ttu-id="e0c6b-158">エラー デバイスの数</span><span class="sxs-lookup"><span data-stu-id="e0c6b-158">Number of error devices</span></span>|
|<span data-ttu-id="e0c6b-159">conflictDeviceCount</span><span class="sxs-lookup"><span data-stu-id="e0c6b-159">conflictDeviceCount</span></span>|<span data-ttu-id="e0c6b-160">Int32</span><span class="sxs-lookup"><span data-stu-id="e0c6b-160">Int32</span></span>|<span data-ttu-id="e0c6b-161">競合デバイスの数</span><span class="sxs-lookup"><span data-stu-id="e0c6b-161">Number of conflict devices</span></span>|



## <a name="response"></a><span data-ttu-id="e0c6b-162">応答</span><span class="sxs-lookup"><span data-stu-id="e0c6b-162">Response</span></span>
<span data-ttu-id="e0c6b-163">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で更新された [deviceCompliancePolicyDeviceStateSummary](../resources/intune-deviceconfig-devicecompliancepolicydevicestatesummary.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="e0c6b-163">If successful, this method returns a `200 OK` response code and an updated [deviceCompliancePolicyDeviceStateSummary](../resources/intune-deviceconfig-devicecompliancepolicydevicestatesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e0c6b-164">例</span><span class="sxs-lookup"><span data-stu-id="e0c6b-164">Example</span></span>

### <a name="request"></a><span data-ttu-id="e0c6b-165">要求</span><span class="sxs-lookup"><span data-stu-id="e0c6b-165">Request</span></span>
<span data-ttu-id="e0c6b-166">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="e0c6b-166">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="e0c6b-167">応答</span><span class="sxs-lookup"><span data-stu-id="e0c6b-167">Response</span></span>
<span data-ttu-id="e0c6b-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="e0c6b-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





