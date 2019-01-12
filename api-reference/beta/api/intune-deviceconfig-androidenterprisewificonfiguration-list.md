---
title: リスト androidEnterpriseWiFiConfigurations
description: AndroidEnterpriseWiFiConfiguration オブジェクトのプロパティと関係を一覧表示します。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 7687224cc13c45e35d3518bd8e8ee35d5b695e21
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27968184"
---
# <a name="list-androidenterprisewificonfigurations"></a><span data-ttu-id="c6d45-103">リスト androidEnterpriseWiFiConfigurations</span><span class="sxs-lookup"><span data-stu-id="c6d45-103">List androidEnterpriseWiFiConfigurations</span></span>

> <span data-ttu-id="c6d45-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="c6d45-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c6d45-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c6d45-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="c6d45-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="c6d45-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="c6d45-107">[AndroidEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-androidenterprisewificonfiguration.md)オブジェクトのプロパティと関係を一覧表示します。</span><span class="sxs-lookup"><span data-stu-id="c6d45-107">List properties and relationships of the [androidEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-androidenterprisewificonfiguration.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="c6d45-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="c6d45-108">Prerequisites</span></span>
<span data-ttu-id="c6d45-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="c6d45-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c6d45-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="c6d45-111">Permission type</span></span>|<span data-ttu-id="c6d45-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="c6d45-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c6d45-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="c6d45-113">Delegated (work or school account)</span></span>|<span data-ttu-id="c6d45-114">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="c6d45-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="c6d45-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="c6d45-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c6d45-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c6d45-116">Not supported.</span></span>|
|<span data-ttu-id="c6d45-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="c6d45-117">Application</span></span>|<span data-ttu-id="c6d45-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c6d45-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c6d45-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="c6d45-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="c6d45-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="c6d45-120">Request headers</span></span>
|<span data-ttu-id="c6d45-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="c6d45-121">Header</span></span>|<span data-ttu-id="c6d45-122">値</span><span class="sxs-lookup"><span data-stu-id="c6d45-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c6d45-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="c6d45-123">Authorization</span></span>|<span data-ttu-id="c6d45-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="c6d45-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c6d45-125">Accept</span><span class="sxs-lookup"><span data-stu-id="c6d45-125">Accept</span></span>|<span data-ttu-id="c6d45-126">application/json</span><span class="sxs-lookup"><span data-stu-id="c6d45-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c6d45-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="c6d45-127">Request body</span></span>
<span data-ttu-id="c6d45-128">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="c6d45-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c6d45-129">応答</span><span class="sxs-lookup"><span data-stu-id="c6d45-129">Response</span></span>
<span data-ttu-id="c6d45-130">かどうかは成功すると、このメソッドが返されます、`200 OK`応答コードおよび応答の本文に[androidEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-androidenterprisewificonfiguration.md)オブジェクトのコレクションです。</span><span class="sxs-lookup"><span data-stu-id="c6d45-130">If successful, this method returns a `200 OK` response code and a collection of [androidEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-androidenterprisewificonfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c6d45-131">例</span><span class="sxs-lookup"><span data-stu-id="c6d45-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="c6d45-132">要求</span><span class="sxs-lookup"><span data-stu-id="c6d45-132">Request</span></span>
<span data-ttu-id="c6d45-133">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="c6d45-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
```

### <a name="response"></a><span data-ttu-id="c6d45-134">応答</span><span class="sxs-lookup"><span data-stu-id="c6d45-134">Response</span></span>
<span data-ttu-id="c6d45-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="c6d45-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1054

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.androidEnterpriseWiFiConfiguration",
      "id": "972edff4-dff4-972e-f4df-2e97f4df2e97",
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
      "wiFiSecurityType": "wpaEnterprise",
      "eapType": "eapTtls",
      "authenticationMethod": "usernameAndPassword",
      "innerAuthenticationProtocolForEapTtls": "challengeHandshakeAuthenticationProtocol",
      "innerAuthenticationProtocolForPeap": "microsoftChapVersionTwo",
      "outerIdentityPrivacyTemporaryValue": "Outer Identity Privacy Temporary Value value"
    }
  ]
}
```





