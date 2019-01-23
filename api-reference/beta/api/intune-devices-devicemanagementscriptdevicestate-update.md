---
title: DeviceManagementScriptDeviceState を更新します。
description: DeviceManagementScriptDeviceState オブジェクトのプロパティを更新します。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 35768793279cdb96494a26dac8854f74e3c267ad
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29395154"
---
# <a name="update-devicemanagementscriptdevicestate"></a><span data-ttu-id="4b5d4-103">DeviceManagementScriptDeviceState を更新します。</span><span class="sxs-lookup"><span data-stu-id="4b5d4-103">Update deviceManagementScriptDeviceState</span></span>

> <span data-ttu-id="4b5d4-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="4b5d4-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="4b5d4-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="4b5d4-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="4b5d4-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="4b5d4-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4b5d4-107">[DeviceManagementScriptDeviceState](../resources/intune-devices-devicemanagementscriptdevicestate.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="4b5d4-107">Update the properties of a [deviceManagementScriptDeviceState](../resources/intune-devices-devicemanagementscriptdevicestate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="4b5d4-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="4b5d4-108">Prerequisites</span></span>
<span data-ttu-id="4b5d4-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/concepts/permissions-reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="4b5d4-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="4b5d4-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="4b5d4-111">Permission type</span></span>|<span data-ttu-id="4b5d4-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="4b5d4-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4b5d4-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="4b5d4-113">Delegated (work or school account)</span></span>|<span data-ttu-id="4b5d4-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4b5d4-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="4b5d4-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="4b5d4-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4b5d4-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="4b5d4-116">Not supported.</span></span>|
|<span data-ttu-id="4b5d4-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="4b5d4-117">Application</span></span>|<span data-ttu-id="4b5d4-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="4b5d4-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="4b5d4-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="4b5d4-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}
PATCH /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/userRunStates/{deviceManagementScriptUserStateId}/deviceRunStates/{deviceManagementScriptDeviceStateId}
```

## <a name="request-headers"></a><span data-ttu-id="4b5d4-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="4b5d4-120">Request headers</span></span>
|<span data-ttu-id="4b5d4-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="4b5d4-121">Header</span></span>|<span data-ttu-id="4b5d4-122">値</span><span class="sxs-lookup"><span data-stu-id="4b5d4-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4b5d4-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="4b5d4-123">Authorization</span></span>|<span data-ttu-id="4b5d4-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="4b5d4-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4b5d4-125">Accept</span><span class="sxs-lookup"><span data-stu-id="4b5d4-125">Accept</span></span>|<span data-ttu-id="4b5d4-126">application/json</span><span class="sxs-lookup"><span data-stu-id="4b5d4-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4b5d4-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="4b5d4-127">Request body</span></span>
<span data-ttu-id="4b5d4-128">要求の本文に[deviceManagementScriptDeviceState](../resources/intune-devices-devicemanagementscriptdevicestate.md)オブジェクトの JSON の形式を指定します。</span><span class="sxs-lookup"><span data-stu-id="4b5d4-128">In the request body, supply a JSON representation for the [deviceManagementScriptDeviceState](../resources/intune-devices-devicemanagementscriptdevicestate.md) object.</span></span>

<span data-ttu-id="4b5d4-129">[DeviceManagementScriptDeviceState](../resources/intune-devices-devicemanagementscriptdevicestate.md)を作成するときに必要なプロパティを次の表に示します。</span><span class="sxs-lookup"><span data-stu-id="4b5d4-129">The following table shows the properties that are required when you create the [deviceManagementScriptDeviceState](../resources/intune-devices-devicemanagementscriptdevicestate.md).</span></span>

|<span data-ttu-id="4b5d4-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="4b5d4-130">Property</span></span>|<span data-ttu-id="4b5d4-131">型</span><span class="sxs-lookup"><span data-stu-id="4b5d4-131">Type</span></span>|<span data-ttu-id="4b5d4-132">説明</span><span class="sxs-lookup"><span data-stu-id="4b5d4-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4b5d4-133">id</span><span class="sxs-lookup"><span data-stu-id="4b5d4-133">id</span></span>|<span data-ttu-id="4b5d4-134">String</span><span class="sxs-lookup"><span data-stu-id="4b5d4-134">String</span></span>|<span data-ttu-id="4b5d4-135">デバイス管理スクリプト デバイス状態のエンティティのキーです。</span><span class="sxs-lookup"><span data-stu-id="4b5d4-135">Key of the device management script device state entity.</span></span>|
|<span data-ttu-id="4b5d4-136">runState</span><span class="sxs-lookup"><span data-stu-id="4b5d4-136">runState</span></span>|[<span data-ttu-id="4b5d4-137">runState</span><span class="sxs-lookup"><span data-stu-id="4b5d4-137">runState</span></span>](../resources/intune-shared-runstate.md)|<span data-ttu-id="4b5d4-138">デバイス管理スクリプトの実行を最新の状態です。</span><span class="sxs-lookup"><span data-stu-id="4b5d4-138">State of latest run of the device management script.</span></span> <span data-ttu-id="4b5d4-139">可能な値は、`unknown`、`success`、`fail` です。</span><span class="sxs-lookup"><span data-stu-id="4b5d4-139">Possible values are: `unknown`, `success`, `fail`.</span></span>|
|<span data-ttu-id="4b5d4-140">resultMessage</span><span class="sxs-lookup"><span data-stu-id="4b5d4-140">resultMessage</span></span>|<span data-ttu-id="4b5d4-141">String</span><span class="sxs-lookup"><span data-stu-id="4b5d4-141">String</span></span>|<span data-ttu-id="4b5d4-142">実行結果の詳細です。</span><span class="sxs-lookup"><span data-stu-id="4b5d4-142">Details of execution output.</span></span>|
|<span data-ttu-id="4b5d4-143">lastStateUpdateDateTime</span><span class="sxs-lookup"><span data-stu-id="4b5d4-143">lastStateUpdateDateTime</span></span>|<span data-ttu-id="4b5d4-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4b5d4-144">DateTimeOffset</span></span>|<span data-ttu-id="4b5d4-145">最新の時間、デバイスの管理スクリプトを実行します。</span><span class="sxs-lookup"><span data-stu-id="4b5d4-145">Latest time the device management script executes.</span></span>|
|<span data-ttu-id="4b5d4-146">errorCode</span><span class="sxs-lookup"><span data-stu-id="4b5d4-146">errorCode</span></span>|<span data-ttu-id="4b5d4-147">Int32</span><span class="sxs-lookup"><span data-stu-id="4b5d4-147">Int32</span></span>|<span data-ttu-id="4b5d4-148">デバイス管理スクリプトの実行がエラーに対応するエラー ・ コードです。</span><span class="sxs-lookup"><span data-stu-id="4b5d4-148">Error code corresponding to erroneous execution of the device management script.</span></span>|
|<span data-ttu-id="4b5d4-149">errorDescription</span><span class="sxs-lookup"><span data-stu-id="4b5d4-149">errorDescription</span></span>|<span data-ttu-id="4b5d4-150">String</span><span class="sxs-lookup"><span data-stu-id="4b5d4-150">String</span></span>|<span data-ttu-id="4b5d4-151">デバイス管理スクリプトの実行がエラーに対応するエラーの説明です。</span><span class="sxs-lookup"><span data-stu-id="4b5d4-151">Error description corresponding to erroneous execution of the device management script.</span></span>|



## <a name="response"></a><span data-ttu-id="4b5d4-152">応答</span><span class="sxs-lookup"><span data-stu-id="4b5d4-152">Response</span></span>
<span data-ttu-id="4b5d4-153">かどうかは成功すると、このメソッドが返されます、`200 OK`応答コードおよび応答の本文に更新された[deviceManagementScriptDeviceState](../resources/intune-devices-devicemanagementscriptdevicestate.md)オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="4b5d4-153">If successful, this method returns a `200 OK` response code and an updated [deviceManagementScriptDeviceState](../resources/intune-devices-devicemanagementscriptdevicestate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4b5d4-154">例</span><span class="sxs-lookup"><span data-stu-id="4b5d4-154">Example</span></span>

### <a name="request"></a><span data-ttu-id="4b5d4-155">要求</span><span class="sxs-lookup"><span data-stu-id="4b5d4-155">Request</span></span>
<span data-ttu-id="4b5d4-156">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="4b5d4-156">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}
Content-type: application/json
Content-length: 281

{
  "@odata.type": "#microsoft.graph.deviceManagementScriptDeviceState",
  "runState": "success",
  "resultMessage": "Result Message value",
  "lastStateUpdateDateTime": "2017-01-01T00:02:58.4418045-08:00",
  "errorCode": 9,
  "errorDescription": "Error Description value"
}
```

### <a name="response"></a><span data-ttu-id="4b5d4-157">応答</span><span class="sxs-lookup"><span data-stu-id="4b5d4-157">Response</span></span>
<span data-ttu-id="4b5d4-p104">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="4b5d4-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 330

{
  "@odata.type": "#microsoft.graph.deviceManagementScriptDeviceState",
  "id": "39440cba-0cba-3944-ba0c-4439ba0c4439",
  "runState": "success",
  "resultMessage": "Result Message value",
  "lastStateUpdateDateTime": "2017-01-01T00:02:58.4418045-08:00",
  "errorCode": 9,
  "errorDescription": "Error Description value"
}
```




