---
title: deviceConfigurationDeviceStateSummary の更新
description: deviceConfigurationDeviceStateSummary オブジェクトのプロパティを更新します。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 1963e00e5f2cf6719932b1b26b388a72fff0fb28
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27832532"
---
# <a name="update-deviceconfigurationdevicestatesummary"></a><span data-ttu-id="ee123-103">deviceConfigurationDeviceStateSummary の更新</span><span class="sxs-lookup"><span data-stu-id="ee123-103">Update deviceConfigurationDeviceStateSummary</span></span>

> <span data-ttu-id="ee123-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="ee123-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ee123-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ee123-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="ee123-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="ee123-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="ee123-107">[deviceConfigurationDeviceStateSummary](../resources/intune-deviceconfig-deviceconfigurationdevicestatesummary.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="ee123-107">Update the properties of a [deviceConfigurationDeviceStateSummary](../resources/intune-deviceconfig-deviceconfigurationdevicestatesummary.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="ee123-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="ee123-108">Prerequisites</span></span>
<span data-ttu-id="ee123-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="ee123-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ee123-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="ee123-111">Permission type</span></span>|<span data-ttu-id="ee123-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="ee123-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ee123-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="ee123-113">Delegated (work or school account)</span></span>|<span data-ttu-id="ee123-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ee123-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="ee123-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="ee123-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ee123-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ee123-116">Not supported.</span></span>|
|<span data-ttu-id="ee123-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="ee123-117">Application</span></span>|<span data-ttu-id="ee123-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ee123-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ee123-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="ee123-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurationDeviceStateSummaries
```

## <a name="request-headers"></a><span data-ttu-id="ee123-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="ee123-120">Request headers</span></span>
|<span data-ttu-id="ee123-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="ee123-121">Header</span></span>|<span data-ttu-id="ee123-122">値</span><span class="sxs-lookup"><span data-stu-id="ee123-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ee123-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="ee123-123">Authorization</span></span>|<span data-ttu-id="ee123-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="ee123-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ee123-125">Accept</span><span class="sxs-lookup"><span data-stu-id="ee123-125">Accept</span></span>|<span data-ttu-id="ee123-126">application/json</span><span class="sxs-lookup"><span data-stu-id="ee123-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ee123-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="ee123-127">Request body</span></span>
<span data-ttu-id="ee123-128">要求本文で、[deviceConfigurationDeviceStateSummary](../resources/intune-deviceconfig-deviceconfigurationdevicestatesummary.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="ee123-128">In the request body, supply a JSON representation for the [deviceConfigurationDeviceStateSummary](../resources/intune-deviceconfig-deviceconfigurationdevicestatesummary.md) object.</span></span>

<span data-ttu-id="ee123-129">次の表に、[deviceConfigurationDeviceStateSummary](../resources/intune-deviceconfig-deviceconfigurationdevicestatesummary.md) の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="ee123-129">The following table shows the properties that are required when you create the [deviceConfigurationDeviceStateSummary](../resources/intune-deviceconfig-deviceconfigurationdevicestatesummary.md).</span></span>

|<span data-ttu-id="ee123-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="ee123-130">Property</span></span>|<span data-ttu-id="ee123-131">種類</span><span class="sxs-lookup"><span data-stu-id="ee123-131">Type</span></span>|<span data-ttu-id="ee123-132">説明</span><span class="sxs-lookup"><span data-stu-id="ee123-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ee123-133">ID</span><span class="sxs-lookup"><span data-stu-id="ee123-133">id</span></span>|<span data-ttu-id="ee123-134">String</span><span class="sxs-lookup"><span data-stu-id="ee123-134">String</span></span>|<span data-ttu-id="ee123-135">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="ee123-135">Key of the entity.</span></span>|
|<span data-ttu-id="ee123-136">unknownDeviceCount</span><span class="sxs-lookup"><span data-stu-id="ee123-136">unknownDeviceCount</span></span>|<span data-ttu-id="ee123-137">Int32</span><span class="sxs-lookup"><span data-stu-id="ee123-137">Int32</span></span>|<span data-ttu-id="ee123-138">不明なデバイスの数</span><span class="sxs-lookup"><span data-stu-id="ee123-138">Number of unknown devices</span></span>|
|<span data-ttu-id="ee123-139">notApplicableDeviceCount</span><span class="sxs-lookup"><span data-stu-id="ee123-139">notApplicableDeviceCount</span></span>|<span data-ttu-id="ee123-140">Int32</span><span class="sxs-lookup"><span data-stu-id="ee123-140">Int32</span></span>|<span data-ttu-id="ee123-141">該当しないデバイスの数</span><span class="sxs-lookup"><span data-stu-id="ee123-141">Number of not applicable devices</span></span>|
|<span data-ttu-id="ee123-142">compliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="ee123-142">compliantDeviceCount</span></span>|<span data-ttu-id="ee123-143">Int32</span><span class="sxs-lookup"><span data-stu-id="ee123-143">Int32</span></span>|<span data-ttu-id="ee123-144">準拠デバイスの数</span><span class="sxs-lookup"><span data-stu-id="ee123-144">Number of compliant devices</span></span>|
|<span data-ttu-id="ee123-145">remediatedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="ee123-145">remediatedDeviceCount</span></span>|<span data-ttu-id="ee123-146">Int32</span><span class="sxs-lookup"><span data-stu-id="ee123-146">Int32</span></span>|<span data-ttu-id="ee123-147">修復済みデバイスの数</span><span class="sxs-lookup"><span data-stu-id="ee123-147">Number of remediated devices</span></span>|
|<span data-ttu-id="ee123-148">nonCompliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="ee123-148">nonCompliantDeviceCount</span></span>|<span data-ttu-id="ee123-149">Int32</span><span class="sxs-lookup"><span data-stu-id="ee123-149">Int32</span></span>|<span data-ttu-id="ee123-150">準拠していないデバイスの数</span><span class="sxs-lookup"><span data-stu-id="ee123-150">Number of NonCompliant devices</span></span>|
|<span data-ttu-id="ee123-151">errorDeviceCount</span><span class="sxs-lookup"><span data-stu-id="ee123-151">errorDeviceCount</span></span>|<span data-ttu-id="ee123-152">Int32</span><span class="sxs-lookup"><span data-stu-id="ee123-152">Int32</span></span>|<span data-ttu-id="ee123-153">エラー デバイスの数</span><span class="sxs-lookup"><span data-stu-id="ee123-153">Number of error devices</span></span>|
|<span data-ttu-id="ee123-154">conflictDeviceCount</span><span class="sxs-lookup"><span data-stu-id="ee123-154">conflictDeviceCount</span></span>|<span data-ttu-id="ee123-155">Int32</span><span class="sxs-lookup"><span data-stu-id="ee123-155">Int32</span></span>|<span data-ttu-id="ee123-156">競合デバイスの数</span><span class="sxs-lookup"><span data-stu-id="ee123-156">Number of conflict devices</span></span>|



## <a name="response"></a><span data-ttu-id="ee123-157">応答</span><span class="sxs-lookup"><span data-stu-id="ee123-157">Response</span></span>
<span data-ttu-id="ee123-158">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で更新された [deviceConfigurationDeviceStateSummary](../resources/intune-deviceconfig-deviceconfigurationdevicestatesummary.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="ee123-158">If successful, this method returns a `200 OK` response code and an updated [deviceConfigurationDeviceStateSummary](../resources/intune-deviceconfig-deviceconfigurationdevicestatesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ee123-159">例</span><span class="sxs-lookup"><span data-stu-id="ee123-159">Example</span></span>
### <a name="request"></a><span data-ttu-id="ee123-160">要求</span><span class="sxs-lookup"><span data-stu-id="ee123-160">Request</span></span>
<span data-ttu-id="ee123-161">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="ee123-161">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="ee123-162">応答</span><span class="sxs-lookup"><span data-stu-id="ee123-162">Response</span></span>
<span data-ttu-id="ee123-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="ee123-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





