---
title: Officeの変更の更新
description: オフィスのプロパティを更新します。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: e452a3743148b4767c1259d68746924d3b0675c4
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35726072"
---
# <a name="update-officeconfiguration"></a><span data-ttu-id="c823c-103">Officeの変更の更新</span><span class="sxs-lookup"><span data-stu-id="c823c-103">Update officeConfiguration</span></span>

> <span data-ttu-id="c823c-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c823c-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c823c-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="c823c-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c823c-106">[オフィス](../resources/intune-cirrus-officeconfiguration.md)のプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="c823c-106">Update the properties of a [officeConfiguration](../resources/intune-cirrus-officeconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c823c-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="c823c-107">Prerequisites</span></span>
<span data-ttu-id="c823c-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="c823c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c823c-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="c823c-110">Permission type</span></span>|<span data-ttu-id="c823c-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="c823c-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c823c-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="c823c-112">Delegated (work or school account)</span></span>|<span data-ttu-id="c823c-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c823c-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="c823c-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="c823c-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c823c-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c823c-115">Not supported.</span></span>|
|<span data-ttu-id="c823c-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="c823c-116">Application</span></span>|<span data-ttu-id="c823c-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c823c-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c823c-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="c823c-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /officeConfiguration
```

## <a name="request-headers"></a><span data-ttu-id="c823c-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="c823c-119">Request headers</span></span>
|<span data-ttu-id="c823c-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="c823c-120">Header</span></span>|<span data-ttu-id="c823c-121">値</span><span class="sxs-lookup"><span data-stu-id="c823c-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c823c-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="c823c-122">Authorization</span></span>|<span data-ttu-id="c823c-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="c823c-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c823c-124">承諾</span><span class="sxs-lookup"><span data-stu-id="c823c-124">Accept</span></span>|<span data-ttu-id="c823c-125">application/json</span><span class="sxs-lookup"><span data-stu-id="c823c-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c823c-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="c823c-126">Request body</span></span>
<span data-ttu-id="c823c-127">要求本文で、[オフィス](../resources/intune-cirrus-officeconfiguration.md)/備品の指定オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="c823c-127">In the request body, supply a JSON representation for the [officeConfiguration](../resources/intune-cirrus-officeconfiguration.md) object.</span></span>

<span data-ttu-id="c823c-128">次の表に、[[オフィス](../resources/intune-cirrus-officeconfiguration.md)] を作成するときに必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="c823c-128">The following table shows the properties that are required when you create the [officeConfiguration](../resources/intune-cirrus-officeconfiguration.md).</span></span>

|<span data-ttu-id="c823c-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="c823c-129">Property</span></span>|<span data-ttu-id="c823c-130">型</span><span class="sxs-lookup"><span data-stu-id="c823c-130">Type</span></span>|<span data-ttu-id="c823c-131">説明</span><span class="sxs-lookup"><span data-stu-id="c823c-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c823c-132">id</span><span class="sxs-lookup"><span data-stu-id="c823c-132">id</span></span>|<span data-ttu-id="c823c-133">String</span><span class="sxs-lookup"><span data-stu-id="c823c-133">String</span></span>|<span data-ttu-id="c823c-134">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="c823c-134">Not yet documented</span></span>|
|<span data-ttu-id="c823c-135">tenantCheckinStatuses</span><span class="sxs-lookup"><span data-stu-id="c823c-135">tenantCheckinStatuses</span></span>|<span data-ttu-id="c823c-136">[officeClientCheckinStatus](../resources/intune-cirrus-officeclientcheckinstatus.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="c823c-136">[officeClientCheckinStatus](../resources/intune-cirrus-officeclientcheckinstatus.md) collection</span></span>|<span data-ttu-id="c823c-137">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="c823c-137">Not yet documented</span></span>|
|<span data-ttu-id="c823c-138">tenantUserCheckinSummary</span><span class="sxs-lookup"><span data-stu-id="c823c-138">tenantUserCheckinSummary</span></span>|[<span data-ttu-id="c823c-139">officeUserCheckinSummary</span><span class="sxs-lookup"><span data-stu-id="c823c-139">officeUserCheckinSummary</span></span>](../resources/intune-cirrus-officeusercheckinsummary.md)|<span data-ttu-id="c823c-140">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="c823c-140">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="c823c-141">応答</span><span class="sxs-lookup"><span data-stu-id="c823c-141">Response</span></span>
<span data-ttu-id="c823c-142">成功した場合、このメソッド`200 OK`は応答コードと、 [](../resources/intune-cirrus-officeconfiguration.md)応答本文で更新された ime オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="c823c-142">If successful, this method returns a `200 OK` response code and an updated [officeConfiguration](../resources/intune-cirrus-officeconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c823c-143">例</span><span class="sxs-lookup"><span data-stu-id="c823c-143">Example</span></span>

### <a name="request"></a><span data-ttu-id="c823c-144">要求</span><span class="sxs-lookup"><span data-stu-id="c823c-144">Request</span></span>
<span data-ttu-id="c823c-145">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="c823c-145">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/officeConfiguration
Content-type: application/json
Content-length: 843

{
  "@odata.type": "#microsoft.graph.officeConfiguration",
  "tenantCheckinStatuses": [
    {
      "@odata.type": "microsoft.graph.officeClientCheckinStatus",
      "userId": "User Id value",
      "userPrincipalName": "User Principal Name value",
      "deviceName": "Device Name value",
      "devicePlatform": "Device Platform value",
      "devicePlatformVersion": "Device Platform Version value",
      "wasSuccessful": true,
      "checkinDateTime": "2016-12-31T23:56:33.9571764-08:00",
      "errorMessage": "Error Message value",
      "appliedPolicies": [
        "Applied Policies value"
      ],
      "lastTaskName": "Last Task Name value"
    }
  ],
  "tenantUserCheckinSummary": {
    "@odata.type": "microsoft.graph.officeUserCheckinSummary",
    "succeededUserCount": 2,
    "failedUserCount": 15
  }
}
```

### <a name="response"></a><span data-ttu-id="c823c-146">応答</span><span class="sxs-lookup"><span data-stu-id="c823c-146">Response</span></span>
<span data-ttu-id="c823c-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="c823c-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 892

{
  "@odata.type": "#microsoft.graph.officeConfiguration",
  "id": "4b5f7085-7085-4b5f-8570-5f4b85705f4b",
  "tenantCheckinStatuses": [
    {
      "@odata.type": "microsoft.graph.officeClientCheckinStatus",
      "userId": "User Id value",
      "userPrincipalName": "User Principal Name value",
      "deviceName": "Device Name value",
      "devicePlatform": "Device Platform value",
      "devicePlatformVersion": "Device Platform Version value",
      "wasSuccessful": true,
      "checkinDateTime": "2016-12-31T23:56:33.9571764-08:00",
      "errorMessage": "Error Message value",
      "appliedPolicies": [
        "Applied Policies value"
      ],
      "lastTaskName": "Last Task Name value"
    }
  ],
  "tenantUserCheckinSummary": {
    "@odata.type": "microsoft.graph.officeUserCheckinSummary",
    "succeededUserCount": 2,
    "failedUserCount": 15
  }
}
```





