---
title: deviceConfigurationDeviceStateSummary の更新
description: deviceConfigurationDeviceStateSummary オブジェクトのプロパティを更新します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: add8609cf9ce7a8f791e350626a3accee8d74b5b
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36017526"
---
# <a name="update-deviceconfigurationdevicestatesummary"></a><span data-ttu-id="aca70-103">deviceConfigurationDeviceStateSummary の更新</span><span class="sxs-lookup"><span data-stu-id="aca70-103">Update deviceConfigurationDeviceStateSummary</span></span>

> <span data-ttu-id="aca70-104">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="aca70-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="aca70-105">[deviceConfigurationDeviceStateSummary](../resources/intune-deviceconfig-deviceconfigurationdevicestatesummary.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="aca70-105">Update the properties of a [deviceConfigurationDeviceStateSummary](../resources/intune-deviceconfig-deviceconfigurationdevicestatesummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="aca70-106">前提条件</span><span class="sxs-lookup"><span data-stu-id="aca70-106">Prerequisites</span></span>
<span data-ttu-id="aca70-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="aca70-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="aca70-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="aca70-109">Permission type</span></span>|<span data-ttu-id="aca70-110">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="aca70-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="aca70-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="aca70-111">Delegated (work or school account)</span></span>|<span data-ttu-id="aca70-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="aca70-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="aca70-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="aca70-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="aca70-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="aca70-114">Not supported.</span></span>|
|<span data-ttu-id="aca70-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="aca70-115">Application</span></span>|<span data-ttu-id="aca70-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="aca70-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="aca70-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="aca70-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurationDeviceStateSummaries
```

## <a name="request-headers"></a><span data-ttu-id="aca70-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="aca70-118">Request headers</span></span>
|<span data-ttu-id="aca70-119">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="aca70-119">Header</span></span>|<span data-ttu-id="aca70-120">値</span><span class="sxs-lookup"><span data-stu-id="aca70-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="aca70-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="aca70-121">Authorization</span></span>|<span data-ttu-id="aca70-122">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="aca70-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="aca70-123">承諾</span><span class="sxs-lookup"><span data-stu-id="aca70-123">Accept</span></span>|<span data-ttu-id="aca70-124">application/json</span><span class="sxs-lookup"><span data-stu-id="aca70-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="aca70-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="aca70-125">Request body</span></span>
<span data-ttu-id="aca70-126">要求本文で、[deviceConfigurationDeviceStateSummary](../resources/intune-deviceconfig-deviceconfigurationdevicestatesummary.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="aca70-126">In the request body, supply a JSON representation for the [deviceConfigurationDeviceStateSummary](../resources/intune-deviceconfig-deviceconfigurationdevicestatesummary.md) object.</span></span>

<span data-ttu-id="aca70-127">次の表に、[deviceConfigurationDeviceStateSummary](../resources/intune-deviceconfig-deviceconfigurationdevicestatesummary.md) の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="aca70-127">The following table shows the properties that are required when you create the [deviceConfigurationDeviceStateSummary](../resources/intune-deviceconfig-deviceconfigurationdevicestatesummary.md).</span></span>

|<span data-ttu-id="aca70-128">プロパティ</span><span class="sxs-lookup"><span data-stu-id="aca70-128">Property</span></span>|<span data-ttu-id="aca70-129">型</span><span class="sxs-lookup"><span data-stu-id="aca70-129">Type</span></span>|<span data-ttu-id="aca70-130">説明</span><span class="sxs-lookup"><span data-stu-id="aca70-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="aca70-131">id</span><span class="sxs-lookup"><span data-stu-id="aca70-131">id</span></span>|<span data-ttu-id="aca70-132">String</span><span class="sxs-lookup"><span data-stu-id="aca70-132">String</span></span>|<span data-ttu-id="aca70-133">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="aca70-133">Key of the entity.</span></span>|
|<span data-ttu-id="aca70-134">unknownDeviceCount</span><span class="sxs-lookup"><span data-stu-id="aca70-134">unknownDeviceCount</span></span>|<span data-ttu-id="aca70-135">Int32</span><span class="sxs-lookup"><span data-stu-id="aca70-135">Int32</span></span>|<span data-ttu-id="aca70-136">不明なデバイスの数</span><span class="sxs-lookup"><span data-stu-id="aca70-136">Number of unknown devices</span></span>|
|<span data-ttu-id="aca70-137">notApplicableDeviceCount</span><span class="sxs-lookup"><span data-stu-id="aca70-137">notApplicableDeviceCount</span></span>|<span data-ttu-id="aca70-138">Int32</span><span class="sxs-lookup"><span data-stu-id="aca70-138">Int32</span></span>|<span data-ttu-id="aca70-139">該当しないデバイスの数</span><span class="sxs-lookup"><span data-stu-id="aca70-139">Number of not applicable devices</span></span>|
|<span data-ttu-id="aca70-140">compliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="aca70-140">compliantDeviceCount</span></span>|<span data-ttu-id="aca70-141">Int32</span><span class="sxs-lookup"><span data-stu-id="aca70-141">Int32</span></span>|<span data-ttu-id="aca70-142">準拠デバイスの数</span><span class="sxs-lookup"><span data-stu-id="aca70-142">Number of compliant devices</span></span>|
|<span data-ttu-id="aca70-143">remediatedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="aca70-143">remediatedDeviceCount</span></span>|<span data-ttu-id="aca70-144">Int32</span><span class="sxs-lookup"><span data-stu-id="aca70-144">Int32</span></span>|<span data-ttu-id="aca70-145">修復済みデバイスの数</span><span class="sxs-lookup"><span data-stu-id="aca70-145">Number of remediated devices</span></span>|
|<span data-ttu-id="aca70-146">nonCompliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="aca70-146">nonCompliantDeviceCount</span></span>|<span data-ttu-id="aca70-147">Int32</span><span class="sxs-lookup"><span data-stu-id="aca70-147">Int32</span></span>|<span data-ttu-id="aca70-148">準拠していないデバイスの数</span><span class="sxs-lookup"><span data-stu-id="aca70-148">Number of NonCompliant devices</span></span>|
|<span data-ttu-id="aca70-149">errorDeviceCount</span><span class="sxs-lookup"><span data-stu-id="aca70-149">errorDeviceCount</span></span>|<span data-ttu-id="aca70-150">Int32</span><span class="sxs-lookup"><span data-stu-id="aca70-150">Int32</span></span>|<span data-ttu-id="aca70-151">エラー デバイスの数</span><span class="sxs-lookup"><span data-stu-id="aca70-151">Number of error devices</span></span>|
|<span data-ttu-id="aca70-152">conflictDeviceCount</span><span class="sxs-lookup"><span data-stu-id="aca70-152">conflictDeviceCount</span></span>|<span data-ttu-id="aca70-153">Int32</span><span class="sxs-lookup"><span data-stu-id="aca70-153">Int32</span></span>|<span data-ttu-id="aca70-154">競合デバイスの数</span><span class="sxs-lookup"><span data-stu-id="aca70-154">Number of conflict devices</span></span>|



## <a name="response"></a><span data-ttu-id="aca70-155">応答</span><span class="sxs-lookup"><span data-stu-id="aca70-155">Response</span></span>
<span data-ttu-id="aca70-156">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で更新された [deviceConfigurationDeviceStateSummary](../resources/intune-deviceconfig-deviceconfigurationdevicestatesummary.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="aca70-156">If successful, this method returns a `200 OK` response code and an updated [deviceConfigurationDeviceStateSummary](../resources/intune-deviceconfig-deviceconfigurationdevicestatesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="aca70-157">例</span><span class="sxs-lookup"><span data-stu-id="aca70-157">Example</span></span>

### <a name="request"></a><span data-ttu-id="aca70-158">要求</span><span class="sxs-lookup"><span data-stu-id="aca70-158">Request</span></span>
<span data-ttu-id="aca70-159">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="aca70-159">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurationDeviceStateSummaries
Content-type: application/json
Content-length: 290

{
  "@odata.type": "#microsoft.graph.deviceConfigurationDeviceStateSummary",
  "unknownDeviceCount": 2,
  "notApplicableDeviceCount": 8,
  "compliantDeviceCount": 4,
  "remediatedDeviceCount": 5,
  "nonCompliantDeviceCount": 7,
  "errorDeviceCount": 0,
  "conflictDeviceCount": 3
}
```

### <a name="response"></a><span data-ttu-id="aca70-160">応答</span><span class="sxs-lookup"><span data-stu-id="aca70-160">Response</span></span>
<span data-ttu-id="aca70-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="aca70-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 339

{
  "@odata.type": "#microsoft.graph.deviceConfigurationDeviceStateSummary",
  "id": "5db26f5a-6f5a-5db2-5a6f-b25d5a6fb25d",
  "unknownDeviceCount": 2,
  "notApplicableDeviceCount": 8,
  "compliantDeviceCount": 4,
  "remediatedDeviceCount": 5,
  "nonCompliantDeviceCount": 7,
  "errorDeviceCount": 0,
  "conflictDeviceCount": 3
}
```



