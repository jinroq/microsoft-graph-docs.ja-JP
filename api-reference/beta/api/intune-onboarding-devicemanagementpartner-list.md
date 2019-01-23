---
title: deviceManagementPartners のリスト
description: deviceManagementPartner オブジェクトのプロパティとリレーションシップをリストします。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: cc57c455ae4464ee94e82b0b8ab51b026fdfa129
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29418324"
---
# <a name="list-devicemanagementpartners"></a><span data-ttu-id="fe802-103">deviceManagementPartners のリスト</span><span class="sxs-lookup"><span data-stu-id="fe802-103">List deviceManagementPartners</span></span>

> <span data-ttu-id="fe802-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="fe802-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="fe802-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="fe802-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="fe802-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="fe802-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fe802-107">[deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="fe802-107">List properties and relationships of the [deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="fe802-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="fe802-108">Prerequisites</span></span>
<span data-ttu-id="fe802-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/concepts/permissions-reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="fe802-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="fe802-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="fe802-111">Permission type</span></span>|<span data-ttu-id="fe802-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="fe802-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="fe802-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="fe802-113">Delegated (work or school account)</span></span>|<span data-ttu-id="fe802-114">DeviceManagementServiceConfig.ReadWrite.All、DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="fe802-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="fe802-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="fe802-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fe802-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="fe802-116">Not supported.</span></span>|
|<span data-ttu-id="fe802-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="fe802-117">Application</span></span>|<span data-ttu-id="fe802-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="fe802-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="fe802-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="fe802-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceManagementPartners
```

## <a name="request-headers"></a><span data-ttu-id="fe802-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="fe802-120">Request headers</span></span>
|<span data-ttu-id="fe802-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="fe802-121">Header</span></span>|<span data-ttu-id="fe802-122">値</span><span class="sxs-lookup"><span data-stu-id="fe802-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="fe802-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="fe802-123">Authorization</span></span>|<span data-ttu-id="fe802-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="fe802-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="fe802-125">Accept</span><span class="sxs-lookup"><span data-stu-id="fe802-125">Accept</span></span>|<span data-ttu-id="fe802-126">application/json</span><span class="sxs-lookup"><span data-stu-id="fe802-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="fe802-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="fe802-127">Request body</span></span>
<span data-ttu-id="fe802-128">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="fe802-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="fe802-129">応答</span><span class="sxs-lookup"><span data-stu-id="fe802-129">Response</span></span>
<span data-ttu-id="fe802-130">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md) オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="fe802-130">If successful, this method returns a `200 OK` response code and a collection of [deviceManagementPartner](../resources/intune-onboarding-devicemanagementpartner.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fe802-131">例</span><span class="sxs-lookup"><span data-stu-id="fe802-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="fe802-132">要求</span><span class="sxs-lookup"><span data-stu-id="fe802-132">Request</span></span>
<span data-ttu-id="fe802-133">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="fe802-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceManagementPartners
```

### <a name="response"></a><span data-ttu-id="fe802-134">応答</span><span class="sxs-lookup"><span data-stu-id="fe802-134">Response</span></span>
<span data-ttu-id="fe802-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="fe802-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




