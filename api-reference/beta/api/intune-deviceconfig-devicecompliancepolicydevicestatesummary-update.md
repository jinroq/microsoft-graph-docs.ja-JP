---
title: deviceCompliancePolicyDeviceStateSummary の更新
description: deviceCompliancePolicyDeviceStateSummary オブジェクトのプロパティを更新します。
ms.openlocfilehash: 045c9ac7aaecac535f3c4d04f587c74cbe84f442
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27070135"
---
# <a name="update-devicecompliancepolicydevicestatesummary"></a><span data-ttu-id="3aafe-103">deviceCompliancePolicyDeviceStateSummary の更新</span><span class="sxs-lookup"><span data-stu-id="3aafe-103">Update deviceCompliancePolicyDeviceStateSummary</span></span>

> <span data-ttu-id="3aafe-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="3aafe-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="3aafe-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="3aafe-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="3aafe-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="3aafe-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="3aafe-107">[deviceCompliancePolicyDeviceStateSummary](../resources/intune-deviceconfig-devicecompliancepolicydevicestatesummary.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="3aafe-107">Update the properties of a [deviceCompliancePolicyDeviceStateSummary](../resources/intune-deviceconfig-devicecompliancepolicydevicestatesummary.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="3aafe-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="3aafe-108">Prerequisites</span></span>
<span data-ttu-id="3aafe-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="3aafe-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3aafe-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="3aafe-111">Permission type</span></span>|<span data-ttu-id="3aafe-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="3aafe-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3aafe-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="3aafe-113">Delegated (work or school account)</span></span>|<span data-ttu-id="3aafe-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3aafe-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="3aafe-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="3aafe-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3aafe-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="3aafe-116">Not supported.</span></span>|
|<span data-ttu-id="3aafe-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="3aafe-117">Application</span></span>|<span data-ttu-id="3aafe-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="3aafe-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="3aafe-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="3aafe-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicyDeviceStateSummary
```

## <a name="request-headers"></a><span data-ttu-id="3aafe-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="3aafe-120">Request headers</span></span>
|<span data-ttu-id="3aafe-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="3aafe-121">Header</span></span>|<span data-ttu-id="3aafe-122">値</span><span class="sxs-lookup"><span data-stu-id="3aafe-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3aafe-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="3aafe-123">Authorization</span></span>|<span data-ttu-id="3aafe-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="3aafe-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3aafe-125">Accept</span><span class="sxs-lookup"><span data-stu-id="3aafe-125">Accept</span></span>|<span data-ttu-id="3aafe-126">application/json</span><span class="sxs-lookup"><span data-stu-id="3aafe-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3aafe-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="3aafe-127">Request body</span></span>
<span data-ttu-id="3aafe-128">要求本文で、[deviceCompliancePolicyDeviceStateSummary](../resources/intune-deviceconfig-devicecompliancepolicydevicestatesummary.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="3aafe-128">In the request body, supply a JSON representation for the [deviceCompliancePolicyDeviceStateSummary](../resources/intune-deviceconfig-devicecompliancepolicydevicestatesummary.md) object.</span></span>

<span data-ttu-id="3aafe-129">次の表に、[deviceCompliancePolicyDeviceStateSummary](../resources/intune-deviceconfig-devicecompliancepolicydevicestatesummary.md) の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="3aafe-129">The following table shows the properties that are required when you create the [deviceCompliancePolicyDeviceStateSummary](../resources/intune-deviceconfig-devicecompliancepolicydevicestatesummary.md).</span></span>

|<span data-ttu-id="3aafe-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="3aafe-130">Property</span></span>|<span data-ttu-id="3aafe-131">型</span><span class="sxs-lookup"><span data-stu-id="3aafe-131">Type</span></span>|<span data-ttu-id="3aafe-132">説明</span><span class="sxs-lookup"><span data-stu-id="3aafe-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3aafe-133">inGracePeriodCount</span><span class="sxs-lookup"><span data-stu-id="3aafe-133">inGracePeriodCount</span></span>|<span data-ttu-id="3aafe-134">Int32</span><span class="sxs-lookup"><span data-stu-id="3aafe-134">Int32</span></span>|<span data-ttu-id="3aafe-135">解約猶予期間内のデバイスの数</span><span class="sxs-lookup"><span data-stu-id="3aafe-135">Number of devices that are in grace period</span></span>|
|<span data-ttu-id="3aafe-136">configManagerCount</span><span class="sxs-lookup"><span data-stu-id="3aafe-136">configManagerCount</span></span>|<span data-ttu-id="3aafe-137">Int32</span><span class="sxs-lookup"><span data-stu-id="3aafe-137">Int32</span></span>|<span data-ttu-id="3aafe-138">System Center Configuration Manager によってコンプライアンスが管理されているデバイスの数</span><span class="sxs-lookup"><span data-stu-id="3aafe-138">Number of devices that have compliance managed by System Center Configuration Manager</span></span>|
|<span data-ttu-id="3aafe-139">id</span><span class="sxs-lookup"><span data-stu-id="3aafe-139">id</span></span>|<span data-ttu-id="3aafe-140">String</span><span class="sxs-lookup"><span data-stu-id="3aafe-140">String</span></span>|<span data-ttu-id="3aafe-141">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="3aafe-141">Key of the entity.</span></span>|
|<span data-ttu-id="3aafe-142">unknownDeviceCount</span><span class="sxs-lookup"><span data-stu-id="3aafe-142">unknownDeviceCount</span></span>|<span data-ttu-id="3aafe-143">Int32</span><span class="sxs-lookup"><span data-stu-id="3aafe-143">Int32</span></span>|<span data-ttu-id="3aafe-144">不明なデバイスの数</span><span class="sxs-lookup"><span data-stu-id="3aafe-144">Number of unknown devices</span></span>|
|<span data-ttu-id="3aafe-145">notApplicableDeviceCount</span><span class="sxs-lookup"><span data-stu-id="3aafe-145">notApplicableDeviceCount</span></span>|<span data-ttu-id="3aafe-146">Int32</span><span class="sxs-lookup"><span data-stu-id="3aafe-146">Int32</span></span>|<span data-ttu-id="3aafe-147">該当しないデバイスの数</span><span class="sxs-lookup"><span data-stu-id="3aafe-147">Number of not applicable devices</span></span>|
|<span data-ttu-id="3aafe-148">compliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="3aafe-148">compliantDeviceCount</span></span>|<span data-ttu-id="3aafe-149">Int32</span><span class="sxs-lookup"><span data-stu-id="3aafe-149">Int32</span></span>|<span data-ttu-id="3aafe-150">準拠デバイスの数</span><span class="sxs-lookup"><span data-stu-id="3aafe-150">Number of compliant devices</span></span>|
|<span data-ttu-id="3aafe-151">remediatedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="3aafe-151">remediatedDeviceCount</span></span>|<span data-ttu-id="3aafe-152">Int32</span><span class="sxs-lookup"><span data-stu-id="3aafe-152">Int32</span></span>|<span data-ttu-id="3aafe-153">修復済みデバイスの数</span><span class="sxs-lookup"><span data-stu-id="3aafe-153">Number of remediated devices</span></span>|
|<span data-ttu-id="3aafe-154">nonCompliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="3aafe-154">nonCompliantDeviceCount</span></span>|<span data-ttu-id="3aafe-155">Int32</span><span class="sxs-lookup"><span data-stu-id="3aafe-155">Int32</span></span>|<span data-ttu-id="3aafe-156">準拠していないデバイスの数</span><span class="sxs-lookup"><span data-stu-id="3aafe-156">Number of NonCompliant devices</span></span>|
|<span data-ttu-id="3aafe-157">errorDeviceCount</span><span class="sxs-lookup"><span data-stu-id="3aafe-157">errorDeviceCount</span></span>|<span data-ttu-id="3aafe-158">Int32</span><span class="sxs-lookup"><span data-stu-id="3aafe-158">Int32</span></span>|<span data-ttu-id="3aafe-159">エラー デバイスの数</span><span class="sxs-lookup"><span data-stu-id="3aafe-159">Number of error devices</span></span>|
|<span data-ttu-id="3aafe-160">conflictDeviceCount</span><span class="sxs-lookup"><span data-stu-id="3aafe-160">conflictDeviceCount</span></span>|<span data-ttu-id="3aafe-161">Int32</span><span class="sxs-lookup"><span data-stu-id="3aafe-161">Int32</span></span>|<span data-ttu-id="3aafe-162">競合デバイスの数</span><span class="sxs-lookup"><span data-stu-id="3aafe-162">Number of conflict devices</span></span>|



## <a name="response"></a><span data-ttu-id="3aafe-163">応答</span><span class="sxs-lookup"><span data-stu-id="3aafe-163">Response</span></span>
<span data-ttu-id="3aafe-164">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で更新された [deviceCompliancePolicyDeviceStateSummary](../resources/intune-deviceconfig-devicecompliancepolicydevicestatesummary.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="3aafe-164">If successful, this method returns a `200 OK` response code and an updated [deviceCompliancePolicyDeviceStateSummary](../resources/intune-deviceconfig-devicecompliancepolicydevicestatesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3aafe-165">例</span><span class="sxs-lookup"><span data-stu-id="3aafe-165">Example</span></span>
### <a name="request"></a><span data-ttu-id="3aafe-166">要求</span><span class="sxs-lookup"><span data-stu-id="3aafe-166">Request</span></span>
<span data-ttu-id="3aafe-167">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="3aafe-167">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicyDeviceStateSummary
Content-type: application/json
Content-length: 270

{
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

### <a name="response"></a><span data-ttu-id="3aafe-168">応答</span><span class="sxs-lookup"><span data-stu-id="3aafe-168">Response</span></span>
<span data-ttu-id="3aafe-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="3aafe-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





