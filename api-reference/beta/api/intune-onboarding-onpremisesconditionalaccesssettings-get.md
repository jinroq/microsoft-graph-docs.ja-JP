---
title: onPremisesConditionalAccessSettings の取得
description: onPremisesConditionalAccessSettings オブジェクトのプロパティとリレーションシップを読み取ります。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: d1962e556de47c23cefc67756a8e4ca16a354a05
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29423063"
---
# <a name="get-onpremisesconditionalaccesssettings"></a><span data-ttu-id="75465-103">onPremisesConditionalAccessSettings の取得</span><span class="sxs-lookup"><span data-stu-id="75465-103">Get onPremisesConditionalAccessSettings</span></span>

> <span data-ttu-id="75465-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="75465-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="75465-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="75465-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="75465-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="75465-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="75465-107">[onPremisesConditionalAccessSettings](../resources/intune-onboarding-onpremisesconditionalaccesssettings.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="75465-107">Read properties and relationships of the [onPremisesConditionalAccessSettings](../resources/intune-onboarding-onpremisesconditionalaccesssettings.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="75465-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="75465-108">Prerequisites</span></span>
<span data-ttu-id="75465-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/concepts/permissions-reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="75465-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="75465-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="75465-111">Permission type</span></span>|<span data-ttu-id="75465-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="75465-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="75465-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="75465-113">Delegated (work or school account)</span></span>|<span data-ttu-id="75465-114">DeviceManagementServiceConfig.ReadWrite.All、DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="75465-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="75465-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="75465-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="75465-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="75465-116">Not supported.</span></span>|
|<span data-ttu-id="75465-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="75465-117">Application</span></span>|<span data-ttu-id="75465-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="75465-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="75465-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="75465-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/conditionalAccessSettings
GET /deviceManagement/exchangeOnPremisesPolicy/conditionalAccessSettings
```

## <a name="optional-query-parameters"></a><span data-ttu-id="75465-120">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="75465-120">Optional query parameters</span></span>
<span data-ttu-id="75465-121">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://docs.microsoft.com/en-us/graph/query-parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="75465-121">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="75465-122">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="75465-122">Request headers</span></span>
|<span data-ttu-id="75465-123">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="75465-123">Header</span></span>|<span data-ttu-id="75465-124">値</span><span class="sxs-lookup"><span data-stu-id="75465-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="75465-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="75465-125">Authorization</span></span>|<span data-ttu-id="75465-126">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="75465-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="75465-127">Accept</span><span class="sxs-lookup"><span data-stu-id="75465-127">Accept</span></span>|<span data-ttu-id="75465-128">application/json</span><span class="sxs-lookup"><span data-stu-id="75465-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="75465-129">要求本文</span><span class="sxs-lookup"><span data-stu-id="75465-129">Request body</span></span>
<span data-ttu-id="75465-130">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="75465-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="75465-131">応答</span><span class="sxs-lookup"><span data-stu-id="75465-131">Response</span></span>
<span data-ttu-id="75465-132">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [onPremisesConditionalAccessSettings](../resources/intune-onboarding-onpremisesconditionalaccesssettings.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="75465-132">If successful, this method returns a `200 OK` response code and [onPremisesConditionalAccessSettings](../resources/intune-onboarding-onpremisesconditionalaccesssettings.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="75465-133">例</span><span class="sxs-lookup"><span data-stu-id="75465-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="75465-134">要求</span><span class="sxs-lookup"><span data-stu-id="75465-134">Request</span></span>
<span data-ttu-id="75465-135">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="75465-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/conditionalAccessSettings
```

### <a name="response"></a><span data-ttu-id="75465-136">応答</span><span class="sxs-lookup"><span data-stu-id="75465-136">Response</span></span>
<span data-ttu-id="75465-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="75465-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 363

{
  "value": {
    "@odata.type": "#microsoft.graph.onPremisesConditionalAccessSettings",
    "id": "a0efde21-de21-a0ef-21de-efa021deefa0",
    "enabled": true,
    "includedGroups": [
      "77c9d466-d466-77c9-66d4-c97766d4c977"
    ],
    "excludedGroups": [
      "2a0afae4-fae4-2a0a-e4fa-0a2ae4fa0a2a"
    ],
    "overrideDefaultRule": true
  }
}
```




