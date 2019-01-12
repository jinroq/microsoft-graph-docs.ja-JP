---
title: Get deviceConfigurationAssignment
description: deviceConfigurationAssignment オブジェクトのプロパティとリレーションシップを読み取ります。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: e8739dee9de548179dc88b68b3bf842ddc11241c
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27930118"
---
# <a name="get-deviceconfigurationassignment"></a><span data-ttu-id="30466-103">Get deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="30466-103">Get deviceConfigurationAssignment</span></span>

> <span data-ttu-id="30466-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="30466-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="30466-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="30466-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="30466-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="30466-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="30466-107">[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="30466-107">Read properties and relationships of the [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="30466-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="30466-108">Prerequisites</span></span>
<span data-ttu-id="30466-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="30466-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="30466-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="30466-111">Permission type</span></span>|<span data-ttu-id="30466-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="30466-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="30466-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="30466-113">Delegated (work or school account)</span></span>|<span data-ttu-id="30466-114">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="30466-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="30466-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="30466-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="30466-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="30466-116">Not supported.</span></span>|
|<span data-ttu-id="30466-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="30466-117">Application</span></span>|<span data-ttu-id="30466-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="30466-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="30466-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="30466-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/assignments/{deviceConfigurationAssignmentId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/rootCertificate/assignments/{deviceConfigurationAssignmentId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/identityCertificate/assignments/{deviceConfigurationAssignmentId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/identityCertificate/rootCertificate/assignments/{deviceConfigurationAssignmentId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.iosScepCertificateProfile/rootCertificate/assignments/{deviceConfigurationAssignmentId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.macOSScepCertificateProfile/rootCertificate/assignments/{deviceConfigurationAssignmentId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsPhone81VpnConfiguration/identityCertificate/assignments/{deviceConfigurationAssignmentId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/identityCertificateForClientAuthentication/assignments/{deviceConfigurationAssignmentId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/rootCertificatesForServerValidation/{windows81TrustedRootCertificateId}/assignments/{deviceConfigurationAssignmentId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="30466-120">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="30466-120">Optional query parameters</span></span>
<span data-ttu-id="30466-121">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="30466-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="30466-122">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="30466-122">Request headers</span></span>
|<span data-ttu-id="30466-123">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="30466-123">Header</span></span>|<span data-ttu-id="30466-124">値</span><span class="sxs-lookup"><span data-stu-id="30466-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="30466-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="30466-125">Authorization</span></span>|<span data-ttu-id="30466-126">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="30466-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="30466-127">Accept</span><span class="sxs-lookup"><span data-stu-id="30466-127">Accept</span></span>|<span data-ttu-id="30466-128">application/json</span><span class="sxs-lookup"><span data-stu-id="30466-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="30466-129">要求本文</span><span class="sxs-lookup"><span data-stu-id="30466-129">Request body</span></span>
<span data-ttu-id="30466-130">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="30466-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="30466-131">応答</span><span class="sxs-lookup"><span data-stu-id="30466-131">Response</span></span>
<span data-ttu-id="30466-132">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="30466-132">If successful, this method returns a `200 OK` response code and [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="30466-133">例</span><span class="sxs-lookup"><span data-stu-id="30466-133">Example</span></span>
### <a name="request"></a><span data-ttu-id="30466-134">要求</span><span class="sxs-lookup"><span data-stu-id="30466-134">Request</span></span>
<span data-ttu-id="30466-135">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="30466-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/assignments/{deviceConfigurationAssignmentId}
```

### <a name="response"></a><span data-ttu-id="30466-136">応答</span><span class="sxs-lookup"><span data-stu-id="30466-136">Response</span></span>
<span data-ttu-id="30466-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="30466-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 247

{
  "value": {
    "@odata.type": "#microsoft.graph.deviceConfigurationAssignment",
    "id": "d59b6342-6342-d59b-4263-9bd542639bd5",
    "target": {
      "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
    }
  }
}
```





