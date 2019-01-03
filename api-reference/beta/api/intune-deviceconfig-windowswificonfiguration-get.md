---
title: WindowsWifiConfiguration を取得します。
description: WindowsWifiConfiguration オブジェクトのプロパティと関係を参照してください。
author: tfitzmac
ms.openlocfilehash: 89a20033e38231dc6ed45918ce58a837ef1cebb9
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27349519"
---
# <a name="get-windowswificonfiguration"></a><span data-ttu-id="96e5b-103">WindowsWifiConfiguration を取得します。</span><span class="sxs-lookup"><span data-stu-id="96e5b-103">Get windowsWifiConfiguration</span></span>

> <span data-ttu-id="96e5b-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="96e5b-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="96e5b-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="96e5b-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="96e5b-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="96e5b-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="96e5b-107">[WindowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)オブジェクトのプロパティと関係を参照してください。</span><span class="sxs-lookup"><span data-stu-id="96e5b-107">Read properties and relationships of the [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="96e5b-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="96e5b-108">Prerequisites</span></span>
<span data-ttu-id="96e5b-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="96e5b-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="96e5b-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="96e5b-111">Permission type</span></span>|<span data-ttu-id="96e5b-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="96e5b-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="96e5b-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="96e5b-113">Delegated (work or school account)</span></span>|<span data-ttu-id="96e5b-114">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="96e5b-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="96e5b-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="96e5b-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="96e5b-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="96e5b-116">Not supported.</span></span>|
|<span data-ttu-id="96e5b-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="96e5b-117">Application</span></span>|<span data-ttu-id="96e5b-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="96e5b-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="96e5b-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="96e5b-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="96e5b-120">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="96e5b-120">Optional query parameters</span></span>
<span data-ttu-id="96e5b-121">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="96e5b-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="96e5b-122">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="96e5b-122">Request headers</span></span>
|<span data-ttu-id="96e5b-123">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="96e5b-123">Header</span></span>|<span data-ttu-id="96e5b-124">値</span><span class="sxs-lookup"><span data-stu-id="96e5b-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="96e5b-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="96e5b-125">Authorization</span></span>|<span data-ttu-id="96e5b-126">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="96e5b-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="96e5b-127">Accept</span><span class="sxs-lookup"><span data-stu-id="96e5b-127">Accept</span></span>|<span data-ttu-id="96e5b-128">application/json</span><span class="sxs-lookup"><span data-stu-id="96e5b-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="96e5b-129">要求本文</span><span class="sxs-lookup"><span data-stu-id="96e5b-129">Request body</span></span>
<span data-ttu-id="96e5b-130">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="96e5b-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="96e5b-131">応答</span><span class="sxs-lookup"><span data-stu-id="96e5b-131">Response</span></span>
<span data-ttu-id="96e5b-132">かどうかは成功すると、このメソッドが返されます、 `200 OK` 、応答の本体で応答コードと[windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)のオブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="96e5b-132">If successful, this method returns a `200 OK` response code and [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="96e5b-133">例</span><span class="sxs-lookup"><span data-stu-id="96e5b-133">Example</span></span>
### <a name="request"></a><span data-ttu-id="96e5b-134">要求</span><span class="sxs-lookup"><span data-stu-id="96e5b-134">Request</span></span>
<span data-ttu-id="96e5b-135">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="96e5b-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

### <a name="response"></a><span data-ttu-id="96e5b-136">応答</span><span class="sxs-lookup"><span data-stu-id="96e5b-136">Response</span></span>
<span data-ttu-id="96e5b-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="96e5b-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1025

{
  "value": {
    "@odata.type": "#microsoft.graph.windowsWifiConfiguration",
    "id": "8a9e790f-790f-8a9e-0f79-9e8a0f799e8a",
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
    "forceFIPSCompliance": true
  }
}
```




