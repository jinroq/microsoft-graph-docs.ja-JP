---
title: IosVpnConfiguration を取得します。
description: IosVpnConfiguration オブジェクトのプロパティと関係を参照してください。
author: tfitzmac
ms.openlocfilehash: 46f8f47054186c2208e29f95f78ce6926ab62fe9
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27302325"
---
# <a name="get-iosvpnconfiguration"></a><span data-ttu-id="c3638-103">IosVpnConfiguration を取得します。</span><span class="sxs-lookup"><span data-stu-id="c3638-103">Get iosVpnConfiguration</span></span>

> <span data-ttu-id="c3638-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="c3638-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c3638-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c3638-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="c3638-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="c3638-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="c3638-107">[IosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md)オブジェクトのプロパティと関係を参照してください。</span><span class="sxs-lookup"><span data-stu-id="c3638-107">Read properties and relationships of the [iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="c3638-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="c3638-108">Prerequisites</span></span>
<span data-ttu-id="c3638-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="c3638-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c3638-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="c3638-111">Permission type</span></span>|<span data-ttu-id="c3638-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="c3638-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c3638-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="c3638-113">Delegated (work or school account)</span></span>|<span data-ttu-id="c3638-114">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="c3638-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="c3638-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="c3638-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c3638-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c3638-116">Not supported.</span></span>|
|<span data-ttu-id="c3638-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="c3638-117">Application</span></span>|<span data-ttu-id="c3638-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c3638-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c3638-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="c3638-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="c3638-120">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="c3638-120">Optional query parameters</span></span>
<span data-ttu-id="c3638-121">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="c3638-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="c3638-122">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="c3638-122">Request headers</span></span>
|<span data-ttu-id="c3638-123">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="c3638-123">Header</span></span>|<span data-ttu-id="c3638-124">値</span><span class="sxs-lookup"><span data-stu-id="c3638-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c3638-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="c3638-125">Authorization</span></span>|<span data-ttu-id="c3638-126">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="c3638-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c3638-127">Accept</span><span class="sxs-lookup"><span data-stu-id="c3638-127">Accept</span></span>|<span data-ttu-id="c3638-128">application/json</span><span class="sxs-lookup"><span data-stu-id="c3638-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c3638-129">要求本文</span><span class="sxs-lookup"><span data-stu-id="c3638-129">Request body</span></span>
<span data-ttu-id="c3638-130">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="c3638-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c3638-131">応答</span><span class="sxs-lookup"><span data-stu-id="c3638-131">Response</span></span>
<span data-ttu-id="c3638-132">かどうかは成功すると、このメソッドが返されます、 `200 OK` 、応答の本体で応答コードと[iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md)のオブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="c3638-132">If successful, this method returns a `200 OK` response code and [iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c3638-133">例</span><span class="sxs-lookup"><span data-stu-id="c3638-133">Example</span></span>
### <a name="request"></a><span data-ttu-id="c3638-134">要求</span><span class="sxs-lookup"><span data-stu-id="c3638-134">Request</span></span>
<span data-ttu-id="c3638-135">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="c3638-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

### <a name="response"></a><span data-ttu-id="c3638-136">応答</span><span class="sxs-lookup"><span data-stu-id="c3638-136">Response</span></span>
<span data-ttu-id="c3638-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="c3638-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2383

{
  "value": {
    "@odata.type": "#microsoft.graph.iosVpnConfiguration",
    "id": "bd12424c-424c-bd12-4c42-12bd4c4212bd",
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
}
```




