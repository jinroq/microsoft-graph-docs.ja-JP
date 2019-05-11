---
title: WindowsWifiEnterpriseEAPConfiguration を取得する
description: WindowsWifiEnterpriseEAPConfiguration オブジェクトのプロパティとリレーションシップを読み取ります。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 8bc00a959488bc3f85bad6e53f11b3787349c02d
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/11/2019
ms.locfileid: "33917163"
---
# <a name="get-windowswifienterpriseeapconfiguration"></a><span data-ttu-id="84675-103">WindowsWifiEnterpriseEAPConfiguration を取得する</span><span class="sxs-lookup"><span data-stu-id="84675-103">Get windowsWifiEnterpriseEAPConfiguration</span></span>

> <span data-ttu-id="84675-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="84675-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="84675-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="84675-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="84675-106">[WindowsWifiEnterpriseEAPConfiguration](../resources/intune-deviceconfig-windowswifienterpriseeapconfiguration.md)オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="84675-106">Read properties and relationships of the [windowsWifiEnterpriseEAPConfiguration](../resources/intune-deviceconfig-windowswifienterpriseeapconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="84675-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="84675-107">Prerequisites</span></span>
<span data-ttu-id="84675-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="84675-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="84675-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="84675-110">Permission type</span></span>|<span data-ttu-id="84675-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="84675-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="84675-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="84675-112">Delegated (work or school account)</span></span>|<span data-ttu-id="84675-113">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="84675-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="84675-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="84675-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="84675-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="84675-115">Not supported.</span></span>|
|<span data-ttu-id="84675-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="84675-116">Application</span></span>|<span data-ttu-id="84675-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="84675-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="84675-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="84675-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="84675-119">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="84675-119">Optional query parameters</span></span>
<span data-ttu-id="84675-120">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://docs.microsoft.com/en-us/graph/query-parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="84675-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="84675-121">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="84675-121">Request headers</span></span>
|<span data-ttu-id="84675-122">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="84675-122">Header</span></span>|<span data-ttu-id="84675-123">値</span><span class="sxs-lookup"><span data-stu-id="84675-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="84675-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="84675-124">Authorization</span></span>|<span data-ttu-id="84675-125">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="84675-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="84675-126">承諾</span><span class="sxs-lookup"><span data-stu-id="84675-126">Accept</span></span>|<span data-ttu-id="84675-127">application/json</span><span class="sxs-lookup"><span data-stu-id="84675-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="84675-128">要求本文</span><span class="sxs-lookup"><span data-stu-id="84675-128">Request body</span></span>
<span data-ttu-id="84675-129">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="84675-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="84675-130">応答</span><span class="sxs-lookup"><span data-stu-id="84675-130">Response</span></span>
<span data-ttu-id="84675-131">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で[windowsWifiEnterpriseEAPConfiguration](../resources/intune-deviceconfig-windowswifienterpriseeapconfiguration.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="84675-131">If successful, this method returns a `200 OK` response code and [windowsWifiEnterpriseEAPConfiguration](../resources/intune-deviceconfig-windowswifienterpriseeapconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="84675-132">例</span><span class="sxs-lookup"><span data-stu-id="84675-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="84675-133">要求</span><span class="sxs-lookup"><span data-stu-id="84675-133">Request</span></span>
<span data-ttu-id="84675-134">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="84675-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

### <a name="response"></a><span data-ttu-id="84675-135">応答</span><span class="sxs-lookup"><span data-stu-id="84675-135">Response</span></span>
<span data-ttu-id="84675-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="84675-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1773

{
  "value": {
    "@odata.type": "#microsoft.graph.windowsWifiEnterpriseEAPConfiguration",
    "id": "7e7183ac-83ac-7e71-ac83-717eac83717e",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
    "roleScopeTagIds": [
      "Role Scope Tag Ids value"
    ],
    "supportsScopeTags": true,
    "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
    "description": "Description value",
    "displayName": "Display Name value",
    "version": 7,
    "preSharedKey": "Pre Shared Key value",
    "wifiSecurityType": "wpaPersonal",
    "meteredConnectionLimit": "fixed",
    "ssid": "Ssid value",
    "networkName": "Network Name value",
    "connectAutomatically": true,
    "connectToPreferredNetwork": true,
    "connectWhenNetworkNameIsHidden": true,
    "proxySetting": "manual",
    "proxyManualAddress": "Proxy Manual Address value",
    "proxyManualPort": 15,
    "proxyAutomaticConfigurationUrl": "https://example.com/proxyAutomaticConfigurationUrl/",
    "forceFIPSCompliance": true,
    "networkSingleSignOn": "prelogon",
    "maximumAuthenticationTimeoutInSeconds": 5,
    "promptForAdditionalAuthenticationCredentials": true,
    "enablePairwiseMasterKeyCaching": true,
    "maximumPairwiseMasterKeyCacheTimeInMinutes": 10,
    "maximumNumberOfPairwiseMasterKeysInCache": 8,
    "enablePreAuthentication": true,
    "maximumPreAuthenticationAttempts": 0,
    "eapType": "leap",
    "trustedServerCertificateNames": [
      "Trusted Server Certificate Names value"
    ],
    "authenticationMethod": "usernameAndPassword",
    "innerAuthenticationProtocolForEAPTTLS": "challengeHandshakeAuthenticationProtocol",
    "outerIdentityPrivacyTemporaryValue": "Outer Identity Privacy Temporary Value value"
  }
}
```




