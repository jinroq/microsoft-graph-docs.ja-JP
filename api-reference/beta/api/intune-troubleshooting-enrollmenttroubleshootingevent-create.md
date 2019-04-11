---
title: enrollmentTroubleshootingEvent の作成
description: 新しい enrollmentTroubleshootingEvent オブジェクトを作成します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: e3d3cdd865bf2d2316d2e50e433375eb875c4406
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/11/2019
ms.locfileid: "31774625"
---
# <a name="create-enrollmenttroubleshootingevent"></a><span data-ttu-id="6a0b2-103">enrollmentTroubleshootingEvent の作成</span><span class="sxs-lookup"><span data-stu-id="6a0b2-103">Create enrollmentTroubleshootingEvent</span></span>

> <span data-ttu-id="6a0b2-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="6a0b2-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6a0b2-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="6a0b2-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6a0b2-106">新しい [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="6a0b2-106">Create a new [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="6a0b2-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="6a0b2-107">Prerequisites</span></span>
<span data-ttu-id="6a0b2-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="6a0b2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6a0b2-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="6a0b2-110">Permission type</span></span>|<span data-ttu-id="6a0b2-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="6a0b2-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6a0b2-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="6a0b2-112">Delegated (work or school account)</span></span>|<span data-ttu-id="6a0b2-113">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6a0b2-113">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="6a0b2-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="6a0b2-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6a0b2-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="6a0b2-115">Not supported.</span></span>|
|<span data-ttu-id="6a0b2-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="6a0b2-116">Application</span></span>|<span data-ttu-id="6a0b2-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="6a0b2-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="6a0b2-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="6a0b2-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/troubleshootingEvents
```

## <a name="request-headers"></a><span data-ttu-id="6a0b2-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="6a0b2-119">Request headers</span></span>
|<span data-ttu-id="6a0b2-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="6a0b2-120">Header</span></span>|<span data-ttu-id="6a0b2-121">値</span><span class="sxs-lookup"><span data-stu-id="6a0b2-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6a0b2-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="6a0b2-122">Authorization</span></span>|<span data-ttu-id="6a0b2-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="6a0b2-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6a0b2-124">承諾</span><span class="sxs-lookup"><span data-stu-id="6a0b2-124">Accept</span></span>|<span data-ttu-id="6a0b2-125">application/json</span><span class="sxs-lookup"><span data-stu-id="6a0b2-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6a0b2-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="6a0b2-126">Request body</span></span>
<span data-ttu-id="6a0b2-127">要求本文で、enrollmentTroubleshootingEvent オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="6a0b2-127">In the request body, supply a JSON representation for the enrollmentTroubleshootingEvent object.</span></span>

<span data-ttu-id="6a0b2-128">次の表に、enrollmentTroubleshootingEvent の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="6a0b2-128">The following table shows the properties that are required when you create the enrollmentTroubleshootingEvent.</span></span>

|<span data-ttu-id="6a0b2-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="6a0b2-129">Property</span></span>|<span data-ttu-id="6a0b2-130">型</span><span class="sxs-lookup"><span data-stu-id="6a0b2-130">Type</span></span>|<span data-ttu-id="6a0b2-131">説明</span><span class="sxs-lookup"><span data-stu-id="6a0b2-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6a0b2-132">id</span><span class="sxs-lookup"><span data-stu-id="6a0b2-132">id</span></span>|<span data-ttu-id="6a0b2-133">String</span><span class="sxs-lookup"><span data-stu-id="6a0b2-133">String</span></span>|<span data-ttu-id="6a0b2-134">オブジェクトの UUID。[deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md) から継承</span><span class="sxs-lookup"><span data-stu-id="6a0b2-134">UUID for the object Inherited from [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="6a0b2-135">eventDateTime</span><span class="sxs-lookup"><span data-stu-id="6a0b2-135">eventDateTime</span></span>|<span data-ttu-id="6a0b2-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6a0b2-136">DateTimeOffset</span></span>|<span data-ttu-id="6a0b2-137">インシデントが発生した時間。</span><span class="sxs-lookup"><span data-stu-id="6a0b2-137">Time when the event occurred .</span></span> <span data-ttu-id="6a0b2-138">[deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="6a0b2-138">Inherited from [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="6a0b2-139">correlationId</span><span class="sxs-lookup"><span data-stu-id="6a0b2-139">correlationId</span></span>|<span data-ttu-id="6a0b2-140">文字列</span><span class="sxs-lookup"><span data-stu-id="6a0b2-140">String</span></span>|<span data-ttu-id="6a0b2-141">サービスのエラーをトレースするための ID。</span><span class="sxs-lookup"><span data-stu-id="6a0b2-141">Id used for tracing the failure in the service.</span></span> <span data-ttu-id="6a0b2-142">[deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="6a0b2-142">Inherited from [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="6a0b2-143">トラブルシューティングのエラーの詳細</span><span class="sxs-lookup"><span data-stu-id="6a0b2-143">troubleshootingErrorDetails</span></span>|[<span data-ttu-id="6a0b2-144">deviceManagementTroubleshootingErrorDetails</span><span class="sxs-lookup"><span data-stu-id="6a0b2-144">deviceManagementTroubleshootingErrorDetails</span></span>](../resources/intune-troubleshooting-devicemanagementtroubleshootingerrordetails.md)|<span data-ttu-id="6a0b2-145">エラーとその修復に関する詳細情報を含むオブジェクト。</span><span class="sxs-lookup"><span data-stu-id="6a0b2-145">Object containing detailed information about the error and its remediation.</span></span> <span data-ttu-id="6a0b2-146">[deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="6a0b2-146">Inherited from [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="6a0b2-147">eventName</span><span class="sxs-lookup"><span data-stu-id="6a0b2-147">eventName</span></span>|<span data-ttu-id="6a0b2-148">文字列</span><span class="sxs-lookup"><span data-stu-id="6a0b2-148">String</span></span>|<span data-ttu-id="6a0b2-149">トラブルシューティングイベントに対応するイベント名。</span><span class="sxs-lookup"><span data-stu-id="6a0b2-149">Event Name corresponding to the Troubleshooting Event.</span></span> <span data-ttu-id="6a0b2-150">[devicemanagementトラブルシューティングイベント](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)から継承されるオプションフィールドです</span><span class="sxs-lookup"><span data-stu-id="6a0b2-150">It is an Optional field Inherited from [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="6a0b2-151">additionalinformation</span><span class="sxs-lookup"><span data-stu-id="6a0b2-151">additionalInformation</span></span>|<span data-ttu-id="6a0b2-152">[keyValuePair](../resources/intune-shared-keyvaluepair.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="6a0b2-152">[keyValuePair](../resources/intune-shared-keyvaluepair.md) collection</span></span>|<span data-ttu-id="6a0b2-153">[devicemanagementトラブルシューティングイベント](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)から継承されたトラブルシューティングイベントに関する追加情報を提供する文字列キーと文字列値のペアのセット。</span><span class="sxs-lookup"><span data-stu-id="6a0b2-153">A set of string key and string value pairs which provides additional information on the Troubleshooting event Inherited from [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="6a0b2-154">managedDeviceIdentifier</span><span class="sxs-lookup"><span data-stu-id="6a0b2-154">managedDeviceIdentifier</span></span>|<span data-ttu-id="6a0b2-155">文字列</span><span class="sxs-lookup"><span data-stu-id="6a0b2-155">String</span></span>|<span data-ttu-id="6a0b2-156">Intune によって作成または収集されるデバイス識別子。</span><span class="sxs-lookup"><span data-stu-id="6a0b2-156">Device identifier created or collected by Intune.</span></span>|
|<span data-ttu-id="6a0b2-157">operatingSystem</span><span class="sxs-lookup"><span data-stu-id="6a0b2-157">operatingSystem</span></span>|<span data-ttu-id="6a0b2-158">文字列</span><span class="sxs-lookup"><span data-stu-id="6a0b2-158">String</span></span>|<span data-ttu-id="6a0b2-159">オペレーティング システム。</span><span class="sxs-lookup"><span data-stu-id="6a0b2-159">Operating System.</span></span>|
|<span data-ttu-id="6a0b2-160">osVersion</span><span class="sxs-lookup"><span data-stu-id="6a0b2-160">osVersion</span></span>|<span data-ttu-id="6a0b2-161">文字列</span><span class="sxs-lookup"><span data-stu-id="6a0b2-161">String</span></span>|<span data-ttu-id="6a0b2-162">OS バージョン。</span><span class="sxs-lookup"><span data-stu-id="6a0b2-162">OS Version.</span></span>|
|<span data-ttu-id="6a0b2-163">userId</span><span class="sxs-lookup"><span data-stu-id="6a0b2-163">userId</span></span>|<span data-ttu-id="6a0b2-164">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="6a0b2-164">String</span></span>|<span data-ttu-id="6a0b2-165">デバイスを登録しようとするユーザーの識別子。</span><span class="sxs-lookup"><span data-stu-id="6a0b2-165">Identifier for the user that tried to enroll the device.</span></span>|
|<span data-ttu-id="6a0b2-166">deviceId</span><span class="sxs-lookup"><span data-stu-id="6a0b2-166">deviceId</span></span>|<span data-ttu-id="6a0b2-167">文字列</span><span class="sxs-lookup"><span data-stu-id="6a0b2-167">String</span></span>|<span data-ttu-id="6a0b2-168">Azure AD デバイス識別子。</span><span class="sxs-lookup"><span data-stu-id="6a0b2-168">Azure AD device identifier.</span></span>|
|<span data-ttu-id="6a0b2-169">enrollmentType</span><span class="sxs-lookup"><span data-stu-id="6a0b2-169">enrollmentType</span></span>|[<span data-ttu-id="6a0b2-170">deviceEnrollmentType</span><span class="sxs-lookup"><span data-stu-id="6a0b2-170">deviceEnrollmentType</span></span>](../resources/intune-shared-deviceenrollmenttype.md)|<span data-ttu-id="6a0b2-171">登録の種類。</span><span class="sxs-lookup"><span data-stu-id="6a0b2-171">Type of the enrollment.</span></span> <span data-ttu-id="6a0b2-172">可能な値は、`unknown`、`userEnrollment`、`deviceEnrollmentManager`、`appleBulkWithUser`、`appleBulkWithoutUser`、`windowsAzureADJoin`、`windowsBulkUserless`、`windowsAutoEnrollment`、`windowsBulkAzureDomainJoin`、`windowsCoManagement` です。</span><span class="sxs-lookup"><span data-stu-id="6a0b2-172">Possible values are: `unknown`, `userEnrollment`, `deviceEnrollmentManager`, `appleBulkWithUser`, `appleBulkWithoutUser`, `windowsAzureADJoin`, `windowsBulkUserless`, `windowsAutoEnrollment`, `windowsBulkAzureDomainJoin`, `windowsCoManagement`.</span></span>|
|<span data-ttu-id="6a0b2-173">failureCategory</span><span class="sxs-lookup"><span data-stu-id="6a0b2-173">failureCategory</span></span>|[<span data-ttu-id="6a0b2-174">deviceEnrollmentFailureReason</span><span class="sxs-lookup"><span data-stu-id="6a0b2-174">deviceEnrollmentFailureReason</span></span>](../resources/intune-troubleshooting-deviceenrollmentfailurereason.md)|<span data-ttu-id="6a0b2-175">高レベルのエラー カテゴリ。</span><span class="sxs-lookup"><span data-stu-id="6a0b2-175">Highlevel failure category.</span></span> <span data-ttu-id="6a0b2-176">可能な値は、`unknown`、`authentication`、`authorization`、`accountValidation`、`userValidation`、`deviceNotSupported`、`inMaintenance`、`badRequest`、`featureNotSupported`、`enrollmentRestrictionsEnforced`、`clientDisconnected`、`userAbandonment` です。</span><span class="sxs-lookup"><span data-stu-id="6a0b2-176">Possible values are: `unknown`, `authentication`, `authorization`, `accountValidation`, `userValidation`, `deviceNotSupported`, `inMaintenance`, `badRequest`, `featureNotSupported`, `enrollmentRestrictionsEnforced`, `clientDisconnected`, `userAbandonment`.</span></span>|
|<span data-ttu-id="6a0b2-177">failureReason</span><span class="sxs-lookup"><span data-stu-id="6a0b2-177">failureReason</span></span>|<span data-ttu-id="6a0b2-178">String</span><span class="sxs-lookup"><span data-stu-id="6a0b2-178">String</span></span>|<span data-ttu-id="6a0b2-179">詳細なエラーの理由。</span><span class="sxs-lookup"><span data-stu-id="6a0b2-179">Detailed failure reason.</span></span>|



## <a name="response"></a><span data-ttu-id="6a0b2-180">応答</span><span class="sxs-lookup"><span data-stu-id="6a0b2-180">Response</span></span>
<span data-ttu-id="6a0b2-181">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="6a0b2-181">If successful, this method returns a `201 Created` response code and a [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6a0b2-182">例</span><span class="sxs-lookup"><span data-stu-id="6a0b2-182">Example</span></span>

### <a name="request"></a><span data-ttu-id="6a0b2-183">要求</span><span class="sxs-lookup"><span data-stu-id="6a0b2-183">Request</span></span>
<span data-ttu-id="6a0b2-184">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="6a0b2-184">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/troubleshootingEvents
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

### <a name="response"></a><span data-ttu-id="6a0b2-185">応答</span><span class="sxs-lookup"><span data-stu-id="6a0b2-185">Response</span></span>
<span data-ttu-id="6a0b2-p108">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="6a0b2-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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



