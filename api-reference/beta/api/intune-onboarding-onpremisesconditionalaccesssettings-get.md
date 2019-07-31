---
title: onPremisesConditionalAccessSettings の取得
description: onPremisesConditionalAccessSettings オブジェクトのプロパティとリレーションシップを読み取ります。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 7e860b8b870730bc97760e9e361686c4f84d12bf
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35995770"
---
# <a name="get-onpremisesconditionalaccesssettings"></a><span data-ttu-id="77126-103">onPremisesConditionalAccessSettings の取得</span><span class="sxs-lookup"><span data-stu-id="77126-103">Get onPremisesConditionalAccessSettings</span></span>

> <span data-ttu-id="77126-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="77126-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="77126-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="77126-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="77126-106">[onPremisesConditionalAccessSettings](../resources/intune-onboarding-onpremisesconditionalaccesssettings.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="77126-106">Read properties and relationships of the [onPremisesConditionalAccessSettings](../resources/intune-onboarding-onpremisesconditionalaccesssettings.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="77126-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="77126-107">Prerequisites</span></span>
<span data-ttu-id="77126-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="77126-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="77126-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="77126-110">Permission type</span></span>|<span data-ttu-id="77126-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="77126-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="77126-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="77126-112">Delegated (work or school account)</span></span>|<span data-ttu-id="77126-113">DeviceManagementServiceConfig.ReadWrite.All、DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="77126-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="77126-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="77126-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="77126-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="77126-115">Not supported.</span></span>|
|<span data-ttu-id="77126-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="77126-116">Application</span></span>|<span data-ttu-id="77126-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="77126-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="77126-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="77126-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/conditionalAccessSettings
GET /deviceManagement/exchangeOnPremisesPolicy/conditionalAccessSettings
```

## <a name="optional-query-parameters"></a><span data-ttu-id="77126-119">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="77126-119">Optional query parameters</span></span>
<span data-ttu-id="77126-120">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://docs.microsoft.com/en-us/graph/query-parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="77126-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="77126-121">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="77126-121">Request headers</span></span>
|<span data-ttu-id="77126-122">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="77126-122">Header</span></span>|<span data-ttu-id="77126-123">値</span><span class="sxs-lookup"><span data-stu-id="77126-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="77126-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="77126-124">Authorization</span></span>|<span data-ttu-id="77126-125">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="77126-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="77126-126">承諾</span><span class="sxs-lookup"><span data-stu-id="77126-126">Accept</span></span>|<span data-ttu-id="77126-127">application/json</span><span class="sxs-lookup"><span data-stu-id="77126-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="77126-128">要求本文</span><span class="sxs-lookup"><span data-stu-id="77126-128">Request body</span></span>
<span data-ttu-id="77126-129">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="77126-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="77126-130">応答</span><span class="sxs-lookup"><span data-stu-id="77126-130">Response</span></span>
<span data-ttu-id="77126-131">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [onPremisesConditionalAccessSettings](../resources/intune-onboarding-onpremisesconditionalaccesssettings.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="77126-131">If successful, this method returns a `200 OK` response code and [onPremisesConditionalAccessSettings](../resources/intune-onboarding-onpremisesconditionalaccesssettings.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="77126-132">例</span><span class="sxs-lookup"><span data-stu-id="77126-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="77126-133">要求</span><span class="sxs-lookup"><span data-stu-id="77126-133">Request</span></span>
<span data-ttu-id="77126-134">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="77126-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/conditionalAccessSettings
```

### <a name="response"></a><span data-ttu-id="77126-135">応答</span><span class="sxs-lookup"><span data-stu-id="77126-135">Response</span></span>
<span data-ttu-id="77126-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="77126-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





