---
title: enrollmentTroubleshootingEvent の更新
description: enrollmentTroubleshootingEvent オブジェクトのプロパティを更新します。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 33f4a789834ee7fdc84c000d065df932203efb0a
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27914473"
---
# <a name="update-enrollmenttroubleshootingevent"></a><span data-ttu-id="605a2-103">enrollmentTroubleshootingEvent の更新</span><span class="sxs-lookup"><span data-stu-id="605a2-103">Update enrollmentTroubleshootingEvent</span></span>

> <span data-ttu-id="605a2-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="605a2-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="605a2-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="605a2-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="605a2-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="605a2-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="605a2-107">[enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="605a2-107">Update the properties of a [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="605a2-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="605a2-108">Prerequisites</span></span>
<span data-ttu-id="605a2-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="605a2-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="605a2-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="605a2-111">Permission type</span></span>|<span data-ttu-id="605a2-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="605a2-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="605a2-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="605a2-113">Delegated (work or school account)</span></span>|<span data-ttu-id="605a2-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="605a2-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="605a2-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="605a2-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="605a2-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="605a2-116">Not supported.</span></span>|
|<span data-ttu-id="605a2-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="605a2-117">Application</span></span>|<span data-ttu-id="605a2-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="605a2-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="605a2-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="605a2-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/troubleshootingEvents/{deviceManagementTroubleshootingEventId}
```

## <a name="request-headers"></a><span data-ttu-id="605a2-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="605a2-120">Request headers</span></span>
|<span data-ttu-id="605a2-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="605a2-121">Header</span></span>|<span data-ttu-id="605a2-122">値</span><span class="sxs-lookup"><span data-stu-id="605a2-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="605a2-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="605a2-123">Authorization</span></span>|<span data-ttu-id="605a2-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="605a2-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="605a2-125">Accept</span><span class="sxs-lookup"><span data-stu-id="605a2-125">Accept</span></span>|<span data-ttu-id="605a2-126">application/json</span><span class="sxs-lookup"><span data-stu-id="605a2-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="605a2-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="605a2-127">Request body</span></span>
<span data-ttu-id="605a2-128">要求本文で、[enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="605a2-128">In the request body, supply a JSON representation for the [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md) object.</span></span>

<span data-ttu-id="605a2-129">次の表に、[enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md) の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="605a2-129">The following table shows the properties that are required when you create the [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md).</span></span>

|<span data-ttu-id="605a2-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="605a2-130">Property</span></span>|<span data-ttu-id="605a2-131">型</span><span class="sxs-lookup"><span data-stu-id="605a2-131">Type</span></span>|<span data-ttu-id="605a2-132">説明</span><span class="sxs-lookup"><span data-stu-id="605a2-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="605a2-133">ID</span><span class="sxs-lookup"><span data-stu-id="605a2-133">id</span></span>|<span data-ttu-id="605a2-134">String</span><span class="sxs-lookup"><span data-stu-id="605a2-134">String</span></span>|<span data-ttu-id="605a2-135">オブジェクトの UUID。[deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md) から継承</span><span class="sxs-lookup"><span data-stu-id="605a2-135">UUID for the object Inherited from [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="605a2-136">eventDateTime</span><span class="sxs-lookup"><span data-stu-id="605a2-136">eventDateTime</span></span>|<span data-ttu-id="605a2-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="605a2-137">DateTimeOffset</span></span>|<span data-ttu-id="605a2-138">インシデントが発生した時間。</span><span class="sxs-lookup"><span data-stu-id="605a2-138">Time when the event occurred .</span></span> <span data-ttu-id="605a2-139">[deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="605a2-139">Inherited from [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="605a2-140">correlationId</span><span class="sxs-lookup"><span data-stu-id="605a2-140">correlationId</span></span>|<span data-ttu-id="605a2-141">String</span><span class="sxs-lookup"><span data-stu-id="605a2-141">String</span></span>|<span data-ttu-id="605a2-142">サービスのエラーをトレースするための ID。</span><span class="sxs-lookup"><span data-stu-id="605a2-142">Id used for tracing the failure in the service.</span></span> <span data-ttu-id="605a2-143">[deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="605a2-143">Inherited from [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="605a2-144">managedDeviceIdentifier</span><span class="sxs-lookup"><span data-stu-id="605a2-144">managedDeviceIdentifier</span></span>|<span data-ttu-id="605a2-145">String</span><span class="sxs-lookup"><span data-stu-id="605a2-145">String</span></span>|<span data-ttu-id="605a2-146">Intune によって作成または収集されるデバイス識別子。</span><span class="sxs-lookup"><span data-stu-id="605a2-146">Device identifier created or collected by Intune.</span></span>|
|<span data-ttu-id="605a2-147">operatingSystem</span><span class="sxs-lookup"><span data-stu-id="605a2-147">operatingSystem</span></span>|<span data-ttu-id="605a2-148">String</span><span class="sxs-lookup"><span data-stu-id="605a2-148">String</span></span>|<span data-ttu-id="605a2-149">オペレーティング システム。</span><span class="sxs-lookup"><span data-stu-id="605a2-149">Operating System.</span></span>|
|<span data-ttu-id="605a2-150">osVersion</span><span class="sxs-lookup"><span data-stu-id="605a2-150">osVersion</span></span>|<span data-ttu-id="605a2-151">String</span><span class="sxs-lookup"><span data-stu-id="605a2-151">String</span></span>|<span data-ttu-id="605a2-152">OS バージョン。</span><span class="sxs-lookup"><span data-stu-id="605a2-152">OS Version.</span></span>|
|<span data-ttu-id="605a2-153">userId</span><span class="sxs-lookup"><span data-stu-id="605a2-153">userId</span></span>|<span data-ttu-id="605a2-154">String</span><span class="sxs-lookup"><span data-stu-id="605a2-154">String</span></span>|<span data-ttu-id="605a2-155">デバイスを登録しようとするユーザーの識別子。</span><span class="sxs-lookup"><span data-stu-id="605a2-155">Identifier for the user that tried to enroll the device.</span></span>|
|<span data-ttu-id="605a2-156">deviceId</span><span class="sxs-lookup"><span data-stu-id="605a2-156">deviceId</span></span>|<span data-ttu-id="605a2-157">String</span><span class="sxs-lookup"><span data-stu-id="605a2-157">String</span></span>|<span data-ttu-id="605a2-158">Azure AD デバイス識別子。</span><span class="sxs-lookup"><span data-stu-id="605a2-158">Azure AD device identifier.</span></span>|
|<span data-ttu-id="605a2-159">enrollmentType</span><span class="sxs-lookup"><span data-stu-id="605a2-159">enrollmentType</span></span>|[<span data-ttu-id="605a2-160">deviceEnrollmentType</span><span class="sxs-lookup"><span data-stu-id="605a2-160">deviceEnrollmentType</span></span>](../resources/intune-shared-deviceenrollmenttype.md)|<span data-ttu-id="605a2-161">登録の種類。</span><span class="sxs-lookup"><span data-stu-id="605a2-161">Type of the enrollment.</span></span> <span data-ttu-id="605a2-162">可能な値は、`unknown`、`userEnrollment`、`deviceEnrollmentManager`、`appleBulkWithUser`、`appleBulkWithoutUser`、`windowsAzureADJoin`、`windowsBulkUserless`、`windowsAutoEnrollment`、`windowsBulkAzureDomainJoin`、`windowsCoManagement` です。</span><span class="sxs-lookup"><span data-stu-id="605a2-162">Possible values are: `unknown`, `userEnrollment`, `deviceEnrollmentManager`, `appleBulkWithUser`, `appleBulkWithoutUser`, `windowsAzureADJoin`, `windowsBulkUserless`, `windowsAutoEnrollment`, `windowsBulkAzureDomainJoin`, `windowsCoManagement`.</span></span>|
|<span data-ttu-id="605a2-163">failureCategory</span><span class="sxs-lookup"><span data-stu-id="605a2-163">failureCategory</span></span>|[<span data-ttu-id="605a2-164">deviceEnrollmentFailureReason</span><span class="sxs-lookup"><span data-stu-id="605a2-164">deviceEnrollmentFailureReason</span></span>](../resources/intune-troubleshooting-deviceenrollmentfailurereason.md)|<span data-ttu-id="605a2-165">高レベルのエラー カテゴリ。</span><span class="sxs-lookup"><span data-stu-id="605a2-165">Highlevel failure category.</span></span> <span data-ttu-id="605a2-166">可能な値は、`unknown`、`authentication`、`authorization`、`accountValidation`、`userValidation`、`deviceNotSupported`、`inMaintenance`、`badRequest`、`featureNotSupported`、`enrollmentRestrictionsEnforced`、`clientDisconnected`、`userAbandonment` です。</span><span class="sxs-lookup"><span data-stu-id="605a2-166">Possible values are: `unknown`, `authentication`, `authorization`, `accountValidation`, `userValidation`, `deviceNotSupported`, `inMaintenance`, `badRequest`, `featureNotSupported`, `enrollmentRestrictionsEnforced`, `clientDisconnected`, `userAbandonment`.</span></span>|
|<span data-ttu-id="605a2-167">failureReason</span><span class="sxs-lookup"><span data-stu-id="605a2-167">failureReason</span></span>|<span data-ttu-id="605a2-168">String</span><span class="sxs-lookup"><span data-stu-id="605a2-168">String</span></span>|<span data-ttu-id="605a2-169">詳細なエラーの理由。</span><span class="sxs-lookup"><span data-stu-id="605a2-169">Detailed failure reason.</span></span>|



## <a name="response"></a><span data-ttu-id="605a2-170">応答</span><span class="sxs-lookup"><span data-stu-id="605a2-170">Response</span></span>
<span data-ttu-id="605a2-171">成功した場合、このメソッドは `200 OK` 応答コードと、更新された [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md) オブジェクトを応答本文で返します。</span><span class="sxs-lookup"><span data-stu-id="605a2-171">If successful, this method returns a `200 OK` response code and an updated [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="605a2-172">例</span><span class="sxs-lookup"><span data-stu-id="605a2-172">Example</span></span>
### <a name="request"></a><span data-ttu-id="605a2-173">要求</span><span class="sxs-lookup"><span data-stu-id="605a2-173">Request</span></span>
<span data-ttu-id="605a2-174">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="605a2-174">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/troubleshootingEvents/{deviceManagementTroubleshootingEventId}
Content-type: application/json
Content-length: 440

{
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

### <a name="response"></a><span data-ttu-id="605a2-175">応答</span><span class="sxs-lookup"><span data-stu-id="605a2-175">Response</span></span>
<span data-ttu-id="605a2-p107">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="605a2-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





