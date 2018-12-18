---
title: getManagedDevicesWithAppFailures 関数
description: 失敗したアプリを使用してデバイスの一覧を取得します。
author: tfitzmac
ms.openlocfilehash: 147ee26644c3e2c425f70434516e13b03407891b
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27352956"
---
# <a name="getmanageddeviceswithappfailures-function"></a><span data-ttu-id="1f16b-103">getManagedDevicesWithAppFailures 関数</span><span class="sxs-lookup"><span data-stu-id="1f16b-103">getManagedDevicesWithAppFailures function</span></span>

> <span data-ttu-id="1f16b-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="1f16b-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="1f16b-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="1f16b-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="1f16b-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="1f16b-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="1f16b-107">失敗したアプリを使用してデバイスの一覧を取得します。</span><span class="sxs-lookup"><span data-stu-id="1f16b-107">Retrieves the list of devices with failed apps</span></span>
## <a name="prerequisites"></a><span data-ttu-id="1f16b-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="1f16b-108">Prerequisites</span></span>
<span data-ttu-id="1f16b-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="1f16b-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1f16b-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="1f16b-111">Permission type</span></span>|<span data-ttu-id="1f16b-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="1f16b-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1f16b-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="1f16b-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="1f16b-114">&nbsp; &nbsp; **トラブルシューティング**</span><span class="sxs-lookup"><span data-stu-id="1f16b-114">&nbsp; &nbsp; **Troubleshooting**</span></span> | <span data-ttu-id="1f16b-115">DeviceManagementManagedDevices.ReadWrite.All、DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="1f16b-115">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="1f16b-116">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="1f16b-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1f16b-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="1f16b-117">Not supported.</span></span>|
|<span data-ttu-id="1f16b-118">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="1f16b-118">Application</span></span>|<span data-ttu-id="1f16b-119">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="1f16b-119">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="1f16b-120">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="1f16b-120">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /users/{usersId}/getManagedDevicesWithAppFailures
```

## <a name="request-headers"></a><span data-ttu-id="1f16b-121">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="1f16b-121">Request headers</span></span>
|<span data-ttu-id="1f16b-122">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="1f16b-122">Header</span></span>|<span data-ttu-id="1f16b-123">値</span><span class="sxs-lookup"><span data-stu-id="1f16b-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1f16b-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="1f16b-124">Authorization</span></span>|<span data-ttu-id="1f16b-125">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="1f16b-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1f16b-126">Accept</span><span class="sxs-lookup"><span data-stu-id="1f16b-126">Accept</span></span>|<span data-ttu-id="1f16b-127">application/json</span><span class="sxs-lookup"><span data-stu-id="1f16b-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1f16b-128">要求本文</span><span class="sxs-lookup"><span data-stu-id="1f16b-128">Request body</span></span>
<span data-ttu-id="1f16b-129">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="1f16b-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1f16b-130">応答</span><span class="sxs-lookup"><span data-stu-id="1f16b-130">Response</span></span>
<span data-ttu-id="1f16b-131">成功した場合、この関数は `200 OK` 応答コードと、応答本文で String コレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="1f16b-131">If successful, this function returns a `200 OK` response code and a String collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1f16b-132">例</span><span class="sxs-lookup"><span data-stu-id="1f16b-132">Example</span></span>
### <a name="request"></a><span data-ttu-id="1f16b-133">要求</span><span class="sxs-lookup"><span data-stu-id="1f16b-133">Request</span></span>
<span data-ttu-id="1f16b-134">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="1f16b-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/users/{usersId}/getManagedDevicesWithAppFailures
```

### <a name="response"></a><span data-ttu-id="1f16b-135">応答</span><span class="sxs-lookup"><span data-stu-id="1f16b-135">Response</span></span>
<span data-ttu-id="1f16b-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="1f16b-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





