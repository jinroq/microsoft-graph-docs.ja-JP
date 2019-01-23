---
title: deviceConfigurationUserStatuses のリスト
description: deviceConfigurationUserStatus オブジェクトのプロパティとリレーションシップをリストします。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 70af6972f358ab34d5ce3dff825be7da19923984
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29420529"
---
# <a name="list-deviceconfigurationuserstatuses"></a><span data-ttu-id="c9a56-103">deviceConfigurationUserStatuses のリスト</span><span class="sxs-lookup"><span data-stu-id="c9a56-103">List deviceConfigurationUserStatuses</span></span>

> <span data-ttu-id="c9a56-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="c9a56-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="c9a56-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c9a56-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="c9a56-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="c9a56-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c9a56-107">[deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="c9a56-107">List properties and relationships of the [deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c9a56-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="c9a56-108">Prerequisites</span></span>
<span data-ttu-id="c9a56-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/concepts/permissions-reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="c9a56-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="c9a56-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="c9a56-111">Permission type</span></span>|<span data-ttu-id="c9a56-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="c9a56-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c9a56-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="c9a56-113">Delegated (work or school account)</span></span>|<span data-ttu-id="c9a56-114">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="c9a56-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="c9a56-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="c9a56-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c9a56-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c9a56-116">Not supported.</span></span>|
|<span data-ttu-id="c9a56-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="c9a56-117">Application</span></span>|<span data-ttu-id="c9a56-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c9a56-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c9a56-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="c9a56-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/userStatuses
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/rootCertificate/userStatuses
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/identityCertificate/userStatuses
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/identityCertificate/rootCertificate/userStatuses
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.iosScepCertificateProfile/rootCertificate/userStatuses
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.macOSScepCertificateProfile/rootCertificate/userStatuses
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsPhone81VpnConfiguration/identityCertificate/userStatuses
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/identityCertificateForClientAuthentication/userStatuses
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/rootCertificatesForServerValidation/{windows81TrustedRootCertificateId}/userStatuses
```

## <a name="request-headers"></a><span data-ttu-id="c9a56-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="c9a56-120">Request headers</span></span>
|<span data-ttu-id="c9a56-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="c9a56-121">Header</span></span>|<span data-ttu-id="c9a56-122">値</span><span class="sxs-lookup"><span data-stu-id="c9a56-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c9a56-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="c9a56-123">Authorization</span></span>|<span data-ttu-id="c9a56-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="c9a56-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c9a56-125">Accept</span><span class="sxs-lookup"><span data-stu-id="c9a56-125">Accept</span></span>|<span data-ttu-id="c9a56-126">application/json</span><span class="sxs-lookup"><span data-stu-id="c9a56-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c9a56-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="c9a56-127">Request body</span></span>
<span data-ttu-id="c9a56-128">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="c9a56-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c9a56-129">応答</span><span class="sxs-lookup"><span data-stu-id="c9a56-129">Response</span></span>
<span data-ttu-id="c9a56-130">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md) オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="c9a56-130">If successful, this method returns a `200 OK` response code and a collection of [deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c9a56-131">例</span><span class="sxs-lookup"><span data-stu-id="c9a56-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="c9a56-132">要求</span><span class="sxs-lookup"><span data-stu-id="c9a56-132">Request</span></span>
<span data-ttu-id="c9a56-133">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="c9a56-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/userStatuses
```

### <a name="response"></a><span data-ttu-id="c9a56-134">応答</span><span class="sxs-lookup"><span data-stu-id="c9a56-134">Response</span></span>
<span data-ttu-id="c9a56-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="c9a56-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 400

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.deviceConfigurationUserStatus",
      "id": "7e323db2-3db2-7e32-b23d-327eb23d327e",
      "userDisplayName": "User Display Name value",
      "devicesCount": 12,
      "status": "notApplicable",
      "lastReportedDateTime": "2017-01-01T00:00:17.7769392-08:00",
      "userPrincipalName": "User Principal Name value"
    }
  ]
}
```




