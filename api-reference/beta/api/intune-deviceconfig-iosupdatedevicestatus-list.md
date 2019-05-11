---
title: iosUpdateDeviceStatuses のリスト
description: iosUpdateDeviceStatus オブジェクトのプロパティとリレーションシップをリストします。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: bf09ec5717485d6dbf069e4c8ecadad9f555e54e
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/11/2019
ms.locfileid: "33923154"
---
# <a name="list-iosupdatedevicestatuses"></a><span data-ttu-id="2eadc-103">iosUpdateDeviceStatuses のリスト</span><span class="sxs-lookup"><span data-stu-id="2eadc-103">List iosUpdateDeviceStatuses</span></span>

> <span data-ttu-id="2eadc-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="2eadc-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2eadc-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="2eadc-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2eadc-106">[iosUpdateDeviceStatus](../resources/intune-deviceconfig-iosupdatedevicestatus.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="2eadc-106">List properties and relationships of the [iosUpdateDeviceStatus](../resources/intune-deviceconfig-iosupdatedevicestatus.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="2eadc-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="2eadc-107">Prerequisites</span></span>
<span data-ttu-id="2eadc-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="2eadc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2eadc-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="2eadc-110">Permission type</span></span>|<span data-ttu-id="2eadc-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="2eadc-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2eadc-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="2eadc-112">Delegated (work or school account)</span></span>|<span data-ttu-id="2eadc-113">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="2eadc-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="2eadc-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="2eadc-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2eadc-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="2eadc-115">Not supported.</span></span>|
|<span data-ttu-id="2eadc-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="2eadc-116">Application</span></span>|<span data-ttu-id="2eadc-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="2eadc-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="2eadc-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="2eadc-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/iosUpdateStatuses
```

## <a name="request-headers"></a><span data-ttu-id="2eadc-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="2eadc-119">Request headers</span></span>
|<span data-ttu-id="2eadc-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="2eadc-120">Header</span></span>|<span data-ttu-id="2eadc-121">値</span><span class="sxs-lookup"><span data-stu-id="2eadc-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2eadc-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="2eadc-122">Authorization</span></span>|<span data-ttu-id="2eadc-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="2eadc-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2eadc-124">承諾</span><span class="sxs-lookup"><span data-stu-id="2eadc-124">Accept</span></span>|<span data-ttu-id="2eadc-125">application/json</span><span class="sxs-lookup"><span data-stu-id="2eadc-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2eadc-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="2eadc-126">Request body</span></span>
<span data-ttu-id="2eadc-127">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="2eadc-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2eadc-128">応答</span><span class="sxs-lookup"><span data-stu-id="2eadc-128">Response</span></span>
<span data-ttu-id="2eadc-129">成功した場合、このメソッドは `200 OK`応答コードと、応答本文で [iosUpdateDeviceStatus](../resources/intune-deviceconfig-iosupdatedevicestatus.md) オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="2eadc-129">If successful, this method returns a `200 OK` response code and a collection of [iosUpdateDeviceStatus](../resources/intune-deviceconfig-iosupdatedevicestatus.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2eadc-130">例</span><span class="sxs-lookup"><span data-stu-id="2eadc-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="2eadc-131">要求</span><span class="sxs-lookup"><span data-stu-id="2eadc-131">Request</span></span>
<span data-ttu-id="2eadc-132">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="2eadc-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/iosUpdateStatuses
```

### <a name="response"></a><span data-ttu-id="2eadc-133">応答</span><span class="sxs-lookup"><span data-stu-id="2eadc-133">Response</span></span>
<span data-ttu-id="2eadc-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="2eadc-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 708

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.iosUpdateDeviceStatus",
      "id": "63a79499-9499-63a7-9994-a7639994a763",
      "installStatus": "available",
      "osVersion": "Os Version value",
      "deviceId": "Device Id value",
      "userId": "User Id value",
      "deviceDisplayName": "Device Display Name value",
      "userName": "User Name value",
      "deviceModel": "Device Model value",
      "platform": 8,
      "complianceGracePeriodExpirationDateTime": "2016-12-31T23:56:44.951111-08:00",
      "status": "notApplicable",
      "lastReportedDateTime": "2017-01-01T00:00:17.7769392-08:00",
      "userPrincipalName": "User Principal Name value"
    }
  ]
}
```




