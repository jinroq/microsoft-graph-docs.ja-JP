---
title: リスト Macoswi/raw Onfigurた
description: MacOSWiFiConfiguration オブジェクトのプロパティとリレーションシップをリストします。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: ff4f73d8fd3ca9749b326513dec52464687b167e
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35946837"
---
# <a name="list-macoswificonfigurations"></a><span data-ttu-id="82dd4-103">リスト Macoswi/raw Onfigurた</span><span class="sxs-lookup"><span data-stu-id="82dd4-103">List macOSWiFiConfigurations</span></span>

> <span data-ttu-id="82dd4-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="82dd4-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="82dd4-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="82dd4-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="82dd4-106">[MacOSWiFiConfiguration](../resources/intune-deviceconfig-macoswificonfiguration.md)オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="82dd4-106">List properties and relationships of the [macOSWiFiConfiguration](../resources/intune-deviceconfig-macoswificonfiguration.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="82dd4-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="82dd4-107">Prerequisites</span></span>
<span data-ttu-id="82dd4-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="82dd4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="82dd4-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="82dd4-110">Permission type</span></span>|<span data-ttu-id="82dd4-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="82dd4-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="82dd4-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="82dd4-112">Delegated (work or school account)</span></span>|<span data-ttu-id="82dd4-113">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="82dd4-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="82dd4-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="82dd4-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="82dd4-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="82dd4-115">Not supported.</span></span>|
|<span data-ttu-id="82dd4-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="82dd4-116">Application</span></span>|<span data-ttu-id="82dd4-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="82dd4-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="82dd4-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="82dd4-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="82dd4-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="82dd4-119">Request headers</span></span>
|<span data-ttu-id="82dd4-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="82dd4-120">Header</span></span>|<span data-ttu-id="82dd4-121">値</span><span class="sxs-lookup"><span data-stu-id="82dd4-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="82dd4-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="82dd4-122">Authorization</span></span>|<span data-ttu-id="82dd4-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="82dd4-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="82dd4-124">承諾</span><span class="sxs-lookup"><span data-stu-id="82dd4-124">Accept</span></span>|<span data-ttu-id="82dd4-125">application/json</span><span class="sxs-lookup"><span data-stu-id="82dd4-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="82dd4-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="82dd4-126">Request body</span></span>
<span data-ttu-id="82dd4-127">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="82dd4-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="82dd4-128">応答</span><span class="sxs-lookup"><span data-stu-id="82dd4-128">Response</span></span>
<span data-ttu-id="82dd4-129">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で[macOSWiFiConfiguration](../resources/intune-deviceconfig-macoswificonfiguration.md)オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="82dd4-129">If successful, this method returns a `200 OK` response code and a collection of [macOSWiFiConfiguration](../resources/intune-deviceconfig-macoswificonfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="82dd4-130">例</span><span class="sxs-lookup"><span data-stu-id="82dd4-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="82dd4-131">要求</span><span class="sxs-lookup"><span data-stu-id="82dd4-131">Request</span></span>
<span data-ttu-id="82dd4-132">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="82dd4-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
```

### <a name="response"></a><span data-ttu-id="82dd4-133">応答</span><span class="sxs-lookup"><span data-stu-id="82dd4-133">Response</span></span>
<span data-ttu-id="82dd4-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="82dd4-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1823

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.macOSWiFiConfiguration",
      "id": "471203fb-03fb-4712-fb03-1247fb031247",
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
      "wiFiSecurityType": "wpaPersonal",
      "proxySettings": "manual",
      "proxyManualAddress": "Proxy Manual Address value",
      "proxyManualPort": 15,
      "proxyAutomaticConfigurationUrl": "https://example.com/proxyAutomaticConfigurationUrl/",
      "preSharedKey": "Pre Shared Key value"
    }
  ]
}
```





