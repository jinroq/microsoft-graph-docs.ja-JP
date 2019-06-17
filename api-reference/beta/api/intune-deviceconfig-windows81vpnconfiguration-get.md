---
title: Windows81VpnConfiguration を取得する
description: Windows81VpnConfiguration オブジェクトのプロパティとリレーションシップを読み取ります。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 8335bd8325e6264a7be97197259ea253c180b749
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/14/2019
ms.locfileid: "34977731"
---
# <a name="get-windows81vpnconfiguration"></a><span data-ttu-id="ce97f-103">Windows81VpnConfiguration を取得する</span><span class="sxs-lookup"><span data-stu-id="ce97f-103">Get windows81VpnConfiguration</span></span>

> <span data-ttu-id="ce97f-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ce97f-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ce97f-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="ce97f-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ce97f-106">[Windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md)オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="ce97f-106">Read properties and relationships of the [windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ce97f-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="ce97f-107">Prerequisites</span></span>
<span data-ttu-id="ce97f-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="ce97f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ce97f-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="ce97f-110">Permission type</span></span>|<span data-ttu-id="ce97f-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="ce97f-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ce97f-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="ce97f-112">Delegated (work or school account)</span></span>|<span data-ttu-id="ce97f-113">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="ce97f-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="ce97f-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="ce97f-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ce97f-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ce97f-115">Not supported.</span></span>|
|<span data-ttu-id="ce97f-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="ce97f-116">Application</span></span>|<span data-ttu-id="ce97f-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ce97f-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ce97f-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="ce97f-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="ce97f-119">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="ce97f-119">Optional query parameters</span></span>
<span data-ttu-id="ce97f-120">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://docs.microsoft.com/en-us/graph/query-parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="ce97f-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="ce97f-121">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="ce97f-121">Request headers</span></span>
|<span data-ttu-id="ce97f-122">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="ce97f-122">Header</span></span>|<span data-ttu-id="ce97f-123">値</span><span class="sxs-lookup"><span data-stu-id="ce97f-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ce97f-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="ce97f-124">Authorization</span></span>|<span data-ttu-id="ce97f-125">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="ce97f-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ce97f-126">承諾</span><span class="sxs-lookup"><span data-stu-id="ce97f-126">Accept</span></span>|<span data-ttu-id="ce97f-127">application/json</span><span class="sxs-lookup"><span data-stu-id="ce97f-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ce97f-128">要求本文</span><span class="sxs-lookup"><span data-stu-id="ce97f-128">Request body</span></span>
<span data-ttu-id="ce97f-129">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="ce97f-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ce97f-130">応答</span><span class="sxs-lookup"><span data-stu-id="ce97f-130">Response</span></span>
<span data-ttu-id="ce97f-131">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で[windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="ce97f-131">If successful, this method returns a `200 OK` response code and [windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ce97f-132">例</span><span class="sxs-lookup"><span data-stu-id="ce97f-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="ce97f-133">要求</span><span class="sxs-lookup"><span data-stu-id="ce97f-133">Request</span></span>
<span data-ttu-id="ce97f-134">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="ce97f-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

### <a name="response"></a><span data-ttu-id="ce97f-135">応答</span><span class="sxs-lookup"><span data-stu-id="ce97f-135">Response</span></span>
<span data-ttu-id="ce97f-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="ce97f-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2087

{
  "value": {
    "@odata.type": "#microsoft.graph.windows81VpnConfiguration",
    "id": "6aa07da3-7da3-6aa0-a37d-a06aa37da06a",
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
    "servers": [
      {
        "@odata.type": "microsoft.graph.vpnServer",
        "description": "Description value",
        "address": "Address value",
        "isDefaultServer": true
      }
    ],
    "customXml": "Y3VzdG9tWG1s",
    "applyOnlyToWindows81": true,
    "connectionType": "f5EdgeClient",
    "loginGroupOrDomain": "Login Group Or Domain value",
    "enableSplitTunneling": true,
    "proxyServer": {
      "@odata.type": "microsoft.graph.windows81VpnProxyServer",
      "automaticConfigurationScriptUrl": "https://example.com/automaticConfigurationScriptUrl/",
      "address": "Address value",
      "port": 4,
      "automaticallyDetectProxySettings": true,
      "bypassProxyServerForLocalAddress": true
    }
  }
}
```





