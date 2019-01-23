---
title: Get deviceConfigurationUserStatus
description: deviceConfigurationUserStatus オブジェクトのプロパティとリレーションシップを読み取ります。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: e823a37356125da855f2bb9ea2f3b01bffd75fe4
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29411877"
---
# <a name="get-deviceconfigurationuserstatus"></a><span data-ttu-id="9d606-103">Get deviceConfigurationUserStatus</span><span class="sxs-lookup"><span data-stu-id="9d606-103">Get deviceConfigurationUserStatus</span></span>

> <span data-ttu-id="9d606-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="9d606-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="9d606-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="9d606-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="9d606-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="9d606-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9d606-107">[deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="9d606-107">Read properties and relationships of the [deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="9d606-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="9d606-108">Prerequisites</span></span>
<span data-ttu-id="9d606-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/concepts/permissions-reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="9d606-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="9d606-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="9d606-111">Permission type</span></span>|<span data-ttu-id="9d606-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="9d606-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9d606-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="9d606-113">Delegated (work or school account)</span></span>|<span data-ttu-id="9d606-114">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="9d606-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="9d606-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="9d606-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9d606-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="9d606-116">Not supported.</span></span>|
|<span data-ttu-id="9d606-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="9d606-117">Application</span></span>|<span data-ttu-id="9d606-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="9d606-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="9d606-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="9d606-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/userStatuses/{deviceConfigurationUserStatusId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/rootCertificate/userStatuses/{deviceConfigurationUserStatusId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/identityCertificate/userStatuses/{deviceConfigurationUserStatusId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/identityCertificate/rootCertificate/userStatuses/{deviceConfigurationUserStatusId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.iosScepCertificateProfile/rootCertificate/userStatuses/{deviceConfigurationUserStatusId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.macOSScepCertificateProfile/rootCertificate/userStatuses/{deviceConfigurationUserStatusId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsPhone81VpnConfiguration/identityCertificate/userStatuses/{deviceConfigurationUserStatusId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/identityCertificateForClientAuthentication/userStatuses/{deviceConfigurationUserStatusId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/rootCertificatesForServerValidation/{windows81TrustedRootCertificateId}/userStatuses/{deviceConfigurationUserStatusId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="9d606-120">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="9d606-120">Optional query parameters</span></span>
<span data-ttu-id="9d606-121">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://docs.microsoft.com/en-us/graph/query-parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="9d606-121">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="9d606-122">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="9d606-122">Request headers</span></span>
|<span data-ttu-id="9d606-123">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="9d606-123">Header</span></span>|<span data-ttu-id="9d606-124">値</span><span class="sxs-lookup"><span data-stu-id="9d606-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9d606-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="9d606-125">Authorization</span></span>|<span data-ttu-id="9d606-126">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="9d606-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9d606-127">Accept</span><span class="sxs-lookup"><span data-stu-id="9d606-127">Accept</span></span>|<span data-ttu-id="9d606-128">application/json</span><span class="sxs-lookup"><span data-stu-id="9d606-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9d606-129">要求本文</span><span class="sxs-lookup"><span data-stu-id="9d606-129">Request body</span></span>
<span data-ttu-id="9d606-130">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="9d606-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9d606-131">応答</span><span class="sxs-lookup"><span data-stu-id="9d606-131">Response</span></span>
<span data-ttu-id="9d606-132">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="9d606-132">If successful, this method returns a `200 OK` response code and [deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9d606-133">例</span><span class="sxs-lookup"><span data-stu-id="9d606-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="9d606-134">要求</span><span class="sxs-lookup"><span data-stu-id="9d606-134">Request</span></span>
<span data-ttu-id="9d606-135">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="9d606-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/userStatuses/{deviceConfigurationUserStatusId}
```

### <a name="response"></a><span data-ttu-id="9d606-136">応答</span><span class="sxs-lookup"><span data-stu-id="9d606-136">Response</span></span>
<span data-ttu-id="9d606-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="9d606-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 372

{
  "value": {
    "@odata.type": "#microsoft.graph.deviceConfigurationUserStatus",
    "id": "7e323db2-3db2-7e32-b23d-327eb23d327e",
    "userDisplayName": "User Display Name value",
    "devicesCount": 12,
    "status": "notApplicable",
    "lastReportedDateTime": "2017-01-01T00:00:17.7769392-08:00",
    "userPrincipalName": "User Principal Name value"
  }
}
```




