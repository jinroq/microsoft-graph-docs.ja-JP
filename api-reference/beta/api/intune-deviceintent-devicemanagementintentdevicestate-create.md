---
title: DeviceManagementIntentDeviceState の作成
description: 新しい deviceManagementIntentDeviceState オブジェクトを作成します。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: f70b2f77808fe4c2b4f15b54198d77d39a484486
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/14/2019
ms.locfileid: "34960294"
---
# <a name="create-devicemanagementintentdevicestate"></a><span data-ttu-id="636f2-103">DeviceManagementIntentDeviceState の作成</span><span class="sxs-lookup"><span data-stu-id="636f2-103">Create deviceManagementIntentDeviceState</span></span>

> <span data-ttu-id="636f2-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="636f2-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="636f2-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="636f2-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="636f2-106">新しい[Devicemanagementintentdevicestate](../resources/intune-deviceintent-devicemanagementintentdevicestate.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="636f2-106">Create a new [deviceManagementIntentDeviceState](../resources/intune-deviceintent-devicemanagementintentdevicestate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="636f2-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="636f2-107">Prerequisites</span></span>
<span data-ttu-id="636f2-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="636f2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="636f2-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="636f2-110">Permission type</span></span>|<span data-ttu-id="636f2-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="636f2-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="636f2-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="636f2-112">Delegated (work or school account)</span></span>|<span data-ttu-id="636f2-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="636f2-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="636f2-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="636f2-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="636f2-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="636f2-115">Not supported.</span></span>|
|<span data-ttu-id="636f2-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="636f2-116">Application</span></span>|<span data-ttu-id="636f2-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="636f2-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="636f2-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="636f2-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/intents/{deviceManagementIntentId}/deviceStates
```

## <a name="request-headers"></a><span data-ttu-id="636f2-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="636f2-119">Request headers</span></span>
|<span data-ttu-id="636f2-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="636f2-120">Header</span></span>|<span data-ttu-id="636f2-121">値</span><span class="sxs-lookup"><span data-stu-id="636f2-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="636f2-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="636f2-122">Authorization</span></span>|<span data-ttu-id="636f2-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="636f2-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="636f2-124">承諾</span><span class="sxs-lookup"><span data-stu-id="636f2-124">Accept</span></span>|<span data-ttu-id="636f2-125">application/json</span><span class="sxs-lookup"><span data-stu-id="636f2-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="636f2-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="636f2-126">Request body</span></span>
<span data-ttu-id="636f2-127">要求本文で、deviceManagementIntentDeviceState オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="636f2-127">In the request body, supply a JSON representation for the deviceManagementIntentDeviceState object.</span></span>

<span data-ttu-id="636f2-128">次の表に、deviceManagementIntentDeviceState の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="636f2-128">The following table shows the properties that are required when you create the deviceManagementIntentDeviceState.</span></span>

|<span data-ttu-id="636f2-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="636f2-129">Property</span></span>|<span data-ttu-id="636f2-130">型</span><span class="sxs-lookup"><span data-stu-id="636f2-130">Type</span></span>|<span data-ttu-id="636f2-131">説明</span><span class="sxs-lookup"><span data-stu-id="636f2-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="636f2-132">id</span><span class="sxs-lookup"><span data-stu-id="636f2-132">id</span></span>|<span data-ttu-id="636f2-133">文字列</span><span class="sxs-lookup"><span data-stu-id="636f2-133">String</span></span>|<span data-ttu-id="636f2-134">ID</span><span class="sxs-lookup"><span data-stu-id="636f2-134">The ID</span></span>|
|<span data-ttu-id="636f2-135">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="636f2-135">userPrincipalName</span></span>|<span data-ttu-id="636f2-136">String</span><span class="sxs-lookup"><span data-stu-id="636f2-136">String</span></span>|<span data-ttu-id="636f2-137">デバイスで報告されているユーザープリンシパル名</span><span class="sxs-lookup"><span data-stu-id="636f2-137">The user principal name that is being reported on a device</span></span>|
|<span data-ttu-id="636f2-138">userName</span><span class="sxs-lookup"><span data-stu-id="636f2-138">userName</span></span>|<span data-ttu-id="636f2-139">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="636f2-139">String</span></span>|<span data-ttu-id="636f2-140">デバイスで報告されているユーザー名</span><span class="sxs-lookup"><span data-stu-id="636f2-140">The user name that is being reported on a device</span></span>|
|<span data-ttu-id="636f2-141">deviceDisplayName</span><span class="sxs-lookup"><span data-stu-id="636f2-141">deviceDisplayName</span></span>|<span data-ttu-id="636f2-142">String</span><span class="sxs-lookup"><span data-stu-id="636f2-142">String</span></span>|<span data-ttu-id="636f2-143">レポートされているデバイス名</span><span class="sxs-lookup"><span data-stu-id="636f2-143">Device name that is being reported</span></span>|
|<span data-ttu-id="636f2-144">lastReportedDateTime</span><span class="sxs-lookup"><span data-stu-id="636f2-144">lastReportedDateTime</span></span>|<span data-ttu-id="636f2-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="636f2-145">DateTimeOffset</span></span>|<span data-ttu-id="636f2-146">インテントレポートの最終更新日時</span><span class="sxs-lookup"><span data-stu-id="636f2-146">Last modified date time of an intent report</span></span>|
|<span data-ttu-id="636f2-147">state</span><span class="sxs-lookup"><span data-stu-id="636f2-147">state</span></span>|[<span data-ttu-id="636f2-148">complianceStatus</span><span class="sxs-lookup"><span data-stu-id="636f2-148">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="636f2-149">目的のデバイス状態。</span><span class="sxs-lookup"><span data-stu-id="636f2-149">Device state for an intent.</span></span> <span data-ttu-id="636f2-150">可能な値は、`unknown`、`notApplicable`、`compliant`、`remediated`、`nonCompliant`、`error`、`conflict`、`notAssigned` です。</span><span class="sxs-lookup"><span data-stu-id="636f2-150">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="636f2-151">deviceId</span><span class="sxs-lookup"><span data-stu-id="636f2-151">deviceId</span></span>|<span data-ttu-id="636f2-152">String</span><span class="sxs-lookup"><span data-stu-id="636f2-152">String</span></span>|<span data-ttu-id="636f2-153">レポートされているデバイス id</span><span class="sxs-lookup"><span data-stu-id="636f2-153">Device id that is being reported</span></span>|



## <a name="response"></a><span data-ttu-id="636f2-154">応答</span><span class="sxs-lookup"><span data-stu-id="636f2-154">Response</span></span>
<span data-ttu-id="636f2-155">成功した場合、このメソッド`201 Created`は応答コードと、応答本文で[Devicemanagementintentdevicestate](../resources/intune-deviceintent-devicemanagementintentdevicestate.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="636f2-155">If successful, this method returns a `201 Created` response code and a [deviceManagementIntentDeviceState](../resources/intune-deviceintent-devicemanagementintentdevicestate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="636f2-156">例</span><span class="sxs-lookup"><span data-stu-id="636f2-156">Example</span></span>

### <a name="request"></a><span data-ttu-id="636f2-157">要求</span><span class="sxs-lookup"><span data-stu-id="636f2-157">Request</span></span>
<span data-ttu-id="636f2-158">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="636f2-158">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/intents/{deviceManagementIntentId}/deviceStates
Content-type: application/json
Content-length: 342

{
  "@odata.type": "#microsoft.graph.deviceManagementIntentDeviceState",
  "userPrincipalName": "User Principal Name value",
  "userName": "User Name value",
  "deviceDisplayName": "Device Display Name value",
  "lastReportedDateTime": "2017-01-01T00:00:17.7769392-08:00",
  "state": "notApplicable",
  "deviceId": "Device Id value"
}
```

### <a name="response"></a><span data-ttu-id="636f2-159">応答</span><span class="sxs-lookup"><span data-stu-id="636f2-159">Response</span></span>
<span data-ttu-id="636f2-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="636f2-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 391

{
  "@odata.type": "#microsoft.graph.deviceManagementIntentDeviceState",
  "id": "8db75881-5881-8db7-8158-b78d8158b78d",
  "userPrincipalName": "User Principal Name value",
  "userName": "User Name value",
  "deviceDisplayName": "Device Display Name value",
  "lastReportedDateTime": "2017-01-01T00:00:17.7769392-08:00",
  "state": "notApplicable",
  "deviceId": "Device Id value"
}
```





