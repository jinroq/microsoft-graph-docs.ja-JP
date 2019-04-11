---
title: Get deviceConfigurationAssignment
description: deviceConfigurationAssignment オブジェクトのプロパティとリレーションシップを読み取ります。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: d4107636965dd2e433423f1b6f4c8e1ebec3a2e6
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/11/2019
ms.locfileid: "31784615"
---
# <a name="get-deviceconfigurationassignment"></a><span data-ttu-id="7db0b-103">Get deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="7db0b-103">Get deviceConfigurationAssignment</span></span>

> <span data-ttu-id="7db0b-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="7db0b-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7db0b-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="7db0b-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7db0b-106">[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="7db0b-106">Read properties and relationships of the [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="7db0b-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="7db0b-107">Prerequisites</span></span>
<span data-ttu-id="7db0b-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="7db0b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7db0b-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="7db0b-110">Permission type</span></span>|<span data-ttu-id="7db0b-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="7db0b-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7db0b-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="7db0b-112">Delegated (work or school account)</span></span>|<span data-ttu-id="7db0b-113">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="7db0b-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="7db0b-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="7db0b-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7db0b-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="7db0b-115">Not supported.</span></span>|
|<span data-ttu-id="7db0b-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="7db0b-116">Application</span></span>|<span data-ttu-id="7db0b-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="7db0b-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="7db0b-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="7db0b-118">HTTP Request</span></span>
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

## <a name="optional-query-parameters"></a><span data-ttu-id="7db0b-119">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="7db0b-119">Optional query parameters</span></span>
<span data-ttu-id="7db0b-120">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://docs.microsoft.com/en-us/graph/query-parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="7db0b-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="7db0b-121">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="7db0b-121">Request headers</span></span>
|<span data-ttu-id="7db0b-122">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="7db0b-122">Header</span></span>|<span data-ttu-id="7db0b-123">値</span><span class="sxs-lookup"><span data-stu-id="7db0b-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7db0b-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="7db0b-124">Authorization</span></span>|<span data-ttu-id="7db0b-125">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="7db0b-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7db0b-126">承諾</span><span class="sxs-lookup"><span data-stu-id="7db0b-126">Accept</span></span>|<span data-ttu-id="7db0b-127">application/json</span><span class="sxs-lookup"><span data-stu-id="7db0b-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7db0b-128">要求本文</span><span class="sxs-lookup"><span data-stu-id="7db0b-128">Request body</span></span>
<span data-ttu-id="7db0b-129">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="7db0b-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7db0b-130">応答</span><span class="sxs-lookup"><span data-stu-id="7db0b-130">Response</span></span>
<span data-ttu-id="7db0b-131">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="7db0b-131">If successful, this method returns a `200 OK` response code and [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7db0b-132">例</span><span class="sxs-lookup"><span data-stu-id="7db0b-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="7db0b-133">要求</span><span class="sxs-lookup"><span data-stu-id="7db0b-133">Request</span></span>
<span data-ttu-id="7db0b-134">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="7db0b-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/assignments/{deviceConfigurationAssignmentId}
```

### <a name="response"></a><span data-ttu-id="7db0b-135">応答</span><span class="sxs-lookup"><span data-stu-id="7db0b-135">Response</span></span>
<span data-ttu-id="7db0b-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="7db0b-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





