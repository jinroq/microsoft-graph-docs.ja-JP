---
title: リスト embeddedSIMActivationCodePools
description: EmbeddedSIMActivationCodePool オブジェクトのプロパティと関係を一覧表示します。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: ff86120b27df8f969e3002b0f2b433eb1791c7d5
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29405213"
---
# <a name="list-embeddedsimactivationcodepools"></a><span data-ttu-id="51e39-103">リスト embeddedSIMActivationCodePools</span><span class="sxs-lookup"><span data-stu-id="51e39-103">List embeddedSIMActivationCodePools</span></span>

> <span data-ttu-id="51e39-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="51e39-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="51e39-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="51e39-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="51e39-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="51e39-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="51e39-107">[EmbeddedSIMActivationCodePool](../resources/intune-esim-embeddedsimactivationcodepool.md)オブジェクトのプロパティと関係を一覧表示します。</span><span class="sxs-lookup"><span data-stu-id="51e39-107">List properties and relationships of the [embeddedSIMActivationCodePool](../resources/intune-esim-embeddedsimactivationcodepool.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="51e39-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="51e39-108">Prerequisites</span></span>
<span data-ttu-id="51e39-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/concepts/permissions-reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="51e39-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="51e39-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="51e39-111">Permission type</span></span>|<span data-ttu-id="51e39-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="51e39-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="51e39-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="51e39-113">Delegated (work or school account)</span></span>|<span data-ttu-id="51e39-114">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="51e39-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="51e39-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="51e39-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="51e39-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="51e39-116">Not supported.</span></span>|
|<span data-ttu-id="51e39-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="51e39-117">Application</span></span>|<span data-ttu-id="51e39-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="51e39-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="51e39-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="51e39-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/embeddedSIMActivationCodePools
```

## <a name="request-headers"></a><span data-ttu-id="51e39-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="51e39-120">Request headers</span></span>
|<span data-ttu-id="51e39-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="51e39-121">Header</span></span>|<span data-ttu-id="51e39-122">値</span><span class="sxs-lookup"><span data-stu-id="51e39-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="51e39-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="51e39-123">Authorization</span></span>|<span data-ttu-id="51e39-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="51e39-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="51e39-125">Accept</span><span class="sxs-lookup"><span data-stu-id="51e39-125">Accept</span></span>|<span data-ttu-id="51e39-126">application/json</span><span class="sxs-lookup"><span data-stu-id="51e39-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="51e39-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="51e39-127">Request body</span></span>
<span data-ttu-id="51e39-128">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="51e39-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="51e39-129">応答</span><span class="sxs-lookup"><span data-stu-id="51e39-129">Response</span></span>
<span data-ttu-id="51e39-130">かどうかは成功すると、このメソッドが返されます、`200 OK`応答コードおよび応答の本文に[embeddedSIMActivationCodePool](../resources/intune-esim-embeddedsimactivationcodepool.md)オブジェクトのコレクションです。</span><span class="sxs-lookup"><span data-stu-id="51e39-130">If successful, this method returns a `200 OK` response code and a collection of [embeddedSIMActivationCodePool](../resources/intune-esim-embeddedsimactivationcodepool.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="51e39-131">例</span><span class="sxs-lookup"><span data-stu-id="51e39-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="51e39-132">要求</span><span class="sxs-lookup"><span data-stu-id="51e39-132">Request</span></span>
<span data-ttu-id="51e39-133">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="51e39-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/embeddedSIMActivationCodePools
```

### <a name="response"></a><span data-ttu-id="51e39-134">応答</span><span class="sxs-lookup"><span data-stu-id="51e39-134">Response</span></span>
<span data-ttu-id="51e39-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="51e39-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 717

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.embeddedSIMActivationCodePool",
      "id": "ec308741-8741-ec30-4187-30ec418730ec",
      "displayName": "Display Name value",
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "modifiedDateTime": "2017-01-01T00:00:22.8983556-08:00",
      "activationCodes": [
        {
          "@odata.type": "microsoft.graph.embeddedSIMActivationCode",
          "integratedCircuitCardIdentifier": "Integrated Circuit Card Identifier value",
          "matchingIdentifier": "Matching Identifier value",
          "smdpPlusServerAddress": "Smdp Plus Server Address value"
        }
      ],
      "activationCodeCount": 3
    }
  ]
}
```




