---
title: Get managedDeviceOverview
description: managedDeviceOverview オブジェクトのプロパティとリレーションシップを読み取ります。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 4515c143de30007104c7addfb148a9965118caad
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27826384"
---
# <a name="get-manageddeviceoverview"></a><span data-ttu-id="95ab4-103">Get managedDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="95ab4-103">Get managedDeviceOverview</span></span>

> <span data-ttu-id="95ab4-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="95ab4-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="95ab4-105">[managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="95ab4-105">Read properties and relationships of the [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="95ab4-106">前提条件</span><span class="sxs-lookup"><span data-stu-id="95ab4-106">Prerequisites</span></span>
<span data-ttu-id="95ab4-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="95ab4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="95ab4-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="95ab4-109">Permission type</span></span>|<span data-ttu-id="95ab4-110">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="95ab4-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="95ab4-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="95ab4-111">Delegated (work or school account)</span></span>|<span data-ttu-id="95ab4-112">DeviceManagementManagedDevices.ReadWrite.All、DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="95ab4-112">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="95ab4-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="95ab4-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="95ab4-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="95ab4-114">Not supported.</span></span>|
|<span data-ttu-id="95ab4-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="95ab4-115">Application</span></span>|<span data-ttu-id="95ab4-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="95ab4-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="95ab4-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="95ab4-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/managedDeviceOverview
```

## <a name="optional-query-parameters"></a><span data-ttu-id="95ab4-118">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="95ab4-118">Optional query parameters</span></span>
<span data-ttu-id="95ab4-119">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="95ab4-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="95ab4-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="95ab4-120">Request headers</span></span>
|<span data-ttu-id="95ab4-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="95ab4-121">Header</span></span>|<span data-ttu-id="95ab4-122">値</span><span class="sxs-lookup"><span data-stu-id="95ab4-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="95ab4-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="95ab4-123">Authorization</span></span>|<span data-ttu-id="95ab4-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="95ab4-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="95ab4-125">Accept</span><span class="sxs-lookup"><span data-stu-id="95ab4-125">Accept</span></span>|<span data-ttu-id="95ab4-126">application/json</span><span class="sxs-lookup"><span data-stu-id="95ab4-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="95ab4-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="95ab4-127">Request body</span></span>
<span data-ttu-id="95ab4-128">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="95ab4-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="95ab4-129">応答</span><span class="sxs-lookup"><span data-stu-id="95ab4-129">Response</span></span>
<span data-ttu-id="95ab4-130">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="95ab4-130">If successful, this method returns a `200 OK` response code and [managedDeviceOverview](../resources/intune-devices-manageddeviceoverview.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="95ab4-131">例</span><span class="sxs-lookup"><span data-stu-id="95ab4-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="95ab4-132">要求</span><span class="sxs-lookup"><span data-stu-id="95ab4-132">Request</span></span>
<span data-ttu-id="95ab4-133">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="95ab4-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/managedDeviceOverview
```

### <a name="response"></a><span data-ttu-id="95ab4-134">応答</span><span class="sxs-lookup"><span data-stu-id="95ab4-134">Response</span></span>
<span data-ttu-id="95ab4-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="95ab4-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 797

{
  "value": {
    "@odata.type": "#microsoft.graph.managedDeviceOverview",
    "id": "42a91653-1653-42a9-5316-a9425316a942",
    "enrolledDeviceCount": 3,
    "mdmEnrolledCount": 0,
    "dualEnrolledDeviceCount": 7,
    "deviceOperatingSystemSummary": {
      "@odata.type": "microsoft.graph.deviceOperatingSystemSummary",
      "androidCount": 12,
      "iosCount": 8,
      "macOSCount": 10,
      "windowsMobileCount": 2,
      "windowsCount": 12,
      "unknownCount": 12
    },
    "deviceExchangeAccessStateSummary": {
      "@odata.type": "microsoft.graph.deviceExchangeAccessStateSummary",
      "allowedDeviceCount": 2,
      "blockedDeviceCount": 2,
      "quarantinedDeviceCount": 6,
      "unknownDeviceCount": 2,
      "unavailableDeviceCount": 6
    }
  }
}
```



