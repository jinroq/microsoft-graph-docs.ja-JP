---
title: Get reportRoot
description: reportRoot オブジェクトのプロパティとリレーションシップを読み取ります。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: ecfdc13e5e4cdfea5a8c3c9cfb40fe9d6872bd92
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/29/2019
ms.locfileid: "30979103"
---
# <a name="get-reportroot"></a><span data-ttu-id="0a93c-103">Get reportRoot</span><span class="sxs-lookup"><span data-stu-id="0a93c-103">Get reportRoot</span></span>

> <span data-ttu-id="0a93c-104">**重要:** Microsoft Graph の/ベータ版の api は変更される可能性があります。</span><span class="sxs-lookup"><span data-stu-id="0a93c-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="0a93c-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="0a93c-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="0a93c-106">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="0a93c-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0a93c-107">[reportRoot](../resources/intune-shared-reportroot.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="0a93c-107">Read properties and relationships of the [reportRoot](../resources/intune-shared-reportroot.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="0a93c-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="0a93c-108">Prerequisites</span></span>
<span data-ttu-id="0a93c-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="0a93c-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0a93c-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="0a93c-111">Permission type</span></span>|<span data-ttu-id="0a93c-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="0a93c-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0a93c-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="0a93c-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="0a93c-114">&nbsp; &nbsp; **デバイス構成**</span><span class="sxs-lookup"><span data-stu-id="0a93c-114">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="0a93c-115">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="0a93c-115">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
| <span data-ttu-id="0a93c-116">&nbsp; &nbsp; **トラブルシューティング**</span><span class="sxs-lookup"><span data-stu-id="0a93c-116">&nbsp; &nbsp; **Troubleshooting**</span></span> | <span data-ttu-id="0a93c-117">DeviceManagementManagedDevices.ReadWrite.All、DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="0a93c-117">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="0a93c-118">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="0a93c-118">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0a93c-119">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="0a93c-119">Not supported.</span></span>|
|<span data-ttu-id="0a93c-120">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="0a93c-120">Application</span></span>|<span data-ttu-id="0a93c-121">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="0a93c-121">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="0a93c-122">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="0a93c-122">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /reports
```

## <a name="optional-query-parameters"></a><span data-ttu-id="0a93c-123">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="0a93c-123">Optional query parameters</span></span>
<span data-ttu-id="0a93c-124">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="0a93c-124">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="0a93c-125">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="0a93c-125">Request headers</span></span>
|<span data-ttu-id="0a93c-126">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="0a93c-126">Header</span></span>|<span data-ttu-id="0a93c-127">値</span><span class="sxs-lookup"><span data-stu-id="0a93c-127">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0a93c-128">Authorization</span><span class="sxs-lookup"><span data-stu-id="0a93c-128">Authorization</span></span>|<span data-ttu-id="0a93c-129">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="0a93c-129">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0a93c-130">承諾</span><span class="sxs-lookup"><span data-stu-id="0a93c-130">Accept</span></span>|<span data-ttu-id="0a93c-131">application/json</span><span class="sxs-lookup"><span data-stu-id="0a93c-131">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0a93c-132">要求本文</span><span class="sxs-lookup"><span data-stu-id="0a93c-132">Request body</span></span>
<span data-ttu-id="0a93c-133">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="0a93c-133">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0a93c-134">応答</span><span class="sxs-lookup"><span data-stu-id="0a93c-134">Response</span></span>
<span data-ttu-id="0a93c-135">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [reportRoot](../resources/intune-shared-reportroot.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="0a93c-135">If successful, this method returns a `200 OK` response code and [reportRoot](../resources/intune-shared-reportroot.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0a93c-136">例</span><span class="sxs-lookup"><span data-stu-id="0a93c-136">Example</span></span>
### <a name="request"></a><span data-ttu-id="0a93c-137">要求</span><span class="sxs-lookup"><span data-stu-id="0a93c-137">Request</span></span>
<span data-ttu-id="0a93c-138">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="0a93c-138">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/reports
```

### <a name="response"></a><span data-ttu-id="0a93c-139">応答</span><span class="sxs-lookup"><span data-stu-id="0a93c-139">Response</span></span>
<span data-ttu-id="0a93c-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="0a93c-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



