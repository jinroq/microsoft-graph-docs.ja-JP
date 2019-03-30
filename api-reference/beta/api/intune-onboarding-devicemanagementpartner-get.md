---
title: Get deviceManagementPartner
description: deviceManagementPartner オブジェクトのプロパティとリレーションシップを読み取ります。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 74ce9e44be6a959ff2b2f28b57d74e83922cc90b
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/29/2019
ms.locfileid: "30987954"
---
# <a name="get-devicemanagementpartner"></a><span data-ttu-id="c7c39-103">Get deviceManagementPartner</span><span class="sxs-lookup"><span data-stu-id="c7c39-103">Get deviceManagementPartner</span></span>

> <span data-ttu-id="c7c39-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c7c39-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c7c39-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="c7c39-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c7c39-106">[deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="c7c39-106">Read properties and relationships of the [deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c7c39-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="c7c39-107">Prerequisites</span></span>
<span data-ttu-id="c7c39-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="c7c39-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c7c39-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="c7c39-110">Permission type</span></span>|<span data-ttu-id="c7c39-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="c7c39-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c7c39-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="c7c39-112">Delegated (work or school account)</span></span>|<span data-ttu-id="c7c39-113">DeviceManagementServiceConfig.ReadWrite.All、DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="c7c39-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="c7c39-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="c7c39-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c7c39-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c7c39-115">Not supported.</span></span>|
|<span data-ttu-id="c7c39-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="c7c39-116">Application</span></span>|<span data-ttu-id="c7c39-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c7c39-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c7c39-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="c7c39-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceManagementPartners/{deviceManagementPartnerId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="c7c39-119">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="c7c39-119">Optional query parameters</span></span>
<span data-ttu-id="c7c39-120">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://docs.microsoft.com/en-us/graph/query-parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="c7c39-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="c7c39-121">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="c7c39-121">Request headers</span></span>
|<span data-ttu-id="c7c39-122">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="c7c39-122">Header</span></span>|<span data-ttu-id="c7c39-123">値</span><span class="sxs-lookup"><span data-stu-id="c7c39-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c7c39-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="c7c39-124">Authorization</span></span>|<span data-ttu-id="c7c39-125">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="c7c39-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c7c39-126">承諾</span><span class="sxs-lookup"><span data-stu-id="c7c39-126">Accept</span></span>|<span data-ttu-id="c7c39-127">application/json</span><span class="sxs-lookup"><span data-stu-id="c7c39-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c7c39-128">要求本文</span><span class="sxs-lookup"><span data-stu-id="c7c39-128">Request body</span></span>
<span data-ttu-id="c7c39-129">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="c7c39-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c7c39-130">応答</span><span class="sxs-lookup"><span data-stu-id="c7c39-130">Response</span></span>
<span data-ttu-id="c7c39-131">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="c7c39-131">If successful, this method returns a `200 OK` response code and [deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c7c39-132">例</span><span class="sxs-lookup"><span data-stu-id="c7c39-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="c7c39-133">要求</span><span class="sxs-lookup"><span data-stu-id="c7c39-133">Request</span></span>
<span data-ttu-id="c7c39-134">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="c7c39-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceManagementPartners/{deviceManagementPartnerId}
```

### <a name="response"></a><span data-ttu-id="c7c39-135">応答</span><span class="sxs-lookup"><span data-stu-id="c7c39-135">Response</span></span>
<span data-ttu-id="c7c39-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="c7c39-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 756

{
  "value": {
    "@odata.type": "#microsoft.graph.deviceManagementPartner",
    "id": "d21e377a-377a-d21e-7a37-1ed27a371ed2",
    "lastHeartbeatDateTime": "2016-12-31T23:59:37.9174975-08:00",
    "partnerState": "unavailable",
    "partnerAppType": "singleTenantApp",
    "singleTenantAppId": "Single Tenant App Id value",
    "displayName": "Display Name value",
    "isConfigured": true,
    "whenPartnerDevicesWillBeRemoved": "2017-01-01T00:00:34.890321-08:00",
    "whenPartnerDevicesWillBeMarkedAsNonCompliant": "2017-01-01T00:02:38.9066046-08:00",
    "whenPartnerDevicesWillBeRemovedDateTime": "2016-12-31T23:56:38.2655023-08:00",
    "whenPartnerDevicesWillBeMarkedAsNonCompliantDateTime": "2016-12-31T23:58:42.2131231-08:00"
  }
}
```




