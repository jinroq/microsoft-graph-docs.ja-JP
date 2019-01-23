---
title: GroupPolicyConfiguration を取得します。
description: GroupPolicyConfiguration オブジェクトのプロパティと関係を参照してください。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 1d2581d670a8d2bd54ba0294fe8966f117eaacd5
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29431595"
---
# <a name="get-grouppolicyconfiguration"></a><span data-ttu-id="73bd8-103">GroupPolicyConfiguration を取得します。</span><span class="sxs-lookup"><span data-stu-id="73bd8-103">Get groupPolicyConfiguration</span></span>

> <span data-ttu-id="73bd8-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="73bd8-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="73bd8-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="73bd8-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="73bd8-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="73bd8-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="73bd8-107">[GroupPolicyConfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md)オブジェクトのプロパティと関係を参照してください。</span><span class="sxs-lookup"><span data-stu-id="73bd8-107">Read properties and relationships of the [groupPolicyConfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="73bd8-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="73bd8-108">Prerequisites</span></span>
<span data-ttu-id="73bd8-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/concepts/permissions-reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="73bd8-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="73bd8-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="73bd8-111">Permission type</span></span>|<span data-ttu-id="73bd8-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="73bd8-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="73bd8-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="73bd8-113">Delegated (work or school account)</span></span>|<span data-ttu-id="73bd8-114">DeviceManagementServiceConfig.ReadWrite.All、DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="73bd8-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="73bd8-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="73bd8-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="73bd8-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="73bd8-116">Not supported.</span></span>|
|<span data-ttu-id="73bd8-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="73bd8-117">Application</span></span>|<span data-ttu-id="73bd8-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="73bd8-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="73bd8-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="73bd8-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="73bd8-120">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="73bd8-120">Optional query parameters</span></span>
<span data-ttu-id="73bd8-121">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://docs.microsoft.com/en-us/graph/query-parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="73bd8-121">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="73bd8-122">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="73bd8-122">Request headers</span></span>
|<span data-ttu-id="73bd8-123">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="73bd8-123">Header</span></span>|<span data-ttu-id="73bd8-124">値</span><span class="sxs-lookup"><span data-stu-id="73bd8-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="73bd8-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="73bd8-125">Authorization</span></span>|<span data-ttu-id="73bd8-126">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="73bd8-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="73bd8-127">Accept</span><span class="sxs-lookup"><span data-stu-id="73bd8-127">Accept</span></span>|<span data-ttu-id="73bd8-128">application/json</span><span class="sxs-lookup"><span data-stu-id="73bd8-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="73bd8-129">要求本文</span><span class="sxs-lookup"><span data-stu-id="73bd8-129">Request body</span></span>
<span data-ttu-id="73bd8-130">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="73bd8-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="73bd8-131">応答</span><span class="sxs-lookup"><span data-stu-id="73bd8-131">Response</span></span>
<span data-ttu-id="73bd8-132">かどうかは成功すると、このメソッドが返されます、 `200 OK` 、応答の本体で応答コードと[groupPolicyConfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md)のオブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="73bd8-132">If successful, this method returns a `200 OK` response code and [groupPolicyConfiguration](../resources/intune-grouppolicy-grouppolicyconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="73bd8-133">例</span><span class="sxs-lookup"><span data-stu-id="73bd8-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="73bd8-134">要求</span><span class="sxs-lookup"><span data-stu-id="73bd8-134">Request</span></span>
<span data-ttu-id="73bd8-135">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="73bd8-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}
```

### <a name="response"></a><span data-ttu-id="73bd8-136">応答</span><span class="sxs-lookup"><span data-stu-id="73bd8-136">Response</span></span>
<span data-ttu-id="73bd8-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="73bd8-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 348

{
  "value": {
    "@odata.type": "#microsoft.graph.groupPolicyConfiguration",
    "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
    "displayName": "Display Name value",
    "description": "Description value",
    "id": "27b935ec-35ec-27b9-ec35-b927ec35b927",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00"
  }
}
```




