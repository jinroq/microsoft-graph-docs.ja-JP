---
title: リスト embeddedSIMActivationCodePools
description: embeddedSIMActivationCodePool オブジェクトのプロパティとリレーションシップをリストします。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: c9c1e54ea0f4094446fe3ccf932a10cf59d36bc9
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/11/2019
ms.locfileid: "31803914"
---
# <a name="list-embeddedsimactivationcodepools"></a><span data-ttu-id="95919-103">リスト embeddedSIMActivationCodePools</span><span class="sxs-lookup"><span data-stu-id="95919-103">List embeddedSIMActivationCodePools</span></span>

> <span data-ttu-id="95919-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="95919-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="95919-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="95919-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="95919-106">[embeddedSIMActivationCodePool](../resources/intune-esim-embeddedsimactivationcodepool.md)オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="95919-106">List properties and relationships of the [embeddedSIMActivationCodePool](../resources/intune-esim-embeddedsimactivationcodepool.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="95919-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="95919-107">Prerequisites</span></span>
<span data-ttu-id="95919-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="95919-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="95919-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="95919-110">Permission type</span></span>|<span data-ttu-id="95919-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="95919-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="95919-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="95919-112">Delegated (work or school account)</span></span>|<span data-ttu-id="95919-113">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="95919-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="95919-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="95919-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="95919-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="95919-115">Not supported.</span></span>|
|<span data-ttu-id="95919-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="95919-116">Application</span></span>|<span data-ttu-id="95919-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="95919-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="95919-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="95919-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/embeddedSIMActivationCodePools
```

## <a name="request-headers"></a><span data-ttu-id="95919-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="95919-119">Request headers</span></span>
|<span data-ttu-id="95919-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="95919-120">Header</span></span>|<span data-ttu-id="95919-121">値</span><span class="sxs-lookup"><span data-stu-id="95919-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="95919-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="95919-122">Authorization</span></span>|<span data-ttu-id="95919-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="95919-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="95919-124">承諾</span><span class="sxs-lookup"><span data-stu-id="95919-124">Accept</span></span>|<span data-ttu-id="95919-125">application/json</span><span class="sxs-lookup"><span data-stu-id="95919-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="95919-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="95919-126">Request body</span></span>
<span data-ttu-id="95919-127">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="95919-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="95919-128">応答</span><span class="sxs-lookup"><span data-stu-id="95919-128">Response</span></span>
<span data-ttu-id="95919-129">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で[embeddedSIMActivationCodePool](../resources/intune-esim-embeddedsimactivationcodepool.md)オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="95919-129">If successful, this method returns a `200 OK` response code and a collection of [embeddedSIMActivationCodePool](../resources/intune-esim-embeddedsimactivationcodepool.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="95919-130">例</span><span class="sxs-lookup"><span data-stu-id="95919-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="95919-131">要求</span><span class="sxs-lookup"><span data-stu-id="95919-131">Request</span></span>
<span data-ttu-id="95919-132">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="95919-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/embeddedSIMActivationCodePools
```

### <a name="response"></a><span data-ttu-id="95919-133">応答</span><span class="sxs-lookup"><span data-stu-id="95919-133">Response</span></span>
<span data-ttu-id="95919-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="95919-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





