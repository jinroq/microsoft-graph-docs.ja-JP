---
title: Get deviceConfigurationDeviceOverview
description: deviceConfigurationDeviceOverview オブジェクトのプロパティとリレーションシップを読み取ります。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: a1803bbdd5bf2d82d698b513ae422286bbf80954
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/11/2019
ms.locfileid: "31776557"
---
# <a name="get-deviceconfigurationdeviceoverview"></a><span data-ttu-id="801be-103">Get deviceConfigurationDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="801be-103">Get deviceConfigurationDeviceOverview</span></span>

> <span data-ttu-id="801be-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="801be-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="801be-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="801be-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="801be-106">[deviceConfigurationDeviceOverview](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="801be-106">Read properties and relationships of the [deviceConfigurationDeviceOverview](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="801be-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="801be-107">Prerequisites</span></span>
<span data-ttu-id="801be-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="801be-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="801be-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="801be-110">Permission type</span></span>|<span data-ttu-id="801be-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="801be-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="801be-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="801be-112">Delegated (work or school account)</span></span>|<span data-ttu-id="801be-113">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="801be-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="801be-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="801be-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="801be-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="801be-115">Not supported.</span></span>|
|<span data-ttu-id="801be-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="801be-116">Application</span></span>|<span data-ttu-id="801be-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="801be-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="801be-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="801be-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/deviceStatusOverview
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/rootCertificate/deviceStatusOverview
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/identityCertificate/deviceStatusOverview
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/identityCertificate/rootCertificate/deviceStatusOverview
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.iosScepCertificateProfile/rootCertificate/deviceStatusOverview
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.macOSScepCertificateProfile/rootCertificate/deviceStatusOverview
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsPhone81VpnConfiguration/identityCertificate/deviceStatusOverview
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/identityCertificateForClientAuthentication/deviceStatusOverview
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/rootCertificatesForServerValidation/{windows81TrustedRootCertificateId}/deviceStatusOverview
```

## <a name="optional-query-parameters"></a><span data-ttu-id="801be-119">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="801be-119">Optional query parameters</span></span>
<span data-ttu-id="801be-120">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://docs.microsoft.com/en-us/graph/query-parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="801be-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="801be-121">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="801be-121">Request headers</span></span>
|<span data-ttu-id="801be-122">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="801be-122">Header</span></span>|<span data-ttu-id="801be-123">値</span><span class="sxs-lookup"><span data-stu-id="801be-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="801be-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="801be-124">Authorization</span></span>|<span data-ttu-id="801be-125">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="801be-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="801be-126">承諾</span><span class="sxs-lookup"><span data-stu-id="801be-126">Accept</span></span>|<span data-ttu-id="801be-127">application/json</span><span class="sxs-lookup"><span data-stu-id="801be-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="801be-128">要求本文</span><span class="sxs-lookup"><span data-stu-id="801be-128">Request body</span></span>
<span data-ttu-id="801be-129">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="801be-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="801be-130">応答</span><span class="sxs-lookup"><span data-stu-id="801be-130">Response</span></span>
<span data-ttu-id="801be-131">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [deviceConfigurationDeviceOverview](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="801be-131">If successful, this method returns a `200 OK` response code and [deviceConfigurationDeviceOverview](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="801be-132">例</span><span class="sxs-lookup"><span data-stu-id="801be-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="801be-133">要求</span><span class="sxs-lookup"><span data-stu-id="801be-133">Request</span></span>
<span data-ttu-id="801be-134">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="801be-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/deviceStatusOverview
```

### <a name="response"></a><span data-ttu-id="801be-135">応答</span><span class="sxs-lookup"><span data-stu-id="801be-135">Response</span></span>
<span data-ttu-id="801be-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="801be-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 435

{
  "value": {
    "@odata.type": "#microsoft.graph.deviceConfigurationDeviceOverview",
    "id": "62d48e3a-8e3a-62d4-3a8e-d4623a8ed462",
    "pendingCount": 12,
    "notApplicableCount": 2,
    "notApplicablePlatformCount": 10,
    "successCount": 12,
    "errorCount": 10,
    "failedCount": 11,
    "conflictCount": 13,
    "lastUpdateDateTime": "2016-12-31T23:58:21.6459442-08:00",
    "configurationVersion": 4
  }
}
```





