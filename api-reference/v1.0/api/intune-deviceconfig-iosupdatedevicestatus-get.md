---
title: Get iosUpdateDeviceStatus
description: iosUpdateDeviceStatus オブジェクトのプロパティとリレーションシップを読み取ります。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 34b8a40bfa0c20ade8b1d33b5d55ab332ab741b5
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/26/2019
ms.locfileid: "30262322"
---
# <a name="get-iosupdatedevicestatus"></a><span data-ttu-id="06c54-103">Get iosUpdateDeviceStatus</span><span class="sxs-lookup"><span data-stu-id="06c54-103">Get iosUpdateDeviceStatus</span></span>

> <span data-ttu-id="06c54-104">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="06c54-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="06c54-105">[iosUpdateDeviceStatus](../resources/intune-deviceconfig-iosupdatedevicestatus.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="06c54-105">Read properties and relationships of the [iosUpdateDeviceStatus](../resources/intune-deviceconfig-iosupdatedevicestatus.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="06c54-106">前提条件</span><span class="sxs-lookup"><span data-stu-id="06c54-106">Prerequisites</span></span>
<span data-ttu-id="06c54-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/concepts/permissions-reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="06c54-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="06c54-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="06c54-109">Permission type</span></span>|<span data-ttu-id="06c54-110">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="06c54-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="06c54-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="06c54-111">Delegated (work or school account)</span></span>|<span data-ttu-id="06c54-112">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="06c54-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="06c54-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="06c54-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="06c54-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="06c54-114">Not supported.</span></span>|
|<span data-ttu-id="06c54-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="06c54-115">Application</span></span>|<span data-ttu-id="06c54-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="06c54-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="06c54-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="06c54-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/iosUpdateStatuses/{iosUpdateDeviceStatusId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="06c54-118">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="06c54-118">Optional query parameters</span></span>
<span data-ttu-id="06c54-119">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://docs.microsoft.com/en-us/graph/query-parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="06c54-119">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="06c54-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="06c54-120">Request headers</span></span>
|<span data-ttu-id="06c54-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="06c54-121">Header</span></span>|<span data-ttu-id="06c54-122">値</span><span class="sxs-lookup"><span data-stu-id="06c54-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="06c54-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="06c54-123">Authorization</span></span>|<span data-ttu-id="06c54-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="06c54-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="06c54-125">承諾</span><span class="sxs-lookup"><span data-stu-id="06c54-125">Accept</span></span>|<span data-ttu-id="06c54-126">application/json</span><span class="sxs-lookup"><span data-stu-id="06c54-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="06c54-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="06c54-127">Request body</span></span>
<span data-ttu-id="06c54-128">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="06c54-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="06c54-129">応答</span><span class="sxs-lookup"><span data-stu-id="06c54-129">Response</span></span>
<span data-ttu-id="06c54-130">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [iosUpdateDeviceStatus](../resources/intune-deviceconfig-iosupdatedevicestatus.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="06c54-130">If successful, this method returns a `200 OK` response code and [iosUpdateDeviceStatus](../resources/intune-deviceconfig-iosupdatedevicestatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="06c54-131">例</span><span class="sxs-lookup"><span data-stu-id="06c54-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="06c54-132">要求</span><span class="sxs-lookup"><span data-stu-id="06c54-132">Request</span></span>
<span data-ttu-id="06c54-133">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="06c54-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/iosUpdateStatuses/{iosUpdateDeviceStatusId}
```

### <a name="response"></a><span data-ttu-id="06c54-134">応答</span><span class="sxs-lookup"><span data-stu-id="06c54-134">Response</span></span>
<span data-ttu-id="06c54-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="06c54-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 646

{
  "value": {
    "@odata.type": "#microsoft.graph.iosUpdateDeviceStatus",
    "id": "63a79499-9499-63a7-9994-a7639994a763",
    "installStatus": "available",
    "osVersion": "Os Version value",
    "deviceId": "Device Id value",
    "userId": "User Id value",
    "deviceDisplayName": "Device Display Name value",
    "userName": "User Name value",
    "deviceModel": "Device Model value",
    "complianceGracePeriodExpirationDateTime": "2016-12-31T23:56:44.951111-08:00",
    "status": "notApplicable",
    "lastReportedDateTime": "2017-01-01T00:00:17.7769392-08:00",
    "userPrincipalName": "User Principal Name value"
  }
}
```



