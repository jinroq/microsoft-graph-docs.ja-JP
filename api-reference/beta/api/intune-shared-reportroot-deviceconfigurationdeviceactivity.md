---
title: deviceConfigurationDeviceActivity 関数
description: デバイス構成のデバイス アクティビティ レポートのメタデータ
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: e73b6158d54872e4cae84b18e9a2d42571efbb31
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29404807"
---
# <a name="deviceconfigurationdeviceactivity-function"></a><span data-ttu-id="a9369-103">deviceConfigurationDeviceActivity 関数</span><span class="sxs-lookup"><span data-stu-id="a9369-103">deviceConfigurationDeviceActivity function</span></span>

> <span data-ttu-id="a9369-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="a9369-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="a9369-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a9369-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="a9369-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="a9369-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a9369-107">デバイス構成のデバイス アクティビティ レポートのメタデータ</span><span class="sxs-lookup"><span data-stu-id="a9369-107">Metadata for the device configuration device activity report</span></span>
## <a name="prerequisites"></a><span data-ttu-id="a9369-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="a9369-108">Prerequisites</span></span>
<span data-ttu-id="a9369-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="a9369-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a9369-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="a9369-111">Permission type</span></span>|<span data-ttu-id="a9369-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="a9369-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a9369-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="a9369-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="a9369-114">&nbsp; &nbsp; **デバイス構成**</span><span class="sxs-lookup"><span data-stu-id="a9369-114">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="a9369-115">DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="a9369-115">DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="a9369-116">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="a9369-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a9369-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a9369-117">Not supported.</span></span>|
|<span data-ttu-id="a9369-118">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="a9369-118">Application</span></span>|<span data-ttu-id="a9369-119">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a9369-119">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a9369-120">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="a9369-120">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /reports/deviceConfigurationDeviceActivity
```

## <a name="request-headers"></a><span data-ttu-id="a9369-121">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="a9369-121">Request headers</span></span>
|<span data-ttu-id="a9369-122">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="a9369-122">Header</span></span>|<span data-ttu-id="a9369-123">値</span><span class="sxs-lookup"><span data-stu-id="a9369-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a9369-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="a9369-124">Authorization</span></span>|<span data-ttu-id="a9369-125">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="a9369-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a9369-126">Accept</span><span class="sxs-lookup"><span data-stu-id="a9369-126">Accept</span></span>|<span data-ttu-id="a9369-127">application/json</span><span class="sxs-lookup"><span data-stu-id="a9369-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a9369-128">要求本文</span><span class="sxs-lookup"><span data-stu-id="a9369-128">Request body</span></span>
<span data-ttu-id="a9369-129">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="a9369-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a9369-130">応答</span><span class="sxs-lookup"><span data-stu-id="a9369-130">Response</span></span>
<span data-ttu-id="a9369-131">成功した場合、この関数は `200 OK` 応答コードと、応答本文で [report](../resources/intune-shared-report.md) を返します。</span><span class="sxs-lookup"><span data-stu-id="a9369-131">If successful, this function returns a `200 OK` response code and a [report](../resources/intune-shared-report.md) in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a9369-132">例</span><span class="sxs-lookup"><span data-stu-id="a9369-132">Example</span></span>
### <a name="request"></a><span data-ttu-id="a9369-133">要求</span><span class="sxs-lookup"><span data-stu-id="a9369-133">Request</span></span>
<span data-ttu-id="a9369-134">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="a9369-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/reports/deviceConfigurationDeviceActivity
```

### <a name="response"></a><span data-ttu-id="a9369-135">応答</span><span class="sxs-lookup"><span data-stu-id="a9369-135">Response</span></span>
<span data-ttu-id="a9369-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="a9369-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 123

{
  "value": {
    "@odata.type": "microsoft.graph.report",
    "content": "<Unknown Primitive Type Edm.Stream>"
  }
}
```



