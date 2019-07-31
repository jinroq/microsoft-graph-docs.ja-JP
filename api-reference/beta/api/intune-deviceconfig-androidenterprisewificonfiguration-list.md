---
title: Androidenterprisewiidmso Onfigurたリスト
description: AndroidEnterpriseWiFiConfiguration オブジェクトのプロパティとリレーションシップをリストします。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 1ab9d813101ae0d2b66e0bdda4254ade55207a03
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35957914"
---
# <a name="list-androidenterprisewificonfigurations"></a><span data-ttu-id="7c825-103">Androidenterprisewiidmso Onfigurたリスト</span><span class="sxs-lookup"><span data-stu-id="7c825-103">List androidEnterpriseWiFiConfigurations</span></span>

> <span data-ttu-id="7c825-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="7c825-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7c825-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="7c825-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7c825-106">[AndroidEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-androidenterprisewificonfiguration.md)オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="7c825-106">List properties and relationships of the [androidEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-androidenterprisewificonfiguration.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="7c825-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="7c825-107">Prerequisites</span></span>
<span data-ttu-id="7c825-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="7c825-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7c825-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="7c825-110">Permission type</span></span>|<span data-ttu-id="7c825-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="7c825-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7c825-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="7c825-112">Delegated (work or school account)</span></span>|<span data-ttu-id="7c825-113">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="7c825-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="7c825-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="7c825-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7c825-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="7c825-115">Not supported.</span></span>|
|<span data-ttu-id="7c825-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="7c825-116">Application</span></span>|<span data-ttu-id="7c825-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="7c825-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="7c825-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="7c825-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="7c825-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="7c825-119">Request headers</span></span>
|<span data-ttu-id="7c825-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="7c825-120">Header</span></span>|<span data-ttu-id="7c825-121">値</span><span class="sxs-lookup"><span data-stu-id="7c825-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7c825-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="7c825-122">Authorization</span></span>|<span data-ttu-id="7c825-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="7c825-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7c825-124">承諾</span><span class="sxs-lookup"><span data-stu-id="7c825-124">Accept</span></span>|<span data-ttu-id="7c825-125">application/json</span><span class="sxs-lookup"><span data-stu-id="7c825-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7c825-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="7c825-126">Request body</span></span>
<span data-ttu-id="7c825-127">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="7c825-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7c825-128">応答</span><span class="sxs-lookup"><span data-stu-id="7c825-128">Response</span></span>
<span data-ttu-id="7c825-129">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で[androidEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-androidenterprisewificonfiguration.md)オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="7c825-129">If successful, this method returns a `200 OK` response code and a collection of [androidEnterpriseWiFiConfiguration](../resources/intune-deviceconfig-androidenterprisewificonfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7c825-130">例</span><span class="sxs-lookup"><span data-stu-id="7c825-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="7c825-131">要求</span><span class="sxs-lookup"><span data-stu-id="7c825-131">Request</span></span>
<span data-ttu-id="7c825-132">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="7c825-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
```

### <a name="response"></a><span data-ttu-id="7c825-133">応答</span><span class="sxs-lookup"><span data-stu-id="7c825-133">Response</span></span>
<span data-ttu-id="7c825-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="7c825-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2084

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
      "outerIdentityPrivacyTemporaryValue": "Outer Identity Privacy Temporary Value value",
      "usernameFormatString": "Username Format String value",
      "passwordFormatString": "Password Format String value",
      "preSharedKey": "Pre Shared Key value"
    }
  ]
}
```





