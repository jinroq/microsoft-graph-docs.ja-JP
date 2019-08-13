---
title: Get windows10TeamGeneralConfiguration
description: windows10TeamGeneralConfiguration オブジェクトのプロパティとリレーションシップを読み取ります。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: f53fd6abdbf453270cf385dff32120e8628a2442
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36344911"
---
# <a name="get-windows10teamgeneralconfiguration"></a><span data-ttu-id="1c5fb-103">Get windows10TeamGeneralConfiguration</span><span class="sxs-lookup"><span data-stu-id="1c5fb-103">Get windows10TeamGeneralConfiguration</span></span>

> <span data-ttu-id="1c5fb-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="1c5fb-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1c5fb-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="1c5fb-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1c5fb-106">[windows10TeamGeneralConfiguration](../resources/intune-deviceconfig-windows10teamgeneralconfiguration.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="1c5fb-106">Read properties and relationships of the [windows10TeamGeneralConfiguration](../resources/intune-deviceconfig-windows10teamgeneralconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="1c5fb-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="1c5fb-107">Prerequisites</span></span>
<span data-ttu-id="1c5fb-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="1c5fb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1c5fb-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="1c5fb-110">Permission type</span></span>|<span data-ttu-id="1c5fb-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="1c5fb-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1c5fb-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="1c5fb-112">Delegated (work or school account)</span></span>|<span data-ttu-id="1c5fb-113">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="1c5fb-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="1c5fb-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="1c5fb-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1c5fb-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="1c5fb-115">Not supported.</span></span>|
|<span data-ttu-id="1c5fb-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="1c5fb-116">Application</span></span>|<span data-ttu-id="1c5fb-117">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="1c5fb-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="1c5fb-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="1c5fb-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="1c5fb-119">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="1c5fb-119">Optional query parameters</span></span>
<span data-ttu-id="1c5fb-120">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://docs.microsoft.com/en-us/graph/query-parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="1c5fb-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="1c5fb-121">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="1c5fb-121">Request headers</span></span>
|<span data-ttu-id="1c5fb-122">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="1c5fb-122">Header</span></span>|<span data-ttu-id="1c5fb-123">値</span><span class="sxs-lookup"><span data-stu-id="1c5fb-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1c5fb-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="1c5fb-124">Authorization</span></span>|<span data-ttu-id="1c5fb-125">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="1c5fb-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1c5fb-126">承諾</span><span class="sxs-lookup"><span data-stu-id="1c5fb-126">Accept</span></span>|<span data-ttu-id="1c5fb-127">application/json</span><span class="sxs-lookup"><span data-stu-id="1c5fb-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1c5fb-128">要求本文</span><span class="sxs-lookup"><span data-stu-id="1c5fb-128">Request body</span></span>
<span data-ttu-id="1c5fb-129">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="1c5fb-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1c5fb-130">応答</span><span class="sxs-lookup"><span data-stu-id="1c5fb-130">Response</span></span>
<span data-ttu-id="1c5fb-131">このメソッドが成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [windows10TeamGeneralConfiguration](../resources/intune-deviceconfig-windows10teamgeneralconfiguration.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="1c5fb-131">If successful, this method returns a `200 OK` response code and [windows10TeamGeneralConfiguration](../resources/intune-deviceconfig-windows10teamgeneralconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1c5fb-132">例</span><span class="sxs-lookup"><span data-stu-id="1c5fb-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="1c5fb-133">要求</span><span class="sxs-lookup"><span data-stu-id="1c5fb-133">Request</span></span>
<span data-ttu-id="1c5fb-134">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="1c5fb-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

### <a name="response"></a><span data-ttu-id="1c5fb-135">応答</span><span class="sxs-lookup"><span data-stu-id="1c5fb-135">Response</span></span>
<span data-ttu-id="1c5fb-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="1c5fb-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2310

{
  "value": {
    "@odata.type": "#microsoft.graph.windows10TeamGeneralConfiguration",
    "id": "0c94aa20-aa20-0c94-20aa-940c20aa940c",
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
    "azureOperationalInsightsBlockTelemetry": true,
    "azureOperationalInsightsWorkspaceId": "Azure Operational Insights Workspace Id value",
    "azureOperationalInsightsWorkspaceKey": "Azure Operational Insights Workspace Key value",
    "connectAppBlockAutoLaunch": true,
    "maintenanceWindowBlocked": true,
    "maintenanceWindowDurationInHours": 0,
    "maintenanceWindowStartTime": "11:59:09.3130000",
    "miracastChannel": "one",
    "miracastBlocked": true,
    "miracastRequirePin": true,
    "settingsBlockMyMeetingsAndFiles": true,
    "settingsBlockSessionResume": true,
    "settingsBlockSigninSuggestions": true,
    "settingsDefaultVolume": 5,
    "settingsScreenTimeoutInMinutes": 14,
    "settingsSessionTimeoutInMinutes": 15,
    "settingsSleepTimeoutInMinutes": 13,
    "welcomeScreenBlockAutomaticWakeUp": true,
    "welcomeScreenBackgroundImageUrl": "https://example.com/welcomeScreenBackgroundImageUrl/",
    "welcomeScreenMeetingInformation": "showOrganizerAndTimeOnly"
  }
}
```






