---
title: deviceConfigurationDeviceOverview の更新
description: deviceConfigurationDeviceOverview オブジェクトのプロパティを更新します。
ms.openlocfilehash: 7eecc3e7871ae1ec8891c5f3f8c7dfde9d517c00
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27022275"
---
# <a name="update-deviceconfigurationdeviceoverview"></a><span data-ttu-id="cc264-103">deviceConfigurationDeviceOverview の更新</span><span class="sxs-lookup"><span data-stu-id="cc264-103">Update deviceConfigurationDeviceOverview</span></span>

> <span data-ttu-id="cc264-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="cc264-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="cc264-105">[deviceConfigurationDeviceOverview](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="cc264-105">Update the properties of a [deviceConfigurationDeviceOverview](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="cc264-106">前提条件</span><span class="sxs-lookup"><span data-stu-id="cc264-106">Prerequisites</span></span>
<span data-ttu-id="cc264-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="cc264-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cc264-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="cc264-109">Permission type</span></span>|<span data-ttu-id="cc264-110">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="cc264-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="cc264-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="cc264-111">Delegated (work or school account)</span></span>|<span data-ttu-id="cc264-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cc264-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="cc264-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="cc264-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="cc264-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="cc264-114">Not supported.</span></span>|
|<span data-ttu-id="cc264-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="cc264-115">Application</span></span>|<span data-ttu-id="cc264-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="cc264-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="cc264-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="cc264-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/deviceStatusOverview
```

## <a name="request-headers"></a><span data-ttu-id="cc264-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="cc264-118">Request headers</span></span>
|<span data-ttu-id="cc264-119">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="cc264-119">Header</span></span>|<span data-ttu-id="cc264-120">値</span><span class="sxs-lookup"><span data-stu-id="cc264-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="cc264-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="cc264-121">Authorization</span></span>|<span data-ttu-id="cc264-122">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="cc264-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="cc264-123">Accept</span><span class="sxs-lookup"><span data-stu-id="cc264-123">Accept</span></span>|<span data-ttu-id="cc264-124">application/json</span><span class="sxs-lookup"><span data-stu-id="cc264-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="cc264-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="cc264-125">Request body</span></span>
<span data-ttu-id="cc264-126">要求本文で、[deviceConfigurationDeviceOverview](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="cc264-126">In the request body, supply a JSON representation for the [deviceConfigurationDeviceOverview](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md) object.</span></span>

<span data-ttu-id="cc264-127">次の表に、[deviceConfigurationDeviceOverview](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md) の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="cc264-127">The following table shows the properties that are required when you create the [deviceConfigurationDeviceOverview](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md).</span></span>

|<span data-ttu-id="cc264-128">プロパティ</span><span class="sxs-lookup"><span data-stu-id="cc264-128">Property</span></span>|<span data-ttu-id="cc264-129">型</span><span class="sxs-lookup"><span data-stu-id="cc264-129">Type</span></span>|<span data-ttu-id="cc264-130">説明</span><span class="sxs-lookup"><span data-stu-id="cc264-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cc264-131">id</span><span class="sxs-lookup"><span data-stu-id="cc264-131">id</span></span>|<span data-ttu-id="cc264-132">String</span><span class="sxs-lookup"><span data-stu-id="cc264-132">String</span></span>|<span data-ttu-id="cc264-133">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="cc264-133">Key of the entity.</span></span>|
|<span data-ttu-id="cc264-134">pendingCount</span><span class="sxs-lookup"><span data-stu-id="cc264-134">pendingCount</span></span>|<span data-ttu-id="cc264-135">Int32</span><span class="sxs-lookup"><span data-stu-id="cc264-135">Int32</span></span>|<span data-ttu-id="cc264-136">保留中のデバイスの数</span><span class="sxs-lookup"><span data-stu-id="cc264-136">Number of pending devices</span></span>|
|<span data-ttu-id="cc264-137">notApplicableCount</span><span class="sxs-lookup"><span data-stu-id="cc264-137">notApplicableCount</span></span>|<span data-ttu-id="cc264-138">Int32</span><span class="sxs-lookup"><span data-stu-id="cc264-138">Int32</span></span>|<span data-ttu-id="cc264-139">該当しないデバイスの数</span><span class="sxs-lookup"><span data-stu-id="cc264-139">Number of not applicable devices</span></span>|
|<span data-ttu-id="cc264-140">successCount</span><span class="sxs-lookup"><span data-stu-id="cc264-140">successCount</span></span>|<span data-ttu-id="cc264-141">Int32</span><span class="sxs-lookup"><span data-stu-id="cc264-141">Int32</span></span>|<span data-ttu-id="cc264-142">成功したデバイスの数</span><span class="sxs-lookup"><span data-stu-id="cc264-142">Number of succeeded devices</span></span>|
|<span data-ttu-id="cc264-143">errorCount</span><span class="sxs-lookup"><span data-stu-id="cc264-143">errorCount</span></span>|<span data-ttu-id="cc264-144">Int32</span><span class="sxs-lookup"><span data-stu-id="cc264-144">Int32</span></span>|<span data-ttu-id="cc264-145">エラー デバイスの数</span><span class="sxs-lookup"><span data-stu-id="cc264-145">Number of error devices</span></span>|
|<span data-ttu-id="cc264-146">failedCount</span><span class="sxs-lookup"><span data-stu-id="cc264-146">failedCount</span></span>|<span data-ttu-id="cc264-147">Int32</span><span class="sxs-lookup"><span data-stu-id="cc264-147">Int32</span></span>|<span data-ttu-id="cc264-148">失敗したデバイスの数</span><span class="sxs-lookup"><span data-stu-id="cc264-148">Number of failed devices</span></span>|
|<span data-ttu-id="cc264-149">lastUpdateDateTime</span><span class="sxs-lookup"><span data-stu-id="cc264-149">lastUpdateDateTime</span></span>|<span data-ttu-id="cc264-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cc264-150">DateTimeOffset</span></span>|<span data-ttu-id="cc264-151">最終更新時刻</span><span class="sxs-lookup"><span data-stu-id="cc264-151">Last update time</span></span>|
|<span data-ttu-id="cc264-152">configurationVersion</span><span class="sxs-lookup"><span data-stu-id="cc264-152">configurationVersion</span></span>|<span data-ttu-id="cc264-153">Int32</span><span class="sxs-lookup"><span data-stu-id="cc264-153">Int32</span></span>|<span data-ttu-id="cc264-154">対象の概要に関するポリシーのバージョン</span><span class="sxs-lookup"><span data-stu-id="cc264-154">Version of the policy for that overview</span></span>|



## <a name="response"></a><span data-ttu-id="cc264-155">応答</span><span class="sxs-lookup"><span data-stu-id="cc264-155">Response</span></span>
<span data-ttu-id="cc264-156">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で更新された [deviceConfigurationDeviceOverview](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="cc264-156">If successful, this method returns a `200 OK` response code and an updated [deviceConfigurationDeviceOverview](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cc264-157">例</span><span class="sxs-lookup"><span data-stu-id="cc264-157">Example</span></span>
### <a name="request"></a><span data-ttu-id="cc264-158">要求</span><span class="sxs-lookup"><span data-stu-id="cc264-158">Request</span></span>
<span data-ttu-id="cc264-159">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="cc264-159">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}/deviceStatusOverview
Content-type: application/json
Content-length: 284

{
  "@odata.type": "#microsoft.graph.deviceConfigurationDeviceOverview",
  "pendingCount": 12,
  "notApplicableCount": 2,
  "successCount": 12,
  "errorCount": 10,
  "failedCount": 11,
  "lastUpdateDateTime": "2016-12-31T23:58:21.6459442-08:00",
  "configurationVersion": 4
}
```

### <a name="response"></a><span data-ttu-id="cc264-160">応答</span><span class="sxs-lookup"><span data-stu-id="cc264-160">Response</span></span>
<span data-ttu-id="cc264-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="cc264-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 333

{
  "@odata.type": "#microsoft.graph.deviceConfigurationDeviceOverview",
  "id": "62d48e3a-8e3a-62d4-3a8e-d4623a8ed462",
  "pendingCount": 12,
  "notApplicableCount": 2,
  "successCount": 12,
  "errorCount": 10,
  "failedCount": 11,
  "lastUpdateDateTime": "2016-12-31T23:58:21.6459442-08:00",
  "configurationVersion": 4
}
```



