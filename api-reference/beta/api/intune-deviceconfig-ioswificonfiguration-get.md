---
title: IosWiFiConfiguration を取得する
description: IosWiFiConfiguration オブジェクトのプロパティとリレーションシップを読み取ります。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: f1223b0ad263c32343a37199779cdec7b5451a51
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35947705"
---
# <a name="get-ioswificonfiguration"></a><span data-ttu-id="8ae52-103">IosWiFiConfiguration を取得する</span><span class="sxs-lookup"><span data-stu-id="8ae52-103">Get iosWiFiConfiguration</span></span>

> <span data-ttu-id="8ae52-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="8ae52-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8ae52-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="8ae52-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8ae52-106">[IosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md)オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="8ae52-106">Read properties and relationships of the [iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="8ae52-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="8ae52-107">Prerequisites</span></span>
<span data-ttu-id="8ae52-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="8ae52-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8ae52-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="8ae52-110">Permission type</span></span>|<span data-ttu-id="8ae52-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="8ae52-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8ae52-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="8ae52-112">Delegated (work or school account)</span></span>|<span data-ttu-id="8ae52-113">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="8ae52-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="8ae52-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="8ae52-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8ae52-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="8ae52-115">Not supported.</span></span>|
|<span data-ttu-id="8ae52-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="8ae52-116">Application</span></span>|<span data-ttu-id="8ae52-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="8ae52-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="8ae52-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="8ae52-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="8ae52-119">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="8ae52-119">Optional query parameters</span></span>
<span data-ttu-id="8ae52-120">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://docs.microsoft.com/en-us/graph/query-parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="8ae52-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="8ae52-121">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="8ae52-121">Request headers</span></span>
|<span data-ttu-id="8ae52-122">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="8ae52-122">Header</span></span>|<span data-ttu-id="8ae52-123">値</span><span class="sxs-lookup"><span data-stu-id="8ae52-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8ae52-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="8ae52-124">Authorization</span></span>|<span data-ttu-id="8ae52-125">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="8ae52-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8ae52-126">承諾</span><span class="sxs-lookup"><span data-stu-id="8ae52-126">Accept</span></span>|<span data-ttu-id="8ae52-127">application/json</span><span class="sxs-lookup"><span data-stu-id="8ae52-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8ae52-128">要求本文</span><span class="sxs-lookup"><span data-stu-id="8ae52-128">Request body</span></span>
<span data-ttu-id="8ae52-129">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="8ae52-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8ae52-130">応答</span><span class="sxs-lookup"><span data-stu-id="8ae52-130">Response</span></span>
<span data-ttu-id="8ae52-131">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で[iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="8ae52-131">If successful, this method returns a `200 OK` response code and [iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8ae52-132">例</span><span class="sxs-lookup"><span data-stu-id="8ae52-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="8ae52-133">要求</span><span class="sxs-lookup"><span data-stu-id="8ae52-133">Request</span></span>
<span data-ttu-id="8ae52-134">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="8ae52-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

### <a name="response"></a><span data-ttu-id="8ae52-135">応答</span><span class="sxs-lookup"><span data-stu-id="8ae52-135">Response</span></span>
<span data-ttu-id="8ae52-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="8ae52-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1723

{
  "value": {
    "@odata.type": "#microsoft.graph.iosWiFiConfiguration",
    "id": "516f9ef9-9ef9-516f-f99e-6f51f99e6f51",
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
}
```





