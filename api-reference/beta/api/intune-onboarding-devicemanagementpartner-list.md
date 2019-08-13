---
title: deviceManagementPartners のリスト
description: deviceManagementPartner オブジェクトのプロパティとリレーションシップをリストします。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 979e54d4da10d6dbd4a3cb3c7bb205f7d9c211b0
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36352659"
---
# <a name="list-devicemanagementpartners"></a><span data-ttu-id="0d505-103">deviceManagementPartners のリスト</span><span class="sxs-lookup"><span data-stu-id="0d505-103">List deviceManagementPartners</span></span>

> <span data-ttu-id="0d505-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="0d505-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0d505-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="0d505-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0d505-106">[deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="0d505-106">List properties and relationships of the [deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="0d505-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="0d505-107">Prerequisites</span></span>
<span data-ttu-id="0d505-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="0d505-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0d505-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="0d505-110">Permission type</span></span>|<span data-ttu-id="0d505-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="0d505-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0d505-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="0d505-112">Delegated (work or school account)</span></span>|<span data-ttu-id="0d505-113">DeviceManagementServiceConfig.ReadWrite.All、DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="0d505-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="0d505-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="0d505-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0d505-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="0d505-115">Not supported.</span></span>|
|<span data-ttu-id="0d505-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="0d505-116">Application</span></span>|<span data-ttu-id="0d505-117">DeviceManagementServiceConfig.ReadWrite.All、DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="0d505-117">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="0d505-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="0d505-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceManagementPartners
```

## <a name="request-headers"></a><span data-ttu-id="0d505-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="0d505-119">Request headers</span></span>
|<span data-ttu-id="0d505-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="0d505-120">Header</span></span>|<span data-ttu-id="0d505-121">値</span><span class="sxs-lookup"><span data-stu-id="0d505-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0d505-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="0d505-122">Authorization</span></span>|<span data-ttu-id="0d505-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="0d505-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0d505-124">承諾</span><span class="sxs-lookup"><span data-stu-id="0d505-124">Accept</span></span>|<span data-ttu-id="0d505-125">application/json</span><span class="sxs-lookup"><span data-stu-id="0d505-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0d505-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="0d505-126">Request body</span></span>
<span data-ttu-id="0d505-127">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="0d505-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0d505-128">応答</span><span class="sxs-lookup"><span data-stu-id="0d505-128">Response</span></span>
<span data-ttu-id="0d505-129">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md) オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="0d505-129">If successful, this method returns a `200 OK` response code and a collection of [deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0d505-130">例</span><span class="sxs-lookup"><span data-stu-id="0d505-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="0d505-131">要求</span><span class="sxs-lookup"><span data-stu-id="0d505-131">Request</span></span>
<span data-ttu-id="0d505-132">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="0d505-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceManagementPartners
```

### <a name="response"></a><span data-ttu-id="0d505-133">応答</span><span class="sxs-lookup"><span data-stu-id="0d505-133">Response</span></span>
<span data-ttu-id="0d505-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="0d505-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 794

{
  "value": [
    {
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
  ]
}
```






