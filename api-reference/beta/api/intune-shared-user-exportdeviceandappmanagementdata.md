---
title: exportDeviceAndAppManagementData 関数
description: まだ文書化されていません
author: rolyon
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 84a58a07778de1b932253bd994e1bcc1456b9187
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35984147"
---
# <a name="exportdeviceandappmanagementdata-function"></a><span data-ttu-id="0ea0a-103">exportDeviceAndAppManagementData 関数</span><span class="sxs-lookup"><span data-stu-id="0ea0a-103">exportDeviceAndAppManagementData function</span></span>

> <span data-ttu-id="0ea0a-104">**重要:** Microsoft Graph の/ベータ版の Api は変更される可能性があります。</span><span class="sxs-lookup"><span data-stu-id="0ea0a-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="0ea0a-105">実稼働アプリケーションでは、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="0ea0a-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="0ea0a-106">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="0ea0a-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0ea0a-107">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="0ea0a-107">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="0ea0a-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="0ea0a-108">Prerequisites</span></span>

<span data-ttu-id="0ea0a-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="0ea0a-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0ea0a-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="0ea0a-111">Permission type</span></span>|<span data-ttu-id="0ea0a-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="0ea0a-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0ea0a-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="0ea0a-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="0ea0a-114">&nbsp; &nbsp; **オンボーディング**</span><span class="sxs-lookup"><span data-stu-id="0ea0a-114">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="0ea0a-115">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0ea0a-115">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="0ea0a-116">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="0ea0a-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0ea0a-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="0ea0a-117">Not supported.</span></span>|
|<span data-ttu-id="0ea0a-118">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="0ea0a-118">Application</span></span>|<span data-ttu-id="0ea0a-119">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="0ea0a-119">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="0ea0a-120">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="0ea0a-120">HTTP Request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /users/{usersId}/exportDeviceAndAppManagementData
```

## <a name="request-headers"></a><span data-ttu-id="0ea0a-121">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="0ea0a-121">Request headers</span></span>

|<span data-ttu-id="0ea0a-122">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="0ea0a-122">Header</span></span>|<span data-ttu-id="0ea0a-123">値</span><span class="sxs-lookup"><span data-stu-id="0ea0a-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0ea0a-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="0ea0a-124">Authorization</span></span>|<span data-ttu-id="0ea0a-125">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="0ea0a-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0ea0a-126">承諾</span><span class="sxs-lookup"><span data-stu-id="0ea0a-126">Accept</span></span>|<span data-ttu-id="0ea0a-127">application/json</span><span class="sxs-lookup"><span data-stu-id="0ea0a-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0ea0a-128">要求本文</span><span class="sxs-lookup"><span data-stu-id="0ea0a-128">Request body</span></span>

<span data-ttu-id="0ea0a-129">次の表に、この関数で使用できるパラメーターを示します。</span><span class="sxs-lookup"><span data-stu-id="0ea0a-129">The following table shows the parameters that can be used with this function.</span></span>

|<span data-ttu-id="0ea0a-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="0ea0a-130">Property</span></span>|<span data-ttu-id="0ea0a-131">型</span><span class="sxs-lookup"><span data-stu-id="0ea0a-131">Type</span></span>|<span data-ttu-id="0ea0a-132">説明</span><span class="sxs-lookup"><span data-stu-id="0ea0a-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0ea0a-133">skip</span><span class="sxs-lookup"><span data-stu-id="0ea0a-133">skip</span></span>|<span data-ttu-id="0ea0a-134">Int32</span><span class="sxs-lookup"><span data-stu-id="0ea0a-134">Int32</span></span>|<span data-ttu-id="0ea0a-135">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="0ea0a-135">Not yet documented</span></span>|
|<span data-ttu-id="0ea0a-136">top</span><span class="sxs-lookup"><span data-stu-id="0ea0a-136">top</span></span>|<span data-ttu-id="0ea0a-137">Int32</span><span class="sxs-lookup"><span data-stu-id="0ea0a-137">Int32</span></span>|<span data-ttu-id="0ea0a-138">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="0ea0a-138">Not yet documented</span></span>|

## <a name="response"></a><span data-ttu-id="0ea0a-139">応答</span><span class="sxs-lookup"><span data-stu-id="0ea0a-139">Response</span></span>

<span data-ttu-id="0ea0a-140">成功した場合、この関数`200 OK`は応答コードと、応答本文で[Deviceandappmanagementdata](../resources/intune-onboarding-deviceandappmanagementdata.md)を返します。</span><span class="sxs-lookup"><span data-stu-id="0ea0a-140">If successful, this function returns a `200 OK` response code and a [deviceAndAppManagementData](../resources/intune-onboarding-deviceandappmanagementdata.md) in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0ea0a-141">例</span><span class="sxs-lookup"><span data-stu-id="0ea0a-141">Example</span></span>

### <a name="request"></a><span data-ttu-id="0ea0a-142">要求</span><span class="sxs-lookup"><span data-stu-id="0ea0a-142">Request</span></span>

<span data-ttu-id="0ea0a-143">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="0ea0a-143">Here is an example of the request.</span></span>

``` http
GET https://graph.microsoft.com/beta/users/{usersId}/exportDeviceAndAppManagementData(skip=4,top=3)
```

### <a name="response"></a><span data-ttu-id="0ea0a-144">応答</span><span class="sxs-lookup"><span data-stu-id="0ea0a-144">Response</span></span>

<span data-ttu-id="0ea0a-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="0ea0a-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

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



