---
title: deviceManagementIntentDeviceStateSummary の更新
description: deviceManagementIntentDeviceStateSummary オブジェクトのプロパティを更新します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: d790aaf3e0218d7313c6999ace76a443925ecec2
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32508296"
---
# <a name="update-devicemanagementintentdevicestatesummary"></a><span data-ttu-id="89ff9-103">deviceManagementIntentDeviceStateSummary の更新</span><span class="sxs-lookup"><span data-stu-id="89ff9-103">Update deviceManagementIntentDeviceStateSummary</span></span>

> <span data-ttu-id="89ff9-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="89ff9-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="89ff9-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="89ff9-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="89ff9-106">[deviceManagementIntentDeviceStateSummary](../resources/intune-deviceintent-devicemanagementintentdevicestatesummary.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="89ff9-106">Update the properties of a [deviceManagementIntentDeviceStateSummary](../resources/intune-deviceintent-devicemanagementintentdevicestatesummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="89ff9-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="89ff9-107">Prerequisites</span></span>
<span data-ttu-id="89ff9-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="89ff9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="89ff9-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="89ff9-110">Permission type</span></span>|<span data-ttu-id="89ff9-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="89ff9-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="89ff9-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="89ff9-112">Delegated (work or school account)</span></span>|<span data-ttu-id="89ff9-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="89ff9-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="89ff9-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="89ff9-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="89ff9-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="89ff9-115">Not supported.</span></span>|
|<span data-ttu-id="89ff9-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="89ff9-116">Application</span></span>|<span data-ttu-id="89ff9-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="89ff9-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="89ff9-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="89ff9-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/intents/{deviceManagementIntentId}/deviceStateSummary
```

## <a name="request-headers"></a><span data-ttu-id="89ff9-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="89ff9-119">Request headers</span></span>
|<span data-ttu-id="89ff9-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="89ff9-120">Header</span></span>|<span data-ttu-id="89ff9-121">値</span><span class="sxs-lookup"><span data-stu-id="89ff9-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="89ff9-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="89ff9-122">Authorization</span></span>|<span data-ttu-id="89ff9-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="89ff9-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="89ff9-124">承諾</span><span class="sxs-lookup"><span data-stu-id="89ff9-124">Accept</span></span>|<span data-ttu-id="89ff9-125">application/json</span><span class="sxs-lookup"><span data-stu-id="89ff9-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="89ff9-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="89ff9-126">Request body</span></span>
<span data-ttu-id="89ff9-127">要求本文で、 [deviceManagementIntentDeviceStateSummary](../resources/intune-deviceintent-devicemanagementintentdevicestatesummary.md)オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="89ff9-127">In the request body, supply a JSON representation for the [deviceManagementIntentDeviceStateSummary](../resources/intune-deviceintent-devicemanagementintentdevicestatesummary.md) object.</span></span>

<span data-ttu-id="89ff9-128">次の表に、 [deviceManagementIntentDeviceStateSummary](../resources/intune-deviceintent-devicemanagementintentdevicestatesummary.md)の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="89ff9-128">The following table shows the properties that are required when you create the [deviceManagementIntentDeviceStateSummary](../resources/intune-deviceintent-devicemanagementintentdevicestatesummary.md).</span></span>

|<span data-ttu-id="89ff9-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="89ff9-129">Property</span></span>|<span data-ttu-id="89ff9-130">型</span><span class="sxs-lookup"><span data-stu-id="89ff9-130">Type</span></span>|<span data-ttu-id="89ff9-131">説明</span><span class="sxs-lookup"><span data-stu-id="89ff9-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="89ff9-132">id</span><span class="sxs-lookup"><span data-stu-id="89ff9-132">id</span></span>|<span data-ttu-id="89ff9-133">String</span><span class="sxs-lookup"><span data-stu-id="89ff9-133">String</span></span>|<span data-ttu-id="89ff9-134">ID</span><span class="sxs-lookup"><span data-stu-id="89ff9-134">The ID</span></span>|
|<span data-ttu-id="89ff9-135">conflictCount</span><span class="sxs-lookup"><span data-stu-id="89ff9-135">conflictCount</span></span>|<span data-ttu-id="89ff9-136">Int32</span><span class="sxs-lookup"><span data-stu-id="89ff9-136">Int32</span></span>|<span data-ttu-id="89ff9-137">競合しているデバイスの数</span><span class="sxs-lookup"><span data-stu-id="89ff9-137">Number of devices in conflict</span></span>|
|<span data-ttu-id="89ff9-138">errorCount</span><span class="sxs-lookup"><span data-stu-id="89ff9-138">errorCount</span></span>|<span data-ttu-id="89ff9-139">Int32</span><span class="sxs-lookup"><span data-stu-id="89ff9-139">Int32</span></span>|<span data-ttu-id="89ff9-140">エラー デバイスの数</span><span class="sxs-lookup"><span data-stu-id="89ff9-140">Number of error devices</span></span>|
|<span data-ttu-id="89ff9-141">failedCount</span><span class="sxs-lookup"><span data-stu-id="89ff9-141">failedCount</span></span>|<span data-ttu-id="89ff9-142">Int32</span><span class="sxs-lookup"><span data-stu-id="89ff9-142">Int32</span></span>|<span data-ttu-id="89ff9-143">失敗したデバイスの数</span><span class="sxs-lookup"><span data-stu-id="89ff9-143">Number of failed devices</span></span>|
|<span data-ttu-id="89ff9-144">notApplicableCount</span><span class="sxs-lookup"><span data-stu-id="89ff9-144">notApplicableCount</span></span>|<span data-ttu-id="89ff9-145">Int32</span><span class="sxs-lookup"><span data-stu-id="89ff9-145">Int32</span></span>|<span data-ttu-id="89ff9-146">該当しないデバイスの数</span><span class="sxs-lookup"><span data-stu-id="89ff9-146">Number of not applicable devices</span></span>|
|<span data-ttu-id="89ff9-147">notApplicablePlatformCount</span><span class="sxs-lookup"><span data-stu-id="89ff9-147">notApplicablePlatformCount</span></span>|<span data-ttu-id="89ff9-148">Int32</span><span class="sxs-lookup"><span data-stu-id="89ff9-148">Int32</span></span>|<span data-ttu-id="89ff9-149">プラットフォームとポリシーの不一致が原因で適用されていないデバイスの数</span><span class="sxs-lookup"><span data-stu-id="89ff9-149">Number of not applicable devices due to mismatch platform and policy</span></span>|
|<span data-ttu-id="89ff9-150">successCount</span><span class="sxs-lookup"><span data-stu-id="89ff9-150">successCount</span></span>|<span data-ttu-id="89ff9-151">Int32</span><span class="sxs-lookup"><span data-stu-id="89ff9-151">Int32</span></span>|<span data-ttu-id="89ff9-152">成功したデバイスの数</span><span class="sxs-lookup"><span data-stu-id="89ff9-152">Number of succeeded devices</span></span>|



## <a name="response"></a><span data-ttu-id="89ff9-153">応答</span><span class="sxs-lookup"><span data-stu-id="89ff9-153">Response</span></span>
<span data-ttu-id="89ff9-154">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で更新された[deviceManagementIntentDeviceStateSummary](../resources/intune-deviceintent-devicemanagementintentdevicestatesummary.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="89ff9-154">If successful, this method returns a `200 OK` response code and an updated [deviceManagementIntentDeviceStateSummary](../resources/intune-deviceintent-devicemanagementintentdevicestatesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="89ff9-155">例</span><span class="sxs-lookup"><span data-stu-id="89ff9-155">Example</span></span>

### <a name="request"></a><span data-ttu-id="89ff9-156">要求</span><span class="sxs-lookup"><span data-stu-id="89ff9-156">Request</span></span>
<span data-ttu-id="89ff9-157">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="89ff9-157">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="89ff9-158">応答</span><span class="sxs-lookup"><span data-stu-id="89ff9-158">Response</span></span>
<span data-ttu-id="89ff9-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="89ff9-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





