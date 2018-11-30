---
title: windowsUpdateForBusinessConfigurations のリスト
description: windowsUpdateForBusinessConfiguration オブジェクトのプロパティとリレーションシップをリストします。
ms.openlocfilehash: 2709109ae523033f38a8e125e3b769051a67a832
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27072744"
---
# <a name="list-windowsupdateforbusinessconfigurations"></a><span data-ttu-id="9e1d8-103">windowsUpdateForBusinessConfigurations のリスト</span><span class="sxs-lookup"><span data-stu-id="9e1d8-103">List windowsUpdateForBusinessConfigurations</span></span>

> <span data-ttu-id="9e1d8-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="9e1d8-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="9e1d8-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="9e1d8-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="9e1d8-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="9e1d8-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="9e1d8-107">[windowsUpdateForBusinessConfiguration](../resources/intune-deviceconfig-windowsupdateforbusinessconfiguration.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="9e1d8-107">List properties and relationships of the [windowsUpdateForBusinessConfiguration](../resources/intune-deviceconfig-windowsupdateforbusinessconfiguration.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="9e1d8-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="9e1d8-108">Prerequisites</span></span>
<span data-ttu-id="9e1d8-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="9e1d8-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9e1d8-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="9e1d8-111">Permission type</span></span>|<span data-ttu-id="9e1d8-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="9e1d8-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9e1d8-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="9e1d8-113">Delegated (work or school account)</span></span>|<span data-ttu-id="9e1d8-114">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="9e1d8-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="9e1d8-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="9e1d8-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9e1d8-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="9e1d8-116">Not supported.</span></span>|
|<span data-ttu-id="9e1d8-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="9e1d8-117">Application</span></span>|<span data-ttu-id="9e1d8-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="9e1d8-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="9e1d8-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="9e1d8-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="9e1d8-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="9e1d8-120">Request headers</span></span>
|<span data-ttu-id="9e1d8-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="9e1d8-121">Header</span></span>|<span data-ttu-id="9e1d8-122">値</span><span class="sxs-lookup"><span data-stu-id="9e1d8-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9e1d8-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="9e1d8-123">Authorization</span></span>|<span data-ttu-id="9e1d8-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="9e1d8-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9e1d8-125">Accept</span><span class="sxs-lookup"><span data-stu-id="9e1d8-125">Accept</span></span>|<span data-ttu-id="9e1d8-126">application/json</span><span class="sxs-lookup"><span data-stu-id="9e1d8-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9e1d8-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="9e1d8-127">Request body</span></span>
<span data-ttu-id="9e1d8-128">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="9e1d8-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9e1d8-129">応答</span><span class="sxs-lookup"><span data-stu-id="9e1d8-129">Response</span></span>
<span data-ttu-id="9e1d8-130">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [windowsUpdateForBusinessConfiguration](../resources/intune-deviceconfig-windowsupdateforbusinessconfiguration.md) オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="9e1d8-130">If successful, this method returns a `200 OK` response code and a collection of [windowsUpdateForBusinessConfiguration](../resources/intune-deviceconfig-windowsupdateforbusinessconfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9e1d8-131">例</span><span class="sxs-lookup"><span data-stu-id="9e1d8-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="9e1d8-132">要求</span><span class="sxs-lookup"><span data-stu-id="9e1d8-132">Request</span></span>
<span data-ttu-id="9e1d8-133">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="9e1d8-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
```

### <a name="response"></a><span data-ttu-id="9e1d8-134">応答</span><span class="sxs-lookup"><span data-stu-id="9e1d8-134">Response</span></span>
<span data-ttu-id="9e1d8-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="9e1d8-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2176

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.windowsUpdateForBusinessConfiguration",
      "id": "4928dd6a-dd6a-4928-6add-28496add2849",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "roleScopeTagIds": [
        "Role Scope Tag Ids value"
      ],
      "supportsScopeTags": true,
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
      "qualityUpdatesPauseStartDateTime": "Quality Updates Pause Start Date Time value",
      "featureUpdatesPauseStartDateTime": "Feature Updates Pause Start Date Time value",
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
      "scheduleImminentRestartWarningInMinutes": 7
    }
  ]
}
```





