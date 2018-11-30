---
title: iosUpdateDeviceStatuses のリスト
description: iosUpdateDeviceStatus オブジェクトのプロパティとリレーションシップをリストします。
ms.openlocfilehash: 4e7cbe8c1899aa4efa17da610be9f85ba6143872
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27023663"
---
# <a name="list-iosupdatedevicestatuses"></a><span data-ttu-id="bdf53-103">iosUpdateDeviceStatuses のリスト</span><span class="sxs-lookup"><span data-stu-id="bdf53-103">List iosUpdateDeviceStatuses</span></span>

> <span data-ttu-id="bdf53-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="bdf53-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="bdf53-105">[iosUpdateDeviceStatus](../resources/intune-deviceconfig-iosupdatedevicestatus.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="bdf53-105">List properties and relationships of the [iosUpdateDeviceStatus](../resources/intune-deviceconfig-iosupdatedevicestatus.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="bdf53-106">前提条件</span><span class="sxs-lookup"><span data-stu-id="bdf53-106">Prerequisites</span></span>
<span data-ttu-id="bdf53-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="bdf53-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bdf53-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="bdf53-109">Permission type</span></span>|<span data-ttu-id="bdf53-110">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="bdf53-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="bdf53-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="bdf53-111">Delegated (work or school account)</span></span>|<span data-ttu-id="bdf53-112">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="bdf53-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="bdf53-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="bdf53-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="bdf53-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="bdf53-114">Not supported.</span></span>|
|<span data-ttu-id="bdf53-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="bdf53-115">Application</span></span>|<span data-ttu-id="bdf53-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="bdf53-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="bdf53-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="bdf53-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/iosUpdateStatuses
```

## <a name="request-headers"></a><span data-ttu-id="bdf53-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="bdf53-118">Request headers</span></span>
|<span data-ttu-id="bdf53-119">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="bdf53-119">Header</span></span>|<span data-ttu-id="bdf53-120">値</span><span class="sxs-lookup"><span data-stu-id="bdf53-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="bdf53-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="bdf53-121">Authorization</span></span>|<span data-ttu-id="bdf53-122">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="bdf53-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="bdf53-123">Accept</span><span class="sxs-lookup"><span data-stu-id="bdf53-123">Accept</span></span>|<span data-ttu-id="bdf53-124">application/json</span><span class="sxs-lookup"><span data-stu-id="bdf53-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="bdf53-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="bdf53-125">Request body</span></span>
<span data-ttu-id="bdf53-126">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="bdf53-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="bdf53-127">応答</span><span class="sxs-lookup"><span data-stu-id="bdf53-127">Response</span></span>
<span data-ttu-id="bdf53-128">成功した場合、このメソッドは `200 OK`応答コードと、応答本文で [iosUpdateDeviceStatus](../resources/intune-deviceconfig-iosupdatedevicestatus.md) オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="bdf53-128">If successful, this method returns a `200 OK` response code and a collection of [iosUpdateDeviceStatus](../resources/intune-deviceconfig-iosupdatedevicestatus.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bdf53-129">例</span><span class="sxs-lookup"><span data-stu-id="bdf53-129">Example</span></span>
### <a name="request"></a><span data-ttu-id="bdf53-130">要求</span><span class="sxs-lookup"><span data-stu-id="bdf53-130">Request</span></span>
<span data-ttu-id="bdf53-131">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="bdf53-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/iosUpdateStatuses
```

### <a name="response"></a><span data-ttu-id="bdf53-132">応答</span><span class="sxs-lookup"><span data-stu-id="bdf53-132">Response</span></span>
<span data-ttu-id="bdf53-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="bdf53-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 686

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
      "complianceGracePeriodExpirationDateTime": "2016-12-31T23:56:44.951111-08:00",
      "status": "notApplicable",
      "lastReportedDateTime": "2017-01-01T00:00:17.7769392-08:00",
      "userPrincipalName": "User Principal Name value"
    }
  ]
}
```



