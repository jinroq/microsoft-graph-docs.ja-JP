---
title: getの appstates 関数
description: まだ文書化されていません
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 575a1d7c33801f474a23451cac900d612dc5bf65
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/11/2019
ms.locfileid: "31809268"
---
# <a name="getrelatedappstates-function"></a><span data-ttu-id="ae87d-103">getの appstates 関数</span><span class="sxs-lookup"><span data-stu-id="ae87d-103">getRelatedAppStates function</span></span>

> <span data-ttu-id="ae87d-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ae87d-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ae87d-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="ae87d-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ae87d-106">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="ae87d-106">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ae87d-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="ae87d-107">Prerequisites</span></span>
<span data-ttu-id="ae87d-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="ae87d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ae87d-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="ae87d-110">Permission type</span></span>|<span data-ttu-id="ae87d-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="ae87d-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ae87d-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="ae87d-112">Delegated (work or school account)</span></span>|<span data-ttu-id="ae87d-113">DeviceManagementApps.ReadWrite.All、DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="ae87d-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="ae87d-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="ae87d-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ae87d-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ae87d-115">Not supported.</span></span>|
|<span data-ttu-id="ae87d-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="ae87d-116">Application</span></span>|<span data-ttu-id="ae87d-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ae87d-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ae87d-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="ae87d-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps/{mobileAppId}/getRelatedAppStates
GET /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app/getRelatedAppStates
GET /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app/getRelatedAppStates
```

## <a name="request-headers"></a><span data-ttu-id="ae87d-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="ae87d-119">Request headers</span></span>
|<span data-ttu-id="ae87d-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="ae87d-120">Header</span></span>|<span data-ttu-id="ae87d-121">値</span><span class="sxs-lookup"><span data-stu-id="ae87d-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ae87d-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="ae87d-122">Authorization</span></span>|<span data-ttu-id="ae87d-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="ae87d-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ae87d-124">承諾</span><span class="sxs-lookup"><span data-stu-id="ae87d-124">Accept</span></span>|<span data-ttu-id="ae87d-125">application/json</span><span class="sxs-lookup"><span data-stu-id="ae87d-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ae87d-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="ae87d-126">Request body</span></span>
<span data-ttu-id="ae87d-127">要求 URL で、次のクエリ パラメーターに値を指定します。</span><span class="sxs-lookup"><span data-stu-id="ae87d-127">In the request URL, provide the following query parameters with values.</span></span>
<span data-ttu-id="ae87d-128">次の表に、この関数で使用できるパラメーターを示します。</span><span class="sxs-lookup"><span data-stu-id="ae87d-128">The following table shows the parameters that can be used with this function.</span></span>

|<span data-ttu-id="ae87d-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="ae87d-129">Property</span></span>|<span data-ttu-id="ae87d-130">型</span><span class="sxs-lookup"><span data-stu-id="ae87d-130">Type</span></span>|<span data-ttu-id="ae87d-131">説明</span><span class="sxs-lookup"><span data-stu-id="ae87d-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ae87d-132">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="ae87d-132">userPrincipalName</span></span>|<span data-ttu-id="ae87d-133">String</span><span class="sxs-lookup"><span data-stu-id="ae87d-133">String</span></span>|<span data-ttu-id="ae87d-134">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="ae87d-134">Not yet documented</span></span>|
|<span data-ttu-id="ae87d-135">deviceId</span><span class="sxs-lookup"><span data-stu-id="ae87d-135">deviceId</span></span>|<span data-ttu-id="ae87d-136">String</span><span class="sxs-lookup"><span data-stu-id="ae87d-136">String</span></span>|<span data-ttu-id="ae87d-137">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="ae87d-137">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="ae87d-138">応答</span><span class="sxs-lookup"><span data-stu-id="ae87d-138">Response</span></span>
<span data-ttu-id="ae87d-139">成功した場合、この関数`200 OK`は応答コードと、応答本文で[mobileAppRelationshipState](../resources/intune-apps-mobileapprelationshipstate.md)コレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="ae87d-139">If successful, this function returns a `200 OK` response code and a [mobileAppRelationshipState](../resources/intune-apps-mobileapprelationshipstate.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ae87d-140">例</span><span class="sxs-lookup"><span data-stu-id="ae87d-140">Example</span></span>

### <a name="request"></a><span data-ttu-id="ae87d-141">要求</span><span class="sxs-lookup"><span data-stu-id="ae87d-141">Request</span></span>
<span data-ttu-id="ae87d-142">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="ae87d-142">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/getRelatedAppStates(userPrincipalName='parameterValue',deviceId='parameterValue')
```

### <a name="response"></a><span data-ttu-id="ae87d-143">応答</span><span class="sxs-lookup"><span data-stu-id="ae87d-143">Response</span></span>
<span data-ttu-id="ae87d-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="ae87d-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 481

{
  "value": [
    {
      "@odata.type": "microsoft.graph.mobileAppRelationshipState",
      "sourceIds": [
        "Source Ids value"
      ],
      "targetId": "Target Id value",
      "targetDisplayName": "Target Display Name value",
      "deviceId": "Device Id value",
      "installState": "failed",
      "installStateDetail": "dependencyFailedToInstall",
      "errorCode": 9,
      "targetLastSyncDateTime": "2017-01-01T00:02:09.7809949-08:00"
    }
  ]
}
```




