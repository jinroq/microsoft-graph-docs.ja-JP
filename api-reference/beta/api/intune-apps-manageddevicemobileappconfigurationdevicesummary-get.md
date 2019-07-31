---
title: managedDeviceMobileAppConfigurationDeviceSummary の取得
description: managedDeviceMobileAppConfigurationDeviceSummary オブジェクトのプロパティとリレーションシップを読み取ります。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: e197e34f8855e2da115b3c08f39e84f0c8d2ba4d
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35961540"
---
# <a name="get-manageddevicemobileappconfigurationdevicesummary"></a><span data-ttu-id="c4135-103">managedDeviceMobileAppConfigurationDeviceSummary の取得</span><span class="sxs-lookup"><span data-stu-id="c4135-103">Get managedDeviceMobileAppConfigurationDeviceSummary</span></span>

> <span data-ttu-id="c4135-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c4135-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c4135-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="c4135-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c4135-106">[managedDeviceMobileAppConfigurationDeviceSummary](../resources/intune-apps-manageddevicemobileappconfigurationdevicesummary.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="c4135-106">Read properties and relationships of the [managedDeviceMobileAppConfigurationDeviceSummary](../resources/intune-apps-manageddevicemobileappconfigurationdevicesummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c4135-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="c4135-107">Prerequisites</span></span>
<span data-ttu-id="c4135-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="c4135-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c4135-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="c4135-110">Permission type</span></span>|<span data-ttu-id="c4135-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="c4135-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c4135-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="c4135-112">Delegated (work or school account)</span></span>|<span data-ttu-id="c4135-113">DeviceManagementApps.ReadWrite.All、DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="c4135-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="c4135-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="c4135-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c4135-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c4135-115">Not supported.</span></span>|
|<span data-ttu-id="c4135-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="c4135-116">Application</span></span>|<span data-ttu-id="c4135-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c4135-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c4135-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="c4135-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/deviceStatusSummary
```

## <a name="optional-query-parameters"></a><span data-ttu-id="c4135-119">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="c4135-119">Optional query parameters</span></span>
<span data-ttu-id="c4135-120">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://docs.microsoft.com/en-us/graph/query-parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="c4135-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="c4135-121">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="c4135-121">Request headers</span></span>
|<span data-ttu-id="c4135-122">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="c4135-122">Header</span></span>|<span data-ttu-id="c4135-123">値</span><span class="sxs-lookup"><span data-stu-id="c4135-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c4135-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="c4135-124">Authorization</span></span>|<span data-ttu-id="c4135-125">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="c4135-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c4135-126">承諾</span><span class="sxs-lookup"><span data-stu-id="c4135-126">Accept</span></span>|<span data-ttu-id="c4135-127">application/json</span><span class="sxs-lookup"><span data-stu-id="c4135-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c4135-128">要求本文</span><span class="sxs-lookup"><span data-stu-id="c4135-128">Request body</span></span>
<span data-ttu-id="c4135-129">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="c4135-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c4135-130">応答</span><span class="sxs-lookup"><span data-stu-id="c4135-130">Response</span></span>
<span data-ttu-id="c4135-131">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [managedDeviceMobileAppConfigurationDeviceSummary](../resources/intune-apps-manageddevicemobileappconfigurationdevicesummary.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="c4135-131">If successful, this method returns a `200 OK` response code and [managedDeviceMobileAppConfigurationDeviceSummary](../resources/intune-apps-manageddevicemobileappconfigurationdevicesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c4135-132">例</span><span class="sxs-lookup"><span data-stu-id="c4135-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="c4135-133">要求</span><span class="sxs-lookup"><span data-stu-id="c4135-133">Request</span></span>
<span data-ttu-id="c4135-134">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="c4135-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/deviceStatusSummary
```

### <a name="response"></a><span data-ttu-id="c4135-135">応答</span><span class="sxs-lookup"><span data-stu-id="c4135-135">Response</span></span>
<span data-ttu-id="c4135-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="c4135-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 450

{
  "value": {
    "@odata.type": "#microsoft.graph.managedDeviceMobileAppConfigurationDeviceSummary",
    "id": "9997c455-c455-9997-55c4-979955c49799",
    "pendingCount": 12,
    "notApplicableCount": 2,
    "notApplicablePlatformCount": 10,
    "successCount": 12,
    "errorCount": 10,
    "failedCount": 11,
    "conflictCount": 13,
    "lastUpdateDateTime": "2016-12-31T23:58:21.6459442-08:00",
    "configurationVersion": 4
  }
}
```





