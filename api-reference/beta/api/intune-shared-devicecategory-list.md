---
title: deviceCategories のリスト
description: deviceCategory オブジェクトのプロパティとリレーションシップをリストします。
author: rolyon
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: e20c9f31c5174dfc60d8d589bae1a5f51de8972a
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/11/2019
ms.locfileid: "33898466"
---
# <a name="list-devicecategories"></a><span data-ttu-id="0e176-103">deviceCategories のリスト</span><span class="sxs-lookup"><span data-stu-id="0e176-103">List deviceCategories</span></span>

> <span data-ttu-id="0e176-104">**重要:** Microsoft Graph の/ベータ版の Api は変更される可能性があります。</span><span class="sxs-lookup"><span data-stu-id="0e176-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="0e176-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="0e176-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="0e176-106">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="0e176-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0e176-107">[deviceCategory](../resources/intune-shared-devicecategory.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="0e176-107">List properties and relationships of the [deviceCategory](../resources/intune-shared-devicecategory.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="0e176-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="0e176-108">Prerequisites</span></span>
<span data-ttu-id="0e176-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="0e176-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0e176-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="0e176-111">Permission type</span></span>|<span data-ttu-id="0e176-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="0e176-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0e176-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="0e176-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="0e176-114">&nbsp; &nbsp; **オンボーディング**</span><span class="sxs-lookup"><span data-stu-id="0e176-114">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="0e176-115">DeviceManagementManagedDevices.ReadWrite.All、DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="0e176-115">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="0e176-116">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="0e176-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0e176-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="0e176-117">Not supported.</span></span>|
|<span data-ttu-id="0e176-118">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="0e176-118">Application</span></span>|<span data-ttu-id="0e176-119">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="0e176-119">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="0e176-120">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="0e176-120">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceCategories
```

## <a name="request-headers"></a><span data-ttu-id="0e176-121">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="0e176-121">Request headers</span></span>

|<span data-ttu-id="0e176-122">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="0e176-122">Header</span></span>|<span data-ttu-id="0e176-123">値</span><span class="sxs-lookup"><span data-stu-id="0e176-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0e176-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="0e176-124">Authorization</span></span>|<span data-ttu-id="0e176-125">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="0e176-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0e176-126">承諾</span><span class="sxs-lookup"><span data-stu-id="0e176-126">Accept</span></span>|<span data-ttu-id="0e176-127">application/json</span><span class="sxs-lookup"><span data-stu-id="0e176-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0e176-128">要求本文</span><span class="sxs-lookup"><span data-stu-id="0e176-128">Request body</span></span>

<span data-ttu-id="0e176-129">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="0e176-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0e176-130">応答</span><span class="sxs-lookup"><span data-stu-id="0e176-130">Response</span></span>

<span data-ttu-id="0e176-131">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [deviceCategory](../resources/intune-shared-devicecategory.md) オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="0e176-131">If successful, this method returns a `200 OK` response code and a collection of [deviceCategory](../resources/intune-shared-devicecategory.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0e176-132">例</span><span class="sxs-lookup"><span data-stu-id="0e176-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="0e176-133">要求</span><span class="sxs-lookup"><span data-stu-id="0e176-133">Request</span></span>

<span data-ttu-id="0e176-134">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="0e176-134">Here is an example of the request.</span></span>

``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceCategories
```

### <a name="response"></a><span data-ttu-id="0e176-135">応答</span><span class="sxs-lookup"><span data-stu-id="0e176-135">Response</span></span>

<span data-ttu-id="0e176-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="0e176-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 233

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.deviceCategory",
      "id": "f881b841-b841-f881-41b8-81f841b881f8",
      "displayName": "Display Name value",
      "description": "Description value"
    }
  ]
}
```



