---
title: IosEnterpriseWiFiConfiguration を取得する
description: IosEnterpriseWiFiConfiguration オブジェクトのプロパティとリレーションシップを読み取ります。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 080dc205b28b512281bfebb88f3c6b76b409d5b0
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/11/2019
ms.locfileid: "33923511"
---
# <a name="get-iosenterprisewificonfiguration"></a><span data-ttu-id="8f956-103">IosEnterpriseWiFiConfiguration を取得する</span><span class="sxs-lookup"><span data-stu-id="8f956-103">Get iosEnterpriseWiFiConfiguration</span></span>

> <span data-ttu-id="8f956-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="8f956-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8f956-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="8f956-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8f956-106">[IosEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-iosenterprisewificonfiguration.md)オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="8f956-106">Read properties and relationships of the [iosEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-iosenterprisewificonfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="8f956-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="8f956-107">Prerequisites</span></span>
<span data-ttu-id="8f956-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="8f956-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8f956-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="8f956-110">Permission type</span></span>|<span data-ttu-id="8f956-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="8f956-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8f956-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="8f956-112">Delegated (work or school account)</span></span>|<span data-ttu-id="8f956-113">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="8f956-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="8f956-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="8f956-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8f956-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="8f956-115">Not supported.</span></span>|
|<span data-ttu-id="8f956-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="8f956-116">Application</span></span>|<span data-ttu-id="8f956-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="8f956-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="8f956-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="8f956-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="8f956-119">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="8f956-119">Optional query parameters</span></span>
<span data-ttu-id="8f956-120">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://docs.microsoft.com/en-us/graph/query-parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="8f956-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="8f956-121">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="8f956-121">Request headers</span></span>
|<span data-ttu-id="8f956-122">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="8f956-122">Header</span></span>|<span data-ttu-id="8f956-123">値</span><span class="sxs-lookup"><span data-stu-id="8f956-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8f956-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="8f956-124">Authorization</span></span>|<span data-ttu-id="8f956-125">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="8f956-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8f956-126">承諾</span><span class="sxs-lookup"><span data-stu-id="8f956-126">Accept</span></span>|<span data-ttu-id="8f956-127">application/json</span><span class="sxs-lookup"><span data-stu-id="8f956-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8f956-128">要求本文</span><span class="sxs-lookup"><span data-stu-id="8f956-128">Request body</span></span>
<span data-ttu-id="8f956-129">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="8f956-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8f956-130">応答</span><span class="sxs-lookup"><span data-stu-id="8f956-130">Response</span></span>
<span data-ttu-id="8f956-131">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で[iosEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-iosenterprisewificonfiguration.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="8f956-131">If successful, this method returns a `200 OK` response code and [iosEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-iosenterprisewificonfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8f956-132">例</span><span class="sxs-lookup"><span data-stu-id="8f956-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="8f956-133">要求</span><span class="sxs-lookup"><span data-stu-id="8f956-133">Request</span></span>
<span data-ttu-id="8f956-134">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="8f956-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

### <a name="response"></a><span data-ttu-id="8f956-135">応答</span><span class="sxs-lookup"><span data-stu-id="8f956-135">Response</span></span>
<span data-ttu-id="8f956-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="8f956-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1454

{
  "value": {
    "@odata.type": "#microsoft.graph.iosEnterpriseWiFiConfiguration",
    "id": "7593f7ba-f7ba-7593-baf7-9375baf79375",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
    "roleScopeTagIds": [
      "Role Scope Tag Ids value"
    ],
    "supportsScopeTags": true,
    "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
    "description": "Description value",
    "displayName": "Display Name value",
    "version": 7,
    "networkName": "Network Name value",
    "ssid": "Ssid value",
    "connectAutomatically": true,
    "connectWhenNetworkNameIsHidden": true,
    "wiFiSecurityType": "wpaPersonal",
    "proxySettings": "manual",
    "proxyManualAddress": "Proxy Manual Address value",
    "proxyManualPort": 15,
    "proxyAutomaticConfigurationUrl": "https://example.com/proxyAutomaticConfigurationUrl/",
    "preSharedKey": "Pre Shared Key value",
    "eapType": "leap",
    "eapFastConfiguration": "useProtectedAccessCredential",
    "trustedServerCertificateNames": [
      "Trusted Server Certificate Names value"
    ],
    "authenticationMethod": "usernameAndPassword",
    "innerAuthenticationProtocolForEapTtls": "challengeHandshakeAuthenticationProtocol",
    "outerIdentityPrivacyTemporaryValue": "Outer Identity Privacy Temporary Value value",
    "usernameFormatString": "Username Format String value",
    "passwordFormatString": "Password Format String value"
  }
}
```




