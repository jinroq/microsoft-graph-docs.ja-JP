---
title: Get deviceComplianceDeviceStatus
description: deviceComplianceDeviceStatus オブジェクトのプロパティとリレーションシップを読み取ります。
ms.openlocfilehash: 4ab52855e522fcddd0edbe38f032d0c82dcf16e9
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27021960"
---
# <a name="get-devicecompliancedevicestatus"></a><span data-ttu-id="ee288-103">Get deviceComplianceDeviceStatus</span><span class="sxs-lookup"><span data-stu-id="ee288-103">Get deviceComplianceDeviceStatus</span></span>

> <span data-ttu-id="ee288-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="ee288-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="ee288-105">[deviceComplianceDeviceStatus](../resources/intune-deviceconfig-devicecompliancedevicestatus.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="ee288-105">Read properties and relationships of the [deviceComplianceDeviceStatus](../resources/intune-deviceconfig-devicecompliancedevicestatus.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="ee288-106">前提条件</span><span class="sxs-lookup"><span data-stu-id="ee288-106">Prerequisites</span></span>
<span data-ttu-id="ee288-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="ee288-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ee288-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="ee288-109">Permission type</span></span>|<span data-ttu-id="ee288-110">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="ee288-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ee288-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="ee288-111">Delegated (work or school account)</span></span>|<span data-ttu-id="ee288-112">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="ee288-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="ee288-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="ee288-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ee288-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ee288-114">Not supported.</span></span>|
|<span data-ttu-id="ee288-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="ee288-115">Application</span></span>|<span data-ttu-id="ee288-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ee288-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ee288-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="ee288-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/deviceStatuses/{deviceComplianceDeviceStatusId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="ee288-118">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="ee288-118">Optional query parameters</span></span>
<span data-ttu-id="ee288-119">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="ee288-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="ee288-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="ee288-120">Request headers</span></span>
|<span data-ttu-id="ee288-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="ee288-121">Header</span></span>|<span data-ttu-id="ee288-122">値</span><span class="sxs-lookup"><span data-stu-id="ee288-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ee288-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="ee288-123">Authorization</span></span>|<span data-ttu-id="ee288-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="ee288-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ee288-125">Accept</span><span class="sxs-lookup"><span data-stu-id="ee288-125">Accept</span></span>|<span data-ttu-id="ee288-126">application/json</span><span class="sxs-lookup"><span data-stu-id="ee288-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ee288-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="ee288-127">Request body</span></span>
<span data-ttu-id="ee288-128">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="ee288-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ee288-129">応答</span><span class="sxs-lookup"><span data-stu-id="ee288-129">Response</span></span>
<span data-ttu-id="ee288-130">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [deviceComplianceDeviceStatus](../resources/intune-deviceconfig-devicecompliancedevicestatus.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="ee288-130">If successful, this method returns a `200 OK` response code and [deviceComplianceDeviceStatus](../resources/intune-deviceconfig-devicecompliancedevicestatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ee288-131">例</span><span class="sxs-lookup"><span data-stu-id="ee288-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="ee288-132">要求</span><span class="sxs-lookup"><span data-stu-id="ee288-132">Request</span></span>
<span data-ttu-id="ee288-133">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="ee288-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/deviceStatuses/{deviceComplianceDeviceStatusId}
```

### <a name="response"></a><span data-ttu-id="ee288-134">応答</span><span class="sxs-lookup"><span data-stu-id="ee288-134">Response</span></span>
<span data-ttu-id="ee288-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="ee288-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 512

{
  "value": {
    "@odata.type": "#microsoft.graph.deviceComplianceDeviceStatus",
    "id": "c6c78124-8124-c6c7-2481-c7c62481c7c6",
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



