---
title: enrollmentTroubleshootingEvent の更新
description: enrollmentTroubleshootingEvent オブジェクトのプロパティを更新します。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: efbc823b4ba7a5e28a0a2e7d82b7708102002a71
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29399788"
---
# <a name="update-enrollmenttroubleshootingevent"></a><span data-ttu-id="58da9-103">enrollmentTroubleshootingEvent の更新</span><span class="sxs-lookup"><span data-stu-id="58da9-103">Update enrollmentTroubleshootingEvent</span></span>

> <span data-ttu-id="58da9-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="58da9-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="58da9-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="58da9-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="58da9-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="58da9-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="58da9-107">[enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="58da9-107">Update the properties of a [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="58da9-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="58da9-108">Prerequisites</span></span>
<span data-ttu-id="58da9-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/concepts/permissions-reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="58da9-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="58da9-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="58da9-111">Permission type</span></span>|<span data-ttu-id="58da9-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="58da9-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="58da9-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="58da9-113">Delegated (work or school account)</span></span>|<span data-ttu-id="58da9-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="58da9-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="58da9-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="58da9-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="58da9-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="58da9-116">Not supported.</span></span>|
|<span data-ttu-id="58da9-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="58da9-117">Application</span></span>|<span data-ttu-id="58da9-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="58da9-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="58da9-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="58da9-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/troubleshootingEvents/{deviceManagementTroubleshootingEventId}
```

## <a name="request-headers"></a><span data-ttu-id="58da9-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="58da9-120">Request headers</span></span>
|<span data-ttu-id="58da9-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="58da9-121">Header</span></span>|<span data-ttu-id="58da9-122">値</span><span class="sxs-lookup"><span data-stu-id="58da9-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="58da9-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="58da9-123">Authorization</span></span>|<span data-ttu-id="58da9-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="58da9-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="58da9-125">Accept</span><span class="sxs-lookup"><span data-stu-id="58da9-125">Accept</span></span>|<span data-ttu-id="58da9-126">application/json</span><span class="sxs-lookup"><span data-stu-id="58da9-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="58da9-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="58da9-127">Request body</span></span>
<span data-ttu-id="58da9-128">要求本文で、[enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="58da9-128">In the request body, supply a JSON representation for the [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md) object.</span></span>

<span data-ttu-id="58da9-129">次の表に、[enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md) の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="58da9-129">The following table shows the properties that are required when you create the [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md).</span></span>

|<span data-ttu-id="58da9-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="58da9-130">Property</span></span>|<span data-ttu-id="58da9-131">型</span><span class="sxs-lookup"><span data-stu-id="58da9-131">Type</span></span>|<span data-ttu-id="58da9-132">説明</span><span class="sxs-lookup"><span data-stu-id="58da9-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="58da9-133">id</span><span class="sxs-lookup"><span data-stu-id="58da9-133">id</span></span>|<span data-ttu-id="58da9-134">String</span><span class="sxs-lookup"><span data-stu-id="58da9-134">String</span></span>|<span data-ttu-id="58da9-135">オブジェクトの UUID。[deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md) から継承</span><span class="sxs-lookup"><span data-stu-id="58da9-135">UUID for the object Inherited from [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="58da9-136">eventDateTime</span><span class="sxs-lookup"><span data-stu-id="58da9-136">eventDateTime</span></span>|<span data-ttu-id="58da9-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="58da9-137">DateTimeOffset</span></span>|<span data-ttu-id="58da9-138">インシデントが発生した時間。</span><span class="sxs-lookup"><span data-stu-id="58da9-138">Time when the event occurred .</span></span> <span data-ttu-id="58da9-139">[deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="58da9-139">Inherited from [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="58da9-140">correlationId</span><span class="sxs-lookup"><span data-stu-id="58da9-140">correlationId</span></span>|<span data-ttu-id="58da9-141">String</span><span class="sxs-lookup"><span data-stu-id="58da9-141">String</span></span>|<span data-ttu-id="58da9-142">サービスのエラーをトレースするための ID。</span><span class="sxs-lookup"><span data-stu-id="58da9-142">Id used for tracing the failure in the service.</span></span> <span data-ttu-id="58da9-143">[deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="58da9-143">Inherited from [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="58da9-144">troubleshootingErrorDetails</span><span class="sxs-lookup"><span data-stu-id="58da9-144">troubleshootingErrorDetails</span></span>|[<span data-ttu-id="58da9-145">deviceManagementTroubleshootingErrorDetails</span><span class="sxs-lookup"><span data-stu-id="58da9-145">deviceManagementTroubleshootingErrorDetails</span></span>](../resources/intune-troubleshooting-devicemanagementtroubleshootingerrordetails.md)|<span data-ttu-id="58da9-146">エラーとその修復に関する詳細情報を含むオブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="58da9-146">Object containing detailed information about the error and its remediation.</span></span> <span data-ttu-id="58da9-147">[deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="58da9-147">Inherited from [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="58da9-148">eventName</span><span class="sxs-lookup"><span data-stu-id="58da9-148">eventName</span></span>|<span data-ttu-id="58da9-149">String</span><span class="sxs-lookup"><span data-stu-id="58da9-149">String</span></span>|<span data-ttu-id="58da9-150">トラブルシューティング イベントに対応するイベントの名前です。</span><span class="sxs-lookup"><span data-stu-id="58da9-150">Event Name corresponding to the Troubleshooting Event.</span></span> <span data-ttu-id="58da9-151">[DeviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)から継承される省略可能なフィールドします。</span><span class="sxs-lookup"><span data-stu-id="58da9-151">It is an Optional field Inherited from [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="58da9-152">について</span><span class="sxs-lookup"><span data-stu-id="58da9-152">additionalInformation</span></span>|<span data-ttu-id="58da9-153">[keyValuePair](../resources/intune-shared-keyvaluepair.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="58da9-153">[keyValuePair](../resources/intune-shared-keyvaluepair.md) collection</span></span>|<span data-ttu-id="58da9-154">[DeviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)から継承されるトラブルシューティング イベントに関する追加情報を提供する文字列キーと文字列値のペアのセット</span><span class="sxs-lookup"><span data-stu-id="58da9-154">A set of string key and string value pairs which provides additional information on the Troubleshooting event Inherited from [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="58da9-155">managedDeviceIdentifier</span><span class="sxs-lookup"><span data-stu-id="58da9-155">managedDeviceIdentifier</span></span>|<span data-ttu-id="58da9-156">String</span><span class="sxs-lookup"><span data-stu-id="58da9-156">String</span></span>|<span data-ttu-id="58da9-157">Intune によって作成または収集されるデバイス識別子。</span><span class="sxs-lookup"><span data-stu-id="58da9-157">Device identifier created or collected by Intune.</span></span>|
|<span data-ttu-id="58da9-158">operatingSystem</span><span class="sxs-lookup"><span data-stu-id="58da9-158">operatingSystem</span></span>|<span data-ttu-id="58da9-159">String</span><span class="sxs-lookup"><span data-stu-id="58da9-159">String</span></span>|<span data-ttu-id="58da9-160">オペレーティング システム。</span><span class="sxs-lookup"><span data-stu-id="58da9-160">Operating System.</span></span>|
|<span data-ttu-id="58da9-161">osVersion</span><span class="sxs-lookup"><span data-stu-id="58da9-161">osVersion</span></span>|<span data-ttu-id="58da9-162">String</span><span class="sxs-lookup"><span data-stu-id="58da9-162">String</span></span>|<span data-ttu-id="58da9-163">OS バージョン。</span><span class="sxs-lookup"><span data-stu-id="58da9-163">OS Version.</span></span>|
|<span data-ttu-id="58da9-164">userId</span><span class="sxs-lookup"><span data-stu-id="58da9-164">userId</span></span>|<span data-ttu-id="58da9-165">String</span><span class="sxs-lookup"><span data-stu-id="58da9-165">String</span></span>|<span data-ttu-id="58da9-166">デバイスを登録しようとするユーザーの識別子。</span><span class="sxs-lookup"><span data-stu-id="58da9-166">Identifier for the user that tried to enroll the device.</span></span>|
|<span data-ttu-id="58da9-167">deviceId</span><span class="sxs-lookup"><span data-stu-id="58da9-167">deviceId</span></span>|<span data-ttu-id="58da9-168">String</span><span class="sxs-lookup"><span data-stu-id="58da9-168">String</span></span>|<span data-ttu-id="58da9-169">Azure AD デバイス識別子。</span><span class="sxs-lookup"><span data-stu-id="58da9-169">Azure AD device identifier.</span></span>|
|<span data-ttu-id="58da9-170">enrollmentType</span><span class="sxs-lookup"><span data-stu-id="58da9-170">enrollmentType</span></span>|[<span data-ttu-id="58da9-171">deviceEnrollmentType</span><span class="sxs-lookup"><span data-stu-id="58da9-171">deviceEnrollmentType</span></span>](../resources/intune-shared-deviceenrollmenttype.md)|<span data-ttu-id="58da9-172">登録の種類。</span><span class="sxs-lookup"><span data-stu-id="58da9-172">Type of the enrollment.</span></span> <span data-ttu-id="58da9-173">可能な値は、`unknown`、`userEnrollment`、`deviceEnrollmentManager`、`appleBulkWithUser`、`appleBulkWithoutUser`、`windowsAzureADJoin`、`windowsBulkUserless`、`windowsAutoEnrollment`、`windowsBulkAzureDomainJoin`、`windowsCoManagement` です。</span><span class="sxs-lookup"><span data-stu-id="58da9-173">Possible values are: `unknown`, `userEnrollment`, `deviceEnrollmentManager`, `appleBulkWithUser`, `appleBulkWithoutUser`, `windowsAzureADJoin`, `windowsBulkUserless`, `windowsAutoEnrollment`, `windowsBulkAzureDomainJoin`, `windowsCoManagement`.</span></span>|
|<span data-ttu-id="58da9-174">failureCategory</span><span class="sxs-lookup"><span data-stu-id="58da9-174">failureCategory</span></span>|[<span data-ttu-id="58da9-175">deviceEnrollmentFailureReason</span><span class="sxs-lookup"><span data-stu-id="58da9-175">deviceEnrollmentFailureReason</span></span>](../resources/intune-troubleshooting-deviceenrollmentfailurereason.md)|<span data-ttu-id="58da9-176">高レベルのエラー カテゴリ。</span><span class="sxs-lookup"><span data-stu-id="58da9-176">Highlevel failure category.</span></span> <span data-ttu-id="58da9-177">可能な値は、`unknown`、`authentication`、`authorization`、`accountValidation`、`userValidation`、`deviceNotSupported`、`inMaintenance`、`badRequest`、`featureNotSupported`、`enrollmentRestrictionsEnforced`、`clientDisconnected`、`userAbandonment` です。</span><span class="sxs-lookup"><span data-stu-id="58da9-177">Possible values are: `unknown`, `authentication`, `authorization`, `accountValidation`, `userValidation`, `deviceNotSupported`, `inMaintenance`, `badRequest`, `featureNotSupported`, `enrollmentRestrictionsEnforced`, `clientDisconnected`, `userAbandonment`.</span></span>|
|<span data-ttu-id="58da9-178">failureReason</span><span class="sxs-lookup"><span data-stu-id="58da9-178">failureReason</span></span>|<span data-ttu-id="58da9-179">String</span><span class="sxs-lookup"><span data-stu-id="58da9-179">String</span></span>|<span data-ttu-id="58da9-180">詳細なエラーの理由。</span><span class="sxs-lookup"><span data-stu-id="58da9-180">Detailed failure reason.</span></span>|



## <a name="response"></a><span data-ttu-id="58da9-181">応答</span><span class="sxs-lookup"><span data-stu-id="58da9-181">Response</span></span>
<span data-ttu-id="58da9-182">成功した場合、このメソッドは `200 OK` 応答コードと、更新された [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md) オブジェクトを応答本文で返します。</span><span class="sxs-lookup"><span data-stu-id="58da9-182">If successful, this method returns a `200 OK` response code and an updated [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="58da9-183">例</span><span class="sxs-lookup"><span data-stu-id="58da9-183">Example</span></span>

### <a name="request"></a><span data-ttu-id="58da9-184">要求</span><span class="sxs-lookup"><span data-stu-id="58da9-184">Request</span></span>
<span data-ttu-id="58da9-185">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="58da9-185">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/troubleshootingEvents/{deviceManagementTroubleshootingEventId}
Content-type: application/json
Content-length: 1182

{
  "@odata.type": "#microsoft.graph.enrollmentTroubleshootingEvent",
  "eventDateTime": "2016-12-31T23:59:23.3984029-08:00",
  "correlationId": "Correlation Id value",
  "troubleshootingErrorDetails": {
    "@odata.type": "microsoft.graph.deviceManagementTroubleshootingErrorDetails",
    "context": "Context value",
    "failure": "Failure value",
    "failureDetails": "Failure Details value",
    "remediation": "Remediation value",
    "resources": [
      {
        "@odata.type": "microsoft.graph.deviceManagementTroubleshootingErrorResource",
        "text": "Text value",
        "link": "Link value"
      }
    ]
  },
  "eventName": "Event Name value",
  "additionalInformation": [
    {
      "@odata.type": "microsoft.graph.keyValuePair",
      "name": "Name value",
      "value": "Value value"
    }
  ],
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

### <a name="response"></a><span data-ttu-id="58da9-186">応答</span><span class="sxs-lookup"><span data-stu-id="58da9-186">Response</span></span>
<span data-ttu-id="58da9-p109">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="58da9-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1231

{
  "@odata.type": "#microsoft.graph.enrollmentTroubleshootingEvent",
  "id": "c4a623f5-23f5-c4a6-f523-a6c4f523a6c4",
  "eventDateTime": "2016-12-31T23:59:23.3984029-08:00",
  "correlationId": "Correlation Id value",
  "troubleshootingErrorDetails": {
    "@odata.type": "microsoft.graph.deviceManagementTroubleshootingErrorDetails",
    "context": "Context value",
    "failure": "Failure value",
    "failureDetails": "Failure Details value",
    "remediation": "Remediation value",
    "resources": [
      {
        "@odata.type": "microsoft.graph.deviceManagementTroubleshootingErrorResource",
        "text": "Text value",
        "link": "Link value"
      }
    ]
  },
  "eventName": "Event Name value",
  "additionalInformation": [
    {
      "@odata.type": "microsoft.graph.keyValuePair",
      "name": "Name value",
      "value": "Value value"
    }
  ],
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




