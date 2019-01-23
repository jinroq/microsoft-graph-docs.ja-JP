---
title: DeviceManagementScriptRunSummary を更新します。
description: DeviceManagementScriptRunSummary オブジェクトのプロパティを更新します。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 55582147aff81bc8d566634a5fb9fdc1ff4ff2fd
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29413991"
---
# <a name="update-devicemanagementscriptrunsummary"></a><span data-ttu-id="8ff56-103">DeviceManagementScriptRunSummary を更新します。</span><span class="sxs-lookup"><span data-stu-id="8ff56-103">Update deviceManagementScriptRunSummary</span></span>

> <span data-ttu-id="8ff56-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="8ff56-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="8ff56-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="8ff56-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="8ff56-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="8ff56-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8ff56-107">[DeviceManagementScriptRunSummary](../resources/intune-devices-devicemanagementscriptrunsummary.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="8ff56-107">Update the properties of a [deviceManagementScriptRunSummary](../resources/intune-devices-devicemanagementscriptrunsummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="8ff56-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="8ff56-108">Prerequisites</span></span>
<span data-ttu-id="8ff56-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/concepts/permissions-reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="8ff56-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="8ff56-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="8ff56-111">Permission type</span></span>|<span data-ttu-id="8ff56-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="8ff56-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8ff56-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="8ff56-113">Delegated (work or school account)</span></span>|<span data-ttu-id="8ff56-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8ff56-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="8ff56-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="8ff56-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8ff56-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="8ff56-116">Not supported.</span></span>|
|<span data-ttu-id="8ff56-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="8ff56-117">Application</span></span>|<span data-ttu-id="8ff56-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="8ff56-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="8ff56-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="8ff56-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/runSummary
```

## <a name="request-headers"></a><span data-ttu-id="8ff56-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="8ff56-120">Request headers</span></span>
|<span data-ttu-id="8ff56-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="8ff56-121">Header</span></span>|<span data-ttu-id="8ff56-122">値</span><span class="sxs-lookup"><span data-stu-id="8ff56-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8ff56-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="8ff56-123">Authorization</span></span>|<span data-ttu-id="8ff56-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="8ff56-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8ff56-125">Accept</span><span class="sxs-lookup"><span data-stu-id="8ff56-125">Accept</span></span>|<span data-ttu-id="8ff56-126">application/json</span><span class="sxs-lookup"><span data-stu-id="8ff56-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8ff56-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="8ff56-127">Request body</span></span>
<span data-ttu-id="8ff56-128">要求の本文に[deviceManagementScriptRunSummary](../resources/intune-devices-devicemanagementscriptrunsummary.md)オブジェクトの JSON の形式を指定します。</span><span class="sxs-lookup"><span data-stu-id="8ff56-128">In the request body, supply a JSON representation for the [deviceManagementScriptRunSummary](../resources/intune-devices-devicemanagementscriptrunsummary.md) object.</span></span>

<span data-ttu-id="8ff56-129">[DeviceManagementScriptRunSummary](../resources/intune-devices-devicemanagementscriptrunsummary.md)を作成するときに必要なプロパティを次の表に示します。</span><span class="sxs-lookup"><span data-stu-id="8ff56-129">The following table shows the properties that are required when you create the [deviceManagementScriptRunSummary](../resources/intune-devices-devicemanagementscriptrunsummary.md).</span></span>

|<span data-ttu-id="8ff56-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="8ff56-130">Property</span></span>|<span data-ttu-id="8ff56-131">型</span><span class="sxs-lookup"><span data-stu-id="8ff56-131">Type</span></span>|<span data-ttu-id="8ff56-132">説明</span><span class="sxs-lookup"><span data-stu-id="8ff56-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8ff56-133">id</span><span class="sxs-lookup"><span data-stu-id="8ff56-133">id</span></span>|<span data-ttu-id="8ff56-134">String</span><span class="sxs-lookup"><span data-stu-id="8ff56-134">String</span></span>|<span data-ttu-id="8ff56-135">デバイス管理スクリプトのキーは、エンティティの概要を実行します。</span><span class="sxs-lookup"><span data-stu-id="8ff56-135">Key of the device management script run summary entity.</span></span>|
|<span data-ttu-id="8ff56-136">successDeviceCount</span><span class="sxs-lookup"><span data-stu-id="8ff56-136">successDeviceCount</span></span>|<span data-ttu-id="8ff56-137">Int32</span><span class="sxs-lookup"><span data-stu-id="8ff56-137">Int32</span></span>|<span data-ttu-id="8ff56-138">成功した場合のデバイスの数。</span><span class="sxs-lookup"><span data-stu-id="8ff56-138">Success device count.</span></span>|
|<span data-ttu-id="8ff56-139">errorDeviceCount</span><span class="sxs-lookup"><span data-stu-id="8ff56-139">errorDeviceCount</span></span>|<span data-ttu-id="8ff56-140">Int32</span><span class="sxs-lookup"><span data-stu-id="8ff56-140">Int32</span></span>|<span data-ttu-id="8ff56-141">デバイスのエラーの数です。</span><span class="sxs-lookup"><span data-stu-id="8ff56-141">Error device count.</span></span>|
|<span data-ttu-id="8ff56-142">successUserCount</span><span class="sxs-lookup"><span data-stu-id="8ff56-142">successUserCount</span></span>|<span data-ttu-id="8ff56-143">Int32</span><span class="sxs-lookup"><span data-stu-id="8ff56-143">Int32</span></span>|<span data-ttu-id="8ff56-144">成功ユーザー カウントです。</span><span class="sxs-lookup"><span data-stu-id="8ff56-144">Success user count.</span></span>|
|<span data-ttu-id="8ff56-145">errorUserCount</span><span class="sxs-lookup"><span data-stu-id="8ff56-145">errorUserCount</span></span>|<span data-ttu-id="8ff56-146">Int32</span><span class="sxs-lookup"><span data-stu-id="8ff56-146">Int32</span></span>|<span data-ttu-id="8ff56-147">ユーザーのエラーの数です。</span><span class="sxs-lookup"><span data-stu-id="8ff56-147">Error user count.</span></span>|



## <a name="response"></a><span data-ttu-id="8ff56-148">応答</span><span class="sxs-lookup"><span data-stu-id="8ff56-148">Response</span></span>
<span data-ttu-id="8ff56-149">かどうかは成功すると、このメソッドが返されます、`200 OK`応答コードおよび応答の本文に更新された[deviceManagementScriptRunSummary](../resources/intune-devices-devicemanagementscriptrunsummary.md)オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="8ff56-149">If successful, this method returns a `200 OK` response code and an updated [deviceManagementScriptRunSummary](../resources/intune-devices-devicemanagementscriptrunsummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8ff56-150">例</span><span class="sxs-lookup"><span data-stu-id="8ff56-150">Example</span></span>

### <a name="request"></a><span data-ttu-id="8ff56-151">要求</span><span class="sxs-lookup"><span data-stu-id="8ff56-151">Request</span></span>
<span data-ttu-id="8ff56-152">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="8ff56-152">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/runSummary
Content-type: application/json
Content-length: 179

{
  "@odata.type": "#microsoft.graph.deviceManagementScriptRunSummary",
  "successDeviceCount": 2,
  "errorDeviceCount": 0,
  "successUserCount": 0,
  "errorUserCount": 14
}
```

### <a name="response"></a><span data-ttu-id="8ff56-153">応答</span><span class="sxs-lookup"><span data-stu-id="8ff56-153">Response</span></span>
<span data-ttu-id="8ff56-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="8ff56-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




