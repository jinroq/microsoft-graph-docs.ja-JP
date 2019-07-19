---
title: Get windowsUpdateForBusinessConfiguration
description: windowsUpdateForBusinessConfiguration オブジェクトのプロパティとリレーションシップを読み取ります。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 4c28c07f343245fe625a2a4b99baf7cdd7014841
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/14/2019
ms.locfileid: "34961309"
---
# <a name="get-windowsupdateforbusinessconfiguration"></a><span data-ttu-id="82278-103">Get windowsUpdateForBusinessConfiguration</span><span class="sxs-lookup"><span data-stu-id="82278-103">Get windowsUpdateForBusinessConfiguration</span></span>

> <span data-ttu-id="82278-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="82278-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="82278-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="82278-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="82278-106">[windowsUpdateForBusinessConfiguration](../resources/intune-deviceconfig-windowsupdateforbusinessconfiguration.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="82278-106">Read properties and relationships of the [windowsUpdateForBusinessConfiguration](../resources/intune-deviceconfig-windowsupdateforbusinessconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="82278-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="82278-107">Prerequisites</span></span>
<span data-ttu-id="82278-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="82278-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="82278-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="82278-110">Permission type</span></span>|<span data-ttu-id="82278-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="82278-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="82278-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="82278-112">Delegated (work or school account)</span></span>|<span data-ttu-id="82278-113">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="82278-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="82278-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="82278-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="82278-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="82278-115">Not supported.</span></span>|
|<span data-ttu-id="82278-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="82278-116">Application</span></span>|<span data-ttu-id="82278-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="82278-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="82278-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="82278-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="82278-119">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="82278-119">Optional query parameters</span></span>
<span data-ttu-id="82278-120">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://docs.microsoft.com/en-us/graph/query-parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="82278-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="82278-121">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="82278-121">Request headers</span></span>
|<span data-ttu-id="82278-122">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="82278-122">Header</span></span>|<span data-ttu-id="82278-123">値</span><span class="sxs-lookup"><span data-stu-id="82278-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="82278-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="82278-124">Authorization</span></span>|<span data-ttu-id="82278-125">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="82278-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="82278-126">承諾</span><span class="sxs-lookup"><span data-stu-id="82278-126">Accept</span></span>|<span data-ttu-id="82278-127">application/json</span><span class="sxs-lookup"><span data-stu-id="82278-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="82278-128">要求本文</span><span class="sxs-lookup"><span data-stu-id="82278-128">Request body</span></span>
<span data-ttu-id="82278-129">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="82278-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="82278-130">応答</span><span class="sxs-lookup"><span data-stu-id="82278-130">Response</span></span>
<span data-ttu-id="82278-131">このメソッドが成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [windowsUpdateForBusinessConfiguration](../resources/intune-deviceconfig-windowsupdateforbusinessconfiguration.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="82278-131">If successful, this method returns a `200 OK` response code and [windowsUpdateForBusinessConfiguration](../resources/intune-deviceconfig-windowsupdateforbusinessconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="82278-132">例</span><span class="sxs-lookup"><span data-stu-id="82278-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="82278-133">要求</span><span class="sxs-lookup"><span data-stu-id="82278-133">Request</span></span>
<span data-ttu-id="82278-134">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="82278-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

### <a name="response"></a><span data-ttu-id="82278-135">応答</span><span class="sxs-lookup"><span data-stu-id="82278-135">Response</span></span>
<span data-ttu-id="82278-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="82278-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 3001

{
  "value": {
    "@odata.type": "#microsoft.graph.windowsUpdateForBusinessConfiguration",
    "id": "4928dd6a-dd6a-4928-6add-28496add2849",
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
    "deliveryOptimizationMode": "httpOnly",
    "prereleaseFeatures": "settingsOnly",
    "automaticUpdateMode": "notifyDownload",
    "microsoftUpdateServiceAllowed": true,
    "driversExcluded": true,
    "installationSchedule": {
      "@odata.type": "microsoft.graph.windowsUpdateScheduledInstall",
      "scheduledInstallDay": "everyday",
      "scheduledInstallTime": "11:59:31.3170000"
    },
    "qualityUpdatesDeferralPeriodInDays": 2,
    "featureUpdatesDeferralPeriodInDays": 2,
    "qualityUpdatesPaused": true,
    "featureUpdatesPaused": true,
    "qualityUpdatesPauseExpiryDateTime": "2017-01-01T00:00:22.9594683-08:00",
    "featureUpdatesPauseExpiryDateTime": "2016-12-31T23:58:08.068669-08:00",
    "businessReadyUpdatesOnly": "all",
    "skipChecksBeforeRestart": true,
    "updateWeeks": "firstWeek",
    "qualityUpdatesPauseStartDate": "<Unknown Primitive Type Edm.Date>",
    "featureUpdatesPauseStartDate": "<Unknown Primitive Type Edm.Date>",
    "featureUpdatesRollbackWindowInDays": 2,
    "qualityUpdatesWillBeRolledBack": true,
    "featureUpdatesWillBeRolledBack": true,
    "qualityUpdatesRollbackStartDateTime": "2016-12-31T23:57:01.05526-08:00",
    "featureUpdatesRollbackStartDateTime": "2017-01-01T00:03:21.6080517-08:00",
    "engagedRestartDeadlineInDays": 12,
    "engagedRestartSnoozeScheduleInDays": 2,
    "engagedRestartTransitionScheduleInDays": 6,
    "autoRestartNotificationDismissal": "automatic",
    "scheduleRestartWarningInHours": 13,
    "scheduleImminentRestartWarningInMinutes": 7,
    "userPauseAccess": "enabled",
    "userWindowsUpdateScanAccess": "enabled",
    "updateNotificationLevel": "defaultNotifications"
  }
}
```





