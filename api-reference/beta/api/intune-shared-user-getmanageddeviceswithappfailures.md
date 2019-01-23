---
title: getManagedDevicesWithAppFailures 関数
description: 失敗したアプリを使用してデバイスの一覧を取得します。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: d4f2800a187c62c1c6a894817f2405f88c6356d0
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29396806"
---
# <a name="getmanageddeviceswithappfailures-function"></a><span data-ttu-id="2b0dd-103">getManagedDevicesWithAppFailures 関数</span><span class="sxs-lookup"><span data-stu-id="2b0dd-103">getManagedDevicesWithAppFailures function</span></span>

> <span data-ttu-id="2b0dd-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="2b0dd-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="2b0dd-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="2b0dd-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="2b0dd-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="2b0dd-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2b0dd-107">失敗したアプリを使用してデバイスの一覧を取得します。</span><span class="sxs-lookup"><span data-stu-id="2b0dd-107">Retrieves the list of devices with failed apps</span></span>
## <a name="prerequisites"></a><span data-ttu-id="2b0dd-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="2b0dd-108">Prerequisites</span></span>
<span data-ttu-id="2b0dd-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="2b0dd-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2b0dd-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="2b0dd-111">Permission type</span></span>|<span data-ttu-id="2b0dd-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="2b0dd-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2b0dd-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="2b0dd-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="2b0dd-114">&nbsp; &nbsp; **トラブルシューティング**</span><span class="sxs-lookup"><span data-stu-id="2b0dd-114">&nbsp; &nbsp; **Troubleshooting**</span></span> | <span data-ttu-id="2b0dd-115">DeviceManagementManagedDevices.ReadWrite.All、DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="2b0dd-115">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="2b0dd-116">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="2b0dd-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2b0dd-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="2b0dd-117">Not supported.</span></span>|
|<span data-ttu-id="2b0dd-118">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="2b0dd-118">Application</span></span>|<span data-ttu-id="2b0dd-119">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="2b0dd-119">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="2b0dd-120">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="2b0dd-120">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /users/{usersId}/getManagedDevicesWithAppFailures
```

## <a name="request-headers"></a><span data-ttu-id="2b0dd-121">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="2b0dd-121">Request headers</span></span>
|<span data-ttu-id="2b0dd-122">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="2b0dd-122">Header</span></span>|<span data-ttu-id="2b0dd-123">値</span><span class="sxs-lookup"><span data-stu-id="2b0dd-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2b0dd-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="2b0dd-124">Authorization</span></span>|<span data-ttu-id="2b0dd-125">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="2b0dd-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2b0dd-126">Accept</span><span class="sxs-lookup"><span data-stu-id="2b0dd-126">Accept</span></span>|<span data-ttu-id="2b0dd-127">application/json</span><span class="sxs-lookup"><span data-stu-id="2b0dd-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2b0dd-128">要求本文</span><span class="sxs-lookup"><span data-stu-id="2b0dd-128">Request body</span></span>
<span data-ttu-id="2b0dd-129">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="2b0dd-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2b0dd-130">応答</span><span class="sxs-lookup"><span data-stu-id="2b0dd-130">Response</span></span>
<span data-ttu-id="2b0dd-131">成功した場合、この関数は `200 OK` 応答コードと、応答本文で String コレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="2b0dd-131">If successful, this function returns a `200 OK` response code and a String collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2b0dd-132">例</span><span class="sxs-lookup"><span data-stu-id="2b0dd-132">Example</span></span>
### <a name="request"></a><span data-ttu-id="2b0dd-133">要求</span><span class="sxs-lookup"><span data-stu-id="2b0dd-133">Request</span></span>
<span data-ttu-id="2b0dd-134">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="2b0dd-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/users/{usersId}/getManagedDevicesWithAppFailures
```

### <a name="response"></a><span data-ttu-id="2b0dd-135">応答</span><span class="sxs-lookup"><span data-stu-id="2b0dd-135">Response</span></span>
<span data-ttu-id="2b0dd-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="2b0dd-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 74

{
  "value": [
    "Get Managed Devices With App Failures value"
  ]
}
```





