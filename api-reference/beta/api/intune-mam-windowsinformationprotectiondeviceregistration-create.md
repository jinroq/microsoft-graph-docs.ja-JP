---
title: WindowsInformationProtectionDeviceRegistration を作成します。
description: 新しい windowsInformationProtectionDeviceRegistration オブジェクトを作成します。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: ea5e3bac32e0511b54e08cb37063084f359e554a
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29428906"
---
# <a name="create-windowsinformationprotectiondeviceregistration"></a><span data-ttu-id="16e68-103">WindowsInformationProtectionDeviceRegistration を作成します。</span><span class="sxs-lookup"><span data-stu-id="16e68-103">Create windowsInformationProtectionDeviceRegistration</span></span>

> <span data-ttu-id="16e68-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="16e68-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="16e68-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="16e68-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="16e68-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="16e68-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="16e68-107">新しい[windowsInformationProtectionDeviceRegistration](../resources/intune-mam-windowsinformationprotectiondeviceregistration.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="16e68-107">Create a new [windowsInformationProtectionDeviceRegistration](../resources/intune-mam-windowsinformationprotectiondeviceregistration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="16e68-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="16e68-108">Prerequisites</span></span>
<span data-ttu-id="16e68-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/concepts/permissions-reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="16e68-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="16e68-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="16e68-111">Permission type</span></span>|<span data-ttu-id="16e68-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="16e68-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="16e68-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="16e68-113">Delegated (work or school account)</span></span>|<span data-ttu-id="16e68-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="16e68-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="16e68-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="16e68-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="16e68-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="16e68-116">Not supported.</span></span>|
|<span data-ttu-id="16e68-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="16e68-117">Application</span></span>|<span data-ttu-id="16e68-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="16e68-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="16e68-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="16e68-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/windowsInformationProtectionDeviceRegistrations
```

## <a name="request-headers"></a><span data-ttu-id="16e68-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="16e68-120">Request headers</span></span>
|<span data-ttu-id="16e68-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="16e68-121">Header</span></span>|<span data-ttu-id="16e68-122">値</span><span class="sxs-lookup"><span data-stu-id="16e68-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="16e68-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="16e68-123">Authorization</span></span>|<span data-ttu-id="16e68-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="16e68-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="16e68-125">Accept</span><span class="sxs-lookup"><span data-stu-id="16e68-125">Accept</span></span>|<span data-ttu-id="16e68-126">application/json</span><span class="sxs-lookup"><span data-stu-id="16e68-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="16e68-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="16e68-127">Request body</span></span>
<span data-ttu-id="16e68-128">要求の本文に windowsInformationProtectionDeviceRegistration オブジェクトの JSON の形式を指定します。</span><span class="sxs-lookup"><span data-stu-id="16e68-128">In the request body, supply a JSON representation for the windowsInformationProtectionDeviceRegistration object.</span></span>

<span data-ttu-id="16e68-129">次の表は、windowsInformationProtectionDeviceRegistration を作成するときに必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="16e68-129">The following table shows the properties that are required when you create the windowsInformationProtectionDeviceRegistration.</span></span>

|<span data-ttu-id="16e68-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="16e68-130">Property</span></span>|<span data-ttu-id="16e68-131">型</span><span class="sxs-lookup"><span data-stu-id="16e68-131">Type</span></span>|<span data-ttu-id="16e68-132">説明</span><span class="sxs-lookup"><span data-stu-id="16e68-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="16e68-133">id</span><span class="sxs-lookup"><span data-stu-id="16e68-133">id</span></span>|<span data-ttu-id="16e68-134">String</span><span class="sxs-lookup"><span data-stu-id="16e68-134">String</span></span>|<span data-ttu-id="16e68-135">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="16e68-135">Key of the entity.</span></span>|
|<span data-ttu-id="16e68-136">userId</span><span class="sxs-lookup"><span data-stu-id="16e68-136">userId</span></span>|<span data-ttu-id="16e68-137">String</span><span class="sxs-lookup"><span data-stu-id="16e68-137">String</span></span>|<span data-ttu-id="16e68-138">このデバイスの登録レコードに関連付けられているユーザーの Id。</span><span class="sxs-lookup"><span data-stu-id="16e68-138">UserId associated with this device registration record.</span></span>|
|<span data-ttu-id="16e68-139">deviceRegistrationId</span><span class="sxs-lookup"><span data-stu-id="16e68-139">deviceRegistrationId</span></span>|<span data-ttu-id="16e68-140">String</span><span class="sxs-lookup"><span data-stu-id="16e68-140">String</span></span>|<span data-ttu-id="16e68-141">このデバイスの登録レコードのデバイスの識別子です。</span><span class="sxs-lookup"><span data-stu-id="16e68-141">Device identifier for this device registration record.</span></span>|
|<span data-ttu-id="16e68-142">deviceName</span><span class="sxs-lookup"><span data-stu-id="16e68-142">deviceName</span></span>|<span data-ttu-id="16e68-143">String</span><span class="sxs-lookup"><span data-stu-id="16e68-143">String</span></span>|<span data-ttu-id="16e68-144">デバイス名。</span><span class="sxs-lookup"><span data-stu-id="16e68-144">Device name.</span></span>|
|<span data-ttu-id="16e68-145">deviceType</span><span class="sxs-lookup"><span data-stu-id="16e68-145">deviceType</span></span>|<span data-ttu-id="16e68-146">String</span><span class="sxs-lookup"><span data-stu-id="16e68-146">String</span></span>|<span data-ttu-id="16e68-147">デバイスの種類、たとえば、Windows のラップトップ コンピューターと Windows phone です。</span><span class="sxs-lookup"><span data-stu-id="16e68-147">Device type, for example, Windows laptop VS Windows phone.</span></span>|
|<span data-ttu-id="16e68-148">deviceMacAddress</span><span class="sxs-lookup"><span data-stu-id="16e68-148">deviceMacAddress</span></span>|<span data-ttu-id="16e68-149">String</span><span class="sxs-lookup"><span data-stu-id="16e68-149">String</span></span>|<span data-ttu-id="16e68-150">デバイスの Mac アドレスです。</span><span class="sxs-lookup"><span data-stu-id="16e68-150">Device Mac address.</span></span>|
|<span data-ttu-id="16e68-151">lastCheckInDateTime</span><span class="sxs-lookup"><span data-stu-id="16e68-151">lastCheckInDateTime</span></span>|<span data-ttu-id="16e68-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="16e68-152">DateTimeOffset</span></span>|<span data-ttu-id="16e68-153">デバイスの最後のチェックインの時間です。</span><span class="sxs-lookup"><span data-stu-id="16e68-153">Last checkin time of the device.</span></span>|



## <a name="response"></a><span data-ttu-id="16e68-154">応答</span><span class="sxs-lookup"><span data-stu-id="16e68-154">Response</span></span>
<span data-ttu-id="16e68-155">かどうかは成功すると、このメソッドが返されます、`201 Created`応答コードおよび応答の本文に[windowsInformationProtectionDeviceRegistration](../resources/intune-mam-windowsinformationprotectiondeviceregistration.md)オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="16e68-155">If successful, this method returns a `201 Created` response code and a [windowsInformationProtectionDeviceRegistration](../resources/intune-mam-windowsinformationprotectiondeviceregistration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="16e68-156">例</span><span class="sxs-lookup"><span data-stu-id="16e68-156">Example</span></span>

### <a name="request"></a><span data-ttu-id="16e68-157">要求</span><span class="sxs-lookup"><span data-stu-id="16e68-157">Request</span></span>
<span data-ttu-id="16e68-158">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="16e68-158">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/windowsInformationProtectionDeviceRegistrations
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

### <a name="response"></a><span data-ttu-id="16e68-159">応答</span><span class="sxs-lookup"><span data-stu-id="16e68-159">Response</span></span>
<span data-ttu-id="16e68-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="16e68-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




