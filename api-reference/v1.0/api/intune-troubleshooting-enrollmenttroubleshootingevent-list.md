---
title: enrollmentTroubleshootingEvent のリスト
description: enrollmentTroubleshootingEvent オブジェクトのプロパティとリレーションシップをリストします。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 106fd47aba30b4df04a08485432dbbea67cb6f03
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32576354"
---
# <a name="list-enrollmenttroubleshootingevents"></a><span data-ttu-id="2cfd3-103">enrollmentTroubleshootingEvent のリスト</span><span class="sxs-lookup"><span data-stu-id="2cfd3-103">List enrollmentTroubleshootingEvents</span></span>

> <span data-ttu-id="2cfd3-104">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="2cfd3-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2cfd3-105">[enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="2cfd3-105">List properties and relationships of the [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="2cfd3-106">前提条件</span><span class="sxs-lookup"><span data-stu-id="2cfd3-106">Prerequisites</span></span>
<span data-ttu-id="2cfd3-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="2cfd3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2cfd3-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="2cfd3-109">Permission type</span></span>|<span data-ttu-id="2cfd3-110">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="2cfd3-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2cfd3-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="2cfd3-111">Delegated (work or school account)</span></span>|<span data-ttu-id="2cfd3-112">DeviceManagementManagedDevices.ReadWrite.All、DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="2cfd3-112">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="2cfd3-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="2cfd3-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2cfd3-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="2cfd3-114">Not supported.</span></span>|
|<span data-ttu-id="2cfd3-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="2cfd3-115">Application</span></span>|<span data-ttu-id="2cfd3-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="2cfd3-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="2cfd3-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="2cfd3-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/troubleshootingEvents
```

## <a name="request-headers"></a><span data-ttu-id="2cfd3-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="2cfd3-118">Request headers</span></span>
|<span data-ttu-id="2cfd3-119">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="2cfd3-119">Header</span></span>|<span data-ttu-id="2cfd3-120">値</span><span class="sxs-lookup"><span data-stu-id="2cfd3-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2cfd3-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="2cfd3-121">Authorization</span></span>|<span data-ttu-id="2cfd3-122">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="2cfd3-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2cfd3-123">承諾</span><span class="sxs-lookup"><span data-stu-id="2cfd3-123">Accept</span></span>|<span data-ttu-id="2cfd3-124">application/json</span><span class="sxs-lookup"><span data-stu-id="2cfd3-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2cfd3-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="2cfd3-125">Request body</span></span>
<span data-ttu-id="2cfd3-126">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="2cfd3-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2cfd3-127">応答</span><span class="sxs-lookup"><span data-stu-id="2cfd3-127">Response</span></span>
<span data-ttu-id="2cfd3-128">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md) オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="2cfd3-128">If successful, this method returns a `200 OK` response code and a collection of [enrollmentTroubleshootingEvent](../resources/intune-troubleshooting-enrollmenttroubleshootingevent.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2cfd3-129">例</span><span class="sxs-lookup"><span data-stu-id="2cfd3-129">Example</span></span>

### <a name="request"></a><span data-ttu-id="2cfd3-130">要求</span><span class="sxs-lookup"><span data-stu-id="2cfd3-130">Request</span></span>
<span data-ttu-id="2cfd3-131">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="2cfd3-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/troubleshootingEvents
```

### <a name="response"></a><span data-ttu-id="2cfd3-132">応答</span><span class="sxs-lookup"><span data-stu-id="2cfd3-132">Response</span></span>
<span data-ttu-id="2cfd3-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="2cfd3-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 639

{
  "value": [
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
  ]
}
```



