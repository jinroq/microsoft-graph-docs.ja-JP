---
title: deviceComplianceDeviceOverview の更新
description: deviceComplianceDeviceOverview オブジェクトのプロパティを更新します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 8033bfbf0064d7515f20178f8614303c9bf42576
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/26/2019
ms.locfileid: "30262749"
---
# <a name="update-devicecompliancedeviceoverview"></a><span data-ttu-id="28ad9-103">deviceComplianceDeviceOverview の更新</span><span class="sxs-lookup"><span data-stu-id="28ad9-103">Update deviceComplianceDeviceOverview</span></span>

> <span data-ttu-id="28ad9-104">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="28ad9-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="28ad9-105">[deviceComplianceDeviceOverview](../resources/intune-deviceconfig-devicecompliancedeviceoverview.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="28ad9-105">Update the properties of a [deviceComplianceDeviceOverview](../resources/intune-deviceconfig-devicecompliancedeviceoverview.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="28ad9-106">前提条件</span><span class="sxs-lookup"><span data-stu-id="28ad9-106">Prerequisites</span></span>
<span data-ttu-id="28ad9-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/concepts/permissions-reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="28ad9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="28ad9-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="28ad9-109">Permission type</span></span>|<span data-ttu-id="28ad9-110">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="28ad9-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="28ad9-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="28ad9-111">Delegated (work or school account)</span></span>|<span data-ttu-id="28ad9-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="28ad9-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="28ad9-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="28ad9-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="28ad9-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="28ad9-114">Not supported.</span></span>|
|<span data-ttu-id="28ad9-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="28ad9-115">Application</span></span>|<span data-ttu-id="28ad9-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="28ad9-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="28ad9-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="28ad9-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/deviceStatusOverview
```

## <a name="request-headers"></a><span data-ttu-id="28ad9-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="28ad9-118">Request headers</span></span>
|<span data-ttu-id="28ad9-119">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="28ad9-119">Header</span></span>|<span data-ttu-id="28ad9-120">値</span><span class="sxs-lookup"><span data-stu-id="28ad9-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="28ad9-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="28ad9-121">Authorization</span></span>|<span data-ttu-id="28ad9-122">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="28ad9-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="28ad9-123">承諾</span><span class="sxs-lookup"><span data-stu-id="28ad9-123">Accept</span></span>|<span data-ttu-id="28ad9-124">application/json</span><span class="sxs-lookup"><span data-stu-id="28ad9-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="28ad9-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="28ad9-125">Request body</span></span>
<span data-ttu-id="28ad9-126">要求本文で、[deviceComplianceDeviceOverview](../resources/intune-deviceconfig-devicecompliancedeviceoverview.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="28ad9-126">In the request body, supply a JSON representation for the [deviceComplianceDeviceOverview](../resources/intune-deviceconfig-devicecompliancedeviceoverview.md) object.</span></span>

<span data-ttu-id="28ad9-127">次の表に、[deviceComplianceDeviceOverview](../resources/intune-deviceconfig-devicecompliancedeviceoverview.md) の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="28ad9-127">The following table shows the properties that are required when you create the [deviceComplianceDeviceOverview](../resources/intune-deviceconfig-devicecompliancedeviceoverview.md).</span></span>

|<span data-ttu-id="28ad9-128">プロパティ</span><span class="sxs-lookup"><span data-stu-id="28ad9-128">Property</span></span>|<span data-ttu-id="28ad9-129">型</span><span class="sxs-lookup"><span data-stu-id="28ad9-129">Type</span></span>|<span data-ttu-id="28ad9-130">説明</span><span class="sxs-lookup"><span data-stu-id="28ad9-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="28ad9-131">id</span><span class="sxs-lookup"><span data-stu-id="28ad9-131">id</span></span>|<span data-ttu-id="28ad9-132">String</span><span class="sxs-lookup"><span data-stu-id="28ad9-132">String</span></span>|<span data-ttu-id="28ad9-133">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="28ad9-133">Key of the entity.</span></span>|
|<span data-ttu-id="28ad9-134">pendingCount</span><span class="sxs-lookup"><span data-stu-id="28ad9-134">pendingCount</span></span>|<span data-ttu-id="28ad9-135">Int32</span><span class="sxs-lookup"><span data-stu-id="28ad9-135">Int32</span></span>|<span data-ttu-id="28ad9-136">保留中のデバイスの数</span><span class="sxs-lookup"><span data-stu-id="28ad9-136">Number of pending devices</span></span>|
|<span data-ttu-id="28ad9-137">notApplicableCount</span><span class="sxs-lookup"><span data-stu-id="28ad9-137">notApplicableCount</span></span>|<span data-ttu-id="28ad9-138">Int32</span><span class="sxs-lookup"><span data-stu-id="28ad9-138">Int32</span></span>|<span data-ttu-id="28ad9-139">該当しないデバイスの数</span><span class="sxs-lookup"><span data-stu-id="28ad9-139">Number of not applicable devices</span></span>|
|<span data-ttu-id="28ad9-140">successCount</span><span class="sxs-lookup"><span data-stu-id="28ad9-140">successCount</span></span>|<span data-ttu-id="28ad9-141">Int32</span><span class="sxs-lookup"><span data-stu-id="28ad9-141">Int32</span></span>|<span data-ttu-id="28ad9-142">成功したデバイスの数</span><span class="sxs-lookup"><span data-stu-id="28ad9-142">Number of succeeded devices</span></span>|
|<span data-ttu-id="28ad9-143">errorCount</span><span class="sxs-lookup"><span data-stu-id="28ad9-143">errorCount</span></span>|<span data-ttu-id="28ad9-144">Int32</span><span class="sxs-lookup"><span data-stu-id="28ad9-144">Int32</span></span>|<span data-ttu-id="28ad9-145">エラー デバイスの数</span><span class="sxs-lookup"><span data-stu-id="28ad9-145">Number of error devices</span></span>|
|<span data-ttu-id="28ad9-146">failedCount</span><span class="sxs-lookup"><span data-stu-id="28ad9-146">failedCount</span></span>|<span data-ttu-id="28ad9-147">Int32</span><span class="sxs-lookup"><span data-stu-id="28ad9-147">Int32</span></span>|<span data-ttu-id="28ad9-148">失敗したデバイスの数</span><span class="sxs-lookup"><span data-stu-id="28ad9-148">Number of failed devices</span></span>|
|<span data-ttu-id="28ad9-149">lastUpdateDateTime</span><span class="sxs-lookup"><span data-stu-id="28ad9-149">lastUpdateDateTime</span></span>|<span data-ttu-id="28ad9-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="28ad9-150">DateTimeOffset</span></span>|<span data-ttu-id="28ad9-151">最終更新時刻</span><span class="sxs-lookup"><span data-stu-id="28ad9-151">Last update time</span></span>|
|<span data-ttu-id="28ad9-152">configurationVersion</span><span class="sxs-lookup"><span data-stu-id="28ad9-152">configurationVersion</span></span>|<span data-ttu-id="28ad9-153">Int32</span><span class="sxs-lookup"><span data-stu-id="28ad9-153">Int32</span></span>|<span data-ttu-id="28ad9-154">対象の概要に関するポリシーのバージョン</span><span class="sxs-lookup"><span data-stu-id="28ad9-154">Version of the policy for that overview</span></span>|



## <a name="response"></a><span data-ttu-id="28ad9-155">応答</span><span class="sxs-lookup"><span data-stu-id="28ad9-155">Response</span></span>
<span data-ttu-id="28ad9-156">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で更新された [deviceComplianceDeviceOverview](../resources/intune-deviceconfig-devicecompliancedeviceoverview.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="28ad9-156">If successful, this method returns a `200 OK` response code and an updated [deviceComplianceDeviceOverview](../resources/intune-deviceconfig-devicecompliancedeviceoverview.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="28ad9-157">例</span><span class="sxs-lookup"><span data-stu-id="28ad9-157">Example</span></span>

### <a name="request"></a><span data-ttu-id="28ad9-158">要求</span><span class="sxs-lookup"><span data-stu-id="28ad9-158">Request</span></span>
<span data-ttu-id="28ad9-159">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="28ad9-159">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/deviceStatusOverview
Content-type: application/json
Content-length: 281

{
  "@odata.type": "#microsoft.graph.deviceComplianceDeviceOverview",
  "pendingCount": 12,
  "notApplicableCount": 2,
  "successCount": 12,
  "errorCount": 10,
  "failedCount": 11,
  "lastUpdateDateTime": "2016-12-31T23:58:21.6459442-08:00",
  "configurationVersion": 4
}
```

### <a name="response"></a><span data-ttu-id="28ad9-160">応答</span><span class="sxs-lookup"><span data-stu-id="28ad9-160">Response</span></span>
<span data-ttu-id="28ad9-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="28ad9-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 330

{
  "@odata.type": "#microsoft.graph.deviceComplianceDeviceOverview",
  "id": "886f167b-167b-886f-7b16-6f887b166f88",
  "pendingCount": 12,
  "notApplicableCount": 2,
  "successCount": 12,
  "errorCount": 10,
  "failedCount": 11,
  "lastUpdateDateTime": "2016-12-31T23:58:21.6459442-08:00",
  "configurationVersion": 4
}
```



