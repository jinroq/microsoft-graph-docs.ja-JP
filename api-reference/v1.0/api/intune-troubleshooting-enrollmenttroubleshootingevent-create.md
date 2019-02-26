---
title: enrollmentTroubleshootingEvent の作成
description: 新しい enrollmentTroubleshootingEvent オブジェクトを作成します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: d501a97d7281aad7fe79039d0fb893777c84c446
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/26/2019
ms.locfileid: "30252869"
---
# <a name="create-enrollmenttroubleshootingevent"></a><span data-ttu-id="b1b93-103">enrollmentTroubleshootingEvent の作成</span><span class="sxs-lookup"><span data-stu-id="b1b93-103">Create enrollmentTroubleshootingEvent</span></span>

> <span data-ttu-id="b1b93-104">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="b1b93-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b1b93-105">新しい [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="b1b93-105">Create a new [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b1b93-106">前提条件</span><span class="sxs-lookup"><span data-stu-id="b1b93-106">Prerequisites</span></span>
<span data-ttu-id="b1b93-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/concepts/permissions-reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="b1b93-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="b1b93-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="b1b93-109">Permission type</span></span>|<span data-ttu-id="b1b93-110">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="b1b93-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b1b93-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="b1b93-111">Delegated (work or school account)</span></span>|<span data-ttu-id="b1b93-112">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b1b93-112">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="b1b93-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="b1b93-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b1b93-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b1b93-114">Not supported.</span></span>|
|<span data-ttu-id="b1b93-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="b1b93-115">Application</span></span>|<span data-ttu-id="b1b93-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b1b93-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b1b93-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="b1b93-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/troubleshootingEvents
```

## <a name="request-headers"></a><span data-ttu-id="b1b93-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="b1b93-118">Request headers</span></span>
|<span data-ttu-id="b1b93-119">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="b1b93-119">Header</span></span>|<span data-ttu-id="b1b93-120">値</span><span class="sxs-lookup"><span data-stu-id="b1b93-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b1b93-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="b1b93-121">Authorization</span></span>|<span data-ttu-id="b1b93-122">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="b1b93-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b1b93-123">承諾</span><span class="sxs-lookup"><span data-stu-id="b1b93-123">Accept</span></span>|<span data-ttu-id="b1b93-124">application/json</span><span class="sxs-lookup"><span data-stu-id="b1b93-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b1b93-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="b1b93-125">Request body</span></span>
<span data-ttu-id="b1b93-126">要求本文で、enrollmentTroubleshootingEvent オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="b1b93-126">In the request body, supply a JSON representation for the enrollmentTroubleshootingEvent object.</span></span>

<span data-ttu-id="b1b93-127">次の表に、enrollmentTroubleshootingEvent の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="b1b93-127">The following table shows the properties that are required when you create the enrollmentTroubleshootingEvent.</span></span>

|<span data-ttu-id="b1b93-128">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b1b93-128">Property</span></span>|<span data-ttu-id="b1b93-129">型</span><span class="sxs-lookup"><span data-stu-id="b1b93-129">Type</span></span>|<span data-ttu-id="b1b93-130">説明</span><span class="sxs-lookup"><span data-stu-id="b1b93-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b1b93-131">id</span><span class="sxs-lookup"><span data-stu-id="b1b93-131">id</span></span>|<span data-ttu-id="b1b93-132">String</span><span class="sxs-lookup"><span data-stu-id="b1b93-132">String</span></span>|<span data-ttu-id="b1b93-133">オブジェクトの UUID。[deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md) から継承</span><span class="sxs-lookup"><span data-stu-id="b1b93-133">UUID for the object Inherited from [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="b1b93-134">eventDateTime</span><span class="sxs-lookup"><span data-stu-id="b1b93-134">eventDateTime</span></span>|<span data-ttu-id="b1b93-135">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b1b93-135">DateTimeOffset</span></span>|<span data-ttu-id="b1b93-136">インシデントが発生した時間。</span><span class="sxs-lookup"><span data-stu-id="b1b93-136">Time when the event occurred .</span></span> <span data-ttu-id="b1b93-137">[deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="b1b93-137">Inherited from [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="b1b93-138">correlationId</span><span class="sxs-lookup"><span data-stu-id="b1b93-138">correlationId</span></span>|<span data-ttu-id="b1b93-139">String</span><span class="sxs-lookup"><span data-stu-id="b1b93-139">String</span></span>|<span data-ttu-id="b1b93-140">サービスのエラーをトレースするための ID。</span><span class="sxs-lookup"><span data-stu-id="b1b93-140">Id used for tracing the failure in the service.</span></span> <span data-ttu-id="b1b93-141">[deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="b1b93-141">Inherited from [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="b1b93-142">managedDeviceIdentifier</span><span class="sxs-lookup"><span data-stu-id="b1b93-142">managedDeviceIdentifier</span></span>|<span data-ttu-id="b1b93-143">String</span><span class="sxs-lookup"><span data-stu-id="b1b93-143">String</span></span>|<span data-ttu-id="b1b93-144">Intune によって作成または収集されるデバイス識別子。</span><span class="sxs-lookup"><span data-stu-id="b1b93-144">Device identifier created or collected by Intune.</span></span>|
|<span data-ttu-id="b1b93-145">operatingSystem</span><span class="sxs-lookup"><span data-stu-id="b1b93-145">operatingSystem</span></span>|<span data-ttu-id="b1b93-146">文字列</span><span class="sxs-lookup"><span data-stu-id="b1b93-146">String</span></span>|<span data-ttu-id="b1b93-147">オペレーティング システム。</span><span class="sxs-lookup"><span data-stu-id="b1b93-147">Operating System.</span></span>|
|<span data-ttu-id="b1b93-148">osVersion</span><span class="sxs-lookup"><span data-stu-id="b1b93-148">osVersion</span></span>|<span data-ttu-id="b1b93-149">String</span><span class="sxs-lookup"><span data-stu-id="b1b93-149">String</span></span>|<span data-ttu-id="b1b93-150">OS バージョン。</span><span class="sxs-lookup"><span data-stu-id="b1b93-150">OS Version.</span></span>|
|<span data-ttu-id="b1b93-151">userId</span><span class="sxs-lookup"><span data-stu-id="b1b93-151">userId</span></span>|<span data-ttu-id="b1b93-152">String</span><span class="sxs-lookup"><span data-stu-id="b1b93-152">String</span></span>|<span data-ttu-id="b1b93-153">デバイスを登録しようとするユーザーの識別子。</span><span class="sxs-lookup"><span data-stu-id="b1b93-153">Identifier for the user that tried to enroll the device.</span></span>|
|<span data-ttu-id="b1b93-154">deviceId</span><span class="sxs-lookup"><span data-stu-id="b1b93-154">deviceId</span></span>|<span data-ttu-id="b1b93-155">String</span><span class="sxs-lookup"><span data-stu-id="b1b93-155">String</span></span>|<span data-ttu-id="b1b93-156">Azure AD デバイス識別子。</span><span class="sxs-lookup"><span data-stu-id="b1b93-156">Azure AD device identifier.</span></span>|
|<span data-ttu-id="b1b93-157">enrollmentType</span><span class="sxs-lookup"><span data-stu-id="b1b93-157">enrollmentType</span></span>|[<span data-ttu-id="b1b93-158">deviceEnrollmentType</span><span class="sxs-lookup"><span data-stu-id="b1b93-158">deviceEnrollmentType</span></span>](../resources/intune-shared-deviceenrollmenttype.md)|<span data-ttu-id="b1b93-159">登録の種類。</span><span class="sxs-lookup"><span data-stu-id="b1b93-159">Type of the enrollment.</span></span> <span data-ttu-id="b1b93-160">可能な値は、`unknown`、`userEnrollment`、`deviceEnrollmentManager`、`appleBulkWithUser`、`appleBulkWithoutUser`、`windowsAzureADJoin`、`windowsBulkUserless`、`windowsAutoEnrollment`、`windowsBulkAzureDomainJoin`、`windowsCoManagement` です。</span><span class="sxs-lookup"><span data-stu-id="b1b93-160">Possible values are: `unknown`, `userEnrollment`, `deviceEnrollmentManager`, `appleBulkWithUser`, `appleBulkWithoutUser`, `windowsAzureADJoin`, `windowsBulkUserless`, `windowsAutoEnrollment`, `windowsBulkAzureDomainJoin`, `windowsCoManagement`.</span></span>|
|<span data-ttu-id="b1b93-161">failureCategory</span><span class="sxs-lookup"><span data-stu-id="b1b93-161">failureCategory</span></span>|[<span data-ttu-id="b1b93-162">deviceEnrollmentFailureReason</span><span class="sxs-lookup"><span data-stu-id="b1b93-162">deviceEnrollmentFailureReason</span></span>](../resources/intune-troubleshooting-deviceenrollmentfailurereason.md)|<span data-ttu-id="b1b93-163">高レベルのエラー カテゴリ。</span><span class="sxs-lookup"><span data-stu-id="b1b93-163">Highlevel failure category.</span></span> <span data-ttu-id="b1b93-164">可能な値は、`unknown`、`authentication`、`authorization`、`accountValidation`、`userValidation`、`deviceNotSupported`、`inMaintenance`、`badRequest`、`featureNotSupported`、`enrollmentRestrictionsEnforced`、`clientDisconnected`、`userAbandonment` です。</span><span class="sxs-lookup"><span data-stu-id="b1b93-164">Possible values are: `unknown`, `authentication`, `authorization`, `accountValidation`, `userValidation`, `deviceNotSupported`, `inMaintenance`, `badRequest`, `featureNotSupported`, `enrollmentRestrictionsEnforced`, `clientDisconnected`, `userAbandonment`.</span></span>|
|<span data-ttu-id="b1b93-165">failureReason</span><span class="sxs-lookup"><span data-stu-id="b1b93-165">failureReason</span></span>|<span data-ttu-id="b1b93-166">String</span><span class="sxs-lookup"><span data-stu-id="b1b93-166">String</span></span>|<span data-ttu-id="b1b93-167">詳細なエラーの理由。</span><span class="sxs-lookup"><span data-stu-id="b1b93-167">Detailed failure reason.</span></span>|



## <a name="response"></a><span data-ttu-id="b1b93-168">応答</span><span class="sxs-lookup"><span data-stu-id="b1b93-168">Response</span></span>
<span data-ttu-id="b1b93-169">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="b1b93-169">If successful, this method returns a `201 Created` response code and a [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b1b93-170">例</span><span class="sxs-lookup"><span data-stu-id="b1b93-170">Example</span></span>

### <a name="request"></a><span data-ttu-id="b1b93-171">要求</span><span class="sxs-lookup"><span data-stu-id="b1b93-171">Request</span></span>
<span data-ttu-id="b1b93-172">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="b1b93-172">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="b1b93-173">応答</span><span class="sxs-lookup"><span data-stu-id="b1b93-173">Response</span></span>
<span data-ttu-id="b1b93-p106">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="b1b93-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



