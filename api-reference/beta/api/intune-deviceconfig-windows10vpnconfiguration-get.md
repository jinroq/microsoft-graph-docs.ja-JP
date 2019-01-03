---
title: Windows10VpnConfiguration を取得します。
description: Windows10VpnConfiguration オブジェクトのプロパティと関係を参照してください。
author: tfitzmac
ms.openlocfilehash: 140de467a4f10d097d84c59e0dae3bb1fb18721a
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27352942"
---
# <a name="get-windows10vpnconfiguration"></a><span data-ttu-id="9430d-103">Windows10VpnConfiguration を取得します。</span><span class="sxs-lookup"><span data-stu-id="9430d-103">Get windows10VpnConfiguration</span></span>

> <span data-ttu-id="9430d-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="9430d-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="9430d-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="9430d-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="9430d-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="9430d-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="9430d-107">[Windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md)オブジェクトのプロパティと関係を参照してください。</span><span class="sxs-lookup"><span data-stu-id="9430d-107">Read properties and relationships of the [windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="9430d-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="9430d-108">Prerequisites</span></span>
<span data-ttu-id="9430d-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="9430d-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9430d-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="9430d-111">Permission type</span></span>|<span data-ttu-id="9430d-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="9430d-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9430d-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="9430d-113">Delegated (work or school account)</span></span>|<span data-ttu-id="9430d-114">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="9430d-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="9430d-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="9430d-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9430d-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="9430d-116">Not supported.</span></span>|
|<span data-ttu-id="9430d-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="9430d-117">Application</span></span>|<span data-ttu-id="9430d-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="9430d-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="9430d-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="9430d-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="9430d-120">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="9430d-120">Optional query parameters</span></span>
<span data-ttu-id="9430d-121">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="9430d-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="9430d-122">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="9430d-122">Request headers</span></span>
|<span data-ttu-id="9430d-123">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="9430d-123">Header</span></span>|<span data-ttu-id="9430d-124">値</span><span class="sxs-lookup"><span data-stu-id="9430d-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9430d-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="9430d-125">Authorization</span></span>|<span data-ttu-id="9430d-126">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="9430d-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9430d-127">Accept</span><span class="sxs-lookup"><span data-stu-id="9430d-127">Accept</span></span>|<span data-ttu-id="9430d-128">application/json</span><span class="sxs-lookup"><span data-stu-id="9430d-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9430d-129">要求本文</span><span class="sxs-lookup"><span data-stu-id="9430d-129">Request body</span></span>
<span data-ttu-id="9430d-130">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="9430d-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9430d-131">応答</span><span class="sxs-lookup"><span data-stu-id="9430d-131">Response</span></span>
<span data-ttu-id="9430d-132">かどうかは成功すると、このメソッドが返されます、 `200 OK` 、応答の本体で応答コードと[windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md)のオブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="9430d-132">If successful, this method returns a `200 OK` response code and [windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9430d-133">例</span><span class="sxs-lookup"><span data-stu-id="9430d-133">Example</span></span>
### <a name="request"></a><span data-ttu-id="9430d-134">要求</span><span class="sxs-lookup"><span data-stu-id="9430d-134">Request</span></span>
<span data-ttu-id="9430d-135">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="9430d-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

### <a name="response"></a><span data-ttu-id="9430d-136">応答</span><span class="sxs-lookup"><span data-stu-id="9430d-136">Response</span></span>
<span data-ttu-id="9430d-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="9430d-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 3676

{
  "value": {
    "@odata.type": "#microsoft.graph.windows10VpnConfiguration",
    "id": "c23c9727-9727-c23c-2797-3cc227973cc2",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
    "roleScopeTagIds": [
      "Role Scope Tag Ids value"
    ],
    "supportsScopeTags": true,
    "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
    "description": "Description value",
    "displayName": "Display Name value",
    "version": 7,
    "connectionName": "Connection Name value",
    "servers": [
      {
        "@odata.type": "microsoft.graph.vpnServer",
        "description": "Description value",
        "address": "Address value",
        "isDefaultServer": true
      }
    ],
    "customXml": "Y3VzdG9tWG1s",
    "profileTarget": "device",
    "connectionType": "f5EdgeClient",
    "enableSplitTunneling": true,
    "enableAlwaysOn": true,
    "enableDeviceTunnel": true,
    "enableDnsRegistration": true,
    "dnsSuffixes": [
      "Dns Suffixes value"
    ],
    "authenticationMethod": "usernameAndPassword",
    "rememberUserCredentials": true,
    "enableConditionalAccess": true,
    "enableSingleSignOnWithAlternateCertificate": true,
    "singleSignOnEku": {
      "@odata.type": "microsoft.graph.extendedKeyUsage",
      "name": "Name value",
      "objectIdentifier": "Object Identifier value"
    },
    "singleSignOnIssuerHash": "Single Sign On Issuer Hash value",
    "eapXml": "ZWFwWG1s",
    "proxyServer": {
      "@odata.type": "microsoft.graph.windows10VpnProxyServer",
      "automaticConfigurationScriptUrl": "https://example.com/automaticConfigurationScriptUrl/",
      "address": "Address value",
      "port": 4,
      "bypassProxyServerForLocalAddress": true
    },
    "associatedApps": [
      {
        "@odata.type": "microsoft.graph.windows10AssociatedApps",
        "appType": "universal",
        "identifier": "Identifier value"
      }
    ],
    "onlyAssociatedAppsCanUseConnection": true,
    "windowsInformationProtectionDomain": "Windows Information Protection Domain value",
    "trafficRules": [
      {
        "@odata.type": "microsoft.graph.vpnTrafficRule",
        "name": "Name value",
        "protocols": 9,
        "localPortRanges": [
          {
            "@odata.type": "microsoft.graph.numberRange",
            "lowerNumber": 11,
            "upperNumber": 11
          }
        ],
        "remotePortRanges": [
          {
            "@odata.type": "microsoft.graph.numberRange",
            "lowerNumber": 11,
            "upperNumber": 11
          }
        ],
        "localAddressRanges": [
          {
            "@odata.type": "microsoft.graph.iPv4Range",
            "lowerAddress": "Lower Address value",
            "upperAddress": "Upper Address value"
          }
        ],
        "remoteAddressRanges": [
          {
            "@odata.type": "microsoft.graph.iPv4Range",
            "lowerAddress": "Lower Address value",
            "upperAddress": "Upper Address value"
          }
        ],
        "appId": "App Id value",
        "appType": "desktop",
        "routingPolicyType": "splitTunnel",
        "claims": "Claims value"
      }
    ],
    "routes": [
      {
        "@odata.type": "microsoft.graph.vpnRoute",
        "destinationPrefix": "Destination Prefix value",
        "prefixSize": 10
      }
    ],
    "dnsRules": [
      {
        "@odata.type": "microsoft.graph.vpnDnsRule",
        "name": "Name value",
        "servers": [
          "Servers value"
        ],
        "proxyServerUri": "Proxy Server Uri value"
      }
    ]
  }
}
```




