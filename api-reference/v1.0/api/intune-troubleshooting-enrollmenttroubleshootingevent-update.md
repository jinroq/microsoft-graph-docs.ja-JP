---
title: enrollmentTroubleshootingEvent の更新
description: enrollmentTroubleshootingEvent オブジェクトのプロパティを更新します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: a16a24a27a56ab1a733b46fa9ad9b7469f0a8ee3
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32576445"
---
# <a name="update-enrollmenttroubleshootingevent"></a><span data-ttu-id="bb9ca-103">enrollmentTroubleshootingEvent の更新</span><span class="sxs-lookup"><span data-stu-id="bb9ca-103">Update enrollmentTroubleshootingEvent</span></span>

> <span data-ttu-id="bb9ca-104">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="bb9ca-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bb9ca-105">[enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="bb9ca-105">Update the properties of a [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="bb9ca-106">前提条件</span><span class="sxs-lookup"><span data-stu-id="bb9ca-106">Prerequisites</span></span>
<span data-ttu-id="bb9ca-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="bb9ca-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bb9ca-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="bb9ca-109">Permission type</span></span>|<span data-ttu-id="bb9ca-110">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="bb9ca-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="bb9ca-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="bb9ca-111">Delegated (work or school account)</span></span>|<span data-ttu-id="bb9ca-112">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bb9ca-112">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="bb9ca-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="bb9ca-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="bb9ca-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="bb9ca-114">Not supported.</span></span>|
|<span data-ttu-id="bb9ca-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="bb9ca-115">Application</span></span>|<span data-ttu-id="bb9ca-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="bb9ca-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="bb9ca-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="bb9ca-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/troubleshootingEvents/{deviceManagementTroubleshootingEventId}
```

## <a name="request-headers"></a><span data-ttu-id="bb9ca-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="bb9ca-118">Request headers</span></span>
|<span data-ttu-id="bb9ca-119">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="bb9ca-119">Header</span></span>|<span data-ttu-id="bb9ca-120">値</span><span class="sxs-lookup"><span data-stu-id="bb9ca-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="bb9ca-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="bb9ca-121">Authorization</span></span>|<span data-ttu-id="bb9ca-122">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="bb9ca-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="bb9ca-123">承諾</span><span class="sxs-lookup"><span data-stu-id="bb9ca-123">Accept</span></span>|<span data-ttu-id="bb9ca-124">application/json</span><span class="sxs-lookup"><span data-stu-id="bb9ca-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="bb9ca-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="bb9ca-125">Request body</span></span>
<span data-ttu-id="bb9ca-126">要求本文で、[enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="bb9ca-126">In the request body, supply a JSON representation for the [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md) object.</span></span>

<span data-ttu-id="bb9ca-127">次の表に、[enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md) の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="bb9ca-127">The following table shows the properties that are required when you create the [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md).</span></span>

|<span data-ttu-id="bb9ca-128">プロパティ</span><span class="sxs-lookup"><span data-stu-id="bb9ca-128">Property</span></span>|<span data-ttu-id="bb9ca-129">型</span><span class="sxs-lookup"><span data-stu-id="bb9ca-129">Type</span></span>|<span data-ttu-id="bb9ca-130">説明</span><span class="sxs-lookup"><span data-stu-id="bb9ca-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bb9ca-131">id</span><span class="sxs-lookup"><span data-stu-id="bb9ca-131">id</span></span>|<span data-ttu-id="bb9ca-132">String</span><span class="sxs-lookup"><span data-stu-id="bb9ca-132">String</span></span>|<span data-ttu-id="bb9ca-133">オブジェクトの UUID。[deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md) から継承</span><span class="sxs-lookup"><span data-stu-id="bb9ca-133">UUID for the object Inherited from [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="bb9ca-134">eventDateTime</span><span class="sxs-lookup"><span data-stu-id="bb9ca-134">eventDateTime</span></span>|<span data-ttu-id="bb9ca-135">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bb9ca-135">DateTimeOffset</span></span>|<span data-ttu-id="bb9ca-136">インシデントが発生した時間。</span><span class="sxs-lookup"><span data-stu-id="bb9ca-136">Time when the event occurred .</span></span> <span data-ttu-id="bb9ca-137">[deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="bb9ca-137">Inherited from [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="bb9ca-138">correlationId</span><span class="sxs-lookup"><span data-stu-id="bb9ca-138">correlationId</span></span>|<span data-ttu-id="bb9ca-139">String</span><span class="sxs-lookup"><span data-stu-id="bb9ca-139">String</span></span>|<span data-ttu-id="bb9ca-140">サービスのエラーをトレースするための ID。</span><span class="sxs-lookup"><span data-stu-id="bb9ca-140">Id used for tracing the failure in the service.</span></span> <span data-ttu-id="bb9ca-141">[deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="bb9ca-141">Inherited from [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="bb9ca-142">managedDeviceIdentifier</span><span class="sxs-lookup"><span data-stu-id="bb9ca-142">managedDeviceIdentifier</span></span>|<span data-ttu-id="bb9ca-143">String</span><span class="sxs-lookup"><span data-stu-id="bb9ca-143">String</span></span>|<span data-ttu-id="bb9ca-144">Intune によって作成または収集されるデバイス識別子。</span><span class="sxs-lookup"><span data-stu-id="bb9ca-144">Device identifier created or collected by Intune.</span></span>|
|<span data-ttu-id="bb9ca-145">operatingSystem</span><span class="sxs-lookup"><span data-stu-id="bb9ca-145">operatingSystem</span></span>|<span data-ttu-id="bb9ca-146">文字列</span><span class="sxs-lookup"><span data-stu-id="bb9ca-146">String</span></span>|<span data-ttu-id="bb9ca-147">オペレーティング システム。</span><span class="sxs-lookup"><span data-stu-id="bb9ca-147">Operating System.</span></span>|
|<span data-ttu-id="bb9ca-148">osVersion</span><span class="sxs-lookup"><span data-stu-id="bb9ca-148">osVersion</span></span>|<span data-ttu-id="bb9ca-149">String</span><span class="sxs-lookup"><span data-stu-id="bb9ca-149">String</span></span>|<span data-ttu-id="bb9ca-150">OS バージョン。</span><span class="sxs-lookup"><span data-stu-id="bb9ca-150">OS Version.</span></span>|
|<span data-ttu-id="bb9ca-151">userId</span><span class="sxs-lookup"><span data-stu-id="bb9ca-151">userId</span></span>|<span data-ttu-id="bb9ca-152">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="bb9ca-152">String</span></span>|<span data-ttu-id="bb9ca-153">デバイスを登録しようとするユーザーの識別子。</span><span class="sxs-lookup"><span data-stu-id="bb9ca-153">Identifier for the user that tried to enroll the device.</span></span>|
|<span data-ttu-id="bb9ca-154">deviceId</span><span class="sxs-lookup"><span data-stu-id="bb9ca-154">deviceId</span></span>|<span data-ttu-id="bb9ca-155">String</span><span class="sxs-lookup"><span data-stu-id="bb9ca-155">String</span></span>|<span data-ttu-id="bb9ca-156">Azure AD デバイス識別子。</span><span class="sxs-lookup"><span data-stu-id="bb9ca-156">Azure AD device identifier.</span></span>|
|<span data-ttu-id="bb9ca-157">enrollmentType</span><span class="sxs-lookup"><span data-stu-id="bb9ca-157">enrollmentType</span></span>|[<span data-ttu-id="bb9ca-158">deviceEnrollmentType</span><span class="sxs-lookup"><span data-stu-id="bb9ca-158">deviceEnrollmentType</span></span>](../resources/intune-shared-deviceenrollmenttype.md)|<span data-ttu-id="bb9ca-159">登録の種類。</span><span class="sxs-lookup"><span data-stu-id="bb9ca-159">Type of the enrollment.</span></span> <span data-ttu-id="bb9ca-160">可能な値は、`unknown`、`userEnrollment`、`deviceEnrollmentManager`、`appleBulkWithUser`、`appleBulkWithoutUser`、`windowsAzureADJoin`、`windowsBulkUserless`、`windowsAutoEnrollment`、`windowsBulkAzureDomainJoin`、`windowsCoManagement` です。</span><span class="sxs-lookup"><span data-stu-id="bb9ca-160">Possible values are: `unknown`, `userEnrollment`, `deviceEnrollmentManager`, `appleBulkWithUser`, `appleBulkWithoutUser`, `windowsAzureADJoin`, `windowsBulkUserless`, `windowsAutoEnrollment`, `windowsBulkAzureDomainJoin`, `windowsCoManagement`.</span></span>|
|<span data-ttu-id="bb9ca-161">failureCategory</span><span class="sxs-lookup"><span data-stu-id="bb9ca-161">failureCategory</span></span>|[<span data-ttu-id="bb9ca-162">deviceEnrollmentFailureReason</span><span class="sxs-lookup"><span data-stu-id="bb9ca-162">deviceEnrollmentFailureReason</span></span>](../resources/intune-troubleshooting-deviceenrollmentfailurereason.md)|<span data-ttu-id="bb9ca-163">高レベルのエラー カテゴリ。</span><span class="sxs-lookup"><span data-stu-id="bb9ca-163">Highlevel failure category.</span></span> <span data-ttu-id="bb9ca-164">可能な値は、`unknown`、`authentication`、`authorization`、`accountValidation`、`userValidation`、`deviceNotSupported`、`inMaintenance`、`badRequest`、`featureNotSupported`、`enrollmentRestrictionsEnforced`、`clientDisconnected`、`userAbandonment` です。</span><span class="sxs-lookup"><span data-stu-id="bb9ca-164">Possible values are: `unknown`, `authentication`, `authorization`, `accountValidation`, `userValidation`, `deviceNotSupported`, `inMaintenance`, `badRequest`, `featureNotSupported`, `enrollmentRestrictionsEnforced`, `clientDisconnected`, `userAbandonment`.</span></span>|
|<span data-ttu-id="bb9ca-165">failureReason</span><span class="sxs-lookup"><span data-stu-id="bb9ca-165">failureReason</span></span>|<span data-ttu-id="bb9ca-166">String</span><span class="sxs-lookup"><span data-stu-id="bb9ca-166">String</span></span>|<span data-ttu-id="bb9ca-167">詳細なエラーの理由。</span><span class="sxs-lookup"><span data-stu-id="bb9ca-167">Detailed failure reason.</span></span>|



## <a name="response"></a><span data-ttu-id="bb9ca-168">応答</span><span class="sxs-lookup"><span data-stu-id="bb9ca-168">Response</span></span>
<span data-ttu-id="bb9ca-169">成功した場合、このメソッドは `200 OK` 応答コードと、更新された [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md) オブジェクトを応答本文で返します。</span><span class="sxs-lookup"><span data-stu-id="bb9ca-169">If successful, this method returns a `200 OK` response code and an updated [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bb9ca-170">例</span><span class="sxs-lookup"><span data-stu-id="bb9ca-170">Example</span></span>

### <a name="request"></a><span data-ttu-id="bb9ca-171">要求</span><span class="sxs-lookup"><span data-stu-id="bb9ca-171">Request</span></span>
<span data-ttu-id="bb9ca-172">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="bb9ca-172">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="bb9ca-173">応答</span><span class="sxs-lookup"><span data-stu-id="bb9ca-173">Response</span></span>
<span data-ttu-id="bb9ca-p106">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="bb9ca-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



