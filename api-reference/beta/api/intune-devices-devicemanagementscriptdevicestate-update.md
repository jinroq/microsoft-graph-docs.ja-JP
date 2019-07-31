---
title: DeviceManagementScriptDeviceState の更新
description: DeviceManagementScriptDeviceState オブジェクトのプロパティを更新します。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: db46807d376decdcbe81484ce097514af849efa7
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35986016"
---
# <a name="update-devicemanagementscriptdevicestate"></a><span data-ttu-id="f77db-103">DeviceManagementScriptDeviceState の更新</span><span class="sxs-lookup"><span data-stu-id="f77db-103">Update deviceManagementScriptDeviceState</span></span>

> <span data-ttu-id="f77db-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f77db-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f77db-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="f77db-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f77db-106">[Devicemanagementscriptdevicestate](../resources/intune-devices-devicemanagementscriptdevicestate.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="f77db-106">Update the properties of a [deviceManagementScriptDeviceState](../resources/intune-devices-devicemanagementscriptdevicestate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f77db-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="f77db-107">Prerequisites</span></span>
<span data-ttu-id="f77db-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="f77db-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f77db-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="f77db-110">Permission type</span></span>|<span data-ttu-id="f77db-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="f77db-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f77db-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="f77db-112">Delegated (work or school account)</span></span>|<span data-ttu-id="f77db-113">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f77db-113">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="f77db-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="f77db-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f77db-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f77db-115">Not supported.</span></span>|
|<span data-ttu-id="f77db-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="f77db-116">Application</span></span>|<span data-ttu-id="f77db-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f77db-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f77db-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="f77db-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}
PATCH /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/userRunStates/{deviceManagementScriptUserStateId}/deviceRunStates/{deviceManagementScriptDeviceStateId}
```

## <a name="request-headers"></a><span data-ttu-id="f77db-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="f77db-119">Request headers</span></span>
|<span data-ttu-id="f77db-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="f77db-120">Header</span></span>|<span data-ttu-id="f77db-121">値</span><span class="sxs-lookup"><span data-stu-id="f77db-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f77db-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="f77db-122">Authorization</span></span>|<span data-ttu-id="f77db-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="f77db-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f77db-124">承諾</span><span class="sxs-lookup"><span data-stu-id="f77db-124">Accept</span></span>|<span data-ttu-id="f77db-125">application/json</span><span class="sxs-lookup"><span data-stu-id="f77db-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f77db-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="f77db-126">Request body</span></span>
<span data-ttu-id="f77db-127">要求本文で、 [Devicemanagementscriptdevicestate](../resources/intune-devices-devicemanagementscriptdevicestate.md)オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="f77db-127">In the request body, supply a JSON representation for the [deviceManagementScriptDeviceState](../resources/intune-devices-devicemanagementscriptdevicestate.md) object.</span></span>

<span data-ttu-id="f77db-128">次の表に、 [Devicemanagementscriptdevicestate](../resources/intune-devices-devicemanagementscriptdevicestate.md)の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="f77db-128">The following table shows the properties that are required when you create the [deviceManagementScriptDeviceState](../resources/intune-devices-devicemanagementscriptdevicestate.md).</span></span>

|<span data-ttu-id="f77db-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="f77db-129">Property</span></span>|<span data-ttu-id="f77db-130">型</span><span class="sxs-lookup"><span data-stu-id="f77db-130">Type</span></span>|<span data-ttu-id="f77db-131">説明</span><span class="sxs-lookup"><span data-stu-id="f77db-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f77db-132">id</span><span class="sxs-lookup"><span data-stu-id="f77db-132">id</span></span>|<span data-ttu-id="f77db-133">String</span><span class="sxs-lookup"><span data-stu-id="f77db-133">String</span></span>|<span data-ttu-id="f77db-134">デバイス管理スクリプトのデバイス状態エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="f77db-134">Key of the device management script device state entity.</span></span>|
|<span data-ttu-id="f77db-135">runState</span><span class="sxs-lookup"><span data-stu-id="f77db-135">runState</span></span>|[<span data-ttu-id="f77db-136">runState</span><span class="sxs-lookup"><span data-stu-id="f77db-136">runState</span></span>](../resources/intune-shared-runstate.md)|<span data-ttu-id="f77db-137">デバイス管理スクリプトの最新の実行の状態。</span><span class="sxs-lookup"><span data-stu-id="f77db-137">State of latest run of the device management script.</span></span> <span data-ttu-id="f77db-138">可能な値は、`unknown`、`success`、`fail` です。</span><span class="sxs-lookup"><span data-stu-id="f77db-138">Possible values are: `unknown`, `success`, `fail`.</span></span>|
|<span data-ttu-id="f77db-139">resultMessage</span><span class="sxs-lookup"><span data-stu-id="f77db-139">resultMessage</span></span>|<span data-ttu-id="f77db-140">String</span><span class="sxs-lookup"><span data-stu-id="f77db-140">String</span></span>|<span data-ttu-id="f77db-141">実行出力の詳細。</span><span class="sxs-lookup"><span data-stu-id="f77db-141">Details of execution output.</span></span>|
|<span data-ttu-id="f77db-142">lastStateUpdateDateTime</span><span class="sxs-lookup"><span data-stu-id="f77db-142">lastStateUpdateDateTime</span></span>|<span data-ttu-id="f77db-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f77db-143">DateTimeOffset</span></span>|<span data-ttu-id="f77db-144">デバイス管理スクリプトが最後に実行された時刻。</span><span class="sxs-lookup"><span data-stu-id="f77db-144">Latest time the device management script executes.</span></span>|
|<span data-ttu-id="f77db-145">errorCode</span><span class="sxs-lookup"><span data-stu-id="f77db-145">errorCode</span></span>|<span data-ttu-id="f77db-146">Int32</span><span class="sxs-lookup"><span data-stu-id="f77db-146">Int32</span></span>|<span data-ttu-id="f77db-147">デバイス管理スクリプトの誤った実行に対応するエラーコード。</span><span class="sxs-lookup"><span data-stu-id="f77db-147">Error code corresponding to erroneous execution of the device management script.</span></span>|
|<span data-ttu-id="f77db-148">errorDescription</span><span class="sxs-lookup"><span data-stu-id="f77db-148">errorDescription</span></span>|<span data-ttu-id="f77db-149">String</span><span class="sxs-lookup"><span data-stu-id="f77db-149">String</span></span>|<span data-ttu-id="f77db-150">デバイス管理スクリプトの誤った実行に対応するエラーの説明。</span><span class="sxs-lookup"><span data-stu-id="f77db-150">Error description corresponding to erroneous execution of the device management script.</span></span>|



## <a name="response"></a><span data-ttu-id="f77db-151">応答</span><span class="sxs-lookup"><span data-stu-id="f77db-151">Response</span></span>
<span data-ttu-id="f77db-152">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で更新された[Devicemanagementscriptdevicestate](../resources/intune-devices-devicemanagementscriptdevicestate.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="f77db-152">If successful, this method returns a `200 OK` response code and an updated [deviceManagementScriptDeviceState](../resources/intune-devices-devicemanagementscriptdevicestate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f77db-153">例</span><span class="sxs-lookup"><span data-stu-id="f77db-153">Example</span></span>

### <a name="request"></a><span data-ttu-id="f77db-154">要求</span><span class="sxs-lookup"><span data-stu-id="f77db-154">Request</span></span>
<span data-ttu-id="f77db-155">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="f77db-155">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="f77db-156">応答</span><span class="sxs-lookup"><span data-stu-id="f77db-156">Response</span></span>
<span data-ttu-id="f77db-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="f77db-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





