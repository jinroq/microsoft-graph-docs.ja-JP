---
title: Get iosLobApp
description: iosLobApp オブジェクトのプロパティとリレーションシップを読み取ります。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 2c50a9a839c218a66492c245e34a4833b72ba248
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/21/2019
ms.locfileid: "30160887"
---
# <a name="get-ioslobapp"></a><span data-ttu-id="7f346-103">Get iosLobApp</span><span class="sxs-lookup"><span data-stu-id="7f346-103">Get iosLobApp</span></span>

> <span data-ttu-id="7f346-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="7f346-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7f346-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="7f346-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7f346-106">[iosLobApp](../resources/intune-apps-ioslobapp.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="7f346-106">Read properties and relationships of the [iosLobApp](../resources/intune-apps-ioslobapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="7f346-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="7f346-107">Prerequisites</span></span>
<span data-ttu-id="7f346-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/concepts/permissions-reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="7f346-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="7f346-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="7f346-110">Permission type</span></span>|<span data-ttu-id="7f346-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="7f346-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7f346-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="7f346-112">Delegated (work or school account)</span></span>|<span data-ttu-id="7f346-113">DeviceManagementApps.ReadWrite.All、DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="7f346-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="7f346-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="7f346-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7f346-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="7f346-115">Not supported.</span></span>|
|<span data-ttu-id="7f346-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="7f346-116">Application</span></span>|<span data-ttu-id="7f346-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="7f346-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="7f346-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="7f346-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps/{mobileAppId}
GET /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
GET /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="optional-query-parameters"></a><span data-ttu-id="7f346-119">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="7f346-119">Optional query parameters</span></span>
<span data-ttu-id="7f346-120">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://docs.microsoft.com/en-us/graph/query-parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="7f346-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="7f346-121">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="7f346-121">Request headers</span></span>
|<span data-ttu-id="7f346-122">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="7f346-122">Header</span></span>|<span data-ttu-id="7f346-123">値</span><span class="sxs-lookup"><span data-stu-id="7f346-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7f346-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="7f346-124">Authorization</span></span>|<span data-ttu-id="7f346-125">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="7f346-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7f346-126">承諾</span><span class="sxs-lookup"><span data-stu-id="7f346-126">Accept</span></span>|<span data-ttu-id="7f346-127">application/json</span><span class="sxs-lookup"><span data-stu-id="7f346-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7f346-128">要求本文</span><span class="sxs-lookup"><span data-stu-id="7f346-128">Request body</span></span>
<span data-ttu-id="7f346-129">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="7f346-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7f346-130">応答</span><span class="sxs-lookup"><span data-stu-id="7f346-130">Response</span></span>
<span data-ttu-id="7f346-131">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [iosLobApp](../resources/intune-apps-ioslobapp.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="7f346-131">If successful, this method returns a `200 OK` response code and [iosLobApp](../resources/intune-apps-ioslobapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7f346-132">例</span><span class="sxs-lookup"><span data-stu-id="7f346-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="7f346-133">要求</span><span class="sxs-lookup"><span data-stu-id="7f346-133">Request</span></span>
<span data-ttu-id="7f346-134">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="7f346-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}
```

### <a name="response"></a><span data-ttu-id="7f346-135">応答</span><span class="sxs-lookup"><span data-stu-id="7f346-135">Response</span></span>
<span data-ttu-id="7f346-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="7f346-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1645

{
  "value": {
    "@odata.type": "#microsoft.graph.iosLobApp",
    "id": "b34052ea-52ea-b340-ea52-40b3ea5240b3",
    "displayName": "Display Name value",
    "description": "Description value",
    "publisher": "Publisher value",
    "largeIcon": {
      "@odata.type": "microsoft.graph.mimeContent",
      "type": "Type value",
      "value": "dmFsdWU="
    },
    "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
    "isFeatured": true,
    "privacyInformationUrl": "https://example.com/privacyInformationUrl/",
    "informationUrl": "https://example.com/informationUrl/",
    "owner": "Owner value",
    "developer": "Developer value",
    "notes": "Notes value",
    "uploadState": 11,
    "publishingState": "processing",
    "isAssigned": true,
    "roleScopeTagIds": [
      "Role Scope Tag Ids value"
    ],
    "committedContentVersion": "Committed Content Version value",
    "fileName": "File Name value",
    "size": 4,
    "bundleId": "Bundle Id value",
    "applicableDeviceType": {
      "@odata.type": "microsoft.graph.iosDeviceType",
      "iPad": true,
      "iPhoneAndIPod": true
    },
    "minimumSupportedOperatingSystem": {
      "@odata.type": "microsoft.graph.iosMinimumOperatingSystem",
      "v8_0": true,
      "v9_0": true,
      "v10_0": true,
      "v11_0": true,
      "v12_0": true
    },
    "expirationDateTime": "2016-12-31T23:57:57.2481234-08:00",
    "versionNumber": "Version Number value",
    "buildNumber": "Build Number value",
    "identityVersion": "Identity Version value"
  }
}
```




