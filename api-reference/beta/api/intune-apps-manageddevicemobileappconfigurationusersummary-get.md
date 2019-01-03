---
title: Get managedDeviceMobileAppConfigurationUserSummary
description: managedDeviceMobileAppConfigurationUserSummary オブジェクトのプロパティとリレーションシップを読み取ります。
author: tfitzmac
ms.openlocfilehash: 06b4972b129c18f8ddda6c1cd9335923517db37e
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27311432"
---
# <a name="get-manageddevicemobileappconfigurationusersummary"></a><span data-ttu-id="abfca-103">Get managedDeviceMobileAppConfigurationUserSummary</span><span class="sxs-lookup"><span data-stu-id="abfca-103">Get managedDeviceMobileAppConfigurationUserSummary</span></span>

> <span data-ttu-id="abfca-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="abfca-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="abfca-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="abfca-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="abfca-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="abfca-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="abfca-107">[managedDeviceMobileAppConfigurationUserSummary](../resources/intune-apps-manageddevicemobileappconfigurationusersummary.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="abfca-107">Read properties and relationships of the [managedDeviceMobileAppConfigurationUserSummary](../resources/intune-apps-manageddevicemobileappconfigurationusersummary.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="abfca-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="abfca-108">Prerequisites</span></span>
<span data-ttu-id="abfca-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="abfca-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="abfca-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="abfca-111">Permission type</span></span>|<span data-ttu-id="abfca-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="abfca-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="abfca-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="abfca-113">Delegated (work or school account)</span></span>|<span data-ttu-id="abfca-114">DeviceManagementApps.ReadWrite.All、DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="abfca-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="abfca-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="abfca-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="abfca-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="abfca-116">Not supported.</span></span>|
|<span data-ttu-id="abfca-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="abfca-117">Application</span></span>|<span data-ttu-id="abfca-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="abfca-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="abfca-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="abfca-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/userStatusSummary
```

## <a name="optional-query-parameters"></a><span data-ttu-id="abfca-120">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="abfca-120">Optional query parameters</span></span>
<span data-ttu-id="abfca-121">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="abfca-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="abfca-122">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="abfca-122">Request headers</span></span>
|<span data-ttu-id="abfca-123">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="abfca-123">Header</span></span>|<span data-ttu-id="abfca-124">値</span><span class="sxs-lookup"><span data-stu-id="abfca-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="abfca-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="abfca-125">Authorization</span></span>|<span data-ttu-id="abfca-126">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="abfca-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="abfca-127">Accept</span><span class="sxs-lookup"><span data-stu-id="abfca-127">Accept</span></span>|<span data-ttu-id="abfca-128">application/json</span><span class="sxs-lookup"><span data-stu-id="abfca-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="abfca-129">要求本文</span><span class="sxs-lookup"><span data-stu-id="abfca-129">Request body</span></span>
<span data-ttu-id="abfca-130">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="abfca-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="abfca-131">応答</span><span class="sxs-lookup"><span data-stu-id="abfca-131">Response</span></span>
<span data-ttu-id="abfca-132">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [managedDeviceMobileAppConfigurationUserSummary](../resources/intune-apps-manageddevicemobileappconfigurationusersummary.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="abfca-132">If successful, this method returns a `200 OK` response code and [managedDeviceMobileAppConfigurationUserSummary](../resources/intune-apps-manageddevicemobileappconfigurationusersummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="abfca-133">例</span><span class="sxs-lookup"><span data-stu-id="abfca-133">Example</span></span>
### <a name="request"></a><span data-ttu-id="abfca-134">要求</span><span class="sxs-lookup"><span data-stu-id="abfca-134">Request</span></span>
<span data-ttu-id="abfca-135">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="abfca-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/userStatusSummary
```

### <a name="response"></a><span data-ttu-id="abfca-136">応答</span><span class="sxs-lookup"><span data-stu-id="abfca-136">Response</span></span>
<span data-ttu-id="abfca-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="abfca-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




