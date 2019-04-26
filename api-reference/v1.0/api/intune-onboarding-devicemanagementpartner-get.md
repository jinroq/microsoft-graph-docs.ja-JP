---
title: Get deviceManagementPartner
description: deviceManagementPartner オブジェクトのプロパティとリレーションシップを読み取ります。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: fd3784e824e8696cbd901a9f60958fa4f57a82f1
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32561566"
---
# <a name="get-devicemanagementpartner"></a><span data-ttu-id="300bd-103">Get deviceManagementPartner</span><span class="sxs-lookup"><span data-stu-id="300bd-103">Get deviceManagementPartner</span></span>

> <span data-ttu-id="300bd-104">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="300bd-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="300bd-105">[deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="300bd-105">Read properties and relationships of the [deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="300bd-106">前提条件</span><span class="sxs-lookup"><span data-stu-id="300bd-106">Prerequisites</span></span>
<span data-ttu-id="300bd-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="300bd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="300bd-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="300bd-109">Permission type</span></span>|<span data-ttu-id="300bd-110">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="300bd-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="300bd-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="300bd-111">Delegated (work or school account)</span></span>|<span data-ttu-id="300bd-112">DeviceManagementServiceConfig.ReadWrite.All、DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="300bd-112">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="300bd-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="300bd-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="300bd-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="300bd-114">Not supported.</span></span>|
|<span data-ttu-id="300bd-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="300bd-115">Application</span></span>|<span data-ttu-id="300bd-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="300bd-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="300bd-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="300bd-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceManagementPartners/{deviceManagementPartnerId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="300bd-118">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="300bd-118">Optional query parameters</span></span>
<span data-ttu-id="300bd-119">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://docs.microsoft.com/en-us/graph/query-parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="300bd-119">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="300bd-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="300bd-120">Request headers</span></span>
|<span data-ttu-id="300bd-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="300bd-121">Header</span></span>|<span data-ttu-id="300bd-122">値</span><span class="sxs-lookup"><span data-stu-id="300bd-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="300bd-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="300bd-123">Authorization</span></span>|<span data-ttu-id="300bd-124">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="300bd-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="300bd-125">承諾</span><span class="sxs-lookup"><span data-stu-id="300bd-125">Accept</span></span>|<span data-ttu-id="300bd-126">application/json</span><span class="sxs-lookup"><span data-stu-id="300bd-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="300bd-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="300bd-127">Request body</span></span>
<span data-ttu-id="300bd-128">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="300bd-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="300bd-129">応答</span><span class="sxs-lookup"><span data-stu-id="300bd-129">Response</span></span>
<span data-ttu-id="300bd-130">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="300bd-130">If successful, this method returns a `200 OK` response code and [deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="300bd-131">例</span><span class="sxs-lookup"><span data-stu-id="300bd-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="300bd-132">要求</span><span class="sxs-lookup"><span data-stu-id="300bd-132">Request</span></span>
<span data-ttu-id="300bd-133">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="300bd-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceManagementPartners/{deviceManagementPartnerId}
```

### <a name="response"></a><span data-ttu-id="300bd-134">応答</span><span class="sxs-lookup"><span data-stu-id="300bd-134">Response</span></span>
<span data-ttu-id="300bd-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="300bd-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 590

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
    "whenPartnerDevicesWillBeRemovedDateTime": "2016-12-31T23:56:38.2655023-08:00",
    "whenPartnerDevicesWillBeMarkedAsNonCompliantDateTime": "2016-12-31T23:58:42.2131231-08:00"
  }
}
```



