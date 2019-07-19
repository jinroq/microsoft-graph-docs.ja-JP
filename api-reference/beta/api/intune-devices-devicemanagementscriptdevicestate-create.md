---
title: DeviceManagementScriptDeviceState の作成
description: 新しい deviceManagementScriptDeviceState オブジェクトを作成します。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 47ff2099073e346358c396bef912e117cb99c6e2
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/14/2019
ms.locfileid: "34958964"
---
# <a name="create-devicemanagementscriptdevicestate"></a><span data-ttu-id="52971-103">DeviceManagementScriptDeviceState の作成</span><span class="sxs-lookup"><span data-stu-id="52971-103">Create deviceManagementScriptDeviceState</span></span>

> <span data-ttu-id="52971-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="52971-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="52971-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="52971-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="52971-106">新しい[Devicemanagementscriptdevicestate](../resources/intune-devices-devicemanagementscriptdevicestate.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="52971-106">Create a new [deviceManagementScriptDeviceState](../resources/intune-devices-devicemanagementscriptdevicestate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="52971-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="52971-107">Prerequisites</span></span>
<span data-ttu-id="52971-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="52971-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="52971-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="52971-110">Permission type</span></span>|<span data-ttu-id="52971-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="52971-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="52971-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="52971-112">Delegated (work or school account)</span></span>|<span data-ttu-id="52971-113">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="52971-113">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="52971-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="52971-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="52971-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="52971-115">Not supported.</span></span>|
|<span data-ttu-id="52971-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="52971-116">Application</span></span>|<span data-ttu-id="52971-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="52971-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="52971-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="52971-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/userRunStates/{deviceManagementScriptUserStateId}/deviceRunStates
```

## <a name="request-headers"></a><span data-ttu-id="52971-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="52971-119">Request headers</span></span>
|<span data-ttu-id="52971-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="52971-120">Header</span></span>|<span data-ttu-id="52971-121">値</span><span class="sxs-lookup"><span data-stu-id="52971-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="52971-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="52971-122">Authorization</span></span>|<span data-ttu-id="52971-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="52971-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="52971-124">承諾</span><span class="sxs-lookup"><span data-stu-id="52971-124">Accept</span></span>|<span data-ttu-id="52971-125">application/json</span><span class="sxs-lookup"><span data-stu-id="52971-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="52971-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="52971-126">Request body</span></span>
<span data-ttu-id="52971-127">要求本文で、deviceManagementScriptDeviceState オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="52971-127">In the request body, supply a JSON representation for the deviceManagementScriptDeviceState object.</span></span>

<span data-ttu-id="52971-128">次の表に、deviceManagementScriptDeviceState の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="52971-128">The following table shows the properties that are required when you create the deviceManagementScriptDeviceState.</span></span>

|<span data-ttu-id="52971-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="52971-129">Property</span></span>|<span data-ttu-id="52971-130">型</span><span class="sxs-lookup"><span data-stu-id="52971-130">Type</span></span>|<span data-ttu-id="52971-131">説明</span><span class="sxs-lookup"><span data-stu-id="52971-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="52971-132">id</span><span class="sxs-lookup"><span data-stu-id="52971-132">id</span></span>|<span data-ttu-id="52971-133">String</span><span class="sxs-lookup"><span data-stu-id="52971-133">String</span></span>|<span data-ttu-id="52971-134">デバイス管理スクリプトのデバイス状態エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="52971-134">Key of the device management script device state entity.</span></span>|
|<span data-ttu-id="52971-135">runState</span><span class="sxs-lookup"><span data-stu-id="52971-135">runState</span></span>|[<span data-ttu-id="52971-136">runState</span><span class="sxs-lookup"><span data-stu-id="52971-136">runState</span></span>](../resources/intune-shared-runstate.md)|<span data-ttu-id="52971-137">デバイス管理スクリプトの最新の実行の状態。</span><span class="sxs-lookup"><span data-stu-id="52971-137">State of latest run of the device management script.</span></span> <span data-ttu-id="52971-138">可能な値は、`unknown`、`success`、`fail` です。</span><span class="sxs-lookup"><span data-stu-id="52971-138">Possible values are: `unknown`, `success`, `fail`.</span></span>|
|<span data-ttu-id="52971-139">resultMessage</span><span class="sxs-lookup"><span data-stu-id="52971-139">resultMessage</span></span>|<span data-ttu-id="52971-140">String</span><span class="sxs-lookup"><span data-stu-id="52971-140">String</span></span>|<span data-ttu-id="52971-141">実行出力の詳細。</span><span class="sxs-lookup"><span data-stu-id="52971-141">Details of execution output.</span></span>|
|<span data-ttu-id="52971-142">lastStateUpdateDateTime</span><span class="sxs-lookup"><span data-stu-id="52971-142">lastStateUpdateDateTime</span></span>|<span data-ttu-id="52971-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="52971-143">DateTimeOffset</span></span>|<span data-ttu-id="52971-144">デバイス管理スクリプトが最後に実行された時刻。</span><span class="sxs-lookup"><span data-stu-id="52971-144">Latest time the device management script executes.</span></span>|
|<span data-ttu-id="52971-145">errorCode</span><span class="sxs-lookup"><span data-stu-id="52971-145">errorCode</span></span>|<span data-ttu-id="52971-146">Int32</span><span class="sxs-lookup"><span data-stu-id="52971-146">Int32</span></span>|<span data-ttu-id="52971-147">デバイス管理スクリプトの誤った実行に対応するエラーコード。</span><span class="sxs-lookup"><span data-stu-id="52971-147">Error code corresponding to erroneous execution of the device management script.</span></span>|
|<span data-ttu-id="52971-148">errorDescription</span><span class="sxs-lookup"><span data-stu-id="52971-148">errorDescription</span></span>|<span data-ttu-id="52971-149">String</span><span class="sxs-lookup"><span data-stu-id="52971-149">String</span></span>|<span data-ttu-id="52971-150">デバイス管理スクリプトの誤った実行に対応するエラーの説明。</span><span class="sxs-lookup"><span data-stu-id="52971-150">Error description corresponding to erroneous execution of the device management script.</span></span>|



## <a name="response"></a><span data-ttu-id="52971-151">応答</span><span class="sxs-lookup"><span data-stu-id="52971-151">Response</span></span>
<span data-ttu-id="52971-152">成功した場合、このメソッド`201 Created`は応答コードと、応答本文で[Devicemanagementscriptdevicestate](../resources/intune-devices-devicemanagementscriptdevicestate.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="52971-152">If successful, this method returns a `201 Created` response code and a [deviceManagementScriptDeviceState](../resources/intune-devices-devicemanagementscriptdevicestate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="52971-153">例</span><span class="sxs-lookup"><span data-stu-id="52971-153">Example</span></span>

### <a name="request"></a><span data-ttu-id="52971-154">要求</span><span class="sxs-lookup"><span data-stu-id="52971-154">Request</span></span>
<span data-ttu-id="52971-155">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="52971-155">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates
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

### <a name="response"></a><span data-ttu-id="52971-156">応答</span><span class="sxs-lookup"><span data-stu-id="52971-156">Response</span></span>
<span data-ttu-id="52971-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="52971-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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





