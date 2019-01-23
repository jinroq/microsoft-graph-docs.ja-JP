---
title: リスト embeddedSIMDeviceStates
description: EmbeddedSIMDeviceState オブジェクトのプロパティと関係を一覧表示します。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 05874888c28b3288e417a1f1212a1ab149b85ff7
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29417638"
---
# <a name="list-embeddedsimdevicestates"></a><span data-ttu-id="14484-103">リスト embeddedSIMDeviceStates</span><span class="sxs-lookup"><span data-stu-id="14484-103">List embeddedSIMDeviceStates</span></span>

> <span data-ttu-id="14484-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="14484-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="14484-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="14484-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="14484-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="14484-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="14484-107">[EmbeddedSIMDeviceState](../resources/intune-esim-embeddedsimdevicestate.md)オブジェクトのプロパティと関係を一覧表示します。</span><span class="sxs-lookup"><span data-stu-id="14484-107">List properties and relationships of the [embeddedSIMDeviceState](../resources/intune-esim-embeddedsimdevicestate.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="14484-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="14484-108">Prerequisites</span></span>
<span data-ttu-id="14484-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/concepts/permissions-reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="14484-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="14484-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="14484-111">Permission type</span></span>|<span data-ttu-id="14484-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="14484-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="14484-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="14484-113">Delegated (work or school account)</span></span>|<span data-ttu-id="14484-114">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="14484-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="14484-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="14484-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="14484-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="14484-116">Not supported.</span></span>|
|<span data-ttu-id="14484-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="14484-117">Application</span></span>|<span data-ttu-id="14484-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="14484-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="14484-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="14484-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/embeddedSIMActivationCodePools/{embeddedSIMActivationCodePoolId}/deviceStates
```

## <a name="request-headers"></a><span data-ttu-id="14484-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="14484-120">Request headers</span></span>
|<span data-ttu-id="14484-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="14484-121">Header</span></span>|<span data-ttu-id="14484-122">値</span><span class="sxs-lookup"><span data-stu-id="14484-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="14484-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="14484-123">Authorization</span></span>|<span data-ttu-id="14484-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="14484-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="14484-125">Accept</span><span class="sxs-lookup"><span data-stu-id="14484-125">Accept</span></span>|<span data-ttu-id="14484-126">application/json</span><span class="sxs-lookup"><span data-stu-id="14484-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="14484-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="14484-127">Request body</span></span>
<span data-ttu-id="14484-128">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="14484-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="14484-129">応答</span><span class="sxs-lookup"><span data-stu-id="14484-129">Response</span></span>
<span data-ttu-id="14484-130">かどうかは成功すると、このメソッドが返されます、`200 OK`応答コードおよび応答の本文に[embeddedSIMDeviceState](../resources/intune-esim-embeddedsimdevicestate.md)オブジェクトのコレクションです。</span><span class="sxs-lookup"><span data-stu-id="14484-130">If successful, this method returns a `200 OK` response code and a collection of [embeddedSIMDeviceState](../resources/intune-esim-embeddedsimdevicestate.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="14484-131">例</span><span class="sxs-lookup"><span data-stu-id="14484-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="14484-132">要求</span><span class="sxs-lookup"><span data-stu-id="14484-132">Request</span></span>
<span data-ttu-id="14484-133">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="14484-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/embeddedSIMActivationCodePools/{embeddedSIMActivationCodePoolId}/deviceStates
```

### <a name="response"></a><span data-ttu-id="14484-134">応答</span><span class="sxs-lookup"><span data-stu-id="14484-134">Response</span></span>
<span data-ttu-id="14484-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="14484-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 602

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.embeddedSIMDeviceState",
      "id": "908884a3-84a3-9088-a384-8890a3848890",
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "modifiedDateTime": "2017-01-01T00:00:22.8983556-08:00",
      "lastSyncDateTime": "2017-01-01T00:02:49.3205976-08:00",
      "universalIntegratedCircuitCardIdentifier": "Universal Integrated Circuit Card Identifier value",
      "deviceName": "Device Name value",
      "userName": "User Name value",
      "state": "failed",
      "stateDetails": "State Details value"
    }
  ]
}
```




