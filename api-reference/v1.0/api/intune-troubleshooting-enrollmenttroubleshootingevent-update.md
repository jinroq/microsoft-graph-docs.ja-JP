---
title: enrollmentTroubleshootingEvent の更新
description: enrollmentTroubleshootingEvent オブジェクトのプロパティを更新します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: e17167d2965102618d0033210a69b39db16686a8
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36025639"
---
# <a name="update-enrollmenttroubleshootingevent"></a><span data-ttu-id="64b48-103">enrollmentTroubleshootingEvent の更新</span><span class="sxs-lookup"><span data-stu-id="64b48-103">Update enrollmentTroubleshootingEvent</span></span>

> <span data-ttu-id="64b48-104">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="64b48-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="64b48-105">[enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="64b48-105">Update the properties of a [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="64b48-106">前提条件</span><span class="sxs-lookup"><span data-stu-id="64b48-106">Prerequisites</span></span>
<span data-ttu-id="64b48-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="64b48-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="64b48-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="64b48-109">Permission type</span></span>|<span data-ttu-id="64b48-110">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="64b48-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="64b48-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="64b48-111">Delegated (work or school account)</span></span>|<span data-ttu-id="64b48-112">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="64b48-112">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="64b48-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="64b48-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="64b48-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="64b48-114">Not supported.</span></span>|
|<span data-ttu-id="64b48-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="64b48-115">Application</span></span>|<span data-ttu-id="64b48-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="64b48-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="64b48-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="64b48-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/troubleshootingEvents/{deviceManagementTroubleshootingEventId}
```

## <a name="request-headers"></a><span data-ttu-id="64b48-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="64b48-118">Request headers</span></span>
|<span data-ttu-id="64b48-119">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="64b48-119">Header</span></span>|<span data-ttu-id="64b48-120">値</span><span class="sxs-lookup"><span data-stu-id="64b48-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="64b48-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="64b48-121">Authorization</span></span>|<span data-ttu-id="64b48-122">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="64b48-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="64b48-123">承諾</span><span class="sxs-lookup"><span data-stu-id="64b48-123">Accept</span></span>|<span data-ttu-id="64b48-124">application/json</span><span class="sxs-lookup"><span data-stu-id="64b48-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="64b48-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="64b48-125">Request body</span></span>
<span data-ttu-id="64b48-126">要求本文で、[enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="64b48-126">In the request body, supply a JSON representation for the [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md) object.</span></span>

<span data-ttu-id="64b48-127">次の表に、[enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md) の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="64b48-127">The following table shows the properties that are required when you create the [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md).</span></span>

|<span data-ttu-id="64b48-128">プロパティ</span><span class="sxs-lookup"><span data-stu-id="64b48-128">Property</span></span>|<span data-ttu-id="64b48-129">型</span><span class="sxs-lookup"><span data-stu-id="64b48-129">Type</span></span>|<span data-ttu-id="64b48-130">説明</span><span class="sxs-lookup"><span data-stu-id="64b48-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="64b48-131">id</span><span class="sxs-lookup"><span data-stu-id="64b48-131">id</span></span>|<span data-ttu-id="64b48-132">文字列</span><span class="sxs-lookup"><span data-stu-id="64b48-132">String</span></span>|<span data-ttu-id="64b48-133">オブジェクトの UUID。[deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md) から継承</span><span class="sxs-lookup"><span data-stu-id="64b48-133">UUID for the object Inherited from [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="64b48-134">eventDateTime</span><span class="sxs-lookup"><span data-stu-id="64b48-134">eventDateTime</span></span>|<span data-ttu-id="64b48-135">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="64b48-135">DateTimeOffset</span></span>|<span data-ttu-id="64b48-136">インシデントが発生した時間。</span><span class="sxs-lookup"><span data-stu-id="64b48-136">Time when the event occurred .</span></span> <span data-ttu-id="64b48-137">[deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="64b48-137">Inherited from [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="64b48-138">correlationId</span><span class="sxs-lookup"><span data-stu-id="64b48-138">correlationId</span></span>|<span data-ttu-id="64b48-139">String</span><span class="sxs-lookup"><span data-stu-id="64b48-139">String</span></span>|<span data-ttu-id="64b48-140">サービスのエラーをトレースするための ID。</span><span class="sxs-lookup"><span data-stu-id="64b48-140">Id used for tracing the failure in the service.</span></span> <span data-ttu-id="64b48-141">[deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="64b48-141">Inherited from [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="64b48-142">managedDeviceIdentifier</span><span class="sxs-lookup"><span data-stu-id="64b48-142">managedDeviceIdentifier</span></span>|<span data-ttu-id="64b48-143">String</span><span class="sxs-lookup"><span data-stu-id="64b48-143">String</span></span>|<span data-ttu-id="64b48-144">Intune によって作成または収集されるデバイス識別子。</span><span class="sxs-lookup"><span data-stu-id="64b48-144">Device identifier created or collected by Intune.</span></span>|
|<span data-ttu-id="64b48-145">operatingSystem</span><span class="sxs-lookup"><span data-stu-id="64b48-145">operatingSystem</span></span>|<span data-ttu-id="64b48-146">文字列</span><span class="sxs-lookup"><span data-stu-id="64b48-146">String</span></span>|<span data-ttu-id="64b48-147">オペレーティング システム。</span><span class="sxs-lookup"><span data-stu-id="64b48-147">Operating System.</span></span>|
|<span data-ttu-id="64b48-148">osVersion</span><span class="sxs-lookup"><span data-stu-id="64b48-148">osVersion</span></span>|<span data-ttu-id="64b48-149">String</span><span class="sxs-lookup"><span data-stu-id="64b48-149">String</span></span>|<span data-ttu-id="64b48-150">OS バージョン。</span><span class="sxs-lookup"><span data-stu-id="64b48-150">OS Version.</span></span>|
|<span data-ttu-id="64b48-151">userId</span><span class="sxs-lookup"><span data-stu-id="64b48-151">userId</span></span>|<span data-ttu-id="64b48-152">String</span><span class="sxs-lookup"><span data-stu-id="64b48-152">String</span></span>|<span data-ttu-id="64b48-153">デバイスを登録しようとするユーザーの識別子。</span><span class="sxs-lookup"><span data-stu-id="64b48-153">Identifier for the user that tried to enroll the device.</span></span>|
|<span data-ttu-id="64b48-154">deviceId</span><span class="sxs-lookup"><span data-stu-id="64b48-154">deviceId</span></span>|<span data-ttu-id="64b48-155">String</span><span class="sxs-lookup"><span data-stu-id="64b48-155">String</span></span>|<span data-ttu-id="64b48-156">Azure AD デバイス識別子。</span><span class="sxs-lookup"><span data-stu-id="64b48-156">Azure AD device identifier.</span></span>|
|<span data-ttu-id="64b48-157">enrollmentType</span><span class="sxs-lookup"><span data-stu-id="64b48-157">enrollmentType</span></span>|[<span data-ttu-id="64b48-158">deviceEnrollmentType</span><span class="sxs-lookup"><span data-stu-id="64b48-158">deviceEnrollmentType</span></span>](../resources/intune-shared-deviceenrollmenttype.md)|<span data-ttu-id="64b48-159">登録の種類。</span><span class="sxs-lookup"><span data-stu-id="64b48-159">Type of the enrollment.</span></span> <span data-ttu-id="64b48-160">可能な値は、`unknown`、`userEnrollment`、`deviceEnrollmentManager`、`appleBulkWithUser`、`appleBulkWithoutUser`、`windowsAzureADJoin`、`windowsBulkUserless`、`windowsAutoEnrollment`、`windowsBulkAzureDomainJoin`、`windowsCoManagement` です。</span><span class="sxs-lookup"><span data-stu-id="64b48-160">Possible values are: `unknown`, `userEnrollment`, `deviceEnrollmentManager`, `appleBulkWithUser`, `appleBulkWithoutUser`, `windowsAzureADJoin`, `windowsBulkUserless`, `windowsAutoEnrollment`, `windowsBulkAzureDomainJoin`, `windowsCoManagement`.</span></span>|
|<span data-ttu-id="64b48-161">failureCategory</span><span class="sxs-lookup"><span data-stu-id="64b48-161">failureCategory</span></span>|[<span data-ttu-id="64b48-162">deviceEnrollmentFailureReason</span><span class="sxs-lookup"><span data-stu-id="64b48-162">deviceEnrollmentFailureReason</span></span>](../resources/intune-troubleshooting-deviceenrollmentfailurereason.md)|<span data-ttu-id="64b48-163">高レベルのエラー カテゴリ。</span><span class="sxs-lookup"><span data-stu-id="64b48-163">Highlevel failure category.</span></span> <span data-ttu-id="64b48-164">可能な値は、`unknown`、`authentication`、`authorization`、`accountValidation`、`userValidation`、`deviceNotSupported`、`inMaintenance`、`badRequest`、`featureNotSupported`、`enrollmentRestrictionsEnforced`、`clientDisconnected`、`userAbandonment` です。</span><span class="sxs-lookup"><span data-stu-id="64b48-164">Possible values are: `unknown`, `authentication`, `authorization`, `accountValidation`, `userValidation`, `deviceNotSupported`, `inMaintenance`, `badRequest`, `featureNotSupported`, `enrollmentRestrictionsEnforced`, `clientDisconnected`, `userAbandonment`.</span></span>|
|<span data-ttu-id="64b48-165">failureReason</span><span class="sxs-lookup"><span data-stu-id="64b48-165">failureReason</span></span>|<span data-ttu-id="64b48-166">String</span><span class="sxs-lookup"><span data-stu-id="64b48-166">String</span></span>|<span data-ttu-id="64b48-167">詳細なエラーの理由。</span><span class="sxs-lookup"><span data-stu-id="64b48-167">Detailed failure reason.</span></span>|



## <a name="response"></a><span data-ttu-id="64b48-168">応答</span><span class="sxs-lookup"><span data-stu-id="64b48-168">Response</span></span>
<span data-ttu-id="64b48-169">成功した場合、このメソッドは `200 OK` 応答コードと、更新された [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md) オブジェクトを応答本文で返します。</span><span class="sxs-lookup"><span data-stu-id="64b48-169">If successful, this method returns a `200 OK` response code and an updated [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="64b48-170">例</span><span class="sxs-lookup"><span data-stu-id="64b48-170">Example</span></span>

### <a name="request"></a><span data-ttu-id="64b48-171">要求</span><span class="sxs-lookup"><span data-stu-id="64b48-171">Request</span></span>
<span data-ttu-id="64b48-172">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="64b48-172">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/troubleshootingEvents/{deviceManagementTroubleshootingEventId}
Content-type: application/json
Content-length: 509

{
  "@odata.type": "#microsoft.graph.enrollmentTroubleshootingEvent",
  "eventDateTime": "2016-12-31T23:59:23.3984029-08:00",
  "correlationId": "Correlation Id value",
  "managedDeviceIdentifier": "Managed Device Identifier value",
  "operatingSystem": "Operating System value",
  "osVersion": "Os Version value",
  "userId": "User Id value",
  "deviceId": "Device Id value",
  "enrollmentType": "userEnrollment",
  "failureCategory": "authentication",
  "failureReason": "Failure Reason value"
}
```

### <a name="response"></a><span data-ttu-id="64b48-173">応答</span><span class="sxs-lookup"><span data-stu-id="64b48-173">Response</span></span>
<span data-ttu-id="64b48-p106">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="64b48-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 558

{
  "@odata.type": "#microsoft.graph.enrollmentTroubleshootingEvent",
  "id": "c4a623f5-23f5-c4a6-f523-a6c4f523a6c4",
  "eventDateTime": "2016-12-31T23:59:23.3984029-08:00",
  "correlationId": "Correlation Id value",
  "managedDeviceIdentifier": "Managed Device Identifier value",
  "operatingSystem": "Operating System value",
  "osVersion": "Os Version value",
  "userId": "User Id value",
  "deviceId": "Device Id value",
  "enrollmentType": "userEnrollment",
  "failureCategory": "authentication",
  "failureReason": "Failure Reason value"
}
```



