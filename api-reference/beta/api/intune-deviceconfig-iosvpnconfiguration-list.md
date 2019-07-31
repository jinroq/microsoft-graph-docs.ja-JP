---
title: IosVpnConfigurations を一覧表示する
description: IosVpnConfiguration オブジェクトのプロパティとリレーションシップをリストします。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 778d1f20c9a8c03e64bb0afa6c9aac230d9d0cde
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35947740"
---
# <a name="list-iosvpnconfigurations"></a><span data-ttu-id="e0035-103">IosVpnConfigurations を一覧表示する</span><span class="sxs-lookup"><span data-stu-id="e0035-103">List iosVpnConfigurations</span></span>

> <span data-ttu-id="e0035-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e0035-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e0035-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="e0035-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e0035-106">[Iosvpnconfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md)オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="e0035-106">List properties and relationships of the [iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e0035-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="e0035-107">Prerequisites</span></span>
<span data-ttu-id="e0035-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="e0035-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e0035-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="e0035-110">Permission type</span></span>|<span data-ttu-id="e0035-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="e0035-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e0035-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="e0035-112">Delegated (work or school account)</span></span>|<span data-ttu-id="e0035-113">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="e0035-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="e0035-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="e0035-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e0035-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e0035-115">Not supported.</span></span>|
|<span data-ttu-id="e0035-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="e0035-116">Application</span></span>|<span data-ttu-id="e0035-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e0035-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e0035-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="e0035-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="e0035-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="e0035-119">Request headers</span></span>
|<span data-ttu-id="e0035-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="e0035-120">Header</span></span>|<span data-ttu-id="e0035-121">値</span><span class="sxs-lookup"><span data-stu-id="e0035-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e0035-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="e0035-122">Authorization</span></span>|<span data-ttu-id="e0035-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="e0035-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e0035-124">承諾</span><span class="sxs-lookup"><span data-stu-id="e0035-124">Accept</span></span>|<span data-ttu-id="e0035-125">application/json</span><span class="sxs-lookup"><span data-stu-id="e0035-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e0035-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="e0035-126">Request body</span></span>
<span data-ttu-id="e0035-127">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="e0035-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e0035-128">応答</span><span class="sxs-lookup"><span data-stu-id="e0035-128">Response</span></span>
<span data-ttu-id="e0035-129">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で[Iosvpnconfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md)オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="e0035-129">If successful, this method returns a `200 OK` response code and a collection of [iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e0035-130">例</span><span class="sxs-lookup"><span data-stu-id="e0035-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="e0035-131">要求</span><span class="sxs-lookup"><span data-stu-id="e0035-131">Request</span></span>
<span data-ttu-id="e0035-132">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="e0035-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
```

### <a name="response"></a><span data-ttu-id="e0035-133">応答</span><span class="sxs-lookup"><span data-stu-id="e0035-133">Response</span></span>
<span data-ttu-id="e0035-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="e0035-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 3404

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.iosVpnConfiguration",
      "id": "bd12424c-424c-bd12-4c42-12bd4c4212bd",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "roleScopeTagIds": [
        "Role Scope Tag Ids value"
      ],
      "supportsScopeTags": true,
      "deviceManagementApplicabilityRuleOsEdition": {
        "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleOsEdition",
        "osEditionTypes": [
          "windows10EnterpriseN"
        ],
        "name": "Name value",
        "ruleType": "exclude"
      },
      "deviceManagementApplicabilityRuleOsVersion": {
        "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleOsVersion",
        "minOSVersion": "Min OSVersion value",
        "maxOSVersion": "Max OSVersion value",
        "name": "Name value",
        "ruleType": "exclude"
      },
      "deviceManagementApplicabilityRuleDeviceMode": {
        "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleDeviceMode",
        "deviceMode": "sModeConfiguration",
        "name": "Name value",
        "ruleType": "exclude"
      },
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "description": "Description value",
      "displayName": "Display Name value",
      "version": 7,
      "connectionName": "Connection Name value",
      "connectionType": "pulseSecure",
      "loginGroupOrDomain": "Login Group Or Domain value",
      "role": "Role value",
      "realm": "Realm value",
      "server": {
        "@odata.type": "microsoft.graph.vpnServer",
        "description": "Description value",
        "address": "Address value",
        "isDefaultServer": true
      },
      "identifier": "Identifier value",
      "customData": [
        {
          "@odata.type": "microsoft.graph.keyValue",
          "key": "Key value",
          "value": "Value value"
        }
      ],
      "customKeyValueData": [
        {
          "@odata.type": "microsoft.graph.keyValuePair",
          "name": "Name value",
          "value": "Value value"
        }
      ],
      "enableSplitTunneling": true,
      "authenticationMethod": "usernameAndPassword",
      "enablePerApp": true,
      "safariDomains": [
        "Safari Domains value"
      ],
      "onDemandRules": [
        {
          "@odata.type": "microsoft.graph.vpnOnDemandRule",
          "ssids": [
            "Ssids value"
          ],
          "dnsSearchDomains": [
            "Dns Search Domains value"
          ],
          "probeUrl": "https://example.com/probeUrl/",
          "action": "evaluateConnection",
          "domainAction": "neverConnect",
          "domains": [
            "Domains value"
          ],
          "probeRequiredUrl": "https://example.com/probeRequiredUrl/"
        }
      ],
      "proxyServer": {
        "@odata.type": "microsoft.graph.vpnProxyServer",
        "automaticConfigurationScriptUrl": "https://example.com/automaticConfigurationScriptUrl/",
        "address": "Address value",
        "port": 4
      },
      "optInToDeviceIdSharing": true,
      "providerType": "appProxy",
      "userDomain": "User Domain value",
      "strictEnforcement": true,
      "cloudName": "Cloud Name value",
      "excludeList": [
        "Exclude List value"
      ]
    }
  ]
}
```





