---
title: リスト windowsPhone81VpnConfigurations
description: WindowsPhone81VpnConfiguration オブジェクトのプロパティとリレーションシップをリストします。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: a912e5490a5e914f968935e202df204d32d4ac7b
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/14/2019
ms.locfileid: "34961498"
---
# <a name="list-windowsphone81vpnconfigurations"></a><span data-ttu-id="eb2da-103">リスト windowsPhone81VpnConfigurations</span><span class="sxs-lookup"><span data-stu-id="eb2da-103">List windowsPhone81VpnConfigurations</span></span>

> <span data-ttu-id="eb2da-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="eb2da-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="eb2da-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="eb2da-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="eb2da-106">[WindowsPhone81VpnConfiguration](../resources/intune-deviceconfig-windowsphone81vpnconfiguration.md)オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="eb2da-106">List properties and relationships of the [windowsPhone81VpnConfiguration](../resources/intune-deviceconfig-windowsphone81vpnconfiguration.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="eb2da-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="eb2da-107">Prerequisites</span></span>
<span data-ttu-id="eb2da-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="eb2da-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="eb2da-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="eb2da-110">Permission type</span></span>|<span data-ttu-id="eb2da-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="eb2da-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="eb2da-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="eb2da-112">Delegated (work or school account)</span></span>|<span data-ttu-id="eb2da-113">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="eb2da-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="eb2da-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="eb2da-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="eb2da-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="eb2da-115">Not supported.</span></span>|
|<span data-ttu-id="eb2da-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="eb2da-116">Application</span></span>|<span data-ttu-id="eb2da-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="eb2da-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="eb2da-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="eb2da-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="eb2da-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="eb2da-119">Request headers</span></span>
|<span data-ttu-id="eb2da-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="eb2da-120">Header</span></span>|<span data-ttu-id="eb2da-121">値</span><span class="sxs-lookup"><span data-stu-id="eb2da-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="eb2da-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="eb2da-122">Authorization</span></span>|<span data-ttu-id="eb2da-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="eb2da-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="eb2da-124">承諾</span><span class="sxs-lookup"><span data-stu-id="eb2da-124">Accept</span></span>|<span data-ttu-id="eb2da-125">application/json</span><span class="sxs-lookup"><span data-stu-id="eb2da-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="eb2da-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="eb2da-126">Request body</span></span>
<span data-ttu-id="eb2da-127">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="eb2da-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="eb2da-128">応答</span><span class="sxs-lookup"><span data-stu-id="eb2da-128">Response</span></span>
<span data-ttu-id="eb2da-129">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で[windowsPhone81VpnConfiguration](../resources/intune-deviceconfig-windowsphone81vpnconfiguration.md)オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="eb2da-129">If successful, this method returns a `200 OK` response code and a collection of [windowsPhone81VpnConfiguration](../resources/intune-deviceconfig-windowsphone81vpnconfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="eb2da-130">例</span><span class="sxs-lookup"><span data-stu-id="eb2da-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="eb2da-131">要求</span><span class="sxs-lookup"><span data-stu-id="eb2da-131">Request</span></span>
<span data-ttu-id="eb2da-132">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="eb2da-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
```

### <a name="response"></a><span data-ttu-id="eb2da-133">応答</span><span class="sxs-lookup"><span data-stu-id="eb2da-133">Response</span></span>
<span data-ttu-id="eb2da-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="eb2da-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2465

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.windowsPhone81VpnConfiguration",
      "id": "7cecc0db-c0db-7cec-dbc0-ec7cdbc0ec7c",
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
      },
      "bypassVpnOnCompanyWifi": true,
      "bypassVpnOnHomeWifi": true,
      "authenticationMethod": "usernameAndPassword",
      "rememberUserCredentials": true,
      "dnsSuffixSearchList": [
        "Dns Suffix Search List value"
      ]
    }
  ]
}
```





