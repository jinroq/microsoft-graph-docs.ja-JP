---
title: deviceConfigurationDeviceStatuses のリスト
description: deviceConfigurationDeviceStatus オブジェクトのプロパティとリレーションシップをリストします。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: dfbf58d62d82b41efa2a1fe3bbe687fec824cf96
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/14/2019
ms.locfileid: "34967686"
---
# <a name="list-deviceconfigurationdevicestatuses"></a><span data-ttu-id="6b055-103">deviceConfigurationDeviceStatuses のリスト</span><span class="sxs-lookup"><span data-stu-id="6b055-103">List deviceConfigurationDeviceStatuses</span></span>

> <span data-ttu-id="6b055-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="6b055-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6b055-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="6b055-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6b055-106">[deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="6b055-106">List properties and relationships of the [deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="6b055-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="6b055-107">Prerequisites</span></span>
<span data-ttu-id="6b055-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="6b055-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6b055-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="6b055-110">Permission type</span></span>|<span data-ttu-id="6b055-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="6b055-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6b055-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="6b055-112">Delegated (work or school account)</span></span>|<span data-ttu-id="6b055-113">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="6b055-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="6b055-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="6b055-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6b055-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="6b055-115">Not supported.</span></span>|
|<span data-ttu-id="6b055-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="6b055-116">Application</span></span>|<span data-ttu-id="6b055-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="6b055-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="6b055-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="6b055-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/deviceStatuses
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/rootCertificate/deviceStatuses
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/identityCertificate/deviceStatuses
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/identityCertificate/rootCertificate/deviceStatuses
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.iosScepCertificateProfile/rootCertificate/deviceStatuses
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.macOSScepCertificateProfile/rootCertificate/deviceStatuses
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsPhone81VpnConfiguration/identityCertificate/deviceStatuses
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/identityCertificateForClientAuthentication/deviceStatuses
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/rootCertificatesForServerValidation/{windows81TrustedRootCertificateId}/deviceStatuses
```

## <a name="request-headers"></a><span data-ttu-id="6b055-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="6b055-119">Request headers</span></span>
|<span data-ttu-id="6b055-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="6b055-120">Header</span></span>|<span data-ttu-id="6b055-121">値</span><span class="sxs-lookup"><span data-stu-id="6b055-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6b055-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="6b055-122">Authorization</span></span>|<span data-ttu-id="6b055-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="6b055-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6b055-124">承諾</span><span class="sxs-lookup"><span data-stu-id="6b055-124">Accept</span></span>|<span data-ttu-id="6b055-125">application/json</span><span class="sxs-lookup"><span data-stu-id="6b055-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6b055-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="6b055-126">Request body</span></span>
<span data-ttu-id="6b055-127">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="6b055-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6b055-128">応答</span><span class="sxs-lookup"><span data-stu-id="6b055-128">Response</span></span>
<span data-ttu-id="6b055-129">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md) オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="6b055-129">If successful, this method returns a `200 OK` response code and a collection of [deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6b055-130">例</span><span class="sxs-lookup"><span data-stu-id="6b055-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="6b055-131">要求</span><span class="sxs-lookup"><span data-stu-id="6b055-131">Request</span></span>
<span data-ttu-id="6b055-132">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="6b055-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/deviceStatuses
```

### <a name="response"></a><span data-ttu-id="6b055-133">応答</span><span class="sxs-lookup"><span data-stu-id="6b055-133">Response</span></span>
<span data-ttu-id="6b055-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="6b055-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 569

{
  "value": [
    {
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
  ]
}
```





