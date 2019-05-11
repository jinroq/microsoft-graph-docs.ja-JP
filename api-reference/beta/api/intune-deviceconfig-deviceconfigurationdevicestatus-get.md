---
title: Get deviceConfigurationDeviceStatus
description: deviceConfigurationDeviceStatus オブジェクトのプロパティとリレーションシップを読み取ります。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: d6f623d813b56be4b1036592c794e8dbd191e34b
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/11/2019
ms.locfileid: "33927350"
---
# <a name="get-deviceconfigurationdevicestatus"></a><span data-ttu-id="2699c-103">Get deviceConfigurationDeviceStatus</span><span class="sxs-lookup"><span data-stu-id="2699c-103">Get deviceConfigurationDeviceStatus</span></span>

> <span data-ttu-id="2699c-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="2699c-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2699c-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="2699c-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2699c-106">[deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="2699c-106">Read properties and relationships of the [deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="2699c-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="2699c-107">Prerequisites</span></span>
<span data-ttu-id="2699c-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="2699c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2699c-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="2699c-110">Permission type</span></span>|<span data-ttu-id="2699c-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="2699c-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2699c-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="2699c-112">Delegated (work or school account)</span></span>|<span data-ttu-id="2699c-113">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="2699c-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="2699c-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="2699c-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2699c-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="2699c-115">Not supported.</span></span>|
|<span data-ttu-id="2699c-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="2699c-116">Application</span></span>|<span data-ttu-id="2699c-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="2699c-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="2699c-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="2699c-118">HTTP Request</span></span>
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

## <a name="optional-query-parameters"></a><span data-ttu-id="2699c-119">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="2699c-119">Optional query parameters</span></span>
<span data-ttu-id="2699c-120">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://docs.microsoft.com/en-us/graph/query-parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="2699c-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="2699c-121">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="2699c-121">Request headers</span></span>
|<span data-ttu-id="2699c-122">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="2699c-122">Header</span></span>|<span data-ttu-id="2699c-123">値</span><span class="sxs-lookup"><span data-stu-id="2699c-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2699c-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="2699c-124">Authorization</span></span>|<span data-ttu-id="2699c-125">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="2699c-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2699c-126">承諾</span><span class="sxs-lookup"><span data-stu-id="2699c-126">Accept</span></span>|<span data-ttu-id="2699c-127">application/json</span><span class="sxs-lookup"><span data-stu-id="2699c-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2699c-128">要求本文</span><span class="sxs-lookup"><span data-stu-id="2699c-128">Request body</span></span>
<span data-ttu-id="2699c-129">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="2699c-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2699c-130">応答</span><span class="sxs-lookup"><span data-stu-id="2699c-130">Response</span></span>
<span data-ttu-id="2699c-131">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="2699c-131">If successful, this method returns a `200 OK` response code and [deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2699c-132">例</span><span class="sxs-lookup"><span data-stu-id="2699c-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="2699c-133">要求</span><span class="sxs-lookup"><span data-stu-id="2699c-133">Request</span></span>
<span data-ttu-id="2699c-134">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="2699c-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/deviceStatuses/{deviceConfigurationDeviceStatusId}
```

### <a name="response"></a><span data-ttu-id="2699c-135">応答</span><span class="sxs-lookup"><span data-stu-id="2699c-135">Response</span></span>
<span data-ttu-id="2699c-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="2699c-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




