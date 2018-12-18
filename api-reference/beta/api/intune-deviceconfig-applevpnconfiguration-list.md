---
title: リスト appleVpnConfigurations
description: AppleVpnConfiguration オブジェクトのプロパティと関係を一覧表示します。
author: tfitzmac
ms.openlocfilehash: d18baf41cd66309207850d155ee5e383808f6205
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27322284"
---
# <a name="list-applevpnconfigurations"></a><span data-ttu-id="f72e1-103">リスト appleVpnConfigurations</span><span class="sxs-lookup"><span data-stu-id="f72e1-103">List appleVpnConfigurations</span></span>

> <span data-ttu-id="f72e1-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="f72e1-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f72e1-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f72e1-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="f72e1-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="f72e1-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="f72e1-107">[AppleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)オブジェクトのプロパティと関係を一覧表示します。</span><span class="sxs-lookup"><span data-stu-id="f72e1-107">List properties and relationships of the [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="f72e1-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="f72e1-108">Prerequisites</span></span>
<span data-ttu-id="f72e1-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="f72e1-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f72e1-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="f72e1-111">Permission type</span></span>|<span data-ttu-id="f72e1-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="f72e1-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f72e1-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="f72e1-113">Delegated (work or school account)</span></span>|<span data-ttu-id="f72e1-114">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="f72e1-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="f72e1-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="f72e1-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f72e1-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f72e1-116">Not supported.</span></span>|
|<span data-ttu-id="f72e1-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="f72e1-117">Application</span></span>|<span data-ttu-id="f72e1-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f72e1-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f72e1-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="f72e1-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="f72e1-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="f72e1-120">Request headers</span></span>
|<span data-ttu-id="f72e1-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="f72e1-121">Header</span></span>|<span data-ttu-id="f72e1-122">値</span><span class="sxs-lookup"><span data-stu-id="f72e1-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f72e1-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="f72e1-123">Authorization</span></span>|<span data-ttu-id="f72e1-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="f72e1-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f72e1-125">Accept</span><span class="sxs-lookup"><span data-stu-id="f72e1-125">Accept</span></span>|<span data-ttu-id="f72e1-126">application/json</span><span class="sxs-lookup"><span data-stu-id="f72e1-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f72e1-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="f72e1-127">Request body</span></span>
<span data-ttu-id="f72e1-128">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="f72e1-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f72e1-129">応答</span><span class="sxs-lookup"><span data-stu-id="f72e1-129">Response</span></span>
<span data-ttu-id="f72e1-130">かどうかは成功すると、このメソッドが返されます、`200 OK`応答コードおよび応答の本文に[appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md)オブジェクトのコレクションです。</span><span class="sxs-lookup"><span data-stu-id="f72e1-130">If successful, this method returns a `200 OK` response code and a collection of [appleVpnConfiguration](../resources/intune-deviceconfig-applevpnconfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f72e1-131">例</span><span class="sxs-lookup"><span data-stu-id="f72e1-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="f72e1-132">要求</span><span class="sxs-lookup"><span data-stu-id="f72e1-132">Request</span></span>
<span data-ttu-id="f72e1-133">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="f72e1-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
```

### <a name="response"></a><span data-ttu-id="f72e1-134">応答</span><span class="sxs-lookup"><span data-stu-id="f72e1-134">Response</span></span>
<span data-ttu-id="f72e1-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="f72e1-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2334

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.appleVpnConfiguration",
      "id": "e31fbd39-bd39-e31f-39bd-1fe339bd1fe3",
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
      "optInToDeviceIdSharing": true
    }
  ]
}
```





