---
title: deviceConfigurationDeviceActivity 関数
description: デバイス構成のデバイス アクティビティ レポートのメタデータ
author: tfitzmac
ms.openlocfilehash: 978ba8d3031f0c8f2bfcbbe6efbbc4433063a1a3
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27326069"
---
# <a name="deviceconfigurationdeviceactivity-function"></a><span data-ttu-id="1cffd-103">deviceConfigurationDeviceActivity 関数</span><span class="sxs-lookup"><span data-stu-id="1cffd-103">deviceConfigurationDeviceActivity function</span></span>

> <span data-ttu-id="1cffd-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="1cffd-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="1cffd-105">デバイス構成のデバイス アクティビティ レポートのメタデータ</span><span class="sxs-lookup"><span data-stu-id="1cffd-105">Metadata for the device configuration device activity report</span></span>

## <a name="prerequisites"></a><span data-ttu-id="1cffd-106">前提条件</span><span class="sxs-lookup"><span data-stu-id="1cffd-106">Prerequisites</span></span>
<span data-ttu-id="1cffd-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="1cffd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1cffd-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="1cffd-109">Permission type</span></span>|<span data-ttu-id="1cffd-110">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="1cffd-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1cffd-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="1cffd-111">Delegated (work or school account)</span></span>||
| <span data-ttu-id="1cffd-112">&nbsp;&nbsp;デバイスの構成</span><span class="sxs-lookup"><span data-stu-id="1cffd-112">&nbsp; &nbsp; Device configuration</span></span> | <span data-ttu-id="1cffd-113">DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="1cffd-113">DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="1cffd-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="1cffd-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1cffd-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="1cffd-115">Not supported.</span></span>|
|<span data-ttu-id="1cffd-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="1cffd-116">Application</span></span>|<span data-ttu-id="1cffd-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="1cffd-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="1cffd-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="1cffd-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /reports/deviceConfigurationDeviceActivity
```

## <a name="request-headers"></a><span data-ttu-id="1cffd-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="1cffd-119">Request headers</span></span>
|<span data-ttu-id="1cffd-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="1cffd-120">Header</span></span>|<span data-ttu-id="1cffd-121">値</span><span class="sxs-lookup"><span data-stu-id="1cffd-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1cffd-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="1cffd-122">Authorization</span></span>|<span data-ttu-id="1cffd-123">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="1cffd-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1cffd-124">Accept</span><span class="sxs-lookup"><span data-stu-id="1cffd-124">Accept</span></span>|<span data-ttu-id="1cffd-125">application/json</span><span class="sxs-lookup"><span data-stu-id="1cffd-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1cffd-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="1cffd-126">Request body</span></span>
<span data-ttu-id="1cffd-127">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="1cffd-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1cffd-128">応答</span><span class="sxs-lookup"><span data-stu-id="1cffd-128">Response</span></span>
<span data-ttu-id="1cffd-129">成功した場合、この関数は `200 OK` 応答コードと、応答本文で [report](../resources/intune-shared-report.md) を返します。</span><span class="sxs-lookup"><span data-stu-id="1cffd-129">If successful, this function returns a `200 OK` response code and a [report](../resources/intune-shared-report.md) in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1cffd-130">例</span><span class="sxs-lookup"><span data-stu-id="1cffd-130">Example</span></span>
### <a name="request"></a><span data-ttu-id="1cffd-131">要求</span><span class="sxs-lookup"><span data-stu-id="1cffd-131">Request</span></span>
<span data-ttu-id="1cffd-132">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="1cffd-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/reports/deviceConfigurationDeviceActivity
```

### <a name="response"></a><span data-ttu-id="1cffd-133">応答</span><span class="sxs-lookup"><span data-stu-id="1cffd-133">Response</span></span>
<span data-ttu-id="1cffd-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="1cffd-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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








