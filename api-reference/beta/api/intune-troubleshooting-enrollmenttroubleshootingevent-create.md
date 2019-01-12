---
title: enrollmentTroubleshootingEvent の作成
description: 新しい enrollmentTroubleshootingEvent オブジェクトを作成します。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 8ae80e2084945b1dd5fb0259b16b178ab2d38ec5
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27924567"
---
# <a name="create-enrollmenttroubleshootingevent"></a><span data-ttu-id="5b51e-103">enrollmentTroubleshootingEvent の作成</span><span class="sxs-lookup"><span data-stu-id="5b51e-103">Create enrollmentTroubleshootingEvent</span></span>

> <span data-ttu-id="5b51e-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中で、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="5b51e-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="5b51e-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="5b51e-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="5b51e-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="5b51e-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="5b51e-107">新しい [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="5b51e-107">Create a new [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="5b51e-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="5b51e-108">Prerequisites</span></span>
<span data-ttu-id="5b51e-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="5b51e-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5b51e-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="5b51e-111">Permission type</span></span>|<span data-ttu-id="5b51e-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="5b51e-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5b51e-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="5b51e-113">Delegated (work or school account)</span></span>|<span data-ttu-id="5b51e-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5b51e-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="5b51e-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="5b51e-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5b51e-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="5b51e-116">Not supported.</span></span>|
|<span data-ttu-id="5b51e-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="5b51e-117">Application</span></span>|<span data-ttu-id="5b51e-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="5b51e-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="5b51e-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="5b51e-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/troubleshootingEvents
```

## <a name="request-headers"></a><span data-ttu-id="5b51e-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="5b51e-120">Request headers</span></span>
|<span data-ttu-id="5b51e-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="5b51e-121">Header</span></span>|<span data-ttu-id="5b51e-122">値</span><span class="sxs-lookup"><span data-stu-id="5b51e-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5b51e-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="5b51e-123">Authorization</span></span>|<span data-ttu-id="5b51e-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="5b51e-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5b51e-125">Accept</span><span class="sxs-lookup"><span data-stu-id="5b51e-125">Accept</span></span>|<span data-ttu-id="5b51e-126">application/json</span><span class="sxs-lookup"><span data-stu-id="5b51e-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5b51e-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="5b51e-127">Request body</span></span>
<span data-ttu-id="5b51e-128">要求本文で、enrollmentTroubleshootingEvent オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="5b51e-128">In the request body, supply a JSON representation for the enrollmentTroubleshootingEvent object.</span></span>

<span data-ttu-id="5b51e-129">次の表に、enrollmentTroubleshootingEvent の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="5b51e-129">The following table shows the properties that are required when you create the enrollmentTroubleshootingEvent.</span></span>

|<span data-ttu-id="5b51e-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="5b51e-130">Property</span></span>|<span data-ttu-id="5b51e-131">型</span><span class="sxs-lookup"><span data-stu-id="5b51e-131">Type</span></span>|<span data-ttu-id="5b51e-132">説明</span><span class="sxs-lookup"><span data-stu-id="5b51e-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5b51e-133">ID</span><span class="sxs-lookup"><span data-stu-id="5b51e-133">id</span></span>|<span data-ttu-id="5b51e-134">String</span><span class="sxs-lookup"><span data-stu-id="5b51e-134">String</span></span>|<span data-ttu-id="5b51e-135">オブジェクトの UUID。[deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md) から継承</span><span class="sxs-lookup"><span data-stu-id="5b51e-135">UUID for the object Inherited from [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="5b51e-136">eventDateTime</span><span class="sxs-lookup"><span data-stu-id="5b51e-136">eventDateTime</span></span>|<span data-ttu-id="5b51e-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5b51e-137">DateTimeOffset</span></span>|<span data-ttu-id="5b51e-138">インシデントが発生した時間。</span><span class="sxs-lookup"><span data-stu-id="5b51e-138">Time when the event occurred .</span></span> <span data-ttu-id="5b51e-139">[deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="5b51e-139">Inherited from [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="5b51e-140">correlationId</span><span class="sxs-lookup"><span data-stu-id="5b51e-140">correlationId</span></span>|<span data-ttu-id="5b51e-141">String</span><span class="sxs-lookup"><span data-stu-id="5b51e-141">String</span></span>|<span data-ttu-id="5b51e-142">サービスのエラーをトレースするための ID。</span><span class="sxs-lookup"><span data-stu-id="5b51e-142">Id used for tracing the failure in the service.</span></span> <span data-ttu-id="5b51e-143">[deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="5b51e-143">Inherited from [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="5b51e-144">managedDeviceIdentifier</span><span class="sxs-lookup"><span data-stu-id="5b51e-144">managedDeviceIdentifier</span></span>|<span data-ttu-id="5b51e-145">String</span><span class="sxs-lookup"><span data-stu-id="5b51e-145">String</span></span>|<span data-ttu-id="5b51e-146">Intune によって作成または収集されるデバイス識別子。</span><span class="sxs-lookup"><span data-stu-id="5b51e-146">Device identifier created or collected by Intune.</span></span>|
|<span data-ttu-id="5b51e-147">operatingSystem</span><span class="sxs-lookup"><span data-stu-id="5b51e-147">operatingSystem</span></span>|<span data-ttu-id="5b51e-148">String</span><span class="sxs-lookup"><span data-stu-id="5b51e-148">String</span></span>|<span data-ttu-id="5b51e-149">オペレーティング システム。</span><span class="sxs-lookup"><span data-stu-id="5b51e-149">Operating System.</span></span>|
|<span data-ttu-id="5b51e-150">osVersion</span><span class="sxs-lookup"><span data-stu-id="5b51e-150">osVersion</span></span>|<span data-ttu-id="5b51e-151">String</span><span class="sxs-lookup"><span data-stu-id="5b51e-151">String</span></span>|<span data-ttu-id="5b51e-152">OS バージョン。</span><span class="sxs-lookup"><span data-stu-id="5b51e-152">OS Version.</span></span>|
|<span data-ttu-id="5b51e-153">userId</span><span class="sxs-lookup"><span data-stu-id="5b51e-153">userId</span></span>|<span data-ttu-id="5b51e-154">String</span><span class="sxs-lookup"><span data-stu-id="5b51e-154">String</span></span>|<span data-ttu-id="5b51e-155">デバイスを登録しようとするユーザーの識別子。</span><span class="sxs-lookup"><span data-stu-id="5b51e-155">Identifier for the user that tried to enroll the device.</span></span>|
|<span data-ttu-id="5b51e-156">deviceId</span><span class="sxs-lookup"><span data-stu-id="5b51e-156">deviceId</span></span>|<span data-ttu-id="5b51e-157">String</span><span class="sxs-lookup"><span data-stu-id="5b51e-157">String</span></span>|<span data-ttu-id="5b51e-158">Azure AD デバイス識別子。</span><span class="sxs-lookup"><span data-stu-id="5b51e-158">Azure AD device identifier.</span></span>|
|<span data-ttu-id="5b51e-159">enrollmentType</span><span class="sxs-lookup"><span data-stu-id="5b51e-159">enrollmentType</span></span>|[<span data-ttu-id="5b51e-160">deviceEnrollmentType</span><span class="sxs-lookup"><span data-stu-id="5b51e-160">deviceEnrollmentType</span></span>](../resources/intune-shared-deviceenrollmenttype.md)|<span data-ttu-id="5b51e-161">登録の種類。</span><span class="sxs-lookup"><span data-stu-id="5b51e-161">Type of the enrollment.</span></span> <span data-ttu-id="5b51e-162">可能な値は、`unknown`、`userEnrollment`、`deviceEnrollmentManager`、`appleBulkWithUser`、`appleBulkWithoutUser`、`windowsAzureADJoin`、`windowsBulkUserless`、`windowsAutoEnrollment`、`windowsBulkAzureDomainJoin`、`windowsCoManagement` です。</span><span class="sxs-lookup"><span data-stu-id="5b51e-162">Possible values are: `unknown`, `userEnrollment`, `deviceEnrollmentManager`, `appleBulkWithUser`, `appleBulkWithoutUser`, `windowsAzureADJoin`, `windowsBulkUserless`, `windowsAutoEnrollment`, `windowsBulkAzureDomainJoin`, `windowsCoManagement`.</span></span>|
|<span data-ttu-id="5b51e-163">failureCategory</span><span class="sxs-lookup"><span data-stu-id="5b51e-163">failureCategory</span></span>|[<span data-ttu-id="5b51e-164">deviceEnrollmentFailureReason</span><span class="sxs-lookup"><span data-stu-id="5b51e-164">deviceEnrollmentFailureReason</span></span>](../resources/intune-troubleshooting-deviceenrollmentfailurereason.md)|<span data-ttu-id="5b51e-165">高レベルのエラー カテゴリ。</span><span class="sxs-lookup"><span data-stu-id="5b51e-165">Highlevel failure category.</span></span> <span data-ttu-id="5b51e-166">可能な値は、`unknown`、`authentication`、`authorization`、`accountValidation`、`userValidation`、`deviceNotSupported`、`inMaintenance`、`badRequest`、`featureNotSupported`、`enrollmentRestrictionsEnforced`、`clientDisconnected`、`userAbandonment` です。</span><span class="sxs-lookup"><span data-stu-id="5b51e-166">Possible values are: `unknown`, `authentication`, `authorization`, `accountValidation`, `userValidation`, `deviceNotSupported`, `inMaintenance`, `badRequest`, `featureNotSupported`, `enrollmentRestrictionsEnforced`, `clientDisconnected`, `userAbandonment`.</span></span>|
|<span data-ttu-id="5b51e-167">failureReason</span><span class="sxs-lookup"><span data-stu-id="5b51e-167">failureReason</span></span>|<span data-ttu-id="5b51e-168">String</span><span class="sxs-lookup"><span data-stu-id="5b51e-168">String</span></span>|<span data-ttu-id="5b51e-169">詳細なエラーの理由。</span><span class="sxs-lookup"><span data-stu-id="5b51e-169">Detailed failure reason.</span></span>|



## <a name="response"></a><span data-ttu-id="5b51e-170">応答</span><span class="sxs-lookup"><span data-stu-id="5b51e-170">Response</span></span>
<span data-ttu-id="5b51e-171">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="5b51e-171">If successful, this method returns a `201 Created` response code and a [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5b51e-172">例</span><span class="sxs-lookup"><span data-stu-id="5b51e-172">Example</span></span>
### <a name="request"></a><span data-ttu-id="5b51e-173">要求</span><span class="sxs-lookup"><span data-stu-id="5b51e-173">Request</span></span>
<span data-ttu-id="5b51e-174">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="5b51e-174">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/troubleshootingEvents
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

### <a name="response"></a><span data-ttu-id="5b51e-175">応答</span><span class="sxs-lookup"><span data-stu-id="5b51e-175">Response</span></span>
<span data-ttu-id="5b51e-p107">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="5b51e-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





