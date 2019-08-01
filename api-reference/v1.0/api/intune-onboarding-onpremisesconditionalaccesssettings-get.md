---
title: onPremisesConditionalAccessSettings の取得
description: onPremisesConditionalAccessSettings オブジェクトのプロパティとリレーションシップを読み取ります。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 3d400227206a681830c4be1ed18d747995c43eb6
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36024092"
---
# <a name="get-onpremisesconditionalaccesssettings"></a><span data-ttu-id="2a846-103">onPremisesConditionalAccessSettings の取得</span><span class="sxs-lookup"><span data-stu-id="2a846-103">Get onPremisesConditionalAccessSettings</span></span>

> <span data-ttu-id="2a846-104">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="2a846-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2a846-105">[onPremisesConditionalAccessSettings](../resources/intune-onboarding-onpremisesconditionalaccesssettings.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="2a846-105">Read properties and relationships of the [onPremisesConditionalAccessSettings](../resources/intune-onboarding-onpremisesconditionalaccesssettings.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="2a846-106">前提条件</span><span class="sxs-lookup"><span data-stu-id="2a846-106">Prerequisites</span></span>
<span data-ttu-id="2a846-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="2a846-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2a846-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="2a846-109">Permission type</span></span>|<span data-ttu-id="2a846-110">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="2a846-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2a846-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="2a846-111">Delegated (work or school account)</span></span>|<span data-ttu-id="2a846-112">DeviceManagementServiceConfig.ReadWrite.All、DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="2a846-112">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="2a846-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="2a846-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2a846-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="2a846-114">Not supported.</span></span>|
|<span data-ttu-id="2a846-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="2a846-115">Application</span></span>|<span data-ttu-id="2a846-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="2a846-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="2a846-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="2a846-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/conditionalAccessSettings
```

## <a name="optional-query-parameters"></a><span data-ttu-id="2a846-118">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="2a846-118">Optional query parameters</span></span>
<span data-ttu-id="2a846-119">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://docs.microsoft.com/en-us/graph/query-parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="2a846-119">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="2a846-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="2a846-120">Request headers</span></span>
|<span data-ttu-id="2a846-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="2a846-121">Header</span></span>|<span data-ttu-id="2a846-122">値</span><span class="sxs-lookup"><span data-stu-id="2a846-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2a846-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="2a846-123">Authorization</span></span>|<span data-ttu-id="2a846-124">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="2a846-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2a846-125">承諾</span><span class="sxs-lookup"><span data-stu-id="2a846-125">Accept</span></span>|<span data-ttu-id="2a846-126">application/json</span><span class="sxs-lookup"><span data-stu-id="2a846-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2a846-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="2a846-127">Request body</span></span>
<span data-ttu-id="2a846-128">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="2a846-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2a846-129">応答</span><span class="sxs-lookup"><span data-stu-id="2a846-129">Response</span></span>
<span data-ttu-id="2a846-130">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [onPremisesConditionalAccessSettings](../resources/intune-onboarding-onpremisesconditionalaccesssettings.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="2a846-130">If successful, this method returns a `200 OK` response code and [onPremisesConditionalAccessSettings](../resources/intune-onboarding-onpremisesconditionalaccesssettings.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2a846-131">例</span><span class="sxs-lookup"><span data-stu-id="2a846-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="2a846-132">要求</span><span class="sxs-lookup"><span data-stu-id="2a846-132">Request</span></span>
<span data-ttu-id="2a846-133">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="2a846-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/conditionalAccessSettings
```

### <a name="response"></a><span data-ttu-id="2a846-134">応答</span><span class="sxs-lookup"><span data-stu-id="2a846-134">Response</span></span>
<span data-ttu-id="2a846-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="2a846-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



