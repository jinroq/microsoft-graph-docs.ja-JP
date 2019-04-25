---
title: リスト embeddedSIMDeviceStates
description: embeddedSIMDeviceState オブジェクトのプロパティとリレーションシップをリストします。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 79f13f5ea9a176dc9aa9281e5bdc39b2770bf042
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32532339"
---
# <a name="list-embeddedsimdevicestates"></a><span data-ttu-id="878ad-103">リスト embeddedSIMDeviceStates</span><span class="sxs-lookup"><span data-stu-id="878ad-103">List embeddedSIMDeviceStates</span></span>

> <span data-ttu-id="878ad-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="878ad-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="878ad-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="878ad-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="878ad-106">[embeddedSIMDeviceState](../resources/intune-esim-embeddedsimdevicestate.md)オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="878ad-106">List properties and relationships of the [embeddedSIMDeviceState](../resources/intune-esim-embeddedsimdevicestate.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="878ad-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="878ad-107">Prerequisites</span></span>
<span data-ttu-id="878ad-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="878ad-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="878ad-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="878ad-110">Permission type</span></span>|<span data-ttu-id="878ad-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="878ad-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="878ad-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="878ad-112">Delegated (work or school account)</span></span>|<span data-ttu-id="878ad-113">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="878ad-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="878ad-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="878ad-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="878ad-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="878ad-115">Not supported.</span></span>|
|<span data-ttu-id="878ad-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="878ad-116">Application</span></span>|<span data-ttu-id="878ad-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="878ad-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="878ad-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="878ad-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/embeddedSIMActivationCodePools/{embeddedSIMActivationCodePoolId}/deviceStates
```

## <a name="request-headers"></a><span data-ttu-id="878ad-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="878ad-119">Request headers</span></span>
|<span data-ttu-id="878ad-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="878ad-120">Header</span></span>|<span data-ttu-id="878ad-121">値</span><span class="sxs-lookup"><span data-stu-id="878ad-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="878ad-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="878ad-122">Authorization</span></span>|<span data-ttu-id="878ad-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="878ad-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="878ad-124">承諾</span><span class="sxs-lookup"><span data-stu-id="878ad-124">Accept</span></span>|<span data-ttu-id="878ad-125">application/json</span><span class="sxs-lookup"><span data-stu-id="878ad-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="878ad-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="878ad-126">Request body</span></span>
<span data-ttu-id="878ad-127">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="878ad-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="878ad-128">応答</span><span class="sxs-lookup"><span data-stu-id="878ad-128">Response</span></span>
<span data-ttu-id="878ad-129">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で[embeddedSIMDeviceState](../resources/intune-esim-embeddedsimdevicestate.md)オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="878ad-129">If successful, this method returns a `200 OK` response code and a collection of [embeddedSIMDeviceState](../resources/intune-esim-embeddedsimdevicestate.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="878ad-130">例</span><span class="sxs-lookup"><span data-stu-id="878ad-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="878ad-131">要求</span><span class="sxs-lookup"><span data-stu-id="878ad-131">Request</span></span>
<span data-ttu-id="878ad-132">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="878ad-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/embeddedSIMActivationCodePools/{embeddedSIMActivationCodePoolId}/deviceStates
```

### <a name="response"></a><span data-ttu-id="878ad-133">応答</span><span class="sxs-lookup"><span data-stu-id="878ad-133">Response</span></span>
<span data-ttu-id="878ad-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="878ad-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





