---
title: WindowsInformationProtectionDeviceRegistration の更新
description: WindowsInformationProtectionDeviceRegistration オブジェクトのプロパティを更新します。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: be0ea7d193a1e585e41005633b37ac31f57a7cc4
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36353478"
---
# <a name="update-windowsinformationprotectiondeviceregistration"></a><span data-ttu-id="62b35-103">WindowsInformationProtectionDeviceRegistration の更新</span><span class="sxs-lookup"><span data-stu-id="62b35-103">Update windowsInformationProtectionDeviceRegistration</span></span>

> <span data-ttu-id="62b35-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="62b35-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="62b35-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="62b35-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="62b35-106">[WindowsInformationProtectionDeviceRegistration](../resources/intune-mam-windowsinformationprotectiondeviceregistration.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="62b35-106">Update the properties of a [windowsInformationProtectionDeviceRegistration](../resources/intune-mam-windowsinformationprotectiondeviceregistration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="62b35-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="62b35-107">Prerequisites</span></span>
<span data-ttu-id="62b35-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="62b35-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="62b35-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="62b35-110">Permission type</span></span>|<span data-ttu-id="62b35-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="62b35-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="62b35-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="62b35-112">Delegated (work or school account)</span></span>|<span data-ttu-id="62b35-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="62b35-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="62b35-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="62b35-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="62b35-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="62b35-115">Not supported.</span></span>|
|<span data-ttu-id="62b35-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="62b35-116">Application</span></span>|<span data-ttu-id="62b35-117">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="62b35-117">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="62b35-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="62b35-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/windowsInformationProtectionDeviceRegistrations/{windowsInformationProtectionDeviceRegistrationId}
```

## <a name="request-headers"></a><span data-ttu-id="62b35-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="62b35-119">Request headers</span></span>
|<span data-ttu-id="62b35-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="62b35-120">Header</span></span>|<span data-ttu-id="62b35-121">値</span><span class="sxs-lookup"><span data-stu-id="62b35-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="62b35-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="62b35-122">Authorization</span></span>|<span data-ttu-id="62b35-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="62b35-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="62b35-124">承諾</span><span class="sxs-lookup"><span data-stu-id="62b35-124">Accept</span></span>|<span data-ttu-id="62b35-125">application/json</span><span class="sxs-lookup"><span data-stu-id="62b35-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="62b35-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="62b35-126">Request body</span></span>
<span data-ttu-id="62b35-127">要求本文で、 [windowsInformationProtectionDeviceRegistration](../resources/intune-mam-windowsinformationprotectiondeviceregistration.md)オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="62b35-127">In the request body, supply a JSON representation for the [windowsInformationProtectionDeviceRegistration](../resources/intune-mam-windowsinformationprotectiondeviceregistration.md) object.</span></span>

<span data-ttu-id="62b35-128">次の表に、 [windowsInformationProtectionDeviceRegistration](../resources/intune-mam-windowsinformationprotectiondeviceregistration.md)の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="62b35-128">The following table shows the properties that are required when you create the [windowsInformationProtectionDeviceRegistration](../resources/intune-mam-windowsinformationprotectiondeviceregistration.md).</span></span>

|<span data-ttu-id="62b35-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="62b35-129">Property</span></span>|<span data-ttu-id="62b35-130">型</span><span class="sxs-lookup"><span data-stu-id="62b35-130">Type</span></span>|<span data-ttu-id="62b35-131">説明</span><span class="sxs-lookup"><span data-stu-id="62b35-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="62b35-132">id</span><span class="sxs-lookup"><span data-stu-id="62b35-132">id</span></span>|<span data-ttu-id="62b35-133">文字列</span><span class="sxs-lookup"><span data-stu-id="62b35-133">String</span></span>|<span data-ttu-id="62b35-134">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="62b35-134">Key of the entity.</span></span>|
|<span data-ttu-id="62b35-135">userId</span><span class="sxs-lookup"><span data-stu-id="62b35-135">userId</span></span>|<span data-ttu-id="62b35-136">String</span><span class="sxs-lookup"><span data-stu-id="62b35-136">String</span></span>|<span data-ttu-id="62b35-137">このデバイス登録レコードに関連付けられている UserId。</span><span class="sxs-lookup"><span data-stu-id="62b35-137">UserId associated with this device registration record.</span></span>|
|<span data-ttu-id="62b35-138">deviceRegistrationId</span><span class="sxs-lookup"><span data-stu-id="62b35-138">deviceRegistrationId</span></span>|<span data-ttu-id="62b35-139">String</span><span class="sxs-lookup"><span data-stu-id="62b35-139">String</span></span>|<span data-ttu-id="62b35-140">このデバイス登録レコードのデバイス識別子。</span><span class="sxs-lookup"><span data-stu-id="62b35-140">Device identifier for this device registration record.</span></span>|
|<span data-ttu-id="62b35-141">deviceName</span><span class="sxs-lookup"><span data-stu-id="62b35-141">deviceName</span></span>|<span data-ttu-id="62b35-142">String</span><span class="sxs-lookup"><span data-stu-id="62b35-142">String</span></span>|<span data-ttu-id="62b35-143">デバイス名。</span><span class="sxs-lookup"><span data-stu-id="62b35-143">Device name.</span></span>|
|<span data-ttu-id="62b35-144">deviceType</span><span class="sxs-lookup"><span data-stu-id="62b35-144">deviceType</span></span>|<span data-ttu-id="62b35-145">String</span><span class="sxs-lookup"><span data-stu-id="62b35-145">String</span></span>|<span data-ttu-id="62b35-146">デバイスの種類。たとえば、Windows ラップトップ VS Windows phone。</span><span class="sxs-lookup"><span data-stu-id="62b35-146">Device type, for example, Windows laptop VS Windows phone.</span></span>|
|<span data-ttu-id="62b35-147">deviceMacAddress</span><span class="sxs-lookup"><span data-stu-id="62b35-147">deviceMacAddress</span></span>|<span data-ttu-id="62b35-148">String</span><span class="sxs-lookup"><span data-stu-id="62b35-148">String</span></span>|<span data-ttu-id="62b35-149">デバイスの Mac アドレス。</span><span class="sxs-lookup"><span data-stu-id="62b35-149">Device Mac address.</span></span>|
|<span data-ttu-id="62b35-150">lastCheckInDateTime</span><span class="sxs-lookup"><span data-stu-id="62b35-150">lastCheckInDateTime</span></span>|<span data-ttu-id="62b35-151">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="62b35-151">DateTimeOffset</span></span>|<span data-ttu-id="62b35-152">デバイスの最終チェックイン時刻。</span><span class="sxs-lookup"><span data-stu-id="62b35-152">Last checkin time of the device.</span></span>|



## <a name="response"></a><span data-ttu-id="62b35-153">応答</span><span class="sxs-lookup"><span data-stu-id="62b35-153">Response</span></span>
<span data-ttu-id="62b35-154">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で更新された[windowsInformationProtectionDeviceRegistration](../resources/intune-mam-windowsinformationprotectiondeviceregistration.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="62b35-154">If successful, this method returns a `200 OK` response code and an updated [windowsInformationProtectionDeviceRegistration](../resources/intune-mam-windowsinformationprotectiondeviceregistration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="62b35-155">例</span><span class="sxs-lookup"><span data-stu-id="62b35-155">Example</span></span>

### <a name="request"></a><span data-ttu-id="62b35-156">要求</span><span class="sxs-lookup"><span data-stu-id="62b35-156">Request</span></span>
<span data-ttu-id="62b35-157">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="62b35-157">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="62b35-158">応答</span><span class="sxs-lookup"><span data-stu-id="62b35-158">Response</span></span>
<span data-ttu-id="62b35-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="62b35-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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






