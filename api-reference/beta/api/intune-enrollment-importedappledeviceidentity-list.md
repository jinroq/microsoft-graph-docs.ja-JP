---
title: リスト importedAppleDeviceIdentities
description: ImportedAppleDeviceIdentity オブジェクトのプロパティとリレーションシップをリストします。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: f9050f21b80c8694138e193123156be4dddef36f
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36356579"
---
# <a name="list-importedappledeviceidentities"></a><span data-ttu-id="dcf02-103">リスト importedAppleDeviceIdentities</span><span class="sxs-lookup"><span data-stu-id="dcf02-103">List importedAppleDeviceIdentities</span></span>

> <span data-ttu-id="dcf02-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="dcf02-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="dcf02-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="dcf02-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="dcf02-106">[ImportedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="dcf02-106">List properties and relationships of the [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="dcf02-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="dcf02-107">Prerequisites</span></span>
<span data-ttu-id="dcf02-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="dcf02-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="dcf02-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="dcf02-110">Permission type</span></span>|<span data-ttu-id="dcf02-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="dcf02-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="dcf02-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="dcf02-112">Delegated (work or school account)</span></span>|<span data-ttu-id="dcf02-113">DeviceManagementServiceConfig.ReadWrite.All、DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="dcf02-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="dcf02-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="dcf02-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="dcf02-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="dcf02-115">Not supported.</span></span>|
|<span data-ttu-id="dcf02-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="dcf02-116">Application</span></span>|<span data-ttu-id="dcf02-117">DeviceManagementServiceConfig.ReadWrite.All、DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="dcf02-117">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="dcf02-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="dcf02-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/importedAppleDeviceIdentities
```

## <a name="request-headers"></a><span data-ttu-id="dcf02-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="dcf02-119">Request headers</span></span>
|<span data-ttu-id="dcf02-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="dcf02-120">Header</span></span>|<span data-ttu-id="dcf02-121">値</span><span class="sxs-lookup"><span data-stu-id="dcf02-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="dcf02-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="dcf02-122">Authorization</span></span>|<span data-ttu-id="dcf02-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="dcf02-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="dcf02-124">承諾</span><span class="sxs-lookup"><span data-stu-id="dcf02-124">Accept</span></span>|<span data-ttu-id="dcf02-125">application/json</span><span class="sxs-lookup"><span data-stu-id="dcf02-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="dcf02-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="dcf02-126">Request body</span></span>
<span data-ttu-id="dcf02-127">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="dcf02-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="dcf02-128">応答</span><span class="sxs-lookup"><span data-stu-id="dcf02-128">Response</span></span>
<span data-ttu-id="dcf02-129">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で[importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md)オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="dcf02-129">If successful, this method returns a `200 OK` response code and a collection of [importedAppleDeviceIdentity](../resources/intune-enrollment-importedappledeviceidentity.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="dcf02-130">例</span><span class="sxs-lookup"><span data-stu-id="dcf02-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="dcf02-131">要求</span><span class="sxs-lookup"><span data-stu-id="dcf02-131">Request</span></span>
<span data-ttu-id="dcf02-132">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="dcf02-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/importedAppleDeviceIdentities
```

### <a name="response"></a><span data-ttu-id="dcf02-133">応答</span><span class="sxs-lookup"><span data-stu-id="dcf02-133">Response</span></span>
<span data-ttu-id="dcf02-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="dcf02-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 686

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.importedAppleDeviceIdentity",
      "id": "352e3c2f-3c2f-352e-2f3c-2e352f3c2e35",
      "serialNumber": "Serial Number value",
      "requestedEnrollmentProfileId": "Requested Enrollment Profile Id value",
      "requestedEnrollmentProfileAssignmentDateTime": "2017-01-01T00:02:32.8167841-08:00",
      "isSupervised": true,
      "discoverySource": "adminImport",
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "lastContactedDateTime": "2016-12-31T23:58:44.2908994-08:00",
      "description": "Description value",
      "enrollmentState": "enrolled",
      "platform": "ios"
    }
  ]
}
```






