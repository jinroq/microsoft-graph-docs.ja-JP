---
title: exportdeviceandappmanagementdata 関数
description: まだ文書化されていません
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: e36936710bcd97c10c4a69c496cf56ceffa43e46
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/29/2019
ms.locfileid: "30961743"
---
# <a name="exportdeviceandappmanagementdata-function"></a><span data-ttu-id="34597-103">exportdeviceandappmanagementdata 関数</span><span class="sxs-lookup"><span data-stu-id="34597-103">exportDeviceAndAppManagementData function</span></span>

> <span data-ttu-id="34597-104">**重要:** Microsoft Graph の/ベータ版の api は変更される可能性があります。</span><span class="sxs-lookup"><span data-stu-id="34597-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="34597-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="34597-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="34597-106">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="34597-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="34597-107">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="34597-107">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="34597-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="34597-108">Prerequisites</span></span>

<span data-ttu-id="34597-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="34597-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="34597-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="34597-111">Permission type</span></span>|<span data-ttu-id="34597-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="34597-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="34597-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="34597-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="34597-114">&nbsp; &nbsp; **オンボーディング**</span><span class="sxs-lookup"><span data-stu-id="34597-114">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="34597-115">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="34597-115">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="34597-116">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="34597-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="34597-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="34597-117">Not supported.</span></span>|
|<span data-ttu-id="34597-118">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="34597-118">Application</span></span>|<span data-ttu-id="34597-119">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="34597-119">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="34597-120">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="34597-120">HTTP Request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /users/{usersId}/exportDeviceAndAppManagementData
```

## <a name="request-headers"></a><span data-ttu-id="34597-121">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="34597-121">Request headers</span></span>

|<span data-ttu-id="34597-122">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="34597-122">Header</span></span>|<span data-ttu-id="34597-123">値</span><span class="sxs-lookup"><span data-stu-id="34597-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="34597-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="34597-124">Authorization</span></span>|<span data-ttu-id="34597-125">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="34597-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="34597-126">承諾</span><span class="sxs-lookup"><span data-stu-id="34597-126">Accept</span></span>|<span data-ttu-id="34597-127">application/json</span><span class="sxs-lookup"><span data-stu-id="34597-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="34597-128">要求本文</span><span class="sxs-lookup"><span data-stu-id="34597-128">Request body</span></span>

<span data-ttu-id="34597-129">次の表に、この関数で使用できるパラメーターを示します。</span><span class="sxs-lookup"><span data-stu-id="34597-129">The following table shows the parameters that can be used with this function.</span></span>

|<span data-ttu-id="34597-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="34597-130">Property</span></span>|<span data-ttu-id="34597-131">型</span><span class="sxs-lookup"><span data-stu-id="34597-131">Type</span></span>|<span data-ttu-id="34597-132">説明</span><span class="sxs-lookup"><span data-stu-id="34597-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="34597-133">skip</span><span class="sxs-lookup"><span data-stu-id="34597-133">skip</span></span>|<span data-ttu-id="34597-134">Int32</span><span class="sxs-lookup"><span data-stu-id="34597-134">Int32</span></span>|<span data-ttu-id="34597-135">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="34597-135">Not yet documented</span></span>|
|<span data-ttu-id="34597-136">top</span><span class="sxs-lookup"><span data-stu-id="34597-136">top</span></span>|<span data-ttu-id="34597-137">Int32</span><span class="sxs-lookup"><span data-stu-id="34597-137">Int32</span></span>|<span data-ttu-id="34597-138">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="34597-138">Not yet documented</span></span>|

## <a name="response"></a><span data-ttu-id="34597-139">応答</span><span class="sxs-lookup"><span data-stu-id="34597-139">Response</span></span>

<span data-ttu-id="34597-140">成功した場合、この関数`200 OK`は応答コードと、応答本文で[deviceandappmanagementdata](../resources/intune-onboarding-deviceandappmanagementdata.md)を返します。</span><span class="sxs-lookup"><span data-stu-id="34597-140">If successful, this function returns a `200 OK` response code and a [deviceAndAppManagementData](../resources/intune-onboarding-deviceandappmanagementdata.md) in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="34597-141">例</span><span class="sxs-lookup"><span data-stu-id="34597-141">Example</span></span>

### <a name="request"></a><span data-ttu-id="34597-142">要求</span><span class="sxs-lookup"><span data-stu-id="34597-142">Request</span></span>

<span data-ttu-id="34597-143">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="34597-143">Here is an example of the request.</span></span>

``` http
GET https://graph.microsoft.com/beta/users/{usersId}/exportDeviceAndAppManagementData(skip=4,top=3)
```

### <a name="response"></a><span data-ttu-id="34597-144">応答</span><span class="sxs-lookup"><span data-stu-id="34597-144">Response</span></span>

<span data-ttu-id="34597-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="34597-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

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



