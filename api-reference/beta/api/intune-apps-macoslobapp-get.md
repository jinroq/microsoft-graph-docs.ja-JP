---
title: MacOSLobApp の取得
description: MacOSLobApp オブジェクトのプロパティとリレーションシップを読み取ります。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: ca3cb8a494a959eb4d3e0e9aa35323dd96df09d0
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35962198"
---
# <a name="get-macoslobapp"></a><span data-ttu-id="d2504-103">MacOSLobApp の取得</span><span class="sxs-lookup"><span data-stu-id="d2504-103">Get macOSLobApp</span></span>

> <span data-ttu-id="d2504-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d2504-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d2504-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="d2504-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d2504-106">[Macoslobapp](../resources/intune-apps-macoslobapp.md)オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="d2504-106">Read properties and relationships of the [macOSLobApp](../resources/intune-apps-macoslobapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d2504-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="d2504-107">Prerequisites</span></span>
<span data-ttu-id="d2504-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="d2504-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d2504-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="d2504-110">Permission type</span></span>|<span data-ttu-id="d2504-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="d2504-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d2504-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="d2504-112">Delegated (work or school account)</span></span>|<span data-ttu-id="d2504-113">DeviceManagementApps.ReadWrite.All、DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="d2504-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="d2504-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="d2504-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d2504-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d2504-115">Not supported.</span></span>|
|<span data-ttu-id="d2504-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="d2504-116">Application</span></span>|<span data-ttu-id="d2504-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d2504-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d2504-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="d2504-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps/{mobileAppId}
GET /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
GET /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="optional-query-parameters"></a><span data-ttu-id="d2504-119">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="d2504-119">Optional query parameters</span></span>
<span data-ttu-id="d2504-120">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://docs.microsoft.com/en-us/graph/query-parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="d2504-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="d2504-121">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="d2504-121">Request headers</span></span>
|<span data-ttu-id="d2504-122">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="d2504-122">Header</span></span>|<span data-ttu-id="d2504-123">値</span><span class="sxs-lookup"><span data-stu-id="d2504-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d2504-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="d2504-124">Authorization</span></span>|<span data-ttu-id="d2504-125">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="d2504-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d2504-126">承諾</span><span class="sxs-lookup"><span data-stu-id="d2504-126">Accept</span></span>|<span data-ttu-id="d2504-127">application/json</span><span class="sxs-lookup"><span data-stu-id="d2504-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d2504-128">要求本文</span><span class="sxs-lookup"><span data-stu-id="d2504-128">Request body</span></span>
<span data-ttu-id="d2504-129">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="d2504-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d2504-130">応答</span><span class="sxs-lookup"><span data-stu-id="d2504-130">Response</span></span>
<span data-ttu-id="d2504-131">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で[Macoslobapp](../resources/intune-apps-macoslobapp.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="d2504-131">If successful, this method returns a `200 OK` response code and [macOSLobApp](../resources/intune-apps-macoslobapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d2504-132">例</span><span class="sxs-lookup"><span data-stu-id="d2504-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="d2504-133">要求</span><span class="sxs-lookup"><span data-stu-id="d2504-133">Request</span></span>
<span data-ttu-id="d2504-134">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="d2504-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}
```

### <a name="response"></a><span data-ttu-id="d2504-135">応答</span><span class="sxs-lookup"><span data-stu-id="d2504-135">Response</span></span>
<span data-ttu-id="d2504-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="d2504-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1875

{
  "value": {
    "@odata.type": "#microsoft.graph.macOSLobApp",
    "id": "7be9250a-250a-7be9-0a25-e97b0a25e97b",
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
    "dependentAppCount": 1,
    "committedContentVersion": "Committed Content Version value",
    "fileName": "File Name value",
    "size": 4,
    "bundleId": "Bundle Id value",
    "minimumSupportedOperatingSystem": {
      "@odata.type": "microsoft.graph.macOSMinimumOperatingSystem",
      "v10_7": true,
      "v10_8": true,
      "v10_9": true,
      "v10_10": true,
      "v10_11": true,
      "v10_12": true,
      "v10_13": true
    },
    "buildNumber": "Build Number value",
    "versionNumber": "Version Number value",
    "childApps": [
      {
        "@odata.type": "microsoft.graph.macOSLobChildApp",
        "bundleId": "Bundle Id value",
        "buildNumber": "Build Number value",
        "versionNumber": "Version Number value"
      }
    ],
    "identityVersion": "Identity Version value",
    "md5HashChunkSize": 0,
    "md5Hash": [
      "Md5Hash value"
    ],
    "ignoreVersionDetection": true
  }
}
```





