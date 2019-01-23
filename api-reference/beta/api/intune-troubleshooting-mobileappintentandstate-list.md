---
title: リスト mobileAppIntentAndStates
description: MobileAppIntentAndState オブジェクトのプロパティと関係を一覧表示します。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 0b0d617df0540a55dd41691e9ea27a899869a178
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29403050"
---
# <a name="list-mobileappintentandstates"></a><span data-ttu-id="44b72-103">リスト mobileAppIntentAndStates</span><span class="sxs-lookup"><span data-stu-id="44b72-103">List mobileAppIntentAndStates</span></span>

> <span data-ttu-id="44b72-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="44b72-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="44b72-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="44b72-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="44b72-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="44b72-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="44b72-107">[MobileAppIntentAndState](../resources/intune-troubleshooting-mobileappintentandstate.md)オブジェクトのプロパティと関係を一覧表示します。</span><span class="sxs-lookup"><span data-stu-id="44b72-107">List properties and relationships of the [mobileAppIntentAndState](../resources/intune-troubleshooting-mobileappintentandstate.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="44b72-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="44b72-108">Prerequisites</span></span>
<span data-ttu-id="44b72-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/concepts/permissions-reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="44b72-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="44b72-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="44b72-111">Permission type</span></span>|<span data-ttu-id="44b72-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="44b72-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="44b72-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="44b72-113">Delegated (work or school account)</span></span>|<span data-ttu-id="44b72-114">DeviceManagementManagedDevices.ReadWrite.All、DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="44b72-114">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="44b72-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="44b72-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="44b72-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="44b72-116">Not supported.</span></span>|
|<span data-ttu-id="44b72-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="44b72-117">Application</span></span>|<span data-ttu-id="44b72-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="44b72-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="44b72-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="44b72-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /users/{usersId}/mobileAppIntentAndStates
```

## <a name="request-headers"></a><span data-ttu-id="44b72-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="44b72-120">Request headers</span></span>
|<span data-ttu-id="44b72-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="44b72-121">Header</span></span>|<span data-ttu-id="44b72-122">値</span><span class="sxs-lookup"><span data-stu-id="44b72-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="44b72-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="44b72-123">Authorization</span></span>|<span data-ttu-id="44b72-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="44b72-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="44b72-125">Accept</span><span class="sxs-lookup"><span data-stu-id="44b72-125">Accept</span></span>|<span data-ttu-id="44b72-126">application/json</span><span class="sxs-lookup"><span data-stu-id="44b72-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="44b72-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="44b72-127">Request body</span></span>
<span data-ttu-id="44b72-128">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="44b72-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="44b72-129">応答</span><span class="sxs-lookup"><span data-stu-id="44b72-129">Response</span></span>
<span data-ttu-id="44b72-130">かどうかは成功すると、このメソッドが返されます、`200 OK`応答コードおよび応答の本文に[mobileAppIntentAndState](../resources/intune-troubleshooting-mobileappintentandstate.md)オブジェクトのコレクションです。</span><span class="sxs-lookup"><span data-stu-id="44b72-130">If successful, this method returns a `200 OK` response code and a collection of [mobileAppIntentAndState](../resources/intune-troubleshooting-mobileappintentandstate.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="44b72-131">例</span><span class="sxs-lookup"><span data-stu-id="44b72-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="44b72-132">要求</span><span class="sxs-lookup"><span data-stu-id="44b72-132">Request</span></span>
<span data-ttu-id="44b72-133">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="44b72-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/users/{usersId}/mobileAppIntentAndStates
```

### <a name="response"></a><span data-ttu-id="44b72-134">応答</span><span class="sxs-lookup"><span data-stu-id="44b72-134">Response</span></span>
<span data-ttu-id="44b72-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="44b72-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1001

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.mobileAppIntentAndState",
      "id": "45a775d6-75d6-45a7-d675-a745d675a745",
      "managedDeviceIdentifier": "Managed Device Identifier value",
      "userId": "User Id value",
      "mobileAppList": [
        {
          "@odata.type": "microsoft.graph.mobileAppIntentAndStateDetail",
          "applicationId": "Application Id value",
          "displayName": "Display Name value",
          "mobileAppIntent": "notAvailable",
          "displayVersion": "Display Version value",
          "installState": "failed",
          "supportedDeviceTypes": [
            {
              "@odata.type": "microsoft.graph.mobileAppSupportedDeviceType",
              "type": "windowsRT",
              "minimumOperatingSystemVersion": "Minimum Operating System Version value",
              "maximumOperatingSystemVersion": "Maximum Operating System Version value"
            }
          ]
        }
      ]
    }
  ]
}
```




