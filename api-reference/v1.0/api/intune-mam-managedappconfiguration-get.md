---
title: Get managedAppConfiguration
description: managedAppConfiguration オブジェクトのプロパティとリレーションシップを読み取ります。
ms.openlocfilehash: 77dcdc5785f3b04825ae8250abebdaa5dc16dd01
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27020805"
---
# <a name="get-managedappconfiguration"></a><span data-ttu-id="30fd1-103">Get managedAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="30fd1-103">Get managedAppConfiguration</span></span>

> <span data-ttu-id="30fd1-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="30fd1-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="30fd1-105">[managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="30fd1-105">Read properties and relationships of the [managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="30fd1-106">前提条件</span><span class="sxs-lookup"><span data-stu-id="30fd1-106">Prerequisites</span></span>
<span data-ttu-id="30fd1-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="30fd1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="30fd1-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="30fd1-109">Permission type</span></span>|<span data-ttu-id="30fd1-110">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="30fd1-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="30fd1-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="30fd1-111">Delegated (work or school account)</span></span>|<span data-ttu-id="30fd1-112">DeviceManagementApps.ReadWrite.All、DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="30fd1-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="30fd1-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="30fd1-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="30fd1-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="30fd1-114">Not supported.</span></span>|
|<span data-ttu-id="30fd1-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="30fd1-115">Application</span></span>|<span data-ttu-id="30fd1-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="30fd1-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="30fd1-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="30fd1-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/managedAppPolicies/{managedAppPolicyId}
GET /deviceAppManagement/managedAppRegistrations/{managedAppRegistrationId}/appliedPolicies/{managedAppPolicyId}
GET /deviceAppManagement/managedAppRegistrations/{managedAppRegistrationId}/intendedPolicies/{managedAppPolicyId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="30fd1-118">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="30fd1-118">Optional query parameters</span></span>
<span data-ttu-id="30fd1-119">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="30fd1-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="30fd1-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="30fd1-120">Request headers</span></span>
|<span data-ttu-id="30fd1-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="30fd1-121">Header</span></span>|<span data-ttu-id="30fd1-122">値</span><span class="sxs-lookup"><span data-stu-id="30fd1-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="30fd1-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="30fd1-123">Authorization</span></span>|<span data-ttu-id="30fd1-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="30fd1-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="30fd1-125">Accept</span><span class="sxs-lookup"><span data-stu-id="30fd1-125">Accept</span></span>|<span data-ttu-id="30fd1-126">application/json</span><span class="sxs-lookup"><span data-stu-id="30fd1-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="30fd1-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="30fd1-127">Request body</span></span>
<span data-ttu-id="30fd1-128">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="30fd1-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="30fd1-129">応答</span><span class="sxs-lookup"><span data-stu-id="30fd1-129">Response</span></span>
<span data-ttu-id="30fd1-130">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="30fd1-130">If successful, this method returns a `200 OK` response code and [managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="30fd1-131">例</span><span class="sxs-lookup"><span data-stu-id="30fd1-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="30fd1-132">要求</span><span class="sxs-lookup"><span data-stu-id="30fd1-132">Request</span></span>
<span data-ttu-id="30fd1-133">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="30fd1-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/managedAppPolicies/{managedAppPolicyId}
```

### <a name="response"></a><span data-ttu-id="30fd1-134">応答</span><span class="sxs-lookup"><span data-stu-id="30fd1-134">Response</span></span>
<span data-ttu-id="30fd1-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="30fd1-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 550

{
  "value": {
    "@odata.type": "#microsoft.graph.managedAppConfiguration",
    "displayName": "Display Name value",
    "description": "Description value",
    "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
    "id": "2ed27cb5-7cb5-2ed2-b57c-d22eb57cd22e",
    "version": "Version value",
    "customSettings": [
      {
        "@odata.type": "microsoft.graph.keyValuePair",
        "name": "Name value",
        "value": "Value value"
      }
    ]
  }
}
```



