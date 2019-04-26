---
title: enrollmentTroubleshootingEvent の作成
description: 新しい enrollmentTroubleshootingEvent オブジェクトを作成します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 574e9c118601e68acdadeb7d1ccccd929438dbbc
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32576550"
---
# <a name="create-enrollmenttroubleshootingevent"></a><span data-ttu-id="1e006-103">enrollmentTroubleshootingEvent の作成</span><span class="sxs-lookup"><span data-stu-id="1e006-103">Create enrollmentTroubleshootingEvent</span></span>

> <span data-ttu-id="1e006-104">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="1e006-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1e006-105">新しい [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="1e006-105">Create a new [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="1e006-106">前提条件</span><span class="sxs-lookup"><span data-stu-id="1e006-106">Prerequisites</span></span>
<span data-ttu-id="1e006-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="1e006-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1e006-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="1e006-109">Permission type</span></span>|<span data-ttu-id="1e006-110">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="1e006-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1e006-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="1e006-111">Delegated (work or school account)</span></span>|<span data-ttu-id="1e006-112">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1e006-112">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="1e006-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="1e006-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1e006-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="1e006-114">Not supported.</span></span>|
|<span data-ttu-id="1e006-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="1e006-115">Application</span></span>|<span data-ttu-id="1e006-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="1e006-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="1e006-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="1e006-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/troubleshootingEvents
```

## <a name="request-headers"></a><span data-ttu-id="1e006-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="1e006-118">Request headers</span></span>
|<span data-ttu-id="1e006-119">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="1e006-119">Header</span></span>|<span data-ttu-id="1e006-120">値</span><span class="sxs-lookup"><span data-stu-id="1e006-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1e006-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="1e006-121">Authorization</span></span>|<span data-ttu-id="1e006-122">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="1e006-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1e006-123">承諾</span><span class="sxs-lookup"><span data-stu-id="1e006-123">Accept</span></span>|<span data-ttu-id="1e006-124">application/json</span><span class="sxs-lookup"><span data-stu-id="1e006-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1e006-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="1e006-125">Request body</span></span>
<span data-ttu-id="1e006-126">要求本文で、enrollmentTroubleshootingEvent オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="1e006-126">In the request body, supply a JSON representation for the enrollmentTroubleshootingEvent object.</span></span>

<span data-ttu-id="1e006-127">次の表に、enrollmentTroubleshootingEvent の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="1e006-127">The following table shows the properties that are required when you create the enrollmentTroubleshootingEvent.</span></span>

|<span data-ttu-id="1e006-128">プロパティ</span><span class="sxs-lookup"><span data-stu-id="1e006-128">Property</span></span>|<span data-ttu-id="1e006-129">型</span><span class="sxs-lookup"><span data-stu-id="1e006-129">Type</span></span>|<span data-ttu-id="1e006-130">説明</span><span class="sxs-lookup"><span data-stu-id="1e006-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1e006-131">id</span><span class="sxs-lookup"><span data-stu-id="1e006-131">id</span></span>|<span data-ttu-id="1e006-132">String</span><span class="sxs-lookup"><span data-stu-id="1e006-132">String</span></span>|<span data-ttu-id="1e006-133">オブジェクトの UUID。[deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md) から継承</span><span class="sxs-lookup"><span data-stu-id="1e006-133">UUID for the object Inherited from [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="1e006-134">eventDateTime</span><span class="sxs-lookup"><span data-stu-id="1e006-134">eventDateTime</span></span>|<span data-ttu-id="1e006-135">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1e006-135">DateTimeOffset</span></span>|<span data-ttu-id="1e006-136">インシデントが発生した時間。</span><span class="sxs-lookup"><span data-stu-id="1e006-136">Time when the event occurred .</span></span> <span data-ttu-id="1e006-137">[deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="1e006-137">Inherited from [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="1e006-138">correlationId</span><span class="sxs-lookup"><span data-stu-id="1e006-138">correlationId</span></span>|<span data-ttu-id="1e006-139">String</span><span class="sxs-lookup"><span data-stu-id="1e006-139">String</span></span>|<span data-ttu-id="1e006-140">サービスのエラーをトレースするための ID。</span><span class="sxs-lookup"><span data-stu-id="1e006-140">Id used for tracing the failure in the service.</span></span> <span data-ttu-id="1e006-141">[deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="1e006-141">Inherited from [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="1e006-142">managedDeviceIdentifier</span><span class="sxs-lookup"><span data-stu-id="1e006-142">managedDeviceIdentifier</span></span>|<span data-ttu-id="1e006-143">String</span><span class="sxs-lookup"><span data-stu-id="1e006-143">String</span></span>|<span data-ttu-id="1e006-144">Intune によって作成または収集されるデバイス識別子。</span><span class="sxs-lookup"><span data-stu-id="1e006-144">Device identifier created or collected by Intune.</span></span>|
|<span data-ttu-id="1e006-145">operatingSystem</span><span class="sxs-lookup"><span data-stu-id="1e006-145">operatingSystem</span></span>|<span data-ttu-id="1e006-146">文字列</span><span class="sxs-lookup"><span data-stu-id="1e006-146">String</span></span>|<span data-ttu-id="1e006-147">オペレーティング システム。</span><span class="sxs-lookup"><span data-stu-id="1e006-147">Operating System.</span></span>|
|<span data-ttu-id="1e006-148">osVersion</span><span class="sxs-lookup"><span data-stu-id="1e006-148">osVersion</span></span>|<span data-ttu-id="1e006-149">String</span><span class="sxs-lookup"><span data-stu-id="1e006-149">String</span></span>|<span data-ttu-id="1e006-150">OS バージョン。</span><span class="sxs-lookup"><span data-stu-id="1e006-150">OS Version.</span></span>|
|<span data-ttu-id="1e006-151">userId</span><span class="sxs-lookup"><span data-stu-id="1e006-151">userId</span></span>|<span data-ttu-id="1e006-152">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="1e006-152">String</span></span>|<span data-ttu-id="1e006-153">デバイスを登録しようとするユーザーの識別子。</span><span class="sxs-lookup"><span data-stu-id="1e006-153">Identifier for the user that tried to enroll the device.</span></span>|
|<span data-ttu-id="1e006-154">deviceId</span><span class="sxs-lookup"><span data-stu-id="1e006-154">deviceId</span></span>|<span data-ttu-id="1e006-155">String</span><span class="sxs-lookup"><span data-stu-id="1e006-155">String</span></span>|<span data-ttu-id="1e006-156">Azure AD デバイス識別子。</span><span class="sxs-lookup"><span data-stu-id="1e006-156">Azure AD device identifier.</span></span>|
|<span data-ttu-id="1e006-157">enrollmentType</span><span class="sxs-lookup"><span data-stu-id="1e006-157">enrollmentType</span></span>|[<span data-ttu-id="1e006-158">deviceEnrollmentType</span><span class="sxs-lookup"><span data-stu-id="1e006-158">deviceEnrollmentType</span></span>](../resources/intune-shared-deviceenrollmenttype.md)|<span data-ttu-id="1e006-159">登録の種類。</span><span class="sxs-lookup"><span data-stu-id="1e006-159">Type of the enrollment.</span></span> <span data-ttu-id="1e006-160">可能な値は、`unknown`、`userEnrollment`、`deviceEnrollmentManager`、`appleBulkWithUser`、`appleBulkWithoutUser`、`windowsAzureADJoin`、`windowsBulkUserless`、`windowsAutoEnrollment`、`windowsBulkAzureDomainJoin`、`windowsCoManagement` です。</span><span class="sxs-lookup"><span data-stu-id="1e006-160">Possible values are: `unknown`, `userEnrollment`, `deviceEnrollmentManager`, `appleBulkWithUser`, `appleBulkWithoutUser`, `windowsAzureADJoin`, `windowsBulkUserless`, `windowsAutoEnrollment`, `windowsBulkAzureDomainJoin`, `windowsCoManagement`.</span></span>|
|<span data-ttu-id="1e006-161">failureCategory</span><span class="sxs-lookup"><span data-stu-id="1e006-161">failureCategory</span></span>|[<span data-ttu-id="1e006-162">deviceEnrollmentFailureReason</span><span class="sxs-lookup"><span data-stu-id="1e006-162">deviceEnrollmentFailureReason</span></span>](../resources/intune-troubleshooting-deviceenrollmentfailurereason.md)|<span data-ttu-id="1e006-163">高レベルのエラー カテゴリ。</span><span class="sxs-lookup"><span data-stu-id="1e006-163">Highlevel failure category.</span></span> <span data-ttu-id="1e006-164">可能な値は、`unknown`、`authentication`、`authorization`、`accountValidation`、`userValidation`、`deviceNotSupported`、`inMaintenance`、`badRequest`、`featureNotSupported`、`enrollmentRestrictionsEnforced`、`clientDisconnected`、`userAbandonment` です。</span><span class="sxs-lookup"><span data-stu-id="1e006-164">Possible values are: `unknown`, `authentication`, `authorization`, `accountValidation`, `userValidation`, `deviceNotSupported`, `inMaintenance`, `badRequest`, `featureNotSupported`, `enrollmentRestrictionsEnforced`, `clientDisconnected`, `userAbandonment`.</span></span>|
|<span data-ttu-id="1e006-165">failureReason</span><span class="sxs-lookup"><span data-stu-id="1e006-165">failureReason</span></span>|<span data-ttu-id="1e006-166">String</span><span class="sxs-lookup"><span data-stu-id="1e006-166">String</span></span>|<span data-ttu-id="1e006-167">詳細なエラーの理由。</span><span class="sxs-lookup"><span data-stu-id="1e006-167">Detailed failure reason.</span></span>|



## <a name="response"></a><span data-ttu-id="1e006-168">応答</span><span class="sxs-lookup"><span data-stu-id="1e006-168">Response</span></span>
<span data-ttu-id="1e006-169">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="1e006-169">If successful, this method returns a `201 Created` response code and a [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1e006-170">例</span><span class="sxs-lookup"><span data-stu-id="1e006-170">Example</span></span>

### <a name="request"></a><span data-ttu-id="1e006-171">要求</span><span class="sxs-lookup"><span data-stu-id="1e006-171">Request</span></span>
<span data-ttu-id="1e006-172">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="1e006-172">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/troubleshootingEvents
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

### <a name="response"></a><span data-ttu-id="1e006-173">応答</span><span class="sxs-lookup"><span data-stu-id="1e006-173">Response</span></span>
<span data-ttu-id="1e006-p106">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="1e006-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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



