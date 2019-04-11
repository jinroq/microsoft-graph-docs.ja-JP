---
title: リスト windows10VpnConfigurations
description: windows10VpnConfiguration オブジェクトのプロパティとリレーションシップをリストします。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 69d588ec5fa433492de0fcdcff1d55ad9fe1bed9
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/11/2019
ms.locfileid: "31778895"
---
# <a name="list-windows10vpnconfigurations"></a><span data-ttu-id="00245-103">リスト windows10VpnConfigurations</span><span class="sxs-lookup"><span data-stu-id="00245-103">List windows10VpnConfigurations</span></span>

> <span data-ttu-id="00245-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="00245-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="00245-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="00245-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="00245-106">[windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md)オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="00245-106">List properties and relationships of the [windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="00245-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="00245-107">Prerequisites</span></span>
<span data-ttu-id="00245-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="00245-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="00245-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="00245-110">Permission type</span></span>|<span data-ttu-id="00245-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="00245-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="00245-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="00245-112">Delegated (work or school account)</span></span>|<span data-ttu-id="00245-113">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="00245-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="00245-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="00245-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="00245-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="00245-115">Not supported.</span></span>|
|<span data-ttu-id="00245-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="00245-116">Application</span></span>|<span data-ttu-id="00245-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="00245-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="00245-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="00245-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="00245-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="00245-119">Request headers</span></span>
|<span data-ttu-id="00245-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="00245-120">Header</span></span>|<span data-ttu-id="00245-121">値</span><span class="sxs-lookup"><span data-stu-id="00245-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="00245-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="00245-122">Authorization</span></span>|<span data-ttu-id="00245-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="00245-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="00245-124">承諾</span><span class="sxs-lookup"><span data-stu-id="00245-124">Accept</span></span>|<span data-ttu-id="00245-125">application/json</span><span class="sxs-lookup"><span data-stu-id="00245-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="00245-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="00245-126">Request body</span></span>
<span data-ttu-id="00245-127">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="00245-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="00245-128">応答</span><span class="sxs-lookup"><span data-stu-id="00245-128">Response</span></span>
<span data-ttu-id="00245-129">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で[windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md)オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="00245-129">If successful, this method returns a `200 OK` response code and a collection of [windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="00245-130">例</span><span class="sxs-lookup"><span data-stu-id="00245-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="00245-131">要求</span><span class="sxs-lookup"><span data-stu-id="00245-131">Request</span></span>
<span data-ttu-id="00245-132">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="00245-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
```

### <a name="response"></a><span data-ttu-id="00245-133">応答</span><span class="sxs-lookup"><span data-stu-id="00245-133">Response</span></span>
<span data-ttu-id="00245-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="00245-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 4064

{
  "value": [
    {
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
          "proxyServerUri": "Proxy Server Uri value",
          "autoTrigger": true,
          "persistent": true
        }
      ],
      "trustedNetworkDomains": [
        "Trusted Network Domains value"
      ]
    }
  ]
}
```





