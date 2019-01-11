---
title: Get deviceConfigurationDeviceStatus
description: deviceConfigurationDeviceStatus オブジェクトのプロパティとリレーションシップを読み取ります。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 63110ec5c71e773e66a15318f16a97c73b13581f
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27852298"
---
# <a name="get-deviceconfigurationdevicestatus"></a><span data-ttu-id="bcac2-103">Get deviceConfigurationDeviceStatus</span><span class="sxs-lookup"><span data-stu-id="bcac2-103">Get deviceConfigurationDeviceStatus</span></span>

> <span data-ttu-id="bcac2-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="bcac2-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="bcac2-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="bcac2-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="bcac2-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="bcac2-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="bcac2-107">[deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="bcac2-107">Read properties and relationships of the [deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="bcac2-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="bcac2-108">Prerequisites</span></span>
<span data-ttu-id="bcac2-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="bcac2-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bcac2-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="bcac2-111">Permission type</span></span>|<span data-ttu-id="bcac2-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="bcac2-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="bcac2-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="bcac2-113">Delegated (work or school account)</span></span>|<span data-ttu-id="bcac2-114">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="bcac2-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="bcac2-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="bcac2-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="bcac2-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="bcac2-116">Not supported.</span></span>|
|<span data-ttu-id="bcac2-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="bcac2-117">Application</span></span>|<span data-ttu-id="bcac2-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="bcac2-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="bcac2-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="bcac2-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/deviceStatuses/{deviceConfigurationDeviceStatusId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/rootCertificate/deviceStatuses/{deviceConfigurationDeviceStatusId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/identityCertificate/deviceStatuses/{deviceConfigurationDeviceStatusId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/identityCertificate/rootCertificate/deviceStatuses/{deviceConfigurationDeviceStatusId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.iosScepCertificateProfile/rootCertificate/deviceStatuses/{deviceConfigurationDeviceStatusId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.macOSScepCertificateProfile/rootCertificate/deviceStatuses/{deviceConfigurationDeviceStatusId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsPhone81VpnConfiguration/identityCertificate/deviceStatuses/{deviceConfigurationDeviceStatusId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/identityCertificateForClientAuthentication/deviceStatuses/{deviceConfigurationDeviceStatusId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/rootCertificatesForServerValidation/{windows81TrustedRootCertificateId}/deviceStatuses/{deviceConfigurationDeviceStatusId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="bcac2-120">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="bcac2-120">Optional query parameters</span></span>
<span data-ttu-id="bcac2-121">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="bcac2-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="bcac2-122">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="bcac2-122">Request headers</span></span>
|<span data-ttu-id="bcac2-123">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="bcac2-123">Header</span></span>|<span data-ttu-id="bcac2-124">値</span><span class="sxs-lookup"><span data-stu-id="bcac2-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="bcac2-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="bcac2-125">Authorization</span></span>|<span data-ttu-id="bcac2-126">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="bcac2-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="bcac2-127">Accept</span><span class="sxs-lookup"><span data-stu-id="bcac2-127">Accept</span></span>|<span data-ttu-id="bcac2-128">application/json</span><span class="sxs-lookup"><span data-stu-id="bcac2-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="bcac2-129">要求本文</span><span class="sxs-lookup"><span data-stu-id="bcac2-129">Request body</span></span>
<span data-ttu-id="bcac2-130">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="bcac2-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="bcac2-131">応答</span><span class="sxs-lookup"><span data-stu-id="bcac2-131">Response</span></span>
<span data-ttu-id="bcac2-132">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="bcac2-132">If successful, this method returns a `200 OK` response code and [deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bcac2-133">例</span><span class="sxs-lookup"><span data-stu-id="bcac2-133">Example</span></span>
### <a name="request"></a><span data-ttu-id="bcac2-134">要求</span><span class="sxs-lookup"><span data-stu-id="bcac2-134">Request</span></span>
<span data-ttu-id="bcac2-135">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="bcac2-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/deviceStatuses/{deviceConfigurationDeviceStatusId}
```

### <a name="response"></a><span data-ttu-id="bcac2-136">応答</span><span class="sxs-lookup"><span data-stu-id="bcac2-136">Response</span></span>
<span data-ttu-id="bcac2-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="bcac2-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 535

{
  "value": {
    "@odata.type": "#microsoft.graph.deviceConfigurationDeviceStatus",
    "id": "674e98e5-98e5-674e-e598-4e67e5984e67",
    "deviceDisplayName": "Device Display Name value",
    "userName": "User Name value",
    "deviceModel": "Device Model value",
    "platform": 8,
    "complianceGracePeriodExpirationDateTime": "2016-12-31T23:56:44.951111-08:00",
    "status": "notApplicable",
    "lastReportedDateTime": "2017-01-01T00:00:17.7769392-08:00",
    "userPrincipalName": "User Principal Name value"
  }
}
```





