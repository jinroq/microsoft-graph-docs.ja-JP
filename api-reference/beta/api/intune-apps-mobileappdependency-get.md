---
title: mobileAppDependency を取得する
description: mobileAppDependency オブジェクトのプロパティとリレーションシップを読み取ります。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: add44c591da6b0a970eedd800822191ef215ef6d
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/11/2019
ms.locfileid: "31809402"
---
# <a name="get-mobileappdependency"></a><span data-ttu-id="aaced-103">mobileAppDependency を取得する</span><span class="sxs-lookup"><span data-stu-id="aaced-103">Get mobileAppDependency</span></span>

> <span data-ttu-id="aaced-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="aaced-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="aaced-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="aaced-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="aaced-106">[mobileAppDependency](../resources/intune-apps-mobileappdependency.md)オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="aaced-106">Read properties and relationships of the [mobileAppDependency](../resources/intune-apps-mobileappdependency.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="aaced-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="aaced-107">Prerequisites</span></span>
<span data-ttu-id="aaced-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="aaced-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="aaced-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="aaced-110">Permission type</span></span>|<span data-ttu-id="aaced-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="aaced-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="aaced-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="aaced-112">Delegated (work or school account)</span></span>|<span data-ttu-id="aaced-113">DeviceManagementApps.ReadWrite.All、DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="aaced-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="aaced-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="aaced-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="aaced-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="aaced-115">Not supported.</span></span>|
|<span data-ttu-id="aaced-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="aaced-116">Application</span></span>|<span data-ttu-id="aaced-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="aaced-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="aaced-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="aaced-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps/{mobileAppId}/relationships/{mobileAppRelationshipId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="aaced-119">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="aaced-119">Optional query parameters</span></span>
<span data-ttu-id="aaced-120">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://docs.microsoft.com/en-us/graph/query-parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="aaced-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="aaced-121">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="aaced-121">Request headers</span></span>
|<span data-ttu-id="aaced-122">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="aaced-122">Header</span></span>|<span data-ttu-id="aaced-123">値</span><span class="sxs-lookup"><span data-stu-id="aaced-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="aaced-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="aaced-124">Authorization</span></span>|<span data-ttu-id="aaced-125">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="aaced-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="aaced-126">承諾</span><span class="sxs-lookup"><span data-stu-id="aaced-126">Accept</span></span>|<span data-ttu-id="aaced-127">application/json</span><span class="sxs-lookup"><span data-stu-id="aaced-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="aaced-128">要求本文</span><span class="sxs-lookup"><span data-stu-id="aaced-128">Request body</span></span>
<span data-ttu-id="aaced-129">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="aaced-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="aaced-130">応答</span><span class="sxs-lookup"><span data-stu-id="aaced-130">Response</span></span>
<span data-ttu-id="aaced-131">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で[mobileAppDependency](../resources/intune-apps-mobileappdependency.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="aaced-131">If successful, this method returns a `200 OK` response code and [mobileAppDependency](../resources/intune-apps-mobileappdependency.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="aaced-132">例</span><span class="sxs-lookup"><span data-stu-id="aaced-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="aaced-133">要求</span><span class="sxs-lookup"><span data-stu-id="aaced-133">Request</span></span>
<span data-ttu-id="aaced-134">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="aaced-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/relationships/{mobileAppRelationshipId}
```

### <a name="response"></a><span data-ttu-id="aaced-135">応答</span><span class="sxs-lookup"><span data-stu-id="aaced-135">Response</span></span>
<span data-ttu-id="aaced-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="aaced-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 291

{
  "value": {
    "@odata.type": "#microsoft.graph.mobileAppDependency",
    "id": "c7f6f9ab-f9ab-c7f6-abf9-f6c7abf9f6c7",
    "targetId": "Target Id value",
    "targetDisplayName": "Target Display Name value",
    "dependencyType": "autoInstall",
    "dependentAppCount": 1
  }
}
```




