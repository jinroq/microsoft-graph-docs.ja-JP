---
title: windowsUpdateForBusinessConfigurations のリスト
description: windowsUpdateForBusinessConfiguration オブジェクトのプロパティとリレーションシップをリストします。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 91bd264458c471efd401b04a9a22152d2dfb330e
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27927759"
---
# <a name="list-windowsupdateforbusinessconfigurations"></a><span data-ttu-id="933b6-103">windowsUpdateForBusinessConfigurations のリスト</span><span class="sxs-lookup"><span data-stu-id="933b6-103">List windowsUpdateForBusinessConfigurations</span></span>

> <span data-ttu-id="933b6-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="933b6-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="933b6-105">[windowsUpdateForBusinessConfiguration](../resources/intune-deviceconfig-windowsupdateforbusinessconfiguration.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="933b6-105">List properties and relationships of the [windowsUpdateForBusinessConfiguration](../resources/intune-deviceconfig-windowsupdateforbusinessconfiguration.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="933b6-106">前提条件</span><span class="sxs-lookup"><span data-stu-id="933b6-106">Prerequisites</span></span>
<span data-ttu-id="933b6-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="933b6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="933b6-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="933b6-109">Permission type</span></span>|<span data-ttu-id="933b6-110">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="933b6-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="933b6-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="933b6-111">Delegated (work or school account)</span></span>|<span data-ttu-id="933b6-112">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="933b6-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="933b6-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="933b6-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="933b6-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="933b6-114">Not supported.</span></span>|
|<span data-ttu-id="933b6-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="933b6-115">Application</span></span>|<span data-ttu-id="933b6-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="933b6-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="933b6-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="933b6-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="933b6-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="933b6-118">Request headers</span></span>
|<span data-ttu-id="933b6-119">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="933b6-119">Header</span></span>|<span data-ttu-id="933b6-120">値</span><span class="sxs-lookup"><span data-stu-id="933b6-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="933b6-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="933b6-121">Authorization</span></span>|<span data-ttu-id="933b6-122">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="933b6-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="933b6-123">Accept</span><span class="sxs-lookup"><span data-stu-id="933b6-123">Accept</span></span>|<span data-ttu-id="933b6-124">application/json</span><span class="sxs-lookup"><span data-stu-id="933b6-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="933b6-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="933b6-125">Request body</span></span>
<span data-ttu-id="933b6-126">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="933b6-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="933b6-127">応答</span><span class="sxs-lookup"><span data-stu-id="933b6-127">Response</span></span>
<span data-ttu-id="933b6-128">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [windowsUpdateForBusinessConfiguration](../resources/intune-deviceconfig-windowsupdateforbusinessconfiguration.md) オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="933b6-128">If successful, this method returns a `200 OK` response code and a collection of [windowsUpdateForBusinessConfiguration](../resources/intune-deviceconfig-windowsupdateforbusinessconfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="933b6-129">例</span><span class="sxs-lookup"><span data-stu-id="933b6-129">Example</span></span>
### <a name="request"></a><span data-ttu-id="933b6-130">要求</span><span class="sxs-lookup"><span data-stu-id="933b6-130">Request</span></span>
<span data-ttu-id="933b6-131">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="933b6-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations
```

### <a name="response"></a><span data-ttu-id="933b6-132">応答</span><span class="sxs-lookup"><span data-stu-id="933b6-132">Response</span></span>
<span data-ttu-id="933b6-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="933b6-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1211

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.windowsUpdateForBusinessConfiguration",
      "id": "4928dd6a-dd6a-4928-6add-28496add2849",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
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
      "businessReadyUpdatesOnly": "all"
    }
  ]
}
```



