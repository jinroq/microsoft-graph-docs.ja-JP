---
title: getLicensesForApp 関数
description: まだ文書化されていません
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: aeb2e008f3df1c230349eac303d529467a652775
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29412787"
---
# <a name="getlicensesforapp-function"></a><span data-ttu-id="7415d-103">getLicensesForApp 関数</span><span class="sxs-lookup"><span data-stu-id="7415d-103">getLicensesForApp function</span></span>

> <span data-ttu-id="7415d-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="7415d-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="7415d-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="7415d-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="7415d-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="7415d-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7415d-107">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="7415d-107">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="7415d-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="7415d-108">Prerequisites</span></span>
<span data-ttu-id="7415d-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/concepts/permissions-reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="7415d-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="7415d-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="7415d-111">Permission type</span></span>|<span data-ttu-id="7415d-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="7415d-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7415d-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="7415d-113">Delegated (work or school account)</span></span>|<span data-ttu-id="7415d-114">DeviceManagementServiceConfig.ReadWrite.All、DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="7415d-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="7415d-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="7415d-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7415d-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="7415d-116">Not supported.</span></span>|
|<span data-ttu-id="7415d-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="7415d-117">Application</span></span>|<span data-ttu-id="7415d-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="7415d-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="7415d-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="7415d-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/vppTokens/getLicensesForApp
```

## <a name="request-headers"></a><span data-ttu-id="7415d-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="7415d-120">Request headers</span></span>
|<span data-ttu-id="7415d-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="7415d-121">Header</span></span>|<span data-ttu-id="7415d-122">値</span><span class="sxs-lookup"><span data-stu-id="7415d-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7415d-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="7415d-123">Authorization</span></span>|<span data-ttu-id="7415d-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="7415d-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7415d-125">Accept</span><span class="sxs-lookup"><span data-stu-id="7415d-125">Accept</span></span>|<span data-ttu-id="7415d-126">application/json</span><span class="sxs-lookup"><span data-stu-id="7415d-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7415d-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="7415d-127">Request body</span></span>
<span data-ttu-id="7415d-128">要求 URL で、次のクエリ パラメーターに値を指定します。</span><span class="sxs-lookup"><span data-stu-id="7415d-128">In the request URL, provide the following query parameters with values.</span></span>
<span data-ttu-id="7415d-129">次の表に、この関数で使用できるパラメーターを示します。</span><span class="sxs-lookup"><span data-stu-id="7415d-129">The following table shows the parameters that can be used with this function.</span></span>

|<span data-ttu-id="7415d-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="7415d-130">Property</span></span>|<span data-ttu-id="7415d-131">型</span><span class="sxs-lookup"><span data-stu-id="7415d-131">Type</span></span>|<span data-ttu-id="7415d-132">説明</span><span class="sxs-lookup"><span data-stu-id="7415d-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7415d-133">bundleId</span><span class="sxs-lookup"><span data-stu-id="7415d-133">bundleId</span></span>|<span data-ttu-id="7415d-134">String</span><span class="sxs-lookup"><span data-stu-id="7415d-134">String</span></span>|<span data-ttu-id="7415d-135">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="7415d-135">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="7415d-136">応答</span><span class="sxs-lookup"><span data-stu-id="7415d-136">Response</span></span>
<span data-ttu-id="7415d-137">かどうかは成功すると、この関数を返します、`200 OK`応答コードおよび応答の本文に[vppTokenLicenseSummary](../resources/intune-onboarding-vpptokenlicensesummary.md)のコレクションです。</span><span class="sxs-lookup"><span data-stu-id="7415d-137">If successful, this function returns a `200 OK` response code and a [vppTokenLicenseSummary](../resources/intune-onboarding-vpptokenlicensesummary.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7415d-138">例</span><span class="sxs-lookup"><span data-stu-id="7415d-138">Example</span></span>

### <a name="request"></a><span data-ttu-id="7415d-139">要求</span><span class="sxs-lookup"><span data-stu-id="7415d-139">Request</span></span>
<span data-ttu-id="7415d-140">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="7415d-140">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/vppTokens/getLicensesForApp(bundleId='parameterValue')
```

### <a name="response"></a><span data-ttu-id="7415d-141">応答</span><span class="sxs-lookup"><span data-stu-id="7415d-141">Response</span></span>
<span data-ttu-id="7415d-p104">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="7415d-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




