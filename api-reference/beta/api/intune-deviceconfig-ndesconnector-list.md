---
title: リスト ndesConnectors
description: NdesConnector オブジェクトのプロパティと関係を一覧表示します。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 52da3f3cf0936a13cc210c4be4092d24dd5b6317
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29402413"
---
# <a name="list-ndesconnectors"></a><span data-ttu-id="44c9c-103">リスト ndesConnectors</span><span class="sxs-lookup"><span data-stu-id="44c9c-103">List ndesConnectors</span></span>

> <span data-ttu-id="44c9c-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="44c9c-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="44c9c-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="44c9c-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="44c9c-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="44c9c-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="44c9c-107">[NdesConnector](../resources/intune-deviceconfig-ndesconnector.md)オブジェクトのプロパティと関係を一覧表示します。</span><span class="sxs-lookup"><span data-stu-id="44c9c-107">List properties and relationships of the [ndesConnector](../resources/intune-deviceconfig-ndesconnector.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="44c9c-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="44c9c-108">Prerequisites</span></span>
<span data-ttu-id="44c9c-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/concepts/permissions-reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="44c9c-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="44c9c-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="44c9c-111">Permission type</span></span>|<span data-ttu-id="44c9c-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="44c9c-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="44c9c-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="44c9c-113">Delegated (work or school account)</span></span>|<span data-ttu-id="44c9c-114">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="44c9c-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="44c9c-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="44c9c-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="44c9c-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="44c9c-116">Not supported.</span></span>|
|<span data-ttu-id="44c9c-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="44c9c-117">Application</span></span>|<span data-ttu-id="44c9c-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="44c9c-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="44c9c-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="44c9c-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/ndesConnectors
```

## <a name="request-headers"></a><span data-ttu-id="44c9c-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="44c9c-120">Request headers</span></span>
|<span data-ttu-id="44c9c-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="44c9c-121">Header</span></span>|<span data-ttu-id="44c9c-122">値</span><span class="sxs-lookup"><span data-stu-id="44c9c-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="44c9c-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="44c9c-123">Authorization</span></span>|<span data-ttu-id="44c9c-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="44c9c-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="44c9c-125">Accept</span><span class="sxs-lookup"><span data-stu-id="44c9c-125">Accept</span></span>|<span data-ttu-id="44c9c-126">application/json</span><span class="sxs-lookup"><span data-stu-id="44c9c-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="44c9c-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="44c9c-127">Request body</span></span>
<span data-ttu-id="44c9c-128">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="44c9c-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="44c9c-129">応答</span><span class="sxs-lookup"><span data-stu-id="44c9c-129">Response</span></span>
<span data-ttu-id="44c9c-130">かどうかは成功すると、このメソッドが返されます、`200 OK`応答コードおよび応答の本文に[ndesConnector](../resources/intune-deviceconfig-ndesconnector.md)オブジェクトのコレクションです。</span><span class="sxs-lookup"><span data-stu-id="44c9c-130">If successful, this method returns a `200 OK` response code and a collection of [ndesConnector](../resources/intune-deviceconfig-ndesconnector.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="44c9c-131">例</span><span class="sxs-lookup"><span data-stu-id="44c9c-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="44c9c-132">要求</span><span class="sxs-lookup"><span data-stu-id="44c9c-132">Request</span></span>
<span data-ttu-id="44c9c-133">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="44c9c-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/ndesConnectors
```

### <a name="response"></a><span data-ttu-id="44c9c-134">応答</span><span class="sxs-lookup"><span data-stu-id="44c9c-134">Response</span></span>
<span data-ttu-id="44c9c-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="44c9c-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 285

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.ndesConnector",
      "id": "e71fa706-a706-e71f-06a7-1fe706a71fe7",
      "lastConnectionDateTime": "2016-12-31T23:58:36.6670033-08:00",
      "state": "active",
      "displayName": "Display Name value"
    }
  ]
}
```




