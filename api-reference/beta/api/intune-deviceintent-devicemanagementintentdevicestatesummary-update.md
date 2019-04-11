---
title: deviceManagementIntentDeviceStateSummary の更新
description: deviceManagementIntentDeviceStateSummary オブジェクトのプロパティを更新します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: d790aaf3e0218d7313c6999ace76a443925ecec2
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/11/2019
ms.locfileid: "31805916"
---
# <a name="update-devicemanagementintentdevicestatesummary"></a><span data-ttu-id="809f3-103">deviceManagementIntentDeviceStateSummary の更新</span><span class="sxs-lookup"><span data-stu-id="809f3-103">Update deviceManagementIntentDeviceStateSummary</span></span>

> <span data-ttu-id="809f3-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="809f3-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="809f3-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="809f3-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="809f3-106">[deviceManagementIntentDeviceStateSummary](../resources/intune-deviceintent-devicemanagementintentdevicestatesummary.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="809f3-106">Update the properties of a [deviceManagementIntentDeviceStateSummary](../resources/intune-deviceintent-devicemanagementintentdevicestatesummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="809f3-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="809f3-107">Prerequisites</span></span>
<span data-ttu-id="809f3-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="809f3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="809f3-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="809f3-110">Permission type</span></span>|<span data-ttu-id="809f3-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="809f3-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="809f3-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="809f3-112">Delegated (work or school account)</span></span>|<span data-ttu-id="809f3-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="809f3-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="809f3-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="809f3-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="809f3-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="809f3-115">Not supported.</span></span>|
|<span data-ttu-id="809f3-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="809f3-116">Application</span></span>|<span data-ttu-id="809f3-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="809f3-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="809f3-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="809f3-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/intents/{deviceManagementIntentId}/deviceStateSummary
```

## <a name="request-headers"></a><span data-ttu-id="809f3-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="809f3-119">Request headers</span></span>
|<span data-ttu-id="809f3-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="809f3-120">Header</span></span>|<span data-ttu-id="809f3-121">値</span><span class="sxs-lookup"><span data-stu-id="809f3-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="809f3-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="809f3-122">Authorization</span></span>|<span data-ttu-id="809f3-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="809f3-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="809f3-124">承諾</span><span class="sxs-lookup"><span data-stu-id="809f3-124">Accept</span></span>|<span data-ttu-id="809f3-125">application/json</span><span class="sxs-lookup"><span data-stu-id="809f3-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="809f3-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="809f3-126">Request body</span></span>
<span data-ttu-id="809f3-127">要求本文で、 [deviceManagementIntentDeviceStateSummary](../resources/intune-deviceintent-devicemanagementintentdevicestatesummary.md)オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="809f3-127">In the request body, supply a JSON representation for the [deviceManagementIntentDeviceStateSummary](../resources/intune-deviceintent-devicemanagementintentdevicestatesummary.md) object.</span></span>

<span data-ttu-id="809f3-128">次の表に、 [deviceManagementIntentDeviceStateSummary](../resources/intune-deviceintent-devicemanagementintentdevicestatesummary.md)の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="809f3-128">The following table shows the properties that are required when you create the [deviceManagementIntentDeviceStateSummary](../resources/intune-deviceintent-devicemanagementintentdevicestatesummary.md).</span></span>

|<span data-ttu-id="809f3-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="809f3-129">Property</span></span>|<span data-ttu-id="809f3-130">型</span><span class="sxs-lookup"><span data-stu-id="809f3-130">Type</span></span>|<span data-ttu-id="809f3-131">説明</span><span class="sxs-lookup"><span data-stu-id="809f3-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="809f3-132">id</span><span class="sxs-lookup"><span data-stu-id="809f3-132">id</span></span>|<span data-ttu-id="809f3-133">String</span><span class="sxs-lookup"><span data-stu-id="809f3-133">String</span></span>|<span data-ttu-id="809f3-134">ID</span><span class="sxs-lookup"><span data-stu-id="809f3-134">The ID</span></span>|
|<span data-ttu-id="809f3-135">conflictCount</span><span class="sxs-lookup"><span data-stu-id="809f3-135">conflictCount</span></span>|<span data-ttu-id="809f3-136">Int32</span><span class="sxs-lookup"><span data-stu-id="809f3-136">Int32</span></span>|<span data-ttu-id="809f3-137">競合しているデバイスの数</span><span class="sxs-lookup"><span data-stu-id="809f3-137">Number of devices in conflict</span></span>|
|<span data-ttu-id="809f3-138">errorCount</span><span class="sxs-lookup"><span data-stu-id="809f3-138">errorCount</span></span>|<span data-ttu-id="809f3-139">Int32</span><span class="sxs-lookup"><span data-stu-id="809f3-139">Int32</span></span>|<span data-ttu-id="809f3-140">エラー デバイスの数</span><span class="sxs-lookup"><span data-stu-id="809f3-140">Number of error devices</span></span>|
|<span data-ttu-id="809f3-141">failedCount</span><span class="sxs-lookup"><span data-stu-id="809f3-141">failedCount</span></span>|<span data-ttu-id="809f3-142">Int32</span><span class="sxs-lookup"><span data-stu-id="809f3-142">Int32</span></span>|<span data-ttu-id="809f3-143">失敗したデバイスの数</span><span class="sxs-lookup"><span data-stu-id="809f3-143">Number of failed devices</span></span>|
|<span data-ttu-id="809f3-144">notApplicableCount</span><span class="sxs-lookup"><span data-stu-id="809f3-144">notApplicableCount</span></span>|<span data-ttu-id="809f3-145">Int32</span><span class="sxs-lookup"><span data-stu-id="809f3-145">Int32</span></span>|<span data-ttu-id="809f3-146">該当しないデバイスの数</span><span class="sxs-lookup"><span data-stu-id="809f3-146">Number of not applicable devices</span></span>|
|<span data-ttu-id="809f3-147">notApplicablePlatformCount</span><span class="sxs-lookup"><span data-stu-id="809f3-147">notApplicablePlatformCount</span></span>|<span data-ttu-id="809f3-148">Int32</span><span class="sxs-lookup"><span data-stu-id="809f3-148">Int32</span></span>|<span data-ttu-id="809f3-149">プラットフォームとポリシーの不一致が原因で適用されていないデバイスの数</span><span class="sxs-lookup"><span data-stu-id="809f3-149">Number of not applicable devices due to mismatch platform and policy</span></span>|
|<span data-ttu-id="809f3-150">successCount</span><span class="sxs-lookup"><span data-stu-id="809f3-150">successCount</span></span>|<span data-ttu-id="809f3-151">Int32</span><span class="sxs-lookup"><span data-stu-id="809f3-151">Int32</span></span>|<span data-ttu-id="809f3-152">成功したデバイスの数</span><span class="sxs-lookup"><span data-stu-id="809f3-152">Number of succeeded devices</span></span>|



## <a name="response"></a><span data-ttu-id="809f3-153">応答</span><span class="sxs-lookup"><span data-stu-id="809f3-153">Response</span></span>
<span data-ttu-id="809f3-154">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で更新された[deviceManagementIntentDeviceStateSummary](../resources/intune-deviceintent-devicemanagementintentdevicestatesummary.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="809f3-154">If successful, this method returns a `200 OK` response code and an updated [deviceManagementIntentDeviceStateSummary](../resources/intune-deviceintent-devicemanagementintentdevicestatesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="809f3-155">例</span><span class="sxs-lookup"><span data-stu-id="809f3-155">Example</span></span>

### <a name="request"></a><span data-ttu-id="809f3-156">要求</span><span class="sxs-lookup"><span data-stu-id="809f3-156">Request</span></span>
<span data-ttu-id="809f3-157">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="809f3-157">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/intents/{deviceManagementIntentId}/deviceStateSummary
Content-type: application/json
Content-length: 237

{
  "@odata.type": "#microsoft.graph.deviceManagementIntentDeviceStateSummary",
  "conflictCount": 13,
  "errorCount": 10,
  "failedCount": 11,
  "notApplicableCount": 2,
  "notApplicablePlatformCount": 10,
  "successCount": 12
}
```

### <a name="response"></a><span data-ttu-id="809f3-158">応答</span><span class="sxs-lookup"><span data-stu-id="809f3-158">Response</span></span>
<span data-ttu-id="809f3-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="809f3-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 286

{
  "@odata.type": "#microsoft.graph.deviceManagementIntentDeviceStateSummary",
  "id": "12230bf9-0bf9-1223-f90b-2312f90b2312",
  "conflictCount": 13,
  "errorCount": 10,
  "failedCount": 11,
  "notApplicableCount": 2,
  "notApplicablePlatformCount": 10,
  "successCount": 12
}
```





