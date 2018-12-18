---
title: deviceConfigurationUserStatuses のリスト
description: deviceConfigurationUserStatus オブジェクトのプロパティとリレーションシップをリストします。
author: tfitzmac
ms.openlocfilehash: 3f8c1910cfc06a40b477f8a4010caaf167b060a3
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27340230"
---
# <a name="list-deviceconfigurationuserstatuses"></a><span data-ttu-id="28134-103">deviceConfigurationUserStatuses のリスト</span><span class="sxs-lookup"><span data-stu-id="28134-103">List deviceConfigurationUserStatuses</span></span>

> <span data-ttu-id="28134-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="28134-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="28134-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="28134-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="28134-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="28134-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="28134-107">[deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="28134-107">List properties and relationships of the [deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="28134-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="28134-108">Prerequisites</span></span>
<span data-ttu-id="28134-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="28134-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="28134-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="28134-111">Permission type</span></span>|<span data-ttu-id="28134-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="28134-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="28134-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="28134-113">Delegated (work or school account)</span></span>|<span data-ttu-id="28134-114">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="28134-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="28134-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="28134-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="28134-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="28134-116">Not supported.</span></span>|
|<span data-ttu-id="28134-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="28134-117">Application</span></span>|<span data-ttu-id="28134-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="28134-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="28134-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="28134-119">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="28134-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="28134-120">Request headers</span></span>
|<span data-ttu-id="28134-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="28134-121">Header</span></span>|<span data-ttu-id="28134-122">値</span><span class="sxs-lookup"><span data-stu-id="28134-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="28134-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="28134-123">Authorization</span></span>|<span data-ttu-id="28134-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="28134-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="28134-125">Accept</span><span class="sxs-lookup"><span data-stu-id="28134-125">Accept</span></span>|<span data-ttu-id="28134-126">application/json</span><span class="sxs-lookup"><span data-stu-id="28134-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="28134-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="28134-127">Request body</span></span>
<span data-ttu-id="28134-128">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="28134-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="28134-129">応答</span><span class="sxs-lookup"><span data-stu-id="28134-129">Response</span></span>
<span data-ttu-id="28134-130">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md) オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="28134-130">If successful, this method returns a `200 OK` response code and a collection of [deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="28134-131">例</span><span class="sxs-lookup"><span data-stu-id="28134-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="28134-132">要求</span><span class="sxs-lookup"><span data-stu-id="28134-132">Request</span></span>
<span data-ttu-id="28134-133">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="28134-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/userStatuses
```

### <a name="response"></a><span data-ttu-id="28134-134">応答</span><span class="sxs-lookup"><span data-stu-id="28134-134">Response</span></span>
<span data-ttu-id="28134-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="28134-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





