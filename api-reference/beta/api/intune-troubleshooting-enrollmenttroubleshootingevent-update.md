---
title: enrollmentTroubleshootingEvent の更新
description: enrollmentTroubleshootingEvent オブジェクトのプロパティを更新します。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: a2512f575bdca87e4fc4c8cfc9b3091a221d6a71
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36347214"
---
# <a name="update-enrollmenttroubleshootingevent"></a><span data-ttu-id="92c95-103">enrollmentTroubleshootingEvent の更新</span><span class="sxs-lookup"><span data-stu-id="92c95-103">Update enrollmentTroubleshootingEvent</span></span>

> <span data-ttu-id="92c95-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="92c95-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="92c95-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="92c95-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="92c95-106">[enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="92c95-106">Update the properties of a [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="92c95-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="92c95-107">Prerequisites</span></span>
<span data-ttu-id="92c95-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="92c95-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="92c95-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="92c95-110">Permission type</span></span>|<span data-ttu-id="92c95-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="92c95-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="92c95-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="92c95-112">Delegated (work or school account)</span></span>|<span data-ttu-id="92c95-113">\* \* TODO: 範囲を決定します \* \*</span><span class="sxs-lookup"><span data-stu-id="92c95-113">\*\*TODO: Determine scopes \*\*</span></span>|
|<span data-ttu-id="92c95-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="92c95-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="92c95-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="92c95-115">Not supported.</span></span>|
|<span data-ttu-id="92c95-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="92c95-116">Application</span></span>|<span data-ttu-id="92c95-117">\* \* TODO: AppOnly スコープを決定します \* \*</span><span class="sxs-lookup"><span data-stu-id="92c95-117">\*\*TODO: Determine AppOnly scopes \*\*</span></span>|

## <a name="http-request"></a><span data-ttu-id="92c95-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="92c95-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/troubleshootingEvents/{deviceManagementTroubleshootingEventId}
```

## <a name="request-headers"></a><span data-ttu-id="92c95-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="92c95-119">Request headers</span></span>
|<span data-ttu-id="92c95-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="92c95-120">Header</span></span>|<span data-ttu-id="92c95-121">値</span><span class="sxs-lookup"><span data-stu-id="92c95-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="92c95-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="92c95-122">Authorization</span></span>|<span data-ttu-id="92c95-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="92c95-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="92c95-124">承諾</span><span class="sxs-lookup"><span data-stu-id="92c95-124">Accept</span></span>|<span data-ttu-id="92c95-125">application/json</span><span class="sxs-lookup"><span data-stu-id="92c95-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="92c95-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="92c95-126">Request body</span></span>
<span data-ttu-id="92c95-127">要求本文で、[enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="92c95-127">In the request body, supply a JSON representation for the [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md) object.</span></span>

<span data-ttu-id="92c95-128">次の表に、[enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md) の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="92c95-128">The following table shows the properties that are required when you create the [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md).</span></span>

|<span data-ttu-id="92c95-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="92c95-129">Property</span></span>|<span data-ttu-id="92c95-130">型</span><span class="sxs-lookup"><span data-stu-id="92c95-130">Type</span></span>|<span data-ttu-id="92c95-131">説明</span><span class="sxs-lookup"><span data-stu-id="92c95-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="92c95-132">id</span><span class="sxs-lookup"><span data-stu-id="92c95-132">id</span></span>|<span data-ttu-id="92c95-133">文字列</span><span class="sxs-lookup"><span data-stu-id="92c95-133">String</span></span>|<span data-ttu-id="92c95-134">オブジェクトの UUID。[deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md) から継承</span><span class="sxs-lookup"><span data-stu-id="92c95-134">UUID for the object Inherited from [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="92c95-135">eventDateTime</span><span class="sxs-lookup"><span data-stu-id="92c95-135">eventDateTime</span></span>|<span data-ttu-id="92c95-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="92c95-136">DateTimeOffset</span></span>|<span data-ttu-id="92c95-137">インシデントが発生した時間。</span><span class="sxs-lookup"><span data-stu-id="92c95-137">Time when the event occurred .</span></span> <span data-ttu-id="92c95-138">[deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="92c95-138">Inherited from [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="92c95-139">correlationId</span><span class="sxs-lookup"><span data-stu-id="92c95-139">correlationId</span></span>|<span data-ttu-id="92c95-140">String</span><span class="sxs-lookup"><span data-stu-id="92c95-140">String</span></span>|<span data-ttu-id="92c95-141">サービスのエラーをトレースするための ID。</span><span class="sxs-lookup"><span data-stu-id="92c95-141">Id used for tracing the failure in the service.</span></span> <span data-ttu-id="92c95-142">[deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="92c95-142">Inherited from [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="92c95-143">トラブルシューティングのエラーの詳細</span><span class="sxs-lookup"><span data-stu-id="92c95-143">troubleshootingErrorDetails</span></span>|[<span data-ttu-id="92c95-144">deviceManagementTroubleshootingErrorDetails</span><span class="sxs-lookup"><span data-stu-id="92c95-144">deviceManagementTroubleshootingErrorDetails</span></span>](../resources/intune-troubleshooting-devicemanagementtroubleshootingerrordetails.md)|<span data-ttu-id="92c95-145">エラーとその修復に関する詳細情報を含むオブジェクト。</span><span class="sxs-lookup"><span data-stu-id="92c95-145">Object containing detailed information about the error and its remediation.</span></span> <span data-ttu-id="92c95-146">[deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="92c95-146">Inherited from [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="92c95-147">eventName</span><span class="sxs-lookup"><span data-stu-id="92c95-147">eventName</span></span>|<span data-ttu-id="92c95-148">String</span><span class="sxs-lookup"><span data-stu-id="92c95-148">String</span></span>|<span data-ttu-id="92c95-149">トラブルシューティングイベントに対応するイベント名。</span><span class="sxs-lookup"><span data-stu-id="92c95-149">Event Name corresponding to the Troubleshooting Event.</span></span> <span data-ttu-id="92c95-150">[Devicemanagementトラブルシューティングイベント](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)から継承されるオプションフィールドです</span><span class="sxs-lookup"><span data-stu-id="92c95-150">It is an Optional field Inherited from [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="92c95-151">additionalInformation</span><span class="sxs-lookup"><span data-stu-id="92c95-151">additionalInformation</span></span>|<span data-ttu-id="92c95-152">[keyValuePair](../resources/intune-shared-keyvaluepair.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="92c95-152">[keyValuePair](../resources/intune-shared-keyvaluepair.md) collection</span></span>|<span data-ttu-id="92c95-153">[Devicemanagementトラブルシューティングイベント](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)から継承されたトラブルシューティングイベントに関する追加情報を提供する文字列キーと文字列値のペアのセット。</span><span class="sxs-lookup"><span data-stu-id="92c95-153">A set of string key and string value pairs which provides additional information on the Troubleshooting event Inherited from [deviceManagementTroubleshootingEvent](../resources/intune-troubleshooting-devicemanagementtroubleshootingevent.md)</span></span>|
|<span data-ttu-id="92c95-154">managedDeviceIdentifier</span><span class="sxs-lookup"><span data-stu-id="92c95-154">managedDeviceIdentifier</span></span>|<span data-ttu-id="92c95-155">String</span><span class="sxs-lookup"><span data-stu-id="92c95-155">String</span></span>|<span data-ttu-id="92c95-156">Intune によって作成または収集されるデバイス識別子。</span><span class="sxs-lookup"><span data-stu-id="92c95-156">Device identifier created or collected by Intune.</span></span>|
|<span data-ttu-id="92c95-157">operatingSystem</span><span class="sxs-lookup"><span data-stu-id="92c95-157">operatingSystem</span></span>|<span data-ttu-id="92c95-158">文字列</span><span class="sxs-lookup"><span data-stu-id="92c95-158">String</span></span>|<span data-ttu-id="92c95-159">オペレーティング システム。</span><span class="sxs-lookup"><span data-stu-id="92c95-159">Operating System.</span></span>|
|<span data-ttu-id="92c95-160">osVersion</span><span class="sxs-lookup"><span data-stu-id="92c95-160">osVersion</span></span>|<span data-ttu-id="92c95-161">String</span><span class="sxs-lookup"><span data-stu-id="92c95-161">String</span></span>|<span data-ttu-id="92c95-162">OS バージョン。</span><span class="sxs-lookup"><span data-stu-id="92c95-162">OS Version.</span></span>|
|<span data-ttu-id="92c95-163">userId</span><span class="sxs-lookup"><span data-stu-id="92c95-163">userId</span></span>|<span data-ttu-id="92c95-164">String</span><span class="sxs-lookup"><span data-stu-id="92c95-164">String</span></span>|<span data-ttu-id="92c95-165">デバイスを登録しようとするユーザーの識別子。</span><span class="sxs-lookup"><span data-stu-id="92c95-165">Identifier for the user that tried to enroll the device.</span></span>|
|<span data-ttu-id="92c95-166">deviceId</span><span class="sxs-lookup"><span data-stu-id="92c95-166">deviceId</span></span>|<span data-ttu-id="92c95-167">String</span><span class="sxs-lookup"><span data-stu-id="92c95-167">String</span></span>|<span data-ttu-id="92c95-168">Azure AD デバイス識別子。</span><span class="sxs-lookup"><span data-stu-id="92c95-168">Azure AD device identifier.</span></span>|
|<span data-ttu-id="92c95-169">enrollmentType</span><span class="sxs-lookup"><span data-stu-id="92c95-169">enrollmentType</span></span>|[<span data-ttu-id="92c95-170">deviceEnrollmentType</span><span class="sxs-lookup"><span data-stu-id="92c95-170">deviceEnrollmentType</span></span>](../resources/intune-shared-deviceenrollmenttype.md)|<span data-ttu-id="92c95-171">登録の種類。</span><span class="sxs-lookup"><span data-stu-id="92c95-171">Type of the enrollment.</span></span> <span data-ttu-id="92c95-172">可能な値は、`unknown`、`userEnrollment`、`deviceEnrollmentManager`、`appleBulkWithUser`、`appleBulkWithoutUser`、`windowsAzureADJoin`、`windowsBulkUserless`、`windowsAutoEnrollment`、`windowsBulkAzureDomainJoin`、`windowsCoManagement` です。</span><span class="sxs-lookup"><span data-stu-id="92c95-172">Possible values are: `unknown`, `userEnrollment`, `deviceEnrollmentManager`, `appleBulkWithUser`, `appleBulkWithoutUser`, `windowsAzureADJoin`, `windowsBulkUserless`, `windowsAutoEnrollment`, `windowsBulkAzureDomainJoin`, `windowsCoManagement`.</span></span>|
|<span data-ttu-id="92c95-173">failureCategory</span><span class="sxs-lookup"><span data-stu-id="92c95-173">failureCategory</span></span>|[<span data-ttu-id="92c95-174">deviceEnrollmentFailureReason</span><span class="sxs-lookup"><span data-stu-id="92c95-174">deviceEnrollmentFailureReason</span></span>](../resources/intune-troubleshooting-deviceenrollmentfailurereason.md)|<span data-ttu-id="92c95-175">高レベルのエラー カテゴリ。</span><span class="sxs-lookup"><span data-stu-id="92c95-175">Highlevel failure category.</span></span> <span data-ttu-id="92c95-176">可能な値は、`unknown`、`authentication`、`authorization`、`accountValidation`、`userValidation`、`deviceNotSupported`、`inMaintenance`、`badRequest`、`featureNotSupported`、`enrollmentRestrictionsEnforced`、`clientDisconnected`、`userAbandonment` です。</span><span class="sxs-lookup"><span data-stu-id="92c95-176">Possible values are: `unknown`, `authentication`, `authorization`, `accountValidation`, `userValidation`, `deviceNotSupported`, `inMaintenance`, `badRequest`, `featureNotSupported`, `enrollmentRestrictionsEnforced`, `clientDisconnected`, `userAbandonment`.</span></span>|
|<span data-ttu-id="92c95-177">failureReason</span><span class="sxs-lookup"><span data-stu-id="92c95-177">failureReason</span></span>|<span data-ttu-id="92c95-178">String</span><span class="sxs-lookup"><span data-stu-id="92c95-178">String</span></span>|<span data-ttu-id="92c95-179">詳細なエラーの理由。</span><span class="sxs-lookup"><span data-stu-id="92c95-179">Detailed failure reason.</span></span>|



## <a name="response"></a><span data-ttu-id="92c95-180">応答</span><span class="sxs-lookup"><span data-stu-id="92c95-180">Response</span></span>
<span data-ttu-id="92c95-181">成功した場合、このメソッドは `200 OK` 応答コードと、更新された [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md) オブジェクトを応答本文で返します。</span><span class="sxs-lookup"><span data-stu-id="92c95-181">If successful, this method returns a `200 OK` response code and an updated [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="92c95-182">例</span><span class="sxs-lookup"><span data-stu-id="92c95-182">Example</span></span>

### <a name="request"></a><span data-ttu-id="92c95-183">要求</span><span class="sxs-lookup"><span data-stu-id="92c95-183">Request</span></span>
<span data-ttu-id="92c95-184">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="92c95-184">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="92c95-185">応答</span><span class="sxs-lookup"><span data-stu-id="92c95-185">Response</span></span>
<span data-ttu-id="92c95-p108">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="92c95-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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






