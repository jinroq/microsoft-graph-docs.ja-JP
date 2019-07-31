---
title: WindowsHealthMonitoringConfiguration を取得する
description: WindowsHealthMonitoringConfiguration オブジェクトのプロパティとリレーションシップを読み取ります。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: b776ce3383545f25458419c42a77e2b4fead0542
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35984952"
---
# <a name="get-windowshealthmonitoringconfiguration"></a><span data-ttu-id="21423-103">WindowsHealthMonitoringConfiguration を取得する</span><span class="sxs-lookup"><span data-stu-id="21423-103">Get windowsHealthMonitoringConfiguration</span></span>

> <span data-ttu-id="21423-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="21423-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="21423-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="21423-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="21423-106">[WindowsHealthMonitoringConfiguration](../resources/intune-deviceconfig-windowshealthmonitoringconfiguration.md)オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="21423-106">Read properties and relationships of the [windowsHealthMonitoringConfiguration](../resources/intune-deviceconfig-windowshealthmonitoringconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="21423-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="21423-107">Prerequisites</span></span>
<span data-ttu-id="21423-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="21423-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="21423-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="21423-110">Permission type</span></span>|<span data-ttu-id="21423-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="21423-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="21423-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="21423-112">Delegated (work or school account)</span></span>|<span data-ttu-id="21423-113">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="21423-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="21423-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="21423-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="21423-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="21423-115">Not supported.</span></span>|
|<span data-ttu-id="21423-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="21423-116">Application</span></span>|<span data-ttu-id="21423-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="21423-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="21423-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="21423-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="21423-119">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="21423-119">Optional query parameters</span></span>
<span data-ttu-id="21423-120">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://docs.microsoft.com/en-us/graph/query-parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="21423-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="21423-121">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="21423-121">Request headers</span></span>
|<span data-ttu-id="21423-122">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="21423-122">Header</span></span>|<span data-ttu-id="21423-123">値</span><span class="sxs-lookup"><span data-stu-id="21423-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="21423-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="21423-124">Authorization</span></span>|<span data-ttu-id="21423-125">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="21423-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="21423-126">承諾</span><span class="sxs-lookup"><span data-stu-id="21423-126">Accept</span></span>|<span data-ttu-id="21423-127">application/json</span><span class="sxs-lookup"><span data-stu-id="21423-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="21423-128">要求本文</span><span class="sxs-lookup"><span data-stu-id="21423-128">Request body</span></span>
<span data-ttu-id="21423-129">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="21423-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="21423-130">応答</span><span class="sxs-lookup"><span data-stu-id="21423-130">Response</span></span>
<span data-ttu-id="21423-131">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で[windowsHealthMonitoringConfiguration](../resources/intune-deviceconfig-windowshealthmonitoringconfiguration.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="21423-131">If successful, this method returns a `200 OK` response code and [windowsHealthMonitoringConfiguration](../resources/intune-deviceconfig-windowshealthmonitoringconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="21423-132">例</span><span class="sxs-lookup"><span data-stu-id="21423-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="21423-133">要求</span><span class="sxs-lookup"><span data-stu-id="21423-133">Request</span></span>
<span data-ttu-id="21423-134">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="21423-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

### <a name="response"></a><span data-ttu-id="21423-135">応答</span><span class="sxs-lookup"><span data-stu-id="21423-135">Response</span></span>
<span data-ttu-id="21423-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="21423-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1505

{
  "value": {
    "@odata.type": "#microsoft.graph.windowsHealthMonitoringConfiguration",
    "id": "3439bcec-bcec-3439-ecbc-3934ecbc3934",
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
    "allowDeviceHealthMonitoring": "enabled",
    "configDeviceHealthMonitoringScope": "healthMonitoring",
    "configDeviceHealthMonitoringCustomScope": "Config Device Health Monitoring Custom Scope value"
  }
}
```





