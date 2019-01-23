---
title: deviceCompliancePolicyDeviceStateSummary の更新
description: deviceCompliancePolicyDeviceStateSummary オブジェクトのプロパティを更新します。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 4874905a7ab1501cad6c72871111792cabf55c22
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29399151"
---
# <a name="update-devicecompliancepolicydevicestatesummary"></a><span data-ttu-id="ebf35-103">deviceCompliancePolicyDeviceStateSummary の更新</span><span class="sxs-lookup"><span data-stu-id="ebf35-103">Update deviceCompliancePolicyDeviceStateSummary</span></span>

> <span data-ttu-id="ebf35-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="ebf35-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="ebf35-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ebf35-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="ebf35-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="ebf35-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ebf35-107">[deviceCompliancePolicyDeviceStateSummary](../resources/intune-deviceconfig-devicecompliancepolicydevicestatesummary.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="ebf35-107">Update the properties of a [deviceCompliancePolicyDeviceStateSummary](../resources/intune-deviceconfig-devicecompliancepolicydevicestatesummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ebf35-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="ebf35-108">Prerequisites</span></span>
<span data-ttu-id="ebf35-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/concepts/permissions-reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="ebf35-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="ebf35-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="ebf35-111">Permission type</span></span>|<span data-ttu-id="ebf35-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="ebf35-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ebf35-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="ebf35-113">Delegated (work or school account)</span></span>|<span data-ttu-id="ebf35-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ebf35-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="ebf35-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="ebf35-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ebf35-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ebf35-116">Not supported.</span></span>|
|<span data-ttu-id="ebf35-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="ebf35-117">Application</span></span>|<span data-ttu-id="ebf35-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ebf35-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ebf35-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="ebf35-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicyDeviceStateSummary
```

## <a name="request-headers"></a><span data-ttu-id="ebf35-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="ebf35-120">Request headers</span></span>
|<span data-ttu-id="ebf35-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="ebf35-121">Header</span></span>|<span data-ttu-id="ebf35-122">値</span><span class="sxs-lookup"><span data-stu-id="ebf35-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ebf35-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="ebf35-123">Authorization</span></span>|<span data-ttu-id="ebf35-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="ebf35-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ebf35-125">Accept</span><span class="sxs-lookup"><span data-stu-id="ebf35-125">Accept</span></span>|<span data-ttu-id="ebf35-126">application/json</span><span class="sxs-lookup"><span data-stu-id="ebf35-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ebf35-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="ebf35-127">Request body</span></span>
<span data-ttu-id="ebf35-128">要求本文で、[deviceCompliancePolicyDeviceStateSummary](../resources/intune-deviceconfig-devicecompliancepolicydevicestatesummary.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="ebf35-128">In the request body, supply a JSON representation for the [deviceCompliancePolicyDeviceStateSummary](../resources/intune-deviceconfig-devicecompliancepolicydevicestatesummary.md) object.</span></span>

<span data-ttu-id="ebf35-129">次の表に、[deviceCompliancePolicyDeviceStateSummary](../resources/intune-deviceconfig-devicecompliancepolicydevicestatesummary.md) の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="ebf35-129">The following table shows the properties that are required when you create the [deviceCompliancePolicyDeviceStateSummary](../resources/intune-deviceconfig-devicecompliancepolicydevicestatesummary.md).</span></span>

|<span data-ttu-id="ebf35-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="ebf35-130">Property</span></span>|<span data-ttu-id="ebf35-131">型</span><span class="sxs-lookup"><span data-stu-id="ebf35-131">Type</span></span>|<span data-ttu-id="ebf35-132">説明</span><span class="sxs-lookup"><span data-stu-id="ebf35-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ebf35-133">inGracePeriodCount</span><span class="sxs-lookup"><span data-stu-id="ebf35-133">inGracePeriodCount</span></span>|<span data-ttu-id="ebf35-134">Int32</span><span class="sxs-lookup"><span data-stu-id="ebf35-134">Int32</span></span>|<span data-ttu-id="ebf35-135">解約猶予期間内のデバイスの数</span><span class="sxs-lookup"><span data-stu-id="ebf35-135">Number of devices that are in grace period</span></span>|
|<span data-ttu-id="ebf35-136">configManagerCount</span><span class="sxs-lookup"><span data-stu-id="ebf35-136">configManagerCount</span></span>|<span data-ttu-id="ebf35-137">Int32</span><span class="sxs-lookup"><span data-stu-id="ebf35-137">Int32</span></span>|<span data-ttu-id="ebf35-138">System Center Configuration Manager によってコンプライアンスが管理されているデバイスの数</span><span class="sxs-lookup"><span data-stu-id="ebf35-138">Number of devices that have compliance managed by System Center Configuration Manager</span></span>|
|<span data-ttu-id="ebf35-139">id</span><span class="sxs-lookup"><span data-stu-id="ebf35-139">id</span></span>|<span data-ttu-id="ebf35-140">String</span><span class="sxs-lookup"><span data-stu-id="ebf35-140">String</span></span>|<span data-ttu-id="ebf35-141">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="ebf35-141">Key of the entity.</span></span>|
|<span data-ttu-id="ebf35-142">unknownDeviceCount</span><span class="sxs-lookup"><span data-stu-id="ebf35-142">unknownDeviceCount</span></span>|<span data-ttu-id="ebf35-143">Int32</span><span class="sxs-lookup"><span data-stu-id="ebf35-143">Int32</span></span>|<span data-ttu-id="ebf35-144">不明なデバイスの数</span><span class="sxs-lookup"><span data-stu-id="ebf35-144">Number of unknown devices</span></span>|
|<span data-ttu-id="ebf35-145">notApplicableDeviceCount</span><span class="sxs-lookup"><span data-stu-id="ebf35-145">notApplicableDeviceCount</span></span>|<span data-ttu-id="ebf35-146">Int32</span><span class="sxs-lookup"><span data-stu-id="ebf35-146">Int32</span></span>|<span data-ttu-id="ebf35-147">該当しないデバイスの数</span><span class="sxs-lookup"><span data-stu-id="ebf35-147">Number of not applicable devices</span></span>|
|<span data-ttu-id="ebf35-148">compliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="ebf35-148">compliantDeviceCount</span></span>|<span data-ttu-id="ebf35-149">Int32</span><span class="sxs-lookup"><span data-stu-id="ebf35-149">Int32</span></span>|<span data-ttu-id="ebf35-150">準拠デバイスの数</span><span class="sxs-lookup"><span data-stu-id="ebf35-150">Number of compliant devices</span></span>|
|<span data-ttu-id="ebf35-151">remediatedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="ebf35-151">remediatedDeviceCount</span></span>|<span data-ttu-id="ebf35-152">Int32</span><span class="sxs-lookup"><span data-stu-id="ebf35-152">Int32</span></span>|<span data-ttu-id="ebf35-153">修復済みデバイスの数</span><span class="sxs-lookup"><span data-stu-id="ebf35-153">Number of remediated devices</span></span>|
|<span data-ttu-id="ebf35-154">nonCompliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="ebf35-154">nonCompliantDeviceCount</span></span>|<span data-ttu-id="ebf35-155">Int32</span><span class="sxs-lookup"><span data-stu-id="ebf35-155">Int32</span></span>|<span data-ttu-id="ebf35-156">準拠していないデバイスの数</span><span class="sxs-lookup"><span data-stu-id="ebf35-156">Number of NonCompliant devices</span></span>|
|<span data-ttu-id="ebf35-157">errorDeviceCount</span><span class="sxs-lookup"><span data-stu-id="ebf35-157">errorDeviceCount</span></span>|<span data-ttu-id="ebf35-158">Int32</span><span class="sxs-lookup"><span data-stu-id="ebf35-158">Int32</span></span>|<span data-ttu-id="ebf35-159">エラー デバイスの数</span><span class="sxs-lookup"><span data-stu-id="ebf35-159">Number of error devices</span></span>|
|<span data-ttu-id="ebf35-160">conflictDeviceCount</span><span class="sxs-lookup"><span data-stu-id="ebf35-160">conflictDeviceCount</span></span>|<span data-ttu-id="ebf35-161">Int32</span><span class="sxs-lookup"><span data-stu-id="ebf35-161">Int32</span></span>|<span data-ttu-id="ebf35-162">競合デバイスの数</span><span class="sxs-lookup"><span data-stu-id="ebf35-162">Number of conflict devices</span></span>|



## <a name="response"></a><span data-ttu-id="ebf35-163">応答</span><span class="sxs-lookup"><span data-stu-id="ebf35-163">Response</span></span>
<span data-ttu-id="ebf35-164">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で更新された [deviceCompliancePolicyDeviceStateSummary](../resources/intune-deviceconfig-devicecompliancepolicydevicestatesummary.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="ebf35-164">If successful, this method returns a `200 OK` response code and an updated [deviceCompliancePolicyDeviceStateSummary](../resources/intune-deviceconfig-devicecompliancepolicydevicestatesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ebf35-165">例</span><span class="sxs-lookup"><span data-stu-id="ebf35-165">Example</span></span>

### <a name="request"></a><span data-ttu-id="ebf35-166">要求</span><span class="sxs-lookup"><span data-stu-id="ebf35-166">Request</span></span>
<span data-ttu-id="ebf35-167">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="ebf35-167">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="ebf35-168">応答</span><span class="sxs-lookup"><span data-stu-id="ebf35-168">Response</span></span>
<span data-ttu-id="ebf35-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="ebf35-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




