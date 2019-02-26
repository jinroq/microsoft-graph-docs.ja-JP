---
title: deviceCategory の取得
description: deviceCategory オブジェクトのプロパティとリレーションシップを読み取ります。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: b62523d4a17571c0ff6931b8ee462f21b4a1daa4
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/21/2019
ms.locfileid: "30174539"
---
# <a name="get-devicecategory"></a><span data-ttu-id="37390-103">deviceCategory の取得</span><span class="sxs-lookup"><span data-stu-id="37390-103">Get deviceCategory</span></span>

> <span data-ttu-id="37390-104">**重要:** Microsoft Graph の/ベータ版の api は変更される可能性があります。</span><span class="sxs-lookup"><span data-stu-id="37390-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="37390-105">実稼働アプリケーションでは、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="37390-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="37390-106">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="37390-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="37390-107">[deviceCategory](../resources/intune-shared-devicecategory.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="37390-107">Read properties and relationships of the [deviceCategory](../resources/intune-shared-devicecategory.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="37390-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="37390-108">Prerequisites</span></span>

<span data-ttu-id="37390-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/concepts/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="37390-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference).</span></span>

|<span data-ttu-id="37390-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="37390-111">Permission type</span></span>|<span data-ttu-id="37390-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="37390-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="37390-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="37390-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="37390-114">&nbsp; &nbsp; **デバイスの管理**</span><span class="sxs-lookup"><span data-stu-id="37390-114">&nbsp; &nbsp; **Device management**</span></span> | <span data-ttu-id="37390-115">DeviceManagementManagedDevices.ReadWrite.All、DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="37390-115">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
| <span data-ttu-id="37390-116">&nbsp; &nbsp; **オンボーディング**</span><span class="sxs-lookup"><span data-stu-id="37390-116">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="37390-117">DeviceManagementManagedDevices.ReadWrite.All、DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="37390-117">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="37390-118">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="37390-118">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="37390-119">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="37390-119">Not supported.</span></span>|
|<span data-ttu-id="37390-120">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="37390-120">Application</span></span>|<span data-ttu-id="37390-121">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="37390-121">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="37390-122">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="37390-122">HTTP Request</span></span>

<span data-ttu-id="37390-123">**デバイスの管理**</span><span class="sxs-lookup"><span data-stu-id="37390-123">**Device management**</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceCategories/{deviceCategoryId}
```

<span data-ttu-id="37390-124">**オンボーディング**</span><span class="sxs-lookup"><span data-stu-id="37390-124">**Onboarding**</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/deviceCategory
```

## <a name="optional-query-parameters"></a><span data-ttu-id="37390-125">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="37390-125">Optional query parameters</span></span>

<span data-ttu-id="37390-126">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="37390-126">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="37390-127">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="37390-127">Request headers</span></span>

|<span data-ttu-id="37390-128">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="37390-128">Header</span></span>|<span data-ttu-id="37390-129">値</span><span class="sxs-lookup"><span data-stu-id="37390-129">Value</span></span>|
|:---|:---|
|<span data-ttu-id="37390-130">Authorization</span><span class="sxs-lookup"><span data-stu-id="37390-130">Authorization</span></span>|<span data-ttu-id="37390-131">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="37390-131">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="37390-132">承諾</span><span class="sxs-lookup"><span data-stu-id="37390-132">Accept</span></span>|<span data-ttu-id="37390-133">application/json</span><span class="sxs-lookup"><span data-stu-id="37390-133">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="37390-134">要求本文</span><span class="sxs-lookup"><span data-stu-id="37390-134">Request body</span></span>

<span data-ttu-id="37390-135">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="37390-135">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="37390-136">応答</span><span class="sxs-lookup"><span data-stu-id="37390-136">Response</span></span>

<span data-ttu-id="37390-137">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [deviceCategory](../resources/intune-shared-devicecategory.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="37390-137">If successful, this method returns a `200 OK` response code and [deviceCategory](../resources/intune-shared-devicecategory.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="37390-138">例</span><span class="sxs-lookup"><span data-stu-id="37390-138">Example</span></span>

### <a name="request"></a><span data-ttu-id="37390-139">要求</span><span class="sxs-lookup"><span data-stu-id="37390-139">Request</span></span>

<span data-ttu-id="37390-140">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="37390-140">Here is are examples of the request.</span></span>

``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/deviceCategory
GET https://graph.microsoft.com/beta/deviceManagement/deviceCategories/{deviceCategoryId}
```

### <a name="response"></a><span data-ttu-id="37390-141">応答</span><span class="sxs-lookup"><span data-stu-id="37390-141">Response</span></span>

<span data-ttu-id="37390-142">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="37390-142">Here is an example of the response.</span></span> <span data-ttu-id="37390-143">注: 簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。</span><span class="sxs-lookup"><span data-stu-id="37390-143">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="37390-144">実際の呼び出しから返されるプロパティは、コンテキストに応じて異なります。</span><span class="sxs-lookup"><span data-stu-id="37390-144">Properties returned from an actual call vary according to context.</span></span>

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



