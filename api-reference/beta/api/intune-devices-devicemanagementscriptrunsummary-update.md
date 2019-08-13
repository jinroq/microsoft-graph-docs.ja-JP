---
title: DeviceManagementScriptRunSummary の更新
description: DeviceManagementScriptRunSummary オブジェクトのプロパティを更新します。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: f07a228ce685ae2ec3fcb502131eac5a6d9271af
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36310291"
---
# <a name="update-devicemanagementscriptrunsummary"></a><span data-ttu-id="1b82e-103">DeviceManagementScriptRunSummary の更新</span><span class="sxs-lookup"><span data-stu-id="1b82e-103">Update deviceManagementScriptRunSummary</span></span>

> <span data-ttu-id="1b82e-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="1b82e-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1b82e-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="1b82e-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1b82e-106">[DeviceManagementScriptRunSummary](../resources/intune-devices-devicemanagementscriptrunsummary.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="1b82e-106">Update the properties of a [deviceManagementScriptRunSummary](../resources/intune-devices-devicemanagementscriptrunsummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="1b82e-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="1b82e-107">Prerequisites</span></span>
<span data-ttu-id="1b82e-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="1b82e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1b82e-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="1b82e-110">Permission type</span></span>|<span data-ttu-id="1b82e-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="1b82e-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1b82e-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="1b82e-112">Delegated (work or school account)</span></span>|<span data-ttu-id="1b82e-113">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1b82e-113">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="1b82e-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="1b82e-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1b82e-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="1b82e-115">Not supported.</span></span>|
|<span data-ttu-id="1b82e-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="1b82e-116">Application</span></span>|<span data-ttu-id="1b82e-117">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1b82e-117">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="1b82e-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="1b82e-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/runSummary
```

## <a name="request-headers"></a><span data-ttu-id="1b82e-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="1b82e-119">Request headers</span></span>
|<span data-ttu-id="1b82e-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="1b82e-120">Header</span></span>|<span data-ttu-id="1b82e-121">値</span><span class="sxs-lookup"><span data-stu-id="1b82e-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1b82e-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="1b82e-122">Authorization</span></span>|<span data-ttu-id="1b82e-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="1b82e-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1b82e-124">承諾</span><span class="sxs-lookup"><span data-stu-id="1b82e-124">Accept</span></span>|<span data-ttu-id="1b82e-125">application/json</span><span class="sxs-lookup"><span data-stu-id="1b82e-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1b82e-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="1b82e-126">Request body</span></span>
<span data-ttu-id="1b82e-127">要求本文で、 [deviceManagementScriptRunSummary](../resources/intune-devices-devicemanagementscriptrunsummary.md)オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="1b82e-127">In the request body, supply a JSON representation for the [deviceManagementScriptRunSummary](../resources/intune-devices-devicemanagementscriptrunsummary.md) object.</span></span>

<span data-ttu-id="1b82e-128">次の表に、 [deviceManagementScriptRunSummary](../resources/intune-devices-devicemanagementscriptrunsummary.md)の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="1b82e-128">The following table shows the properties that are required when you create the [deviceManagementScriptRunSummary](../resources/intune-devices-devicemanagementscriptrunsummary.md).</span></span>

|<span data-ttu-id="1b82e-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="1b82e-129">Property</span></span>|<span data-ttu-id="1b82e-130">型</span><span class="sxs-lookup"><span data-stu-id="1b82e-130">Type</span></span>|<span data-ttu-id="1b82e-131">説明</span><span class="sxs-lookup"><span data-stu-id="1b82e-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1b82e-132">id</span><span class="sxs-lookup"><span data-stu-id="1b82e-132">id</span></span>|<span data-ttu-id="1b82e-133">String</span><span class="sxs-lookup"><span data-stu-id="1b82e-133">String</span></span>|<span data-ttu-id="1b82e-134">デバイス管理スクリプト実行の概要エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="1b82e-134">Key of the device management script run summary entity.</span></span>|
|<span data-ttu-id="1b82e-135">successDeviceCount</span><span class="sxs-lookup"><span data-stu-id="1b82e-135">successDeviceCount</span></span>|<span data-ttu-id="1b82e-136">Int32</span><span class="sxs-lookup"><span data-stu-id="1b82e-136">Int32</span></span>|<span data-ttu-id="1b82e-137">成功したデバイス数。</span><span class="sxs-lookup"><span data-stu-id="1b82e-137">Success device count.</span></span>|
|<span data-ttu-id="1b82e-138">errorDeviceCount</span><span class="sxs-lookup"><span data-stu-id="1b82e-138">errorDeviceCount</span></span>|<span data-ttu-id="1b82e-139">Int32</span><span class="sxs-lookup"><span data-stu-id="1b82e-139">Int32</span></span>|<span data-ttu-id="1b82e-140">エラーデバイス数。</span><span class="sxs-lookup"><span data-stu-id="1b82e-140">Error device count.</span></span>|
|<span data-ttu-id="1b82e-141">compliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="1b82e-141">compliantDeviceCount</span></span>|<span data-ttu-id="1b82e-142">Int32</span><span class="sxs-lookup"><span data-stu-id="1b82e-142">Int32</span></span>|<span data-ttu-id="1b82e-143">準拠しているデバイスの数。</span><span class="sxs-lookup"><span data-stu-id="1b82e-143">Compliant device count.</span></span>|
|<span data-ttu-id="1b82e-144">notCompliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="1b82e-144">notCompliantDeviceCount</span></span>|<span data-ttu-id="1b82e-145">Int32</span><span class="sxs-lookup"><span data-stu-id="1b82e-145">Int32</span></span>|<span data-ttu-id="1b82e-146">準拠していないデバイス数。</span><span class="sxs-lookup"><span data-stu-id="1b82e-146">Not Compliant device count.</span></span>|
|<span data-ttu-id="1b82e-147">pendingDeviceCount</span><span class="sxs-lookup"><span data-stu-id="1b82e-147">pendingDeviceCount</span></span>|<span data-ttu-id="1b82e-148">Int32</span><span class="sxs-lookup"><span data-stu-id="1b82e-148">Int32</span></span>|<span data-ttu-id="1b82e-149">保留中のデバイス数。</span><span class="sxs-lookup"><span data-stu-id="1b82e-149">Pending device count.</span></span>|
|<span data-ttu-id="1b82e-150">successUserCount</span><span class="sxs-lookup"><span data-stu-id="1b82e-150">successUserCount</span></span>|<span data-ttu-id="1b82e-151">Int32</span><span class="sxs-lookup"><span data-stu-id="1b82e-151">Int32</span></span>|<span data-ttu-id="1b82e-152">成功したユーザー数。</span><span class="sxs-lookup"><span data-stu-id="1b82e-152">Success user count.</span></span>|
|<span data-ttu-id="1b82e-153">errorUserCount</span><span class="sxs-lookup"><span data-stu-id="1b82e-153">errorUserCount</span></span>|<span data-ttu-id="1b82e-154">Int32</span><span class="sxs-lookup"><span data-stu-id="1b82e-154">Int32</span></span>|<span data-ttu-id="1b82e-155">エラーユーザー数。</span><span class="sxs-lookup"><span data-stu-id="1b82e-155">Error user count.</span></span>|



## <a name="response"></a><span data-ttu-id="1b82e-156">応答</span><span class="sxs-lookup"><span data-stu-id="1b82e-156">Response</span></span>
<span data-ttu-id="1b82e-157">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で更新された[deviceManagementScriptRunSummary](../resources/intune-devices-devicemanagementscriptrunsummary.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="1b82e-157">If successful, this method returns a `200 OK` response code and an updated [deviceManagementScriptRunSummary](../resources/intune-devices-devicemanagementscriptrunsummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1b82e-158">例</span><span class="sxs-lookup"><span data-stu-id="1b82e-158">Example</span></span>

### <a name="request"></a><span data-ttu-id="1b82e-159">要求</span><span class="sxs-lookup"><span data-stu-id="1b82e-159">Request</span></span>
<span data-ttu-id="1b82e-160">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="1b82e-160">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/runSummary
Content-type: application/json
Content-length: 270

{
  "@odata.type": "#microsoft.graph.deviceManagementScriptRunSummary",
  "successDeviceCount": 2,
  "errorDeviceCount": 0,
  "compliantDeviceCount": 4,
  "notCompliantDeviceCount": 7,
  "pendingDeviceCount": 2,
  "successUserCount": 0,
  "errorUserCount": 14
}
```

### <a name="response"></a><span data-ttu-id="1b82e-161">応答</span><span class="sxs-lookup"><span data-stu-id="1b82e-161">Response</span></span>
<span data-ttu-id="1b82e-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="1b82e-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 319

{
  "@odata.type": "#microsoft.graph.deviceManagementScriptRunSummary",
  "id": "514d5d38-5d38-514d-385d-4d51385d4d51",
  "successDeviceCount": 2,
  "errorDeviceCount": 0,
  "compliantDeviceCount": 4,
  "notCompliantDeviceCount": 7,
  "pendingDeviceCount": 2,
  "successUserCount": 0,
  "errorUserCount": 14
}
```






