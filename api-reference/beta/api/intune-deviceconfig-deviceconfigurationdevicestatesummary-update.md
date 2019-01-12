---
title: deviceConfigurationDeviceStateSummary の更新
description: deviceConfigurationDeviceStateSummary オブジェクトのプロパティを更新します。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 599411d60bc723e95297926c600359bda3c70fc1
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27924595"
---
# <a name="update-deviceconfigurationdevicestatesummary"></a><span data-ttu-id="8f757-103">deviceConfigurationDeviceStateSummary の更新</span><span class="sxs-lookup"><span data-stu-id="8f757-103">Update deviceConfigurationDeviceStateSummary</span></span>

> <span data-ttu-id="8f757-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="8f757-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="8f757-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="8f757-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="8f757-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="8f757-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="8f757-107">[deviceConfigurationDeviceStateSummary](../resources/intune-deviceconfig-deviceconfigurationdevicestatesummary.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="8f757-107">Update the properties of a [deviceConfigurationDeviceStateSummary](../resources/intune-deviceconfig-deviceconfigurationdevicestatesummary.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="8f757-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="8f757-108">Prerequisites</span></span>
<span data-ttu-id="8f757-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="8f757-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8f757-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="8f757-111">Permission type</span></span>|<span data-ttu-id="8f757-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="8f757-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8f757-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="8f757-113">Delegated (work or school account)</span></span>|<span data-ttu-id="8f757-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8f757-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="8f757-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="8f757-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8f757-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="8f757-116">Not supported.</span></span>|
|<span data-ttu-id="8f757-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="8f757-117">Application</span></span>|<span data-ttu-id="8f757-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="8f757-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="8f757-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="8f757-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurationDeviceStateSummaries
```

## <a name="request-headers"></a><span data-ttu-id="8f757-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="8f757-120">Request headers</span></span>
|<span data-ttu-id="8f757-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="8f757-121">Header</span></span>|<span data-ttu-id="8f757-122">値</span><span class="sxs-lookup"><span data-stu-id="8f757-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8f757-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="8f757-123">Authorization</span></span>|<span data-ttu-id="8f757-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="8f757-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8f757-125">Accept</span><span class="sxs-lookup"><span data-stu-id="8f757-125">Accept</span></span>|<span data-ttu-id="8f757-126">application/json</span><span class="sxs-lookup"><span data-stu-id="8f757-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8f757-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="8f757-127">Request body</span></span>
<span data-ttu-id="8f757-128">要求本文で、[deviceConfigurationDeviceStateSummary](../resources/intune-deviceconfig-deviceconfigurationdevicestatesummary.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="8f757-128">In the request body, supply a JSON representation for the [deviceConfigurationDeviceStateSummary](../resources/intune-deviceconfig-deviceconfigurationdevicestatesummary.md) object.</span></span>

<span data-ttu-id="8f757-129">次の表に、[deviceConfigurationDeviceStateSummary](../resources/intune-deviceconfig-deviceconfigurationdevicestatesummary.md) の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="8f757-129">The following table shows the properties that are required when you create the [deviceConfigurationDeviceStateSummary](../resources/intune-deviceconfig-deviceconfigurationdevicestatesummary.md).</span></span>

|<span data-ttu-id="8f757-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="8f757-130">Property</span></span>|<span data-ttu-id="8f757-131">型</span><span class="sxs-lookup"><span data-stu-id="8f757-131">Type</span></span>|<span data-ttu-id="8f757-132">説明</span><span class="sxs-lookup"><span data-stu-id="8f757-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8f757-133">ID</span><span class="sxs-lookup"><span data-stu-id="8f757-133">id</span></span>|<span data-ttu-id="8f757-134">String</span><span class="sxs-lookup"><span data-stu-id="8f757-134">String</span></span>|<span data-ttu-id="8f757-135">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="8f757-135">Key of the entity.</span></span>|
|<span data-ttu-id="8f757-136">unknownDeviceCount</span><span class="sxs-lookup"><span data-stu-id="8f757-136">unknownDeviceCount</span></span>|<span data-ttu-id="8f757-137">Int32</span><span class="sxs-lookup"><span data-stu-id="8f757-137">Int32</span></span>|<span data-ttu-id="8f757-138">不明なデバイスの数</span><span class="sxs-lookup"><span data-stu-id="8f757-138">Number of unknown devices</span></span>|
|<span data-ttu-id="8f757-139">notApplicableDeviceCount</span><span class="sxs-lookup"><span data-stu-id="8f757-139">notApplicableDeviceCount</span></span>|<span data-ttu-id="8f757-140">Int32</span><span class="sxs-lookup"><span data-stu-id="8f757-140">Int32</span></span>|<span data-ttu-id="8f757-141">該当しないデバイスの数</span><span class="sxs-lookup"><span data-stu-id="8f757-141">Number of not applicable devices</span></span>|
|<span data-ttu-id="8f757-142">compliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="8f757-142">compliantDeviceCount</span></span>|<span data-ttu-id="8f757-143">Int32</span><span class="sxs-lookup"><span data-stu-id="8f757-143">Int32</span></span>|<span data-ttu-id="8f757-144">準拠デバイスの数</span><span class="sxs-lookup"><span data-stu-id="8f757-144">Number of compliant devices</span></span>|
|<span data-ttu-id="8f757-145">remediatedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="8f757-145">remediatedDeviceCount</span></span>|<span data-ttu-id="8f757-146">Int32</span><span class="sxs-lookup"><span data-stu-id="8f757-146">Int32</span></span>|<span data-ttu-id="8f757-147">修復済みデバイスの数</span><span class="sxs-lookup"><span data-stu-id="8f757-147">Number of remediated devices</span></span>|
|<span data-ttu-id="8f757-148">nonCompliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="8f757-148">nonCompliantDeviceCount</span></span>|<span data-ttu-id="8f757-149">Int32</span><span class="sxs-lookup"><span data-stu-id="8f757-149">Int32</span></span>|<span data-ttu-id="8f757-150">準拠していないデバイスの数</span><span class="sxs-lookup"><span data-stu-id="8f757-150">Number of NonCompliant devices</span></span>|
|<span data-ttu-id="8f757-151">errorDeviceCount</span><span class="sxs-lookup"><span data-stu-id="8f757-151">errorDeviceCount</span></span>|<span data-ttu-id="8f757-152">Int32</span><span class="sxs-lookup"><span data-stu-id="8f757-152">Int32</span></span>|<span data-ttu-id="8f757-153">エラー デバイスの数</span><span class="sxs-lookup"><span data-stu-id="8f757-153">Number of error devices</span></span>|
|<span data-ttu-id="8f757-154">conflictDeviceCount</span><span class="sxs-lookup"><span data-stu-id="8f757-154">conflictDeviceCount</span></span>|<span data-ttu-id="8f757-155">Int32</span><span class="sxs-lookup"><span data-stu-id="8f757-155">Int32</span></span>|<span data-ttu-id="8f757-156">競合デバイスの数</span><span class="sxs-lookup"><span data-stu-id="8f757-156">Number of conflict devices</span></span>|



## <a name="response"></a><span data-ttu-id="8f757-157">応答</span><span class="sxs-lookup"><span data-stu-id="8f757-157">Response</span></span>
<span data-ttu-id="8f757-158">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で更新された [deviceConfigurationDeviceStateSummary](../resources/intune-deviceconfig-deviceconfigurationdevicestatesummary.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="8f757-158">If successful, this method returns a `200 OK` response code and an updated [deviceConfigurationDeviceStateSummary](../resources/intune-deviceconfig-deviceconfigurationdevicestatesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8f757-159">例</span><span class="sxs-lookup"><span data-stu-id="8f757-159">Example</span></span>
### <a name="request"></a><span data-ttu-id="8f757-160">要求</span><span class="sxs-lookup"><span data-stu-id="8f757-160">Request</span></span>
<span data-ttu-id="8f757-161">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="8f757-161">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurationDeviceStateSummaries
Content-type: application/json
Content-length: 214

{
  "unknownDeviceCount": 2,
  "notApplicableDeviceCount": 8,
  "compliantDeviceCount": 4,
  "remediatedDeviceCount": 5,
  "nonCompliantDeviceCount": 7,
  "errorDeviceCount": 0,
  "conflictDeviceCount": 3
}
```

### <a name="response"></a><span data-ttu-id="8f757-162">応答</span><span class="sxs-lookup"><span data-stu-id="8f757-162">Response</span></span>
<span data-ttu-id="8f757-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="8f757-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





