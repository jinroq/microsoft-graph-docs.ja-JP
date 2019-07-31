---
title: リスト Androidwork Profileenterprisewioffonfigur捜索
description: AndroidWorkProfileEnterpriseWiFiConfiguration オブジェクトのプロパティとリレーションシップをリストします。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: fd77b88a72362af45e0d50d7d90007312997584b
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35950848"
---
# <a name="list-androidworkprofileenterprisewificonfigurations"></a><span data-ttu-id="38670-103">リスト Androidwork Profileenterprisewioffonfigur捜索</span><span class="sxs-lookup"><span data-stu-id="38670-103">List androidWorkProfileEnterpriseWiFiConfigurations</span></span>

> <span data-ttu-id="38670-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="38670-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="38670-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="38670-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="38670-106">[AndroidWorkProfileEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-androidworkprofileenterprisewificonfiguration.md)オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="38670-106">List properties and relationships of the [androidWorkProfileEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-androidworkprofileenterprisewificonfiguration.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="38670-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="38670-107">Prerequisites</span></span>
<span data-ttu-id="38670-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="38670-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="38670-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="38670-110">Permission type</span></span>|<span data-ttu-id="38670-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="38670-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="38670-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="38670-112">Delegated (work or school account)</span></span>|<span data-ttu-id="38670-113">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="38670-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="38670-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="38670-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="38670-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="38670-115">Not supported.</span></span>|
|<span data-ttu-id="38670-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="38670-116">Application</span></span>|<span data-ttu-id="38670-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="38670-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="38670-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="38670-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="38670-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="38670-119">Request headers</span></span>
|<span data-ttu-id="38670-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="38670-120">Header</span></span>|<span data-ttu-id="38670-121">値</span><span class="sxs-lookup"><span data-stu-id="38670-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="38670-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="38670-122">Authorization</span></span>|<span data-ttu-id="38670-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="38670-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="38670-124">承諾</span><span class="sxs-lookup"><span data-stu-id="38670-124">Accept</span></span>|<span data-ttu-id="38670-125">application/json</span><span class="sxs-lookup"><span data-stu-id="38670-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="38670-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="38670-126">Request body</span></span>
<span data-ttu-id="38670-127">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="38670-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="38670-128">応答</span><span class="sxs-lookup"><span data-stu-id="38670-128">Response</span></span>
<span data-ttu-id="38670-129">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で[androidWorkProfileEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-androidworkprofileenterprisewificonfiguration.md)オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="38670-129">If successful, this method returns a `200 OK` response code and a collection of [androidWorkProfileEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-androidworkprofileenterprisewificonfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="38670-130">例</span><span class="sxs-lookup"><span data-stu-id="38670-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="38670-131">要求</span><span class="sxs-lookup"><span data-stu-id="38670-131">Request</span></span>
<span data-ttu-id="38670-132">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="38670-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
```

### <a name="response"></a><span data-ttu-id="38670-133">応答</span><span class="sxs-lookup"><span data-stu-id="38670-133">Response</span></span>
<span data-ttu-id="38670-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="38670-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1922

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.androidWorkProfileEnterpriseWiFiConfiguration",
      "id": "c48cd726-d726-c48c-26d7-8cc426d78cc4",
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





