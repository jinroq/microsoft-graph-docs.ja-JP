---
title: DeviceManagementScriptRunSummary を更新します。
description: DeviceManagementScriptRunSummary オブジェクトのプロパティを更新します。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: c7a82b01ccae7e3f5ca1e8c3b3b784791fe08df3
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27858325"
---
# <a name="update-devicemanagementscriptrunsummary"></a><span data-ttu-id="af0f8-103">DeviceManagementScriptRunSummary を更新します。</span><span class="sxs-lookup"><span data-stu-id="af0f8-103">Update deviceManagementScriptRunSummary</span></span>

> <span data-ttu-id="af0f8-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="af0f8-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="af0f8-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="af0f8-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="af0f8-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="af0f8-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="af0f8-107">[DeviceManagementScriptRunSummary](../resources/intune-devices-devicemanagementscriptrunsummary.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="af0f8-107">Update the properties of a [deviceManagementScriptRunSummary](../resources/intune-devices-devicemanagementscriptrunsummary.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="af0f8-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="af0f8-108">Prerequisites</span></span>
<span data-ttu-id="af0f8-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="af0f8-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="af0f8-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="af0f8-111">Permission type</span></span>|<span data-ttu-id="af0f8-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="af0f8-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="af0f8-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="af0f8-113">Delegated (work or school account)</span></span>|<span data-ttu-id="af0f8-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="af0f8-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="af0f8-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="af0f8-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="af0f8-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="af0f8-116">Not supported.</span></span>|
|<span data-ttu-id="af0f8-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="af0f8-117">Application</span></span>|<span data-ttu-id="af0f8-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="af0f8-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="af0f8-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="af0f8-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/runSummary
```

## <a name="request-headers"></a><span data-ttu-id="af0f8-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="af0f8-120">Request headers</span></span>
|<span data-ttu-id="af0f8-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="af0f8-121">Header</span></span>|<span data-ttu-id="af0f8-122">値</span><span class="sxs-lookup"><span data-stu-id="af0f8-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="af0f8-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="af0f8-123">Authorization</span></span>|<span data-ttu-id="af0f8-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="af0f8-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="af0f8-125">Accept</span><span class="sxs-lookup"><span data-stu-id="af0f8-125">Accept</span></span>|<span data-ttu-id="af0f8-126">application/json</span><span class="sxs-lookup"><span data-stu-id="af0f8-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="af0f8-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="af0f8-127">Request body</span></span>
<span data-ttu-id="af0f8-128">要求の本文に[deviceManagementScriptRunSummary](../resources/intune-devices-devicemanagementscriptrunsummary.md)オブジェクトの JSON の形式を指定します。</span><span class="sxs-lookup"><span data-stu-id="af0f8-128">In the request body, supply a JSON representation for the [deviceManagementScriptRunSummary](../resources/intune-devices-devicemanagementscriptrunsummary.md) object.</span></span>

<span data-ttu-id="af0f8-129">[DeviceManagementScriptRunSummary](../resources/intune-devices-devicemanagementscriptrunsummary.md)を作成するときに必要なプロパティを次の表に示します。</span><span class="sxs-lookup"><span data-stu-id="af0f8-129">The following table shows the properties that are required when you create the [deviceManagementScriptRunSummary](../resources/intune-devices-devicemanagementscriptrunsummary.md).</span></span>

|<span data-ttu-id="af0f8-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="af0f8-130">Property</span></span>|<span data-ttu-id="af0f8-131">種類</span><span class="sxs-lookup"><span data-stu-id="af0f8-131">Type</span></span>|<span data-ttu-id="af0f8-132">説明</span><span class="sxs-lookup"><span data-stu-id="af0f8-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="af0f8-133">ID</span><span class="sxs-lookup"><span data-stu-id="af0f8-133">id</span></span>|<span data-ttu-id="af0f8-134">String</span><span class="sxs-lookup"><span data-stu-id="af0f8-134">String</span></span>|<span data-ttu-id="af0f8-135">デバイス管理スクリプトのキーは、エンティティの概要を実行します。</span><span class="sxs-lookup"><span data-stu-id="af0f8-135">Key of the device management script run summary entity.</span></span>|
|<span data-ttu-id="af0f8-136">successDeviceCount</span><span class="sxs-lookup"><span data-stu-id="af0f8-136">successDeviceCount</span></span>|<span data-ttu-id="af0f8-137">Int32</span><span class="sxs-lookup"><span data-stu-id="af0f8-137">Int32</span></span>|<span data-ttu-id="af0f8-138">成功した場合のデバイスの数。</span><span class="sxs-lookup"><span data-stu-id="af0f8-138">Success device count.</span></span>|
|<span data-ttu-id="af0f8-139">errorDeviceCount</span><span class="sxs-lookup"><span data-stu-id="af0f8-139">errorDeviceCount</span></span>|<span data-ttu-id="af0f8-140">Int32</span><span class="sxs-lookup"><span data-stu-id="af0f8-140">Int32</span></span>|<span data-ttu-id="af0f8-141">デバイスのエラーの数です。</span><span class="sxs-lookup"><span data-stu-id="af0f8-141">Error device count.</span></span>|
|<span data-ttu-id="af0f8-142">successUserCount</span><span class="sxs-lookup"><span data-stu-id="af0f8-142">successUserCount</span></span>|<span data-ttu-id="af0f8-143">Int32</span><span class="sxs-lookup"><span data-stu-id="af0f8-143">Int32</span></span>|<span data-ttu-id="af0f8-144">成功ユーザー カウントです。</span><span class="sxs-lookup"><span data-stu-id="af0f8-144">Success user count.</span></span>|
|<span data-ttu-id="af0f8-145">errorUserCount</span><span class="sxs-lookup"><span data-stu-id="af0f8-145">errorUserCount</span></span>|<span data-ttu-id="af0f8-146">Int32</span><span class="sxs-lookup"><span data-stu-id="af0f8-146">Int32</span></span>|<span data-ttu-id="af0f8-147">ユーザーのエラーの数です。</span><span class="sxs-lookup"><span data-stu-id="af0f8-147">Error user count.</span></span>|



## <a name="response"></a><span data-ttu-id="af0f8-148">応答</span><span class="sxs-lookup"><span data-stu-id="af0f8-148">Response</span></span>
<span data-ttu-id="af0f8-149">かどうかは成功すると、このメソッドが返されます、`200 OK`応答コードおよび応答の本文に更新された[deviceManagementScriptRunSummary](../resources/intune-devices-devicemanagementscriptrunsummary.md)オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="af0f8-149">If successful, this method returns a `200 OK` response code and an updated [deviceManagementScriptRunSummary](../resources/intune-devices-devicemanagementscriptrunsummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="af0f8-150">例</span><span class="sxs-lookup"><span data-stu-id="af0f8-150">Example</span></span>
### <a name="request"></a><span data-ttu-id="af0f8-151">要求</span><span class="sxs-lookup"><span data-stu-id="af0f8-151">Request</span></span>
<span data-ttu-id="af0f8-152">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="af0f8-152">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/runSummary
Content-type: application/json
Content-length: 108

{
  "successDeviceCount": 2,
  "errorDeviceCount": 0,
  "successUserCount": 0,
  "errorUserCount": 14
}
```

### <a name="response"></a><span data-ttu-id="af0f8-153">応答</span><span class="sxs-lookup"><span data-stu-id="af0f8-153">Response</span></span>
<span data-ttu-id="af0f8-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="af0f8-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 228

{
  "@odata.type": "#microsoft.graph.deviceManagementScriptRunSummary",
  "id": "514d5d38-5d38-514d-385d-4d51385d4d51",
  "successDeviceCount": 2,
  "errorDeviceCount": 0,
  "successUserCount": 0,
  "errorUserCount": 14
}
```





