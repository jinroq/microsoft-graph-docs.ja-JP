---
title: importDeviceIdentityList アクション
description: まだ文書化されていません
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: deb721bcc086575a1dfee35f893da07b49f8ab69
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27930447"
---
# <a name="importdeviceidentitylist-action"></a><span data-ttu-id="3f3ef-103">importDeviceIdentityList アクション</span><span class="sxs-lookup"><span data-stu-id="3f3ef-103">importDeviceIdentityList action</span></span>

> <span data-ttu-id="3f3ef-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="3f3ef-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="3f3ef-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="3f3ef-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="3f3ef-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="3f3ef-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="3f3ef-107">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="3f3ef-107">Not yet documented</span></span>
## <a name="prerequisites"></a><span data-ttu-id="3f3ef-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="3f3ef-108">Prerequisites</span></span>
<span data-ttu-id="3f3ef-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="3f3ef-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3f3ef-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="3f3ef-111">Permission type</span></span>|<span data-ttu-id="3f3ef-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="3f3ef-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3f3ef-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="3f3ef-113">Delegated (work or school account)</span></span>|<span data-ttu-id="3f3ef-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3f3ef-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="3f3ef-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="3f3ef-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3f3ef-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="3f3ef-116">Not supported.</span></span>|
|<span data-ttu-id="3f3ef-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="3f3ef-117">Application</span></span>|<span data-ttu-id="3f3ef-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="3f3ef-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="3f3ef-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="3f3ef-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/importedDeviceIdentities/importDeviceIdentityList
```

## <a name="request-headers"></a><span data-ttu-id="3f3ef-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="3f3ef-120">Request headers</span></span>
|<span data-ttu-id="3f3ef-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="3f3ef-121">Header</span></span>|<span data-ttu-id="3f3ef-122">値</span><span class="sxs-lookup"><span data-stu-id="3f3ef-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3f3ef-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="3f3ef-123">Authorization</span></span>|<span data-ttu-id="3f3ef-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="3f3ef-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3f3ef-125">Accept</span><span class="sxs-lookup"><span data-stu-id="3f3ef-125">Accept</span></span>|<span data-ttu-id="3f3ef-126">application/json</span><span class="sxs-lookup"><span data-stu-id="3f3ef-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3f3ef-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="3f3ef-127">Request body</span></span>
<span data-ttu-id="3f3ef-128">要求本文で、パラメーターの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="3f3ef-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="3f3ef-129">次の表に、このアクションで使用できるパラメーターを示します。</span><span class="sxs-lookup"><span data-stu-id="3f3ef-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="3f3ef-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="3f3ef-130">Property</span></span>|<span data-ttu-id="3f3ef-131">種類</span><span class="sxs-lookup"><span data-stu-id="3f3ef-131">Type</span></span>|<span data-ttu-id="3f3ef-132">説明</span><span class="sxs-lookup"><span data-stu-id="3f3ef-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3f3ef-133">importedDeviceIdentities</span><span class="sxs-lookup"><span data-stu-id="3f3ef-133">importedDeviceIdentities</span></span>|<span data-ttu-id="3f3ef-134">[importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="3f3ef-134">[importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md) collection</span></span>|<span data-ttu-id="3f3ef-135">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="3f3ef-135">Not yet documented</span></span>|
|<span data-ttu-id="3f3ef-136">overwriteImportedDeviceIdentities</span><span class="sxs-lookup"><span data-stu-id="3f3ef-136">overwriteImportedDeviceIdentities</span></span>|<span data-ttu-id="3f3ef-137">ブール値</span><span class="sxs-lookup"><span data-stu-id="3f3ef-137">Boolean</span></span>|<span data-ttu-id="3f3ef-138">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="3f3ef-138">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="3f3ef-139">応答</span><span class="sxs-lookup"><span data-stu-id="3f3ef-139">Response</span></span>
<span data-ttu-id="3f3ef-140">かどうか、成功を返すアクション、`200 OK`応答コードおよび応答の本文に[importedDeviceIdentityResult](../resources/intune-enrollment-importeddeviceidentityresult.md)のコレクションです。</span><span class="sxs-lookup"><span data-stu-id="3f3ef-140">If successful, this action returns a `200 OK` response code and a [importedDeviceIdentityResult](../resources/intune-enrollment-importeddeviceidentityresult.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3f3ef-141">例</span><span class="sxs-lookup"><span data-stu-id="3f3ef-141">Example</span></span>
### <a name="request"></a><span data-ttu-id="3f3ef-142">要求</span><span class="sxs-lookup"><span data-stu-id="3f3ef-142">Request</span></span>
<span data-ttu-id="3f3ef-143">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="3f3ef-143">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="3f3ef-144">応答</span><span class="sxs-lookup"><span data-stu-id="3f3ef-144">Response</span></span>
<span data-ttu-id="3f3ef-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="3f3ef-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





