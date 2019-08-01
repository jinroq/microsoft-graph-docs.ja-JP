---
title: remoteAssistancePartners のリスト
description: remoteAssistancePartner オブジェクトのプロパティとリレーションシップをリストします。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: c10535d281661fff6036e8d3392857d6f70b8105
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36023567"
---
# <a name="list-remoteassistancepartners"></a><span data-ttu-id="6dbbe-103">remoteAssistancePartners のリスト</span><span class="sxs-lookup"><span data-stu-id="6dbbe-103">List remoteAssistancePartners</span></span>

> <span data-ttu-id="6dbbe-104">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="6dbbe-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6dbbe-105">[remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="6dbbe-105">List properties and relationships of the [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="6dbbe-106">前提条件</span><span class="sxs-lookup"><span data-stu-id="6dbbe-106">Prerequisites</span></span>
<span data-ttu-id="6dbbe-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="6dbbe-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6dbbe-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="6dbbe-109">Permission type</span></span>|<span data-ttu-id="6dbbe-110">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="6dbbe-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6dbbe-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="6dbbe-111">Delegated (work or school account)</span></span>|<span data-ttu-id="6dbbe-112">DeviceManagementServiceConfig.ReadWrite.All、DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="6dbbe-112">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="6dbbe-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="6dbbe-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6dbbe-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="6dbbe-114">Not supported.</span></span>|
|<span data-ttu-id="6dbbe-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="6dbbe-115">Application</span></span>|<span data-ttu-id="6dbbe-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="6dbbe-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="6dbbe-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="6dbbe-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/remoteAssistancePartners
```

## <a name="request-headers"></a><span data-ttu-id="6dbbe-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="6dbbe-118">Request headers</span></span>
|<span data-ttu-id="6dbbe-119">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="6dbbe-119">Header</span></span>|<span data-ttu-id="6dbbe-120">値</span><span class="sxs-lookup"><span data-stu-id="6dbbe-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6dbbe-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="6dbbe-121">Authorization</span></span>|<span data-ttu-id="6dbbe-122">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="6dbbe-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6dbbe-123">承諾</span><span class="sxs-lookup"><span data-stu-id="6dbbe-123">Accept</span></span>|<span data-ttu-id="6dbbe-124">application/json</span><span class="sxs-lookup"><span data-stu-id="6dbbe-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6dbbe-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="6dbbe-125">Request body</span></span>
<span data-ttu-id="6dbbe-126">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="6dbbe-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6dbbe-127">応答</span><span class="sxs-lookup"><span data-stu-id="6dbbe-127">Response</span></span>
<span data-ttu-id="6dbbe-128">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md) オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="6dbbe-128">If successful, this method returns a `200 OK` response code and a collection of [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6dbbe-129">例</span><span class="sxs-lookup"><span data-stu-id="6dbbe-129">Example</span></span>

### <a name="request"></a><span data-ttu-id="6dbbe-130">要求</span><span class="sxs-lookup"><span data-stu-id="6dbbe-130">Request</span></span>
<span data-ttu-id="6dbbe-131">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="6dbbe-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/remoteAssistancePartners
```

### <a name="response"></a><span data-ttu-id="6dbbe-132">応答</span><span class="sxs-lookup"><span data-stu-id="6dbbe-132">Response</span></span>
<span data-ttu-id="6dbbe-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="6dbbe-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 372

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.remoteAssistancePartner",
      "id": "7443c8b9-c8b9-7443-b9c8-4374b9c84374",
      "displayName": "Display Name value",
      "onboardingUrl": "https://example.com/onboardingUrl/",
      "onboardingStatus": "onboarding",
      "lastConnectionDateTime": "2016-12-31T23:58:36.6670033-08:00"
    }
  ]
}
```



