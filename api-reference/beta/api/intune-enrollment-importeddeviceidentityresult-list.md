---
title: リスト importedDeviceIdentityResults
description: ImportedDeviceIdentityResult オブジェクトのプロパティとリレーションシップをリストします。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 4692a7b1305f8fceee73a59000fc4259b9668c23
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/11/2019
ms.locfileid: "33908442"
---
# <a name="list-importeddeviceidentityresults"></a><span data-ttu-id="f24a8-103">リスト importedDeviceIdentityResults</span><span class="sxs-lookup"><span data-stu-id="f24a8-103">List importedDeviceIdentityResults</span></span>

> <span data-ttu-id="f24a8-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f24a8-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f24a8-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="f24a8-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f24a8-106">[ImportedDeviceIdentityResult](../resources/intune-enrollment-importeddeviceidentityresult.md)オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="f24a8-106">List properties and relationships of the [importedDeviceIdentityResult](../resources/intune-enrollment-importeddeviceidentityresult.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f24a8-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="f24a8-107">Prerequisites</span></span>
<span data-ttu-id="f24a8-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="f24a8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f24a8-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="f24a8-110">Permission type</span></span>|<span data-ttu-id="f24a8-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="f24a8-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f24a8-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="f24a8-112">Delegated (work or school account)</span></span>|<span data-ttu-id="f24a8-113">DeviceManagementServiceConfig.ReadWrite.All、DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="f24a8-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="f24a8-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="f24a8-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f24a8-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f24a8-115">Not supported.</span></span>|
|<span data-ttu-id="f24a8-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="f24a8-116">Application</span></span>|<span data-ttu-id="f24a8-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f24a8-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f24a8-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="f24a8-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/importedDeviceIdentities
```

## <a name="request-headers"></a><span data-ttu-id="f24a8-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="f24a8-119">Request headers</span></span>
|<span data-ttu-id="f24a8-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="f24a8-120">Header</span></span>|<span data-ttu-id="f24a8-121">値</span><span class="sxs-lookup"><span data-stu-id="f24a8-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f24a8-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="f24a8-122">Authorization</span></span>|<span data-ttu-id="f24a8-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="f24a8-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f24a8-124">承諾</span><span class="sxs-lookup"><span data-stu-id="f24a8-124">Accept</span></span>|<span data-ttu-id="f24a8-125">application/json</span><span class="sxs-lookup"><span data-stu-id="f24a8-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f24a8-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="f24a8-126">Request body</span></span>
<span data-ttu-id="f24a8-127">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="f24a8-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f24a8-128">応答</span><span class="sxs-lookup"><span data-stu-id="f24a8-128">Response</span></span>
<span data-ttu-id="f24a8-129">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で[importedDeviceIdentityResult](../resources/intune-enrollment-importeddeviceidentityresult.md)オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="f24a8-129">If successful, this method returns a `200 OK` response code and a collection of [importedDeviceIdentityResult](../resources/intune-enrollment-importeddeviceidentityresult.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f24a8-130">例</span><span class="sxs-lookup"><span data-stu-id="f24a8-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="f24a8-131">要求</span><span class="sxs-lookup"><span data-stu-id="f24a8-131">Request</span></span>
<span data-ttu-id="f24a8-132">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="f24a8-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/importedDeviceIdentities
```

### <a name="response"></a><span data-ttu-id="f24a8-133">応答</span><span class="sxs-lookup"><span data-stu-id="f24a8-133">Response</span></span>
<span data-ttu-id="f24a8-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="f24a8-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




