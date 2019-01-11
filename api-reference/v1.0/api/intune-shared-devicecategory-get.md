---
title: deviceCategory の取得
description: deviceCategory オブジェクトのプロパティとリレーションシップを読み取ります。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: ba5fdee5ba2290b25bdf9485b94307f0f637649a
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27872192"
---
# <a name="get-devicecategory"></a><span data-ttu-id="dbbc4-103">deviceCategory の取得</span><span class="sxs-lookup"><span data-stu-id="dbbc4-103">Get deviceCategory</span></span>



> <span data-ttu-id="dbbc4-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="dbbc4-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="dbbc4-105">[deviceCategory](../resources/intune-shared-devicecategory.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="dbbc4-105">Read properties and relationships of the [deviceCategory](../resources/intune-shared-devicecategory.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="dbbc4-106">前提条件</span><span class="sxs-lookup"><span data-stu-id="dbbc4-106">Prerequisites</span></span>
<span data-ttu-id="dbbc4-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="dbbc4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="dbbc4-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="dbbc4-109">Permission type</span></span>|<span data-ttu-id="dbbc4-110">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="dbbc4-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="dbbc4-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="dbbc4-111">Delegated (work or school account)</span></span>||
| <span data-ttu-id="dbbc4-112">&nbsp; &nbsp; **デバイスの管理**</span><span class="sxs-lookup"><span data-stu-id="dbbc4-112">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="dbbc4-113">DeviceManagementManagedDevices.ReadWrite.All、DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="dbbc4-113">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
| <span data-ttu-id="dbbc4-114">&nbsp;&nbsp; **契約時**</span><span class="sxs-lookup"><span data-stu-id="dbbc4-114">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="dbbc4-115">DeviceManagementManagedDevices.ReadWrite.All、DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="dbbc4-115">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="dbbc4-116">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="dbbc4-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="dbbc4-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="dbbc4-117">Not supported.</span></span>|
|<span data-ttu-id="dbbc4-118">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="dbbc4-118">Application</span></span>|<span data-ttu-id="dbbc4-119">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="dbbc4-119">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="dbbc4-120">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="dbbc4-120">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/detectedApps/{detectedAppId}/managedDevices/{managedDeviceId}/deviceCategory
GET /deviceManagement/deviceCategories/{deviceCategoryId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="dbbc4-121">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="dbbc4-121">Optional query parameters</span></span>
<span data-ttu-id="dbbc4-122">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="dbbc4-122">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="dbbc4-123">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="dbbc4-123">Request headers</span></span>
|<span data-ttu-id="dbbc4-124">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="dbbc4-124">Header</span></span>|<span data-ttu-id="dbbc4-125">値</span><span class="sxs-lookup"><span data-stu-id="dbbc4-125">Value</span></span>|
|:---|:---|
|<span data-ttu-id="dbbc4-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="dbbc4-126">Authorization</span></span>|<span data-ttu-id="dbbc4-127">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="dbbc4-127">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="dbbc4-128">Accept</span><span class="sxs-lookup"><span data-stu-id="dbbc4-128">Accept</span></span>|<span data-ttu-id="dbbc4-129">application/json</span><span class="sxs-lookup"><span data-stu-id="dbbc4-129">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="dbbc4-130">要求本文</span><span class="sxs-lookup"><span data-stu-id="dbbc4-130">Request body</span></span>
<span data-ttu-id="dbbc4-131">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="dbbc4-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="dbbc4-132">応答</span><span class="sxs-lookup"><span data-stu-id="dbbc4-132">Response</span></span>
<span data-ttu-id="dbbc4-133">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [deviceCategory](../resources/intune-shared-devicecategory.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="dbbc4-133">If successful, this method returns a `200 OK` response code and [deviceCategory](../resources/intune-shared-devicecategory.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="dbbc4-134">例</span><span class="sxs-lookup"><span data-stu-id="dbbc4-134">Example</span></span>

### <a name="request"></a><span data-ttu-id="dbbc4-135">要求</span><span class="sxs-lookup"><span data-stu-id="dbbc4-135">Request</span></span>
<span data-ttu-id="dbbc4-136">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="dbbc4-136">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/detectedApps/{detectedAppId}/managedDevices/{managedDeviceId}/deviceCategory
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceCategories/{deviceCategoryId}

```

### <a name="response"></a><span data-ttu-id="dbbc4-137">応答</span><span class="sxs-lookup"><span data-stu-id="dbbc4-137">Response</span></span>
<span data-ttu-id="dbbc4-138">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="dbbc4-138">Here is an example of the response.</span></span> <span data-ttu-id="dbbc4-139">注: 簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。</span><span class="sxs-lookup"><span data-stu-id="dbbc4-139">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="dbbc4-140">実際の呼び出しから返されるプロパティは、コンテキストによって異なります。</span><span class="sxs-lookup"><span data-stu-id="dbbc4-140">Properties returned from an actual call vary according to context.</span></span>

``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 211

{
  "value": {
    "@odata.type": "#microsoft.graph.deviceCategory",
    "id": "f881b841-b841-f881-41b8-81f841b881f8",
    "displayName": "Display Name value",
    "description": "Description value"
  }
}
```



