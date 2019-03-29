---
title: enrollmentTroubleshootingEvent のリスト
description: enrollmentTroubleshootingEvent オブジェクトのプロパティとリレーションシップをリストします。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: e0fbe2d03a96af0dfe28fe08ce9bdd7e3a06f6c5
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/29/2019
ms.locfileid: "30960518"
---
# <a name="list-enrollmenttroubleshootingevents"></a><span data-ttu-id="0ac70-103">enrollmentTroubleshootingEvent のリスト</span><span class="sxs-lookup"><span data-stu-id="0ac70-103">List enrollmentTroubleshootingEvents</span></span>

> <span data-ttu-id="0ac70-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="0ac70-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0ac70-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="0ac70-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0ac70-106">[enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="0ac70-106">List properties and relationships of the [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="0ac70-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="0ac70-107">Prerequisites</span></span>
<span data-ttu-id="0ac70-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="0ac70-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0ac70-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="0ac70-110">Permission type</span></span>|<span data-ttu-id="0ac70-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="0ac70-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0ac70-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="0ac70-112">Delegated (work or school account)</span></span>|<span data-ttu-id="0ac70-113">DeviceManagementManagedDevices.ReadWrite.All、DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="0ac70-113">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="0ac70-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="0ac70-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0ac70-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="0ac70-115">Not supported.</span></span>|
|<span data-ttu-id="0ac70-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="0ac70-116">Application</span></span>|<span data-ttu-id="0ac70-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="0ac70-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="0ac70-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="0ac70-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/troubleshootingEvents
```

## <a name="request-headers"></a><span data-ttu-id="0ac70-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="0ac70-119">Request headers</span></span>
|<span data-ttu-id="0ac70-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="0ac70-120">Header</span></span>|<span data-ttu-id="0ac70-121">値</span><span class="sxs-lookup"><span data-stu-id="0ac70-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0ac70-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="0ac70-122">Authorization</span></span>|<span data-ttu-id="0ac70-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="0ac70-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0ac70-124">承諾</span><span class="sxs-lookup"><span data-stu-id="0ac70-124">Accept</span></span>|<span data-ttu-id="0ac70-125">application/json</span><span class="sxs-lookup"><span data-stu-id="0ac70-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0ac70-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="0ac70-126">Request body</span></span>
<span data-ttu-id="0ac70-127">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="0ac70-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0ac70-128">応答</span><span class="sxs-lookup"><span data-stu-id="0ac70-128">Response</span></span>
<span data-ttu-id="0ac70-129">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md) オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="0ac70-129">If successful, this method returns a `200 OK` response code and a collection of [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0ac70-130">例</span><span class="sxs-lookup"><span data-stu-id="0ac70-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="0ac70-131">要求</span><span class="sxs-lookup"><span data-stu-id="0ac70-131">Request</span></span>
<span data-ttu-id="0ac70-132">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="0ac70-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/troubleshootingEvents
```

### <a name="response"></a><span data-ttu-id="0ac70-133">応答</span><span class="sxs-lookup"><span data-stu-id="0ac70-133">Response</span></span>
<span data-ttu-id="0ac70-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="0ac70-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1400

{
  "value": [
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
  ]
}
```




