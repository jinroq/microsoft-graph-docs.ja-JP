---
title: Get managedDeviceMobileAppConfigurationUserSummary
description: managedDeviceMobileAppConfigurationUserSummary オブジェクトのプロパティとリレーションシップを読み取ります。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 03f7d2e1ac38503c4ae6123ecd0a84ddd8712f23
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35961442"
---
# <a name="get-manageddevicemobileappconfigurationusersummary"></a><span data-ttu-id="d05e2-103">Get managedDeviceMobileAppConfigurationUserSummary</span><span class="sxs-lookup"><span data-stu-id="d05e2-103">Get managedDeviceMobileAppConfigurationUserSummary</span></span>

> <span data-ttu-id="d05e2-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d05e2-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d05e2-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="d05e2-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d05e2-106">[managedDeviceMobileAppConfigurationUserSummary](../resources/intune-apps-manageddevicemobileappconfigurationusersummary.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="d05e2-106">Read properties and relationships of the [managedDeviceMobileAppConfigurationUserSummary](../resources/intune-apps-manageddevicemobileappconfigurationusersummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d05e2-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="d05e2-107">Prerequisites</span></span>
<span data-ttu-id="d05e2-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="d05e2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d05e2-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="d05e2-110">Permission type</span></span>|<span data-ttu-id="d05e2-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="d05e2-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d05e2-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="d05e2-112">Delegated (work or school account)</span></span>|<span data-ttu-id="d05e2-113">DeviceManagementApps.ReadWrite.All、DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="d05e2-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="d05e2-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="d05e2-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d05e2-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d05e2-115">Not supported.</span></span>|
|<span data-ttu-id="d05e2-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="d05e2-116">Application</span></span>|<span data-ttu-id="d05e2-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d05e2-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d05e2-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="d05e2-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/userStatusSummary
```

## <a name="optional-query-parameters"></a><span data-ttu-id="d05e2-119">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="d05e2-119">Optional query parameters</span></span>
<span data-ttu-id="d05e2-120">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://docs.microsoft.com/en-us/graph/query-parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="d05e2-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="d05e2-121">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="d05e2-121">Request headers</span></span>
|<span data-ttu-id="d05e2-122">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="d05e2-122">Header</span></span>|<span data-ttu-id="d05e2-123">値</span><span class="sxs-lookup"><span data-stu-id="d05e2-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d05e2-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="d05e2-124">Authorization</span></span>|<span data-ttu-id="d05e2-125">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="d05e2-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d05e2-126">承諾</span><span class="sxs-lookup"><span data-stu-id="d05e2-126">Accept</span></span>|<span data-ttu-id="d05e2-127">application/json</span><span class="sxs-lookup"><span data-stu-id="d05e2-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d05e2-128">要求本文</span><span class="sxs-lookup"><span data-stu-id="d05e2-128">Request body</span></span>
<span data-ttu-id="d05e2-129">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="d05e2-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d05e2-130">応答</span><span class="sxs-lookup"><span data-stu-id="d05e2-130">Response</span></span>
<span data-ttu-id="d05e2-131">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [managedDeviceMobileAppConfigurationUserSummary](../resources/intune-apps-manageddevicemobileappconfigurationusersummary.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="d05e2-131">If successful, this method returns a `200 OK` response code and [managedDeviceMobileAppConfigurationUserSummary](../resources/intune-apps-manageddevicemobileappconfigurationusersummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d05e2-132">例</span><span class="sxs-lookup"><span data-stu-id="d05e2-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="d05e2-133">要求</span><span class="sxs-lookup"><span data-stu-id="d05e2-133">Request</span></span>
<span data-ttu-id="d05e2-134">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="d05e2-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/userStatusSummary
```

### <a name="response"></a><span data-ttu-id="d05e2-135">応答</span><span class="sxs-lookup"><span data-stu-id="d05e2-135">Response</span></span>
<span data-ttu-id="d05e2-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="d05e2-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 409

{
  "value": {
    "@odata.type": "#microsoft.graph.managedDeviceMobileAppConfigurationUserSummary",
    "id": "7b953742-3742-7b95-4237-957b4237957b",
    "pendingCount": 12,
    "notApplicableCount": 2,
    "successCount": 12,
    "errorCount": 10,
    "failedCount": 11,
    "conflictCount": 13,
    "lastUpdateDateTime": "2016-12-31T23:58:21.6459442-08:00",
    "configurationVersion": 4
  }
}
```





