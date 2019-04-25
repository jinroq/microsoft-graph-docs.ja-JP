---
title: getManagedDevicesWithAppFailures 関数
description: エラーが発生したアプリを含むデバイスの一覧を取得します
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: d4f2800a187c62c1c6a894817f2405f88c6356d0
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32526840"
---
# <a name="getmanageddeviceswithappfailures-function"></a><span data-ttu-id="ce5da-103">getManagedDevicesWithAppFailures 関数</span><span class="sxs-lookup"><span data-stu-id="ce5da-103">getManagedDevicesWithAppFailures function</span></span>

> <span data-ttu-id="ce5da-104">**重要:** Microsoft Graph の/ベータ版の api は変更される可能性があります。</span><span class="sxs-lookup"><span data-stu-id="ce5da-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="ce5da-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ce5da-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="ce5da-106">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="ce5da-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ce5da-107">エラーが発生したアプリを含むデバイスの一覧を取得します</span><span class="sxs-lookup"><span data-stu-id="ce5da-107">Retrieves the list of devices with failed apps</span></span>
## <a name="prerequisites"></a><span data-ttu-id="ce5da-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="ce5da-108">Prerequisites</span></span>
<span data-ttu-id="ce5da-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="ce5da-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ce5da-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="ce5da-111">Permission type</span></span>|<span data-ttu-id="ce5da-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="ce5da-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ce5da-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="ce5da-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="ce5da-114">&nbsp; &nbsp; **トラブルシューティング**</span><span class="sxs-lookup"><span data-stu-id="ce5da-114">&nbsp; &nbsp; **Troubleshooting**</span></span> | <span data-ttu-id="ce5da-115">DeviceManagementManagedDevices.ReadWrite.All、DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="ce5da-115">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="ce5da-116">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="ce5da-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ce5da-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ce5da-117">Not supported.</span></span>|
|<span data-ttu-id="ce5da-118">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="ce5da-118">Application</span></span>|<span data-ttu-id="ce5da-119">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ce5da-119">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ce5da-120">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="ce5da-120">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /users/{usersId}/getManagedDevicesWithAppFailures
```

## <a name="request-headers"></a><span data-ttu-id="ce5da-121">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="ce5da-121">Request headers</span></span>
|<span data-ttu-id="ce5da-122">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="ce5da-122">Header</span></span>|<span data-ttu-id="ce5da-123">値</span><span class="sxs-lookup"><span data-stu-id="ce5da-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ce5da-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="ce5da-124">Authorization</span></span>|<span data-ttu-id="ce5da-125">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="ce5da-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ce5da-126">承諾</span><span class="sxs-lookup"><span data-stu-id="ce5da-126">Accept</span></span>|<span data-ttu-id="ce5da-127">application/json</span><span class="sxs-lookup"><span data-stu-id="ce5da-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ce5da-128">要求本文</span><span class="sxs-lookup"><span data-stu-id="ce5da-128">Request body</span></span>
<span data-ttu-id="ce5da-129">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="ce5da-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ce5da-130">応答</span><span class="sxs-lookup"><span data-stu-id="ce5da-130">Response</span></span>
<span data-ttu-id="ce5da-131">成功した場合、この関数は `200 OK` 応答コードと、応答本文で文字列コレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="ce5da-131">If successful, this function returns a `200 OK` response code and a String collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ce5da-132">例</span><span class="sxs-lookup"><span data-stu-id="ce5da-132">Example</span></span>
### <a name="request"></a><span data-ttu-id="ce5da-133">要求</span><span class="sxs-lookup"><span data-stu-id="ce5da-133">Request</span></span>
<span data-ttu-id="ce5da-134">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="ce5da-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/users/{usersId}/getManagedDevicesWithAppFailures
```

### <a name="response"></a><span data-ttu-id="ce5da-135">応答</span><span class="sxs-lookup"><span data-stu-id="ce5da-135">Response</span></span>
<span data-ttu-id="ce5da-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="ce5da-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





