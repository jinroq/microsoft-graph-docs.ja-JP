---
title: Get windows10EnterpriseModernAppManagementConfiguration
description: windows10EnterpriseModernAppManagementConfiguration オブジェクトのプロパティとリレーションシップを読み取ります。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 8f9661101616bd26478de0fec5c76178d84c1318
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27930020"
---
# <a name="get-windows10enterprisemodernappmanagementconfiguration"></a><span data-ttu-id="c8bd9-103">Get windows10EnterpriseModernAppManagementConfiguration</span><span class="sxs-lookup"><span data-stu-id="c8bd9-103">Get windows10EnterpriseModernAppManagementConfiguration</span></span>

> <span data-ttu-id="c8bd9-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="c8bd9-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="c8bd9-105">[windows10EnterpriseModernAppManagementConfiguration](../resources/intune-deviceconfig-windows10enterprisemodernappmanagementconfiguration.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="c8bd9-105">Read properties and relationships of the [windows10EnterpriseModernAppManagementConfiguration](../resources/intune-deviceconfig-windows10enterprisemodernappmanagementconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="c8bd9-106">前提条件</span><span class="sxs-lookup"><span data-stu-id="c8bd9-106">Prerequisites</span></span>
<span data-ttu-id="c8bd9-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="c8bd9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c8bd9-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="c8bd9-109">Permission type</span></span>|<span data-ttu-id="c8bd9-110">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="c8bd9-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c8bd9-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="c8bd9-111">Delegated (work or school account)</span></span>|<span data-ttu-id="c8bd9-112">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="c8bd9-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="c8bd9-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="c8bd9-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c8bd9-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c8bd9-114">Not supported.</span></span>|
|<span data-ttu-id="c8bd9-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="c8bd9-115">Application</span></span>|<span data-ttu-id="c8bd9-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c8bd9-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c8bd9-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="c8bd9-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="c8bd9-118">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="c8bd9-118">Optional query parameters</span></span>
<span data-ttu-id="c8bd9-119">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="c8bd9-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="c8bd9-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="c8bd9-120">Request headers</span></span>
|<span data-ttu-id="c8bd9-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="c8bd9-121">Header</span></span>|<span data-ttu-id="c8bd9-122">値</span><span class="sxs-lookup"><span data-stu-id="c8bd9-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c8bd9-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="c8bd9-123">Authorization</span></span>|<span data-ttu-id="c8bd9-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="c8bd9-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c8bd9-125">Accept</span><span class="sxs-lookup"><span data-stu-id="c8bd9-125">Accept</span></span>|<span data-ttu-id="c8bd9-126">application/json</span><span class="sxs-lookup"><span data-stu-id="c8bd9-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c8bd9-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="c8bd9-127">Request body</span></span>
<span data-ttu-id="c8bd9-128">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="c8bd9-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c8bd9-129">応答</span><span class="sxs-lookup"><span data-stu-id="c8bd9-129">Response</span></span>
<span data-ttu-id="c8bd9-130">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [windows10EnterpriseModernAppManagementConfiguration](../resources/intune-deviceconfig-windows10enterprisemodernappmanagementconfiguration.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="c8bd9-130">If successful, this method returns a `200 OK` response code and [windows10EnterpriseModernAppManagementConfiguration](../resources/intune-deviceconfig-windows10enterprisemodernappmanagementconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c8bd9-131">例</span><span class="sxs-lookup"><span data-stu-id="c8bd9-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="c8bd9-132">要求</span><span class="sxs-lookup"><span data-stu-id="c8bd9-132">Request</span></span>
<span data-ttu-id="c8bd9-133">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="c8bd9-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

### <a name="response"></a><span data-ttu-id="c8bd9-134">応答</span><span class="sxs-lookup"><span data-stu-id="c8bd9-134">Response</span></span>
<span data-ttu-id="c8bd9-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="c8bd9-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 429

{
  "value": {
    "@odata.type": "#microsoft.graph.windows10EnterpriseModernAppManagementConfiguration",
    "id": "d6577687-7687-d657-8776-57d6877657d6",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
    "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
    "description": "Description value",
    "displayName": "Display Name value",
    "version": 7,
    "uninstallBuiltInApps": true
  }
}
```



