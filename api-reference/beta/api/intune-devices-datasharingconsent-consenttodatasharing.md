---
title: consentToDataSharing アクション
description: まだ文書化されていません
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 2f1e379fb28e6e48b581514f8efde30b9c9f8673
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29420032"
---
# <a name="consenttodatasharing-action"></a><span data-ttu-id="095dc-103">consentToDataSharing アクション</span><span class="sxs-lookup"><span data-stu-id="095dc-103">consentToDataSharing action</span></span>

> <span data-ttu-id="095dc-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="095dc-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="095dc-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="095dc-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="095dc-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="095dc-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="095dc-107">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="095dc-107">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="095dc-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="095dc-108">Prerequisites</span></span>
<span data-ttu-id="095dc-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/concepts/permissions-reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="095dc-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="095dc-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="095dc-111">Permission type</span></span>|<span data-ttu-id="095dc-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="095dc-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="095dc-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="095dc-113">Delegated (work or school account)</span></span>|<span data-ttu-id="095dc-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="095dc-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="095dc-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="095dc-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="095dc-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="095dc-116">Not supported.</span></span>|
|<span data-ttu-id="095dc-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="095dc-117">Application</span></span>|<span data-ttu-id="095dc-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="095dc-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="095dc-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="095dc-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/dataSharingConsents/{dataSharingConsentId}/consentToDataSharing
```

## <a name="request-headers"></a><span data-ttu-id="095dc-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="095dc-120">Request headers</span></span>
|<span data-ttu-id="095dc-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="095dc-121">Header</span></span>|<span data-ttu-id="095dc-122">値</span><span class="sxs-lookup"><span data-stu-id="095dc-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="095dc-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="095dc-123">Authorization</span></span>|<span data-ttu-id="095dc-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="095dc-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="095dc-125">Accept</span><span class="sxs-lookup"><span data-stu-id="095dc-125">Accept</span></span>|<span data-ttu-id="095dc-126">application/json</span><span class="sxs-lookup"><span data-stu-id="095dc-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="095dc-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="095dc-127">Request body</span></span>
<span data-ttu-id="095dc-128">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="095dc-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="095dc-129">応答</span><span class="sxs-lookup"><span data-stu-id="095dc-129">Response</span></span>
<span data-ttu-id="095dc-130">かどうか、成功を返すアクション、`200 OK`応答コードおよび応答の本文には[dataSharingConsent](../resources/intune-devices-datasharingconsent.md)です。</span><span class="sxs-lookup"><span data-stu-id="095dc-130">If successful, this action returns a `200 OK` response code and a [dataSharingConsent](../resources/intune-devices-datasharingconsent.md) in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="095dc-131">例</span><span class="sxs-lookup"><span data-stu-id="095dc-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="095dc-132">要求</span><span class="sxs-lookup"><span data-stu-id="095dc-132">Request</span></span>
<span data-ttu-id="095dc-133">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="095dc-133">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/dataSharingConsents/{dataSharingConsentId}/consentToDataSharing
```

### <a name="response"></a><span data-ttu-id="095dc-134">応答</span><span class="sxs-lookup"><span data-stu-id="095dc-134">Response</span></span>
<span data-ttu-id="095dc-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="095dc-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 417

{
  "value": {
    "@odata.type": "#microsoft.graph.dataSharingConsent",
    "id": "333387f7-87f7-3333-f787-3333f7873333",
    "serviceDisplayName": "Service Display Name value",
    "termsUrl": "https://example.com/termsUrl/",
    "granted": true,
    "grantDateTime": "2016-12-31T23:59:55.7154191-08:00",
    "grantedByUpn": "Granted By Upn value",
    "grantedByUserId": "Granted By User Id value"
  }
}
```




