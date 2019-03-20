---
title: searchexistingidentities アクション
description: まだ文書化されていません
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 1d8917d7a19f7a0186fe85e88aea4db65124b599
ms.sourcegitcommit: 8eb88cfb48b0eb8f992570caebef577dfa2f30d3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/14/2019
ms.locfileid: "30631576"
---
# <a name="searchexistingidentities-action"></a><span data-ttu-id="641b0-103">searchexistingidentities アクション</span><span class="sxs-lookup"><span data-stu-id="641b0-103">searchExistingIdentities action</span></span>

> <span data-ttu-id="641b0-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="641b0-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="641b0-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="641b0-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="641b0-106">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="641b0-106">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="641b0-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="641b0-107">Prerequisites</span></span>
<span data-ttu-id="641b0-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/concepts/permissions-reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="641b0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="641b0-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="641b0-110">Permission type</span></span>|<span data-ttu-id="641b0-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="641b0-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="641b0-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="641b0-112">Delegated (work or school account)</span></span>|<span data-ttu-id="641b0-113">DeviceManagementServiceConfig.ReadWrite.All、DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="641b0-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="641b0-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="641b0-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="641b0-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="641b0-115">Not supported.</span></span>|
|<span data-ttu-id="641b0-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="641b0-116">Application</span></span>|<span data-ttu-id="641b0-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="641b0-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="641b0-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="641b0-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/importedDeviceIdentities/searchExistingIdentities
```

## <a name="request-headers"></a><span data-ttu-id="641b0-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="641b0-119">Request headers</span></span>
|<span data-ttu-id="641b0-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="641b0-120">Header</span></span>|<span data-ttu-id="641b0-121">値</span><span class="sxs-lookup"><span data-stu-id="641b0-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="641b0-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="641b0-122">Authorization</span></span>|<span data-ttu-id="641b0-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="641b0-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="641b0-124">承諾</span><span class="sxs-lookup"><span data-stu-id="641b0-124">Accept</span></span>|<span data-ttu-id="641b0-125">application/json</span><span class="sxs-lookup"><span data-stu-id="641b0-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="641b0-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="641b0-126">Request body</span></span>
<span data-ttu-id="641b0-127">要求本文で、パラメーターの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="641b0-127">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="641b0-128">次の表に、このアクションで使用できるパラメーターを示します。</span><span class="sxs-lookup"><span data-stu-id="641b0-128">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="641b0-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="641b0-129">Property</span></span>|<span data-ttu-id="641b0-130">型</span><span class="sxs-lookup"><span data-stu-id="641b0-130">Type</span></span>|<span data-ttu-id="641b0-131">説明</span><span class="sxs-lookup"><span data-stu-id="641b0-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="641b0-132">importedDeviceIdentities</span><span class="sxs-lookup"><span data-stu-id="641b0-132">importedDeviceIdentities</span></span>|<span data-ttu-id="641b0-133">[importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="641b0-133">[importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md) collection</span></span>|<span data-ttu-id="641b0-134">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="641b0-134">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="641b0-135">応答</span><span class="sxs-lookup"><span data-stu-id="641b0-135">Response</span></span>
<span data-ttu-id="641b0-136">成功した場合、このアクション`200 OK`は応答コードと、応答本文で[importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)コレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="641b0-136">If successful, this action returns a `200 OK` response code and a [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="641b0-137">例</span><span class="sxs-lookup"><span data-stu-id="641b0-137">Example</span></span>

### <a name="request"></a><span data-ttu-id="641b0-138">要求</span><span class="sxs-lookup"><span data-stu-id="641b0-138">Request</span></span>
<span data-ttu-id="641b0-139">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="641b0-139">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/importedDeviceIdentities/searchExistingIdentities

Content-type: application/json
Content-length: 596

{
  "importedDeviceIdentities": [
    {
      "@odata.type": "#microsoft.graph.importedDeviceIdentity",
      "id": "9f70a12f-a12f-9f70-2fa1-709f2fa1709f",
      "importedDeviceIdentifier": "Imported Device Identifier value",
      "importedDeviceIdentityType": "imei",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "lastContactedDateTime": "2016-12-31T23:58:44.2908994-08:00",
      "description": "Description value",
      "enrollmentState": "enrolled",
      "platform": "ios"
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="641b0-140">応答</span><span class="sxs-lookup"><span data-stu-id="641b0-140">Response</span></span>
<span data-ttu-id="641b0-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="641b0-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 577

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.importedDeviceIdentity",
      "id": "9f70a12f-a12f-9f70-2fa1-709f2fa1709f",
      "importedDeviceIdentifier": "Imported Device Identifier value",
      "importedDeviceIdentityType": "imei",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "lastContactedDateTime": "2016-12-31T23:58:44.2908994-08:00",
      "description": "Description value",
      "enrollmentState": "enrolled",
      "platform": "ios"
    }
  ]
}
```



