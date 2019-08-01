---
title: Get reportRoot
description: reportRoot オブジェクトのプロパティとリレーションシップを読み取ります。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 6b767ae43a4b38a86665ad2f9d67c89acca33f81
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36023413"
---
# <a name="get-reportroot"></a><span data-ttu-id="76dc2-103">Get reportRoot</span><span class="sxs-lookup"><span data-stu-id="76dc2-103">Get reportRoot</span></span>

> <span data-ttu-id="76dc2-104">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="76dc2-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="76dc2-105">[reportRoot](../resources/intune-shared-reportroot.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="76dc2-105">Read properties and relationships of the [reportRoot](../resources/intune-shared-reportroot.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="76dc2-106">前提条件</span><span class="sxs-lookup"><span data-stu-id="76dc2-106">Prerequisites</span></span>
<span data-ttu-id="76dc2-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="76dc2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="76dc2-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="76dc2-109">Permission type</span></span>|<span data-ttu-id="76dc2-110">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="76dc2-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="76dc2-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="76dc2-111">Delegated (work or school account)</span></span>||
| <span data-ttu-id="76dc2-112">&nbsp;&nbsp;デバイス構成</span><span class="sxs-lookup"><span data-stu-id="76dc2-112">&nbsp; &nbsp; Device configuration</span></span> | <span data-ttu-id="76dc2-113">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="76dc2-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
| <span data-ttu-id="76dc2-114">&nbsp;&nbsp;トラブルシューティング</span><span class="sxs-lookup"><span data-stu-id="76dc2-114">&nbsp; &nbsp; Troubleshooting</span></span> | <span data-ttu-id="76dc2-115">DeviceManagementManagedDevices.ReadWrite.All、DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="76dc2-115">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="76dc2-116">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="76dc2-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="76dc2-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="76dc2-117">Not supported.</span></span>|
|<span data-ttu-id="76dc2-118">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="76dc2-118">Application</span></span>|<span data-ttu-id="76dc2-119">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="76dc2-119">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="76dc2-120">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="76dc2-120">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /reports
```

## <a name="optional-query-parameters"></a><span data-ttu-id="76dc2-121">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="76dc2-121">Optional query parameters</span></span>
<span data-ttu-id="76dc2-122">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="76dc2-122">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="76dc2-123">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="76dc2-123">Request headers</span></span>
|<span data-ttu-id="76dc2-124">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="76dc2-124">Header</span></span>|<span data-ttu-id="76dc2-125">値</span><span class="sxs-lookup"><span data-stu-id="76dc2-125">Value</span></span>|
|:---|:---|
|<span data-ttu-id="76dc2-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="76dc2-126">Authorization</span></span>|<span data-ttu-id="76dc2-127">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="76dc2-127">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="76dc2-128">承諾</span><span class="sxs-lookup"><span data-stu-id="76dc2-128">Accept</span></span>|<span data-ttu-id="76dc2-129">application/json</span><span class="sxs-lookup"><span data-stu-id="76dc2-129">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="76dc2-130">要求本文</span><span class="sxs-lookup"><span data-stu-id="76dc2-130">Request body</span></span>
<span data-ttu-id="76dc2-131">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="76dc2-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="76dc2-132">応答</span><span class="sxs-lookup"><span data-stu-id="76dc2-132">Response</span></span>
<span data-ttu-id="76dc2-133">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [reportRoot](../resources/intune-shared-reportroot.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="76dc2-133">If successful, this method returns a `200 OK` response code and [reportRoot](../resources/intune-shared-reportroot.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="76dc2-134">例</span><span class="sxs-lookup"><span data-stu-id="76dc2-134">Example</span></span>
### <a name="request"></a><span data-ttu-id="76dc2-135">要求</span><span class="sxs-lookup"><span data-stu-id="76dc2-135">Request</span></span>
<span data-ttu-id="76dc2-136">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="76dc2-136">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/reports
```

### <a name="response"></a><span data-ttu-id="76dc2-137">応答</span><span class="sxs-lookup"><span data-stu-id="76dc2-137">Response</span></span>
<span data-ttu-id="76dc2-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="76dc2-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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








