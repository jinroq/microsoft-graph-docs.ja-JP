---
title: enrollmentTroubleshootingEvent の取得
description: enrollmentTroubleshootingEvent オブジェクトのプロパティとリレーションシップを読み取ります。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: d10b4168514c1254f706165c26400620e9042e3c
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/21/2019
ms.locfileid: "30174735"
---
# <a name="get-enrollmenttroubleshootingevent"></a><span data-ttu-id="ae484-103">enrollmentTroubleshootingEvent の取得</span><span class="sxs-lookup"><span data-stu-id="ae484-103">Get enrollmentTroubleshootingEvent</span></span>

> <span data-ttu-id="ae484-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ae484-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ae484-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="ae484-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ae484-106">[enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="ae484-106">Read properties and relationships of the [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ae484-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="ae484-107">Prerequisites</span></span>
<span data-ttu-id="ae484-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/concepts/permissions-reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="ae484-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="ae484-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="ae484-110">Permission type</span></span>|<span data-ttu-id="ae484-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="ae484-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ae484-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="ae484-112">Delegated (work or school account)</span></span>|<span data-ttu-id="ae484-113">DeviceManagementManagedDevices.ReadWrite.All、DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="ae484-113">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="ae484-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="ae484-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ae484-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ae484-115">Not supported.</span></span>|
|<span data-ttu-id="ae484-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="ae484-116">Application</span></span>|<span data-ttu-id="ae484-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ae484-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ae484-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="ae484-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/troubleshootingEvents/{deviceManagementTroubleshootingEventId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="ae484-119">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="ae484-119">Optional query parameters</span></span>
<span data-ttu-id="ae484-120">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://docs.microsoft.com/en-us/graph/query-parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="ae484-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="ae484-121">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="ae484-121">Request headers</span></span>
|<span data-ttu-id="ae484-122">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="ae484-122">Header</span></span>|<span data-ttu-id="ae484-123">値</span><span class="sxs-lookup"><span data-stu-id="ae484-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ae484-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="ae484-124">Authorization</span></span>|<span data-ttu-id="ae484-125">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="ae484-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ae484-126">承諾</span><span class="sxs-lookup"><span data-stu-id="ae484-126">Accept</span></span>|<span data-ttu-id="ae484-127">application/json</span><span class="sxs-lookup"><span data-stu-id="ae484-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ae484-128">要求本文</span><span class="sxs-lookup"><span data-stu-id="ae484-128">Request body</span></span>
<span data-ttu-id="ae484-129">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="ae484-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ae484-130">応答</span><span class="sxs-lookup"><span data-stu-id="ae484-130">Response</span></span>
<span data-ttu-id="ae484-131">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="ae484-131">If successful, this method returns a `200 OK` response code and [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ae484-132">例</span><span class="sxs-lookup"><span data-stu-id="ae484-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="ae484-133">要求</span><span class="sxs-lookup"><span data-stu-id="ae484-133">Request</span></span>
<span data-ttu-id="ae484-134">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="ae484-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/troubleshootingEvents/{deviceManagementTroubleshootingEventId}
```

### <a name="response"></a><span data-ttu-id="ae484-135">応答</span><span class="sxs-lookup"><span data-stu-id="ae484-135">Response</span></span>
<span data-ttu-id="ae484-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="ae484-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1318

{
  "value": {
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
}
```




