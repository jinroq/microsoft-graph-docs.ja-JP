---
title: ndesconnector の取得
description: ndesconnector オブジェクトのプロパティとリレーションシップを読み取ります。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: b9c4dfa2a808b382d6178da7338b861bb6443168
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/11/2019
ms.locfileid: "31806371"
---
# <a name="get-ndesconnector"></a><span data-ttu-id="650ec-103">ndesconnector の取得</span><span class="sxs-lookup"><span data-stu-id="650ec-103">Get ndesConnector</span></span>

> <span data-ttu-id="650ec-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="650ec-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="650ec-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="650ec-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="650ec-106">[ndesconnector](../resources/intune-deviceconfig-ndesconnector.md)オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="650ec-106">Read properties and relationships of the [ndesConnector](../resources/intune-deviceconfig-ndesconnector.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="650ec-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="650ec-107">Prerequisites</span></span>
<span data-ttu-id="650ec-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="650ec-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="650ec-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="650ec-110">Permission type</span></span>|<span data-ttu-id="650ec-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="650ec-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="650ec-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="650ec-112">Delegated (work or school account)</span></span>|<span data-ttu-id="650ec-113">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="650ec-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="650ec-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="650ec-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="650ec-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="650ec-115">Not supported.</span></span>|
|<span data-ttu-id="650ec-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="650ec-116">Application</span></span>|<span data-ttu-id="650ec-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="650ec-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="650ec-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="650ec-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/ndesConnectors/{ndesConnectorId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="650ec-119">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="650ec-119">Optional query parameters</span></span>
<span data-ttu-id="650ec-120">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://docs.microsoft.com/en-us/graph/query-parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="650ec-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="650ec-121">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="650ec-121">Request headers</span></span>
|<span data-ttu-id="650ec-122">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="650ec-122">Header</span></span>|<span data-ttu-id="650ec-123">値</span><span class="sxs-lookup"><span data-stu-id="650ec-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="650ec-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="650ec-124">Authorization</span></span>|<span data-ttu-id="650ec-125">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="650ec-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="650ec-126">承諾</span><span class="sxs-lookup"><span data-stu-id="650ec-126">Accept</span></span>|<span data-ttu-id="650ec-127">application/json</span><span class="sxs-lookup"><span data-stu-id="650ec-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="650ec-128">要求本文</span><span class="sxs-lookup"><span data-stu-id="650ec-128">Request body</span></span>
<span data-ttu-id="650ec-129">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="650ec-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="650ec-130">応答</span><span class="sxs-lookup"><span data-stu-id="650ec-130">Response</span></span>
<span data-ttu-id="650ec-131">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で[ndesconnector](../resources/intune-deviceconfig-ndesconnector.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="650ec-131">If successful, this method returns a `200 OK` response code and [ndesConnector](../resources/intune-deviceconfig-ndesconnector.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="650ec-132">例</span><span class="sxs-lookup"><span data-stu-id="650ec-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="650ec-133">要求</span><span class="sxs-lookup"><span data-stu-id="650ec-133">Request</span></span>
<span data-ttu-id="650ec-134">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="650ec-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/ndesConnectors/{ndesConnectorId}
```

### <a name="response"></a><span data-ttu-id="650ec-135">応答</span><span class="sxs-lookup"><span data-stu-id="650ec-135">Response</span></span>
<span data-ttu-id="650ec-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="650ec-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 261

{
  "value": {
    "@odata.type": "#microsoft.graph.ndesConnector",
    "id": "e71fa706-a706-e71f-06a7-1fe706a71fe7",
    "lastConnectionDateTime": "2016-12-31T23:58:36.6670033-08:00",
    "state": "active",
    "displayName": "Display Name value"
  }
}
```





