---
title: WindowsInformationProtectionDeviceRegistration を更新します。
description: WindowsInformationProtectionDeviceRegistration オブジェクトのプロパティを更新します。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 0c84f81dd8d9df54c6f05b1435ee4644a1a75342
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29430396"
---
# <a name="update-windowsinformationprotectiondeviceregistration"></a><span data-ttu-id="07ec0-103">WindowsInformationProtectionDeviceRegistration を更新します。</span><span class="sxs-lookup"><span data-stu-id="07ec0-103">Update windowsInformationProtectionDeviceRegistration</span></span>

> <span data-ttu-id="07ec0-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="07ec0-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="07ec0-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="07ec0-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="07ec0-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="07ec0-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="07ec0-107">[WindowsInformationProtectionDeviceRegistration](../resources/intune-mam-windowsinformationprotectiondeviceregistration.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="07ec0-107">Update the properties of a [windowsInformationProtectionDeviceRegistration](../resources/intune-mam-windowsinformationprotectiondeviceregistration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="07ec0-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="07ec0-108">Prerequisites</span></span>
<span data-ttu-id="07ec0-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/concepts/permissions-reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="07ec0-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="07ec0-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="07ec0-111">Permission type</span></span>|<span data-ttu-id="07ec0-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="07ec0-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="07ec0-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="07ec0-113">Delegated (work or school account)</span></span>|<span data-ttu-id="07ec0-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="07ec0-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="07ec0-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="07ec0-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="07ec0-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="07ec0-116">Not supported.</span></span>|
|<span data-ttu-id="07ec0-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="07ec0-117">Application</span></span>|<span data-ttu-id="07ec0-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="07ec0-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="07ec0-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="07ec0-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/windowsInformationProtectionDeviceRegistrations/{windowsInformationProtectionDeviceRegistrationId}
```

## <a name="request-headers"></a><span data-ttu-id="07ec0-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="07ec0-120">Request headers</span></span>
|<span data-ttu-id="07ec0-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="07ec0-121">Header</span></span>|<span data-ttu-id="07ec0-122">値</span><span class="sxs-lookup"><span data-stu-id="07ec0-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="07ec0-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="07ec0-123">Authorization</span></span>|<span data-ttu-id="07ec0-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="07ec0-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="07ec0-125">Accept</span><span class="sxs-lookup"><span data-stu-id="07ec0-125">Accept</span></span>|<span data-ttu-id="07ec0-126">application/json</span><span class="sxs-lookup"><span data-stu-id="07ec0-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="07ec0-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="07ec0-127">Request body</span></span>
<span data-ttu-id="07ec0-128">要求の本文に[windowsInformationProtectionDeviceRegistration](../resources/intune-mam-windowsinformationprotectiondeviceregistration.md)オブジェクトの JSON の形式を指定します。</span><span class="sxs-lookup"><span data-stu-id="07ec0-128">In the request body, supply a JSON representation for the [windowsInformationProtectionDeviceRegistration](../resources/intune-mam-windowsinformationprotectiondeviceregistration.md) object.</span></span>

<span data-ttu-id="07ec0-129">[WindowsInformationProtectionDeviceRegistration](../resources/intune-mam-windowsinformationprotectiondeviceregistration.md)を作成するときに必要なプロパティを次の表に示します。</span><span class="sxs-lookup"><span data-stu-id="07ec0-129">The following table shows the properties that are required when you create the [windowsInformationProtectionDeviceRegistration](../resources/intune-mam-windowsinformationprotectiondeviceregistration.md).</span></span>

|<span data-ttu-id="07ec0-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="07ec0-130">Property</span></span>|<span data-ttu-id="07ec0-131">型</span><span class="sxs-lookup"><span data-stu-id="07ec0-131">Type</span></span>|<span data-ttu-id="07ec0-132">説明</span><span class="sxs-lookup"><span data-stu-id="07ec0-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="07ec0-133">id</span><span class="sxs-lookup"><span data-stu-id="07ec0-133">id</span></span>|<span data-ttu-id="07ec0-134">String</span><span class="sxs-lookup"><span data-stu-id="07ec0-134">String</span></span>|<span data-ttu-id="07ec0-135">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="07ec0-135">Key of the entity.</span></span>|
|<span data-ttu-id="07ec0-136">userId</span><span class="sxs-lookup"><span data-stu-id="07ec0-136">userId</span></span>|<span data-ttu-id="07ec0-137">String</span><span class="sxs-lookup"><span data-stu-id="07ec0-137">String</span></span>|<span data-ttu-id="07ec0-138">このデバイスの登録レコードに関連付けられているユーザーの Id。</span><span class="sxs-lookup"><span data-stu-id="07ec0-138">UserId associated with this device registration record.</span></span>|
|<span data-ttu-id="07ec0-139">deviceRegistrationId</span><span class="sxs-lookup"><span data-stu-id="07ec0-139">deviceRegistrationId</span></span>|<span data-ttu-id="07ec0-140">String</span><span class="sxs-lookup"><span data-stu-id="07ec0-140">String</span></span>|<span data-ttu-id="07ec0-141">このデバイスの登録レコードのデバイスの識別子です。</span><span class="sxs-lookup"><span data-stu-id="07ec0-141">Device identifier for this device registration record.</span></span>|
|<span data-ttu-id="07ec0-142">deviceName</span><span class="sxs-lookup"><span data-stu-id="07ec0-142">deviceName</span></span>|<span data-ttu-id="07ec0-143">String</span><span class="sxs-lookup"><span data-stu-id="07ec0-143">String</span></span>|<span data-ttu-id="07ec0-144">デバイス名。</span><span class="sxs-lookup"><span data-stu-id="07ec0-144">Device name.</span></span>|
|<span data-ttu-id="07ec0-145">deviceType</span><span class="sxs-lookup"><span data-stu-id="07ec0-145">deviceType</span></span>|<span data-ttu-id="07ec0-146">String</span><span class="sxs-lookup"><span data-stu-id="07ec0-146">String</span></span>|<span data-ttu-id="07ec0-147">デバイスの種類、たとえば、Windows のラップトップ コンピューターと Windows phone です。</span><span class="sxs-lookup"><span data-stu-id="07ec0-147">Device type, for example, Windows laptop VS Windows phone.</span></span>|
|<span data-ttu-id="07ec0-148">deviceMacAddress</span><span class="sxs-lookup"><span data-stu-id="07ec0-148">deviceMacAddress</span></span>|<span data-ttu-id="07ec0-149">String</span><span class="sxs-lookup"><span data-stu-id="07ec0-149">String</span></span>|<span data-ttu-id="07ec0-150">デバイスの Mac アドレスです。</span><span class="sxs-lookup"><span data-stu-id="07ec0-150">Device Mac address.</span></span>|
|<span data-ttu-id="07ec0-151">lastCheckInDateTime</span><span class="sxs-lookup"><span data-stu-id="07ec0-151">lastCheckInDateTime</span></span>|<span data-ttu-id="07ec0-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="07ec0-152">DateTimeOffset</span></span>|<span data-ttu-id="07ec0-153">デバイスの最後のチェックインの時間です。</span><span class="sxs-lookup"><span data-stu-id="07ec0-153">Last checkin time of the device.</span></span>|



## <a name="response"></a><span data-ttu-id="07ec0-154">応答</span><span class="sxs-lookup"><span data-stu-id="07ec0-154">Response</span></span>
<span data-ttu-id="07ec0-155">かどうかは成功すると、このメソッドが返されます、`200 OK`応答コードおよび応答の本文に更新された[windowsInformationProtectionDeviceRegistration](../resources/intune-mam-windowsinformationprotectiondeviceregistration.md)オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="07ec0-155">If successful, this method returns a `200 OK` response code and an updated [windowsInformationProtectionDeviceRegistration](../resources/intune-mam-windowsinformationprotectiondeviceregistration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="07ec0-156">例</span><span class="sxs-lookup"><span data-stu-id="07ec0-156">Example</span></span>

### <a name="request"></a><span data-ttu-id="07ec0-157">要求</span><span class="sxs-lookup"><span data-stu-id="07ec0-157">Request</span></span>
<span data-ttu-id="07ec0-158">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="07ec0-158">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/windowsInformationProtectionDeviceRegistrations/{windowsInformationProtectionDeviceRegistrationId}
Content-type: application/json
Content-length: 366

{
  "@odata.type": "#microsoft.graph.windowsInformationProtectionDeviceRegistration",
  "userId": "User Id value",
  "deviceRegistrationId": "Device Registration Id value",
  "deviceName": "Device Name value",
  "deviceType": "Device Type value",
  "deviceMacAddress": "Device Mac Address value",
  "lastCheckInDateTime": "2016-12-31T23:59:56.413532-08:00"
}
```

### <a name="response"></a><span data-ttu-id="07ec0-159">応答</span><span class="sxs-lookup"><span data-stu-id="07ec0-159">Response</span></span>
<span data-ttu-id="07ec0-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="07ec0-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 415

{
  "@odata.type": "#microsoft.graph.windowsInformationProtectionDeviceRegistration",
  "id": "dd72e2c8-e2c8-dd72-c8e2-72ddc8e272dd",
  "userId": "User Id value",
  "deviceRegistrationId": "Device Registration Id value",
  "deviceName": "Device Name value",
  "deviceType": "Device Type value",
  "deviceMacAddress": "Device Mac Address value",
  "lastCheckInDateTime": "2016-12-31T23:59:56.413532-08:00"
}
```




