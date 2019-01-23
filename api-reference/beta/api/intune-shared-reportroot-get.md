---
title: Get reportRoot
description: reportRoot オブジェクトのプロパティとリレーションシップを読み取ります。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: ecfdc13e5e4cdfea5a8c3c9cfb40fe9d6872bd92
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29402931"
---
# <a name="get-reportroot"></a><span data-ttu-id="ca7a6-103">Get reportRoot</span><span class="sxs-lookup"><span data-stu-id="ca7a6-103">Get reportRoot</span></span>

> <span data-ttu-id="ca7a6-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="ca7a6-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="ca7a6-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ca7a6-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="ca7a6-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="ca7a6-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ca7a6-107">[reportRoot](../resources/intune-shared-reportroot.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="ca7a6-107">Read properties and relationships of the [reportRoot](../resources/intune-shared-reportroot.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="ca7a6-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="ca7a6-108">Prerequisites</span></span>
<span data-ttu-id="ca7a6-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="ca7a6-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ca7a6-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="ca7a6-111">Permission type</span></span>|<span data-ttu-id="ca7a6-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="ca7a6-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ca7a6-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="ca7a6-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="ca7a6-114">&nbsp; &nbsp; **デバイス構成**</span><span class="sxs-lookup"><span data-stu-id="ca7a6-114">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="ca7a6-115">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="ca7a6-115">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
| <span data-ttu-id="ca7a6-116">&nbsp; &nbsp; **トラブルシューティング**</span><span class="sxs-lookup"><span data-stu-id="ca7a6-116">&nbsp; &nbsp; **Troubleshooting**</span></span> | <span data-ttu-id="ca7a6-117">DeviceManagementManagedDevices.ReadWrite.All、DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="ca7a6-117">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="ca7a6-118">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="ca7a6-118">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ca7a6-119">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ca7a6-119">Not supported.</span></span>|
|<span data-ttu-id="ca7a6-120">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="ca7a6-120">Application</span></span>|<span data-ttu-id="ca7a6-121">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ca7a6-121">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ca7a6-122">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="ca7a6-122">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /reports
```

## <a name="optional-query-parameters"></a><span data-ttu-id="ca7a6-123">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="ca7a6-123">Optional query parameters</span></span>
<span data-ttu-id="ca7a6-124">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="ca7a6-124">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="ca7a6-125">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="ca7a6-125">Request headers</span></span>
|<span data-ttu-id="ca7a6-126">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="ca7a6-126">Header</span></span>|<span data-ttu-id="ca7a6-127">値</span><span class="sxs-lookup"><span data-stu-id="ca7a6-127">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ca7a6-128">Authorization</span><span class="sxs-lookup"><span data-stu-id="ca7a6-128">Authorization</span></span>|<span data-ttu-id="ca7a6-129">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="ca7a6-129">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ca7a6-130">Accept</span><span class="sxs-lookup"><span data-stu-id="ca7a6-130">Accept</span></span>|<span data-ttu-id="ca7a6-131">application/json</span><span class="sxs-lookup"><span data-stu-id="ca7a6-131">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ca7a6-132">要求本文</span><span class="sxs-lookup"><span data-stu-id="ca7a6-132">Request body</span></span>
<span data-ttu-id="ca7a6-133">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="ca7a6-133">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ca7a6-134">応答</span><span class="sxs-lookup"><span data-stu-id="ca7a6-134">Response</span></span>
<span data-ttu-id="ca7a6-135">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [reportRoot](../resources/intune-shared-reportroot.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="ca7a6-135">If successful, this method returns a `200 OK` response code and [reportRoot](../resources/intune-shared-reportroot.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ca7a6-136">例</span><span class="sxs-lookup"><span data-stu-id="ca7a6-136">Example</span></span>
### <a name="request"></a><span data-ttu-id="ca7a6-137">要求</span><span class="sxs-lookup"><span data-stu-id="ca7a6-137">Request</span></span>
<span data-ttu-id="ca7a6-138">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="ca7a6-138">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/reports
```

### <a name="response"></a><span data-ttu-id="ca7a6-139">応答</span><span class="sxs-lookup"><span data-stu-id="ca7a6-139">Response</span></span>
<span data-ttu-id="ca7a6-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="ca7a6-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 124

{
  "value": {
    "@odata.type": "#microsoft.graph.reportRoot",
    "id": "9ab6b3dd-b3dd-9ab6-ddb3-b69addb3b69a"
  }
}
```



