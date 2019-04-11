---
title: getLicensesForApp 関数
description: まだ文書化されていません
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: fc97c48b7c4b5505808d8370e7181f2d7ca0d0ee
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/11/2019
ms.locfileid: "31780407"
---
# <a name="getlicensesforapp-function"></a><span data-ttu-id="80d3a-103">getLicensesForApp 関数</span><span class="sxs-lookup"><span data-stu-id="80d3a-103">getLicensesForApp function</span></span>

> <span data-ttu-id="80d3a-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="80d3a-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="80d3a-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="80d3a-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="80d3a-106">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="80d3a-106">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="80d3a-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="80d3a-107">Prerequisites</span></span>
<span data-ttu-id="80d3a-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="80d3a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="80d3a-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="80d3a-110">Permission type</span></span>|<span data-ttu-id="80d3a-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="80d3a-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="80d3a-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="80d3a-112">Delegated (work or school account)</span></span>|<span data-ttu-id="80d3a-113">DeviceManagementServiceConfig.ReadWrite.All、DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="80d3a-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="80d3a-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="80d3a-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="80d3a-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="80d3a-115">Not supported.</span></span>|
|<span data-ttu-id="80d3a-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="80d3a-116">Application</span></span>|<span data-ttu-id="80d3a-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="80d3a-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="80d3a-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="80d3a-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/vppTokens/getLicensesForApp
```

## <a name="request-headers"></a><span data-ttu-id="80d3a-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="80d3a-119">Request headers</span></span>
|<span data-ttu-id="80d3a-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="80d3a-120">Header</span></span>|<span data-ttu-id="80d3a-121">値</span><span class="sxs-lookup"><span data-stu-id="80d3a-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="80d3a-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="80d3a-122">Authorization</span></span>|<span data-ttu-id="80d3a-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="80d3a-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="80d3a-124">承諾</span><span class="sxs-lookup"><span data-stu-id="80d3a-124">Accept</span></span>|<span data-ttu-id="80d3a-125">application/json</span><span class="sxs-lookup"><span data-stu-id="80d3a-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="80d3a-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="80d3a-126">Request body</span></span>
<span data-ttu-id="80d3a-127">要求 URL で、次のクエリ パラメーターに値を指定します。</span><span class="sxs-lookup"><span data-stu-id="80d3a-127">In the request URL, provide the following query parameters with values.</span></span>
<span data-ttu-id="80d3a-128">次の表に、この関数で使用できるパラメーターを示します。</span><span class="sxs-lookup"><span data-stu-id="80d3a-128">The following table shows the parameters that can be used with this function.</span></span>

|<span data-ttu-id="80d3a-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="80d3a-129">Property</span></span>|<span data-ttu-id="80d3a-130">型</span><span class="sxs-lookup"><span data-stu-id="80d3a-130">Type</span></span>|<span data-ttu-id="80d3a-131">説明</span><span class="sxs-lookup"><span data-stu-id="80d3a-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="80d3a-132">bundleId</span><span class="sxs-lookup"><span data-stu-id="80d3a-132">bundleId</span></span>|<span data-ttu-id="80d3a-133">String</span><span class="sxs-lookup"><span data-stu-id="80d3a-133">String</span></span>|<span data-ttu-id="80d3a-134">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="80d3a-134">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="80d3a-135">応答</span><span class="sxs-lookup"><span data-stu-id="80d3a-135">Response</span></span>
<span data-ttu-id="80d3a-136">成功した場合、この関数`200 OK`は応答コードと、応答本文で[vpptokenlicensesummary](../resources/intune-onboarding-vpptokenlicensesummary.md)コレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="80d3a-136">If successful, this function returns a `200 OK` response code and a [vppTokenLicenseSummary](../resources/intune-onboarding-vpptokenlicensesummary.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="80d3a-137">例</span><span class="sxs-lookup"><span data-stu-id="80d3a-137">Example</span></span>

### <a name="request"></a><span data-ttu-id="80d3a-138">要求</span><span class="sxs-lookup"><span data-stu-id="80d3a-138">Request</span></span>
<span data-ttu-id="80d3a-139">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="80d3a-139">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/vppTokens/getLicensesForApp(bundleId='parameterValue')
```

### <a name="response"></a><span data-ttu-id="80d3a-140">応答</span><span class="sxs-lookup"><span data-stu-id="80d3a-140">Response</span></span>
<span data-ttu-id="80d3a-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="80d3a-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 298

{
  "value": [
    {
      "@odata.type": "microsoft.graph.vppTokenLicenseSummary",
      "vppTokenId": "Vpp Token Id value",
      "appleId": "Apple Id value",
      "organizationName": "Organization Name value",
      "availableLicenseCount": 5,
      "usedLicenseCount": 0
    }
  ]
}
```





