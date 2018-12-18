---
title: リスト windows10NetworkBoundaryConfigurations
description: Windows10NetworkBoundaryConfiguration オブジェクトのプロパティと関係を一覧表示します。
author: tfitzmac
ms.openlocfilehash: b00f450e05d99c2fad5943093622762fc5b24772
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27355539"
---
# <a name="list-windows10networkboundaryconfigurations"></a><span data-ttu-id="d6517-103">リスト windows10NetworkBoundaryConfigurations</span><span class="sxs-lookup"><span data-stu-id="d6517-103">List windows10NetworkBoundaryConfigurations</span></span>

> <span data-ttu-id="d6517-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="d6517-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d6517-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d6517-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="d6517-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="d6517-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="d6517-107">[Windows10NetworkBoundaryConfiguration](../resources/intune-deviceconfig-windows10networkboundaryconfiguration.md)オブジェクトのプロパティと関係を一覧表示します。</span><span class="sxs-lookup"><span data-stu-id="d6517-107">List properties and relationships of the [windows10NetworkBoundaryConfiguration](../resources/intune-deviceconfig-windows10networkboundaryconfiguration.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="d6517-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="d6517-108">Prerequisites</span></span>
<span data-ttu-id="d6517-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="d6517-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d6517-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="d6517-111">Permission type</span></span>|<span data-ttu-id="d6517-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="d6517-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d6517-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="d6517-113">Delegated (work or school account)</span></span>|<span data-ttu-id="d6517-114">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="d6517-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="d6517-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="d6517-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d6517-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d6517-116">Not supported.</span></span>|
|<span data-ttu-id="d6517-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="d6517-117">Application</span></span>|<span data-ttu-id="d6517-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d6517-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d6517-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="d6517-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="d6517-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="d6517-120">Request headers</span></span>
|<span data-ttu-id="d6517-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="d6517-121">Header</span></span>|<span data-ttu-id="d6517-122">値</span><span class="sxs-lookup"><span data-stu-id="d6517-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d6517-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="d6517-123">Authorization</span></span>|<span data-ttu-id="d6517-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="d6517-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d6517-125">Accept</span><span class="sxs-lookup"><span data-stu-id="d6517-125">Accept</span></span>|<span data-ttu-id="d6517-126">application/json</span><span class="sxs-lookup"><span data-stu-id="d6517-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d6517-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="d6517-127">Request body</span></span>
<span data-ttu-id="d6517-128">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="d6517-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d6517-129">応答</span><span class="sxs-lookup"><span data-stu-id="d6517-129">Response</span></span>
<span data-ttu-id="d6517-130">かどうかは成功すると、このメソッドが返されます、`200 OK`応答コードおよび応答の本文に[windows10NetworkBoundaryConfiguration](../resources/intune-deviceconfig-windows10networkboundaryconfiguration.md)オブジェクトのコレクションです。</span><span class="sxs-lookup"><span data-stu-id="d6517-130">If successful, this method returns a `200 OK` response code and a collection of [windows10NetworkBoundaryConfiguration](../resources/intune-deviceconfig-windows10networkboundaryconfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d6517-131">例</span><span class="sxs-lookup"><span data-stu-id="d6517-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="d6517-132">要求</span><span class="sxs-lookup"><span data-stu-id="d6517-132">Request</span></span>
<span data-ttu-id="d6517-133">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="d6517-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
```

### <a name="response"></a><span data-ttu-id="d6517-134">応答</span><span class="sxs-lookup"><span data-stu-id="d6517-134">Response</span></span>
<span data-ttu-id="d6517-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="d6517-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1617

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.windows10NetworkBoundaryConfiguration",
      "id": "afbc9e01-9e01-afbc-019e-bcaf019ebcaf",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "roleScopeTagIds": [
        "Role Scope Tag Ids value"
      ],
      "supportsScopeTags": true,
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "description": "Description value",
      "displayName": "Display Name value",
      "version": 7,
      "windowsNetworkIsolationPolicy": {
        "@odata.type": "microsoft.graph.windowsNetworkIsolationPolicy",
        "enterpriseNetworkDomainNames": [
          "Enterprise Network Domain Names value"
        ],
        "enterpriseCloudResources": [
          {
            "@odata.type": "microsoft.graph.proxiedDomain",
            "ipAddressOrFQDN": "Ip Address Or FQDN value",
            "proxy": "Proxy value"
          }
        ],
        "enterpriseIPRanges": [
          {
            "@odata.type": "microsoft.graph.iPv6Range",
            "lowerAddress": "Lower Address value",
            "upperAddress": "Upper Address value"
          }
        ],
        "enterpriseInternalProxyServers": [
          "Enterprise Internal Proxy Servers value"
        ],
        "enterpriseIPRangesAreAuthoritative": true,
        "enterpriseProxyServers": [
          "Enterprise Proxy Servers value"
        ],
        "enterpriseProxyServersAreAuthoritative": true,
        "neutralDomainResources": [
          "Neutral Domain Resources value"
        ]
      }
    }
  ]
}
```





