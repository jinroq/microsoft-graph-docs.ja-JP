---
title: deviceConfigurationDeviceActivity 関数
description: デバイス構成のデバイス アクティビティ レポートのメタデータ
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: ef5a8367ec47242138cdf13cb30447c844bd050e
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27831757"
---
# <a name="deviceconfigurationdeviceactivity-function"></a><span data-ttu-id="4a1e7-103">deviceConfigurationDeviceActivity 関数</span><span class="sxs-lookup"><span data-stu-id="4a1e7-103">deviceConfigurationDeviceActivity function</span></span>

> <span data-ttu-id="4a1e7-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="4a1e7-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="4a1e7-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="4a1e7-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="4a1e7-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="4a1e7-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="4a1e7-107">デバイス構成のデバイス アクティビティ レポートのメタデータ</span><span class="sxs-lookup"><span data-stu-id="4a1e7-107">Metadata for the device configuration device activity report</span></span>
## <a name="prerequisites"></a><span data-ttu-id="4a1e7-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="4a1e7-108">Prerequisites</span></span>
<span data-ttu-id="4a1e7-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="4a1e7-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4a1e7-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="4a1e7-111">Permission type</span></span>|<span data-ttu-id="4a1e7-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="4a1e7-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4a1e7-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="4a1e7-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="4a1e7-114">&nbsp; &nbsp; **デバイス構成**</span><span class="sxs-lookup"><span data-stu-id="4a1e7-114">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="4a1e7-115">DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="4a1e7-115">DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="4a1e7-116">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="4a1e7-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4a1e7-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="4a1e7-117">Not supported.</span></span>|
|<span data-ttu-id="4a1e7-118">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="4a1e7-118">Application</span></span>|<span data-ttu-id="4a1e7-119">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="4a1e7-119">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="4a1e7-120">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="4a1e7-120">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /reports/deviceConfigurationDeviceActivity
```

## <a name="request-headers"></a><span data-ttu-id="4a1e7-121">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="4a1e7-121">Request headers</span></span>
|<span data-ttu-id="4a1e7-122">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="4a1e7-122">Header</span></span>|<span data-ttu-id="4a1e7-123">値</span><span class="sxs-lookup"><span data-stu-id="4a1e7-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4a1e7-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="4a1e7-124">Authorization</span></span>|<span data-ttu-id="4a1e7-125">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="4a1e7-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4a1e7-126">Accept</span><span class="sxs-lookup"><span data-stu-id="4a1e7-126">Accept</span></span>|<span data-ttu-id="4a1e7-127">application/json</span><span class="sxs-lookup"><span data-stu-id="4a1e7-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4a1e7-128">要求本文</span><span class="sxs-lookup"><span data-stu-id="4a1e7-128">Request body</span></span>
<span data-ttu-id="4a1e7-129">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="4a1e7-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4a1e7-130">応答</span><span class="sxs-lookup"><span data-stu-id="4a1e7-130">Response</span></span>
<span data-ttu-id="4a1e7-131">成功した場合、この関数は `200 OK` 応答コードと、応答本文で [report](../resources/intune-shared-report.md) を返します。</span><span class="sxs-lookup"><span data-stu-id="4a1e7-131">If successful, this function returns a `200 OK` response code and a [report](../resources/intune-shared-report.md) in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4a1e7-132">例</span><span class="sxs-lookup"><span data-stu-id="4a1e7-132">Example</span></span>
### <a name="request"></a><span data-ttu-id="4a1e7-133">要求</span><span class="sxs-lookup"><span data-stu-id="4a1e7-133">Request</span></span>
<span data-ttu-id="4a1e7-134">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="4a1e7-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/reports/deviceConfigurationDeviceActivity
```

### <a name="response"></a><span data-ttu-id="4a1e7-135">応答</span><span class="sxs-lookup"><span data-stu-id="4a1e7-135">Response</span></span>
<span data-ttu-id="4a1e7-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="4a1e7-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



