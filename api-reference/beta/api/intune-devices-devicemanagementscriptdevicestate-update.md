---
title: DeviceManagementScriptDeviceState を更新します。
description: DeviceManagementScriptDeviceState オブジェクトのプロパティを更新します。
author: tfitzmac
ms.openlocfilehash: a5dee56ac260642d1a0c105d62ee26499d7276df
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27305314"
---
# <a name="update-devicemanagementscriptdevicestate"></a><span data-ttu-id="af110-103">DeviceManagementScriptDeviceState を更新します。</span><span class="sxs-lookup"><span data-stu-id="af110-103">Update deviceManagementScriptDeviceState</span></span>

> <span data-ttu-id="af110-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="af110-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="af110-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="af110-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="af110-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="af110-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="af110-107">[DeviceManagementScriptDeviceState](../resources/intune-devices-devicemanagementscriptdevicestate.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="af110-107">Update the properties of a [deviceManagementScriptDeviceState](../resources/intune-devices-devicemanagementscriptdevicestate.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="af110-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="af110-108">Prerequisites</span></span>
<span data-ttu-id="af110-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="af110-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="af110-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="af110-111">Permission type</span></span>|<span data-ttu-id="af110-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="af110-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="af110-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="af110-113">Delegated (work or school account)</span></span>|<span data-ttu-id="af110-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="af110-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="af110-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="af110-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="af110-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="af110-116">Not supported.</span></span>|
|<span data-ttu-id="af110-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="af110-117">Application</span></span>|<span data-ttu-id="af110-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="af110-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="af110-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="af110-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}
PATCH /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/userRunStates/{deviceManagementScriptUserStateId}/deviceRunStates/{deviceManagementScriptDeviceStateId}
```

## <a name="request-headers"></a><span data-ttu-id="af110-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="af110-120">Request headers</span></span>
|<span data-ttu-id="af110-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="af110-121">Header</span></span>|<span data-ttu-id="af110-122">値</span><span class="sxs-lookup"><span data-stu-id="af110-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="af110-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="af110-123">Authorization</span></span>|<span data-ttu-id="af110-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="af110-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="af110-125">Accept</span><span class="sxs-lookup"><span data-stu-id="af110-125">Accept</span></span>|<span data-ttu-id="af110-126">application/json</span><span class="sxs-lookup"><span data-stu-id="af110-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="af110-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="af110-127">Request body</span></span>
<span data-ttu-id="af110-128">要求の本文に[deviceManagementScriptDeviceState](../resources/intune-devices-devicemanagementscriptdevicestate.md)オブジェクトの JSON の形式を指定します。</span><span class="sxs-lookup"><span data-stu-id="af110-128">In the request body, supply a JSON representation for the [deviceManagementScriptDeviceState](../resources/intune-devices-devicemanagementscriptdevicestate.md) object.</span></span>

<span data-ttu-id="af110-129">[DeviceManagementScriptDeviceState](../resources/intune-devices-devicemanagementscriptdevicestate.md)を作成するときに必要なプロパティを次の表に示します。</span><span class="sxs-lookup"><span data-stu-id="af110-129">The following table shows the properties that are required when you create the [deviceManagementScriptDeviceState](../resources/intune-devices-devicemanagementscriptdevicestate.md).</span></span>

|<span data-ttu-id="af110-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="af110-130">Property</span></span>|<span data-ttu-id="af110-131">種類</span><span class="sxs-lookup"><span data-stu-id="af110-131">Type</span></span>|<span data-ttu-id="af110-132">説明</span><span class="sxs-lookup"><span data-stu-id="af110-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="af110-133">ID</span><span class="sxs-lookup"><span data-stu-id="af110-133">id</span></span>|<span data-ttu-id="af110-134">String</span><span class="sxs-lookup"><span data-stu-id="af110-134">String</span></span>|<span data-ttu-id="af110-135">デバイス管理スクリプト デバイス状態のエンティティのキーです。</span><span class="sxs-lookup"><span data-stu-id="af110-135">Key of the device management script device state entity.</span></span>|
|<span data-ttu-id="af110-136">runState</span><span class="sxs-lookup"><span data-stu-id="af110-136">runState</span></span>|[<span data-ttu-id="af110-137">runState</span><span class="sxs-lookup"><span data-stu-id="af110-137">runState</span></span>](../resources/intune-shared-runstate.md)|<span data-ttu-id="af110-138">デバイス管理スクリプトの実行を最新の状態です。</span><span class="sxs-lookup"><span data-stu-id="af110-138">State of latest run of the device management script.</span></span> <span data-ttu-id="af110-139">可能な値は、`unknown`、`success`、`fail` です。</span><span class="sxs-lookup"><span data-stu-id="af110-139">Possible values are: `unknown`, `success`, `fail`.</span></span>|
|<span data-ttu-id="af110-140">resultMessage</span><span class="sxs-lookup"><span data-stu-id="af110-140">resultMessage</span></span>|<span data-ttu-id="af110-141">String</span><span class="sxs-lookup"><span data-stu-id="af110-141">String</span></span>|<span data-ttu-id="af110-142">実行結果の詳細です。</span><span class="sxs-lookup"><span data-stu-id="af110-142">Details of execution output.</span></span>|
|<span data-ttu-id="af110-143">lastStateUpdateDateTime</span><span class="sxs-lookup"><span data-stu-id="af110-143">lastStateUpdateDateTime</span></span>|<span data-ttu-id="af110-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="af110-144">DateTimeOffset</span></span>|<span data-ttu-id="af110-145">最新の時間、デバイスの管理スクリプトを実行します。</span><span class="sxs-lookup"><span data-stu-id="af110-145">Latest time the device management script executes.</span></span>|
|<span data-ttu-id="af110-146">errorCode</span><span class="sxs-lookup"><span data-stu-id="af110-146">errorCode</span></span>|<span data-ttu-id="af110-147">Int32</span><span class="sxs-lookup"><span data-stu-id="af110-147">Int32</span></span>|<span data-ttu-id="af110-148">デバイス管理スクリプトの実行がエラーに対応するエラー ・ コードです。</span><span class="sxs-lookup"><span data-stu-id="af110-148">Error code corresponding to erroneous execution of the device management script.</span></span>|
|<span data-ttu-id="af110-149">errorDescription</span><span class="sxs-lookup"><span data-stu-id="af110-149">errorDescription</span></span>|<span data-ttu-id="af110-150">String</span><span class="sxs-lookup"><span data-stu-id="af110-150">String</span></span>|<span data-ttu-id="af110-151">デバイス管理スクリプトの実行がエラーに対応するエラーの説明です。</span><span class="sxs-lookup"><span data-stu-id="af110-151">Error description corresponding to erroneous execution of the device management script.</span></span>|



## <a name="response"></a><span data-ttu-id="af110-152">応答</span><span class="sxs-lookup"><span data-stu-id="af110-152">Response</span></span>
<span data-ttu-id="af110-153">かどうかは成功すると、このメソッドが返されます、`200 OK`応答コードおよび応答の本文に更新された[deviceManagementScriptDeviceState](../resources/intune-devices-devicemanagementscriptdevicestate.md)オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="af110-153">If successful, this method returns a `200 OK` response code and an updated [deviceManagementScriptDeviceState](../resources/intune-devices-devicemanagementscriptdevicestate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="af110-154">例</span><span class="sxs-lookup"><span data-stu-id="af110-154">Example</span></span>
### <a name="request"></a><span data-ttu-id="af110-155">要求</span><span class="sxs-lookup"><span data-stu-id="af110-155">Request</span></span>
<span data-ttu-id="af110-156">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="af110-156">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}
Content-type: application/json
Content-length: 209

{
  "runState": "success",
  "resultMessage": "Result Message value",
  "lastStateUpdateDateTime": "2017-01-01T00:02:58.4418045-08:00",
  "errorCode": 9,
  "errorDescription": "Error Description value"
}
```

### <a name="response"></a><span data-ttu-id="af110-157">応答</span><span class="sxs-lookup"><span data-stu-id="af110-157">Response</span></span>
<span data-ttu-id="af110-p104">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="af110-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





