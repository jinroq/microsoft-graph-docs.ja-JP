---
title: importDeviceIdentityList アクション
description: まだ文書化されていません
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 2c3fc1f00d64a5705b15ffc297b51a84101a9f50
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36356432"
---
# <a name="importdeviceidentitylist-action"></a><span data-ttu-id="ebf27-103">importDeviceIdentityList アクション</span><span class="sxs-lookup"><span data-stu-id="ebf27-103">importDeviceIdentityList action</span></span>

> <span data-ttu-id="ebf27-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ebf27-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ebf27-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="ebf27-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ebf27-106">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="ebf27-106">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ebf27-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="ebf27-107">Prerequisites</span></span>
<span data-ttu-id="ebf27-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="ebf27-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ebf27-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="ebf27-110">Permission type</span></span>|<span data-ttu-id="ebf27-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="ebf27-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ebf27-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="ebf27-112">Delegated (work or school account)</span></span>|<span data-ttu-id="ebf27-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ebf27-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="ebf27-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="ebf27-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ebf27-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ebf27-115">Not supported.</span></span>|
|<span data-ttu-id="ebf27-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="ebf27-116">Application</span></span>|<span data-ttu-id="ebf27-117">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ebf27-117">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="ebf27-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="ebf27-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/importedDeviceIdentities/importDeviceIdentityList
```

## <a name="request-headers"></a><span data-ttu-id="ebf27-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="ebf27-119">Request headers</span></span>
|<span data-ttu-id="ebf27-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="ebf27-120">Header</span></span>|<span data-ttu-id="ebf27-121">値</span><span class="sxs-lookup"><span data-stu-id="ebf27-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ebf27-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="ebf27-122">Authorization</span></span>|<span data-ttu-id="ebf27-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="ebf27-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ebf27-124">承諾</span><span class="sxs-lookup"><span data-stu-id="ebf27-124">Accept</span></span>|<span data-ttu-id="ebf27-125">application/json</span><span class="sxs-lookup"><span data-stu-id="ebf27-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ebf27-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="ebf27-126">Request body</span></span>
<span data-ttu-id="ebf27-127">要求本文で、パラメーターの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="ebf27-127">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="ebf27-128">次の表に、このアクションで使用できるパラメーターを示します。</span><span class="sxs-lookup"><span data-stu-id="ebf27-128">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="ebf27-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="ebf27-129">Property</span></span>|<span data-ttu-id="ebf27-130">型</span><span class="sxs-lookup"><span data-stu-id="ebf27-130">Type</span></span>|<span data-ttu-id="ebf27-131">説明</span><span class="sxs-lookup"><span data-stu-id="ebf27-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ebf27-132">importedDeviceIdentities</span><span class="sxs-lookup"><span data-stu-id="ebf27-132">importedDeviceIdentities</span></span>|<span data-ttu-id="ebf27-133">[importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="ebf27-133">[importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md) collection</span></span>|<span data-ttu-id="ebf27-134">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="ebf27-134">Not yet documented</span></span>|
|<span data-ttu-id="ebf27-135">overwriteImportedDeviceIdentities</span><span class="sxs-lookup"><span data-stu-id="ebf27-135">overwriteImportedDeviceIdentities</span></span>|<span data-ttu-id="ebf27-136">ブール型 (Boolean)</span><span class="sxs-lookup"><span data-stu-id="ebf27-136">Boolean</span></span>|<span data-ttu-id="ebf27-137">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="ebf27-137">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="ebf27-138">応答</span><span class="sxs-lookup"><span data-stu-id="ebf27-138">Response</span></span>
<span data-ttu-id="ebf27-139">成功した場合、このアクション`200 OK`は応答コードと、応答本文で[importedDeviceIdentityResult](../resources/intune-enrollment-importeddeviceidentityresult.md)コレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="ebf27-139">If successful, this action returns a `200 OK` response code and a [importedDeviceIdentityResult](../resources/intune-enrollment-importeddeviceidentityresult.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ebf27-140">例</span><span class="sxs-lookup"><span data-stu-id="ebf27-140">Example</span></span>

### <a name="request"></a><span data-ttu-id="ebf27-141">要求</span><span class="sxs-lookup"><span data-stu-id="ebf27-141">Request</span></span>
<span data-ttu-id="ebf27-142">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="ebf27-142">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/importedDeviceIdentities/importDeviceIdentityList

Content-type: application/json
Content-length: 642

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
  ],
  "overwriteImportedDeviceIdentities": true
}
```

### <a name="response"></a><span data-ttu-id="ebf27-143">応答</span><span class="sxs-lookup"><span data-stu-id="ebf27-143">Response</span></span>
<span data-ttu-id="ebf27-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="ebf27-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 606

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.importedDeviceIdentityResult",
      "id": "9dfd3690-3690-9dfd-9036-fd9d9036fd9d",
      "importedDeviceIdentifier": "Imported Device Identifier value",
      "importedDeviceIdentityType": "imei",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "lastContactedDateTime": "2016-12-31T23:58:44.2908994-08:00",
      "description": "Description value",
      "enrollmentState": "enrolled",
      "platform": "ios",
      "status": true
    }
  ]
}
```






