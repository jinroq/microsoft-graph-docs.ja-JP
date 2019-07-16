---
title: exportDeviceAndAppManagementData 関数
description: まだ文書化されていません
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 9fd7b9ddcf82ce8ec65e2e58d97ea1a8b08f2ea7
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35741462"
---
# <a name="exportdeviceandappmanagementdata-function"></a><span data-ttu-id="d2b45-103">exportDeviceAndAppManagementData 関数</span><span class="sxs-lookup"><span data-stu-id="d2b45-103">exportDeviceAndAppManagementData function</span></span>

> <span data-ttu-id="d2b45-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d2b45-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d2b45-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="d2b45-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d2b45-106">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="d2b45-106">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d2b45-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="d2b45-107">Prerequisites</span></span>
<span data-ttu-id="d2b45-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="d2b45-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d2b45-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="d2b45-110">Permission type</span></span>|<span data-ttu-id="d2b45-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="d2b45-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d2b45-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="d2b45-112">Delegated (work or school account)</span></span>|<span data-ttu-id="d2b45-113">DeviceManagementServiceConfig.ReadWrite.All、DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="d2b45-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="d2b45-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="d2b45-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d2b45-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d2b45-115">Not supported.</span></span>|
|<span data-ttu-id="d2b45-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="d2b45-116">Application</span></span>|<span data-ttu-id="d2b45-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d2b45-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d2b45-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="d2b45-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /users/{usersId}/exportDeviceAndAppManagementData
```

## <a name="request-headers"></a><span data-ttu-id="d2b45-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="d2b45-119">Request headers</span></span>
|<span data-ttu-id="d2b45-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="d2b45-120">Header</span></span>|<span data-ttu-id="d2b45-121">値</span><span class="sxs-lookup"><span data-stu-id="d2b45-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d2b45-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="d2b45-122">Authorization</span></span>|<span data-ttu-id="d2b45-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="d2b45-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d2b45-124">承諾</span><span class="sxs-lookup"><span data-stu-id="d2b45-124">Accept</span></span>|<span data-ttu-id="d2b45-125">application/json</span><span class="sxs-lookup"><span data-stu-id="d2b45-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d2b45-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="d2b45-126">Request body</span></span>
<span data-ttu-id="d2b45-127">要求 URL で、次のクエリ パラメーターに値を指定します。</span><span class="sxs-lookup"><span data-stu-id="d2b45-127">In the request URL, provide the following query parameters with values.</span></span>
<span data-ttu-id="d2b45-128">次の表に、この関数で使用できるパラメーターを示します。</span><span class="sxs-lookup"><span data-stu-id="d2b45-128">The following table shows the parameters that can be used with this function.</span></span>

|<span data-ttu-id="d2b45-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="d2b45-129">Property</span></span>|<span data-ttu-id="d2b45-130">型</span><span class="sxs-lookup"><span data-stu-id="d2b45-130">Type</span></span>|<span data-ttu-id="d2b45-131">説明</span><span class="sxs-lookup"><span data-stu-id="d2b45-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d2b45-132">skip</span><span class="sxs-lookup"><span data-stu-id="d2b45-132">skip</span></span>|<span data-ttu-id="d2b45-133">Int32</span><span class="sxs-lookup"><span data-stu-id="d2b45-133">Int32</span></span>|<span data-ttu-id="d2b45-134">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="d2b45-134">Not yet documented</span></span>|
|<span data-ttu-id="d2b45-135">top</span><span class="sxs-lookup"><span data-stu-id="d2b45-135">top</span></span>|<span data-ttu-id="d2b45-136">Int32</span><span class="sxs-lookup"><span data-stu-id="d2b45-136">Int32</span></span>|<span data-ttu-id="d2b45-137">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="d2b45-137">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="d2b45-138">応答</span><span class="sxs-lookup"><span data-stu-id="d2b45-138">Response</span></span>
<span data-ttu-id="d2b45-139">成功した場合、この関数`200 OK`は応答コードと、応答本文で[Deviceandappmanagementdata](../resources/intune-onboarding-deviceandappmanagementdata.md)を返します。</span><span class="sxs-lookup"><span data-stu-id="d2b45-139">If successful, this function returns a `200 OK` response code and a [deviceAndAppManagementData](../resources/intune-onboarding-deviceandappmanagementdata.md) in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d2b45-140">例</span><span class="sxs-lookup"><span data-stu-id="d2b45-140">Example</span></span>

### <a name="request"></a><span data-ttu-id="d2b45-141">要求</span><span class="sxs-lookup"><span data-stu-id="d2b45-141">Request</span></span>
<span data-ttu-id="d2b45-142">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="d2b45-142">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/users/{usersId}/exportDeviceAndAppManagementData(skip=4,top=3)
```

### <a name="response"></a><span data-ttu-id="d2b45-143">応答</span><span class="sxs-lookup"><span data-stu-id="d2b45-143">Response</span></span>
<span data-ttu-id="d2b45-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="d2b45-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 143

{
  "value": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementData",
    "content": "<Unknown Primitive Type Edm.Stream>"
  }
}
```





