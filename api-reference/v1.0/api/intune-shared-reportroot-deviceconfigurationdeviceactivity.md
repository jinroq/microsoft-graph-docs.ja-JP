---
title: deviceConfigurationDeviceActivity 関数
description: デバイス構成のデバイス アクティビティ レポートのメタデータ
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 7bbe0531df6f4a975fd9192838339ca424650c04
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27867705"
---
# <a name="deviceconfigurationdeviceactivity-function"></a><span data-ttu-id="22200-103">deviceConfigurationDeviceActivity 関数</span><span class="sxs-lookup"><span data-stu-id="22200-103">deviceConfigurationDeviceActivity function</span></span>

> <span data-ttu-id="22200-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="22200-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="22200-105">デバイス構成のデバイス アクティビティ レポートのメタデータ</span><span class="sxs-lookup"><span data-stu-id="22200-105">Metadata for the device configuration device activity report</span></span>

## <a name="prerequisites"></a><span data-ttu-id="22200-106">前提条件</span><span class="sxs-lookup"><span data-stu-id="22200-106">Prerequisites</span></span>
<span data-ttu-id="22200-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="22200-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="22200-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="22200-109">Permission type</span></span>|<span data-ttu-id="22200-110">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="22200-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="22200-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="22200-111">Delegated (work or school account)</span></span>||
| <span data-ttu-id="22200-112">&nbsp;&nbsp;デバイスの構成</span><span class="sxs-lookup"><span data-stu-id="22200-112">&nbsp; &nbsp; Device configuration</span></span> | <span data-ttu-id="22200-113">DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="22200-113">DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="22200-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="22200-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="22200-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="22200-115">Not supported.</span></span>|
|<span data-ttu-id="22200-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="22200-116">Application</span></span>|<span data-ttu-id="22200-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="22200-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="22200-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="22200-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /reports/deviceConfigurationDeviceActivity
```

## <a name="request-headers"></a><span data-ttu-id="22200-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="22200-119">Request headers</span></span>
|<span data-ttu-id="22200-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="22200-120">Header</span></span>|<span data-ttu-id="22200-121">値</span><span class="sxs-lookup"><span data-stu-id="22200-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="22200-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="22200-122">Authorization</span></span>|<span data-ttu-id="22200-123">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="22200-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="22200-124">Accept</span><span class="sxs-lookup"><span data-stu-id="22200-124">Accept</span></span>|<span data-ttu-id="22200-125">application/json</span><span class="sxs-lookup"><span data-stu-id="22200-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="22200-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="22200-126">Request body</span></span>
<span data-ttu-id="22200-127">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="22200-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="22200-128">応答</span><span class="sxs-lookup"><span data-stu-id="22200-128">Response</span></span>
<span data-ttu-id="22200-129">成功した場合、この関数は `200 OK` 応答コードと、応答本文で [report](../resources/intune-shared-report.md) を返します。</span><span class="sxs-lookup"><span data-stu-id="22200-129">If successful, this function returns a `200 OK` response code and a [report](../resources/intune-shared-report.md) in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="22200-130">例</span><span class="sxs-lookup"><span data-stu-id="22200-130">Example</span></span>
### <a name="request"></a><span data-ttu-id="22200-131">要求</span><span class="sxs-lookup"><span data-stu-id="22200-131">Request</span></span>
<span data-ttu-id="22200-132">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="22200-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/reports/deviceConfigurationDeviceActivity
```

### <a name="response"></a><span data-ttu-id="22200-133">応答</span><span class="sxs-lookup"><span data-stu-id="22200-133">Response</span></span>
<span data-ttu-id="22200-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="22200-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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








