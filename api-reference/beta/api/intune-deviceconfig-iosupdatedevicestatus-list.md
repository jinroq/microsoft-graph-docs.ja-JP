---
title: iosUpdateDeviceStatuses のリスト
description: iosUpdateDeviceStatus オブジェクトのプロパティとリレーションシップをリストします。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 4699e4c2c1632136fd92ce7ffb987562c5bd4b06
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/21/2019
ms.locfileid: "30155357"
---
# <a name="list-iosupdatedevicestatuses"></a><span data-ttu-id="584c4-103">iosUpdateDeviceStatuses のリスト</span><span class="sxs-lookup"><span data-stu-id="584c4-103">List iosUpdateDeviceStatuses</span></span>

> <span data-ttu-id="584c4-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="584c4-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="584c4-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="584c4-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="584c4-106">[iosUpdateDeviceStatus](../resources/intune-deviceconfig-iosupdatedevicestatus.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="584c4-106">List properties and relationships of the [iosUpdateDeviceStatus](../resources/intune-deviceconfig-iosupdatedevicestatus.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="584c4-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="584c4-107">Prerequisites</span></span>
<span data-ttu-id="584c4-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/concepts/permissions-reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="584c4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="584c4-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="584c4-110">Permission type</span></span>|<span data-ttu-id="584c4-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="584c4-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="584c4-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="584c4-112">Delegated (work or school account)</span></span>|<span data-ttu-id="584c4-113">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="584c4-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="584c4-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="584c4-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="584c4-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="584c4-115">Not supported.</span></span>|
|<span data-ttu-id="584c4-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="584c4-116">Application</span></span>|<span data-ttu-id="584c4-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="584c4-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="584c4-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="584c4-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/iosUpdateStatuses
```

## <a name="request-headers"></a><span data-ttu-id="584c4-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="584c4-119">Request headers</span></span>
|<span data-ttu-id="584c4-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="584c4-120">Header</span></span>|<span data-ttu-id="584c4-121">値</span><span class="sxs-lookup"><span data-stu-id="584c4-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="584c4-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="584c4-122">Authorization</span></span>|<span data-ttu-id="584c4-123">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="584c4-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="584c4-124">承諾</span><span class="sxs-lookup"><span data-stu-id="584c4-124">Accept</span></span>|<span data-ttu-id="584c4-125">application/json</span><span class="sxs-lookup"><span data-stu-id="584c4-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="584c4-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="584c4-126">Request body</span></span>
<span data-ttu-id="584c4-127">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="584c4-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="584c4-128">応答</span><span class="sxs-lookup"><span data-stu-id="584c4-128">Response</span></span>
<span data-ttu-id="584c4-129">成功した場合、このメソッドは `200 OK`応答コードと、応答本文で [iosUpdateDeviceStatus](../resources/intune-deviceconfig-iosupdatedevicestatus.md) オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="584c4-129">If successful, this method returns a `200 OK` response code and a collection of [iosUpdateDeviceStatus](../resources/intune-deviceconfig-iosupdatedevicestatus.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="584c4-130">例</span><span class="sxs-lookup"><span data-stu-id="584c4-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="584c4-131">要求</span><span class="sxs-lookup"><span data-stu-id="584c4-131">Request</span></span>
<span data-ttu-id="584c4-132">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="584c4-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/iosUpdateStatuses
```

### <a name="response"></a><span data-ttu-id="584c4-133">応答</span><span class="sxs-lookup"><span data-stu-id="584c4-133">Response</span></span>
<span data-ttu-id="584c4-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="584c4-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




