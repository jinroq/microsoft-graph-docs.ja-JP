---
title: Get iosVppApp
description: iosVppApp オブジェクトのプロパティとリレーションシップを読み取ります。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: b9bb63df09cd3ace432d56dd92756fe5e12c78cc
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36330525"
---
# <a name="get-iosvppapp"></a><span data-ttu-id="f3478-103">Get iosVppApp</span><span class="sxs-lookup"><span data-stu-id="f3478-103">Get iosVppApp</span></span>

> <span data-ttu-id="f3478-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f3478-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f3478-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="f3478-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f3478-106">[iosVppApp](../resources/intune-apps-iosvppapp.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="f3478-106">Read properties and relationships of the [iosVppApp](../resources/intune-apps-iosvppapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f3478-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="f3478-107">Prerequisites</span></span>
<span data-ttu-id="f3478-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="f3478-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f3478-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="f3478-110">Permission type</span></span>|<span data-ttu-id="f3478-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="f3478-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f3478-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="f3478-112">Delegated (work or school account)</span></span>|<span data-ttu-id="f3478-113">DeviceManagementApps.ReadWrite.All、DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="f3478-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="f3478-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="f3478-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f3478-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f3478-115">Not supported.</span></span>|
|<span data-ttu-id="f3478-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="f3478-116">Application</span></span>|<span data-ttu-id="f3478-117">DeviceManagementApps.ReadWrite.All、DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="f3478-117">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="f3478-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="f3478-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps/{mobileAppId}
GET /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
GET /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="optional-query-parameters"></a><span data-ttu-id="f3478-119">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="f3478-119">Optional query parameters</span></span>
<span data-ttu-id="f3478-120">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://docs.microsoft.com/en-us/graph/query-parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="f3478-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="f3478-121">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="f3478-121">Request headers</span></span>
|<span data-ttu-id="f3478-122">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="f3478-122">Header</span></span>|<span data-ttu-id="f3478-123">値</span><span class="sxs-lookup"><span data-stu-id="f3478-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f3478-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="f3478-124">Authorization</span></span>|<span data-ttu-id="f3478-125">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="f3478-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f3478-126">承諾</span><span class="sxs-lookup"><span data-stu-id="f3478-126">Accept</span></span>|<span data-ttu-id="f3478-127">application/json</span><span class="sxs-lookup"><span data-stu-id="f3478-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f3478-128">要求本文</span><span class="sxs-lookup"><span data-stu-id="f3478-128">Request body</span></span>
<span data-ttu-id="f3478-129">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="f3478-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f3478-130">応答</span><span class="sxs-lookup"><span data-stu-id="f3478-130">Response</span></span>
<span data-ttu-id="f3478-131">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [iosVppApp](../resources/intune-apps-iosvppapp.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="f3478-131">If successful, this method returns a `200 OK` response code and [iosVppApp](../resources/intune-apps-iosvppapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f3478-132">例</span><span class="sxs-lookup"><span data-stu-id="f3478-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="f3478-133">要求</span><span class="sxs-lookup"><span data-stu-id="f3478-133">Request</span></span>
<span data-ttu-id="f3478-134">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="f3478-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}
```

### <a name="response"></a><span data-ttu-id="f3478-135">応答</span><span class="sxs-lookup"><span data-stu-id="f3478-135">Response</span></span>
<span data-ttu-id="f3478-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="f3478-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2310

{
  "value": {
    "@odata.type": "#microsoft.graph.iosVppApp",
    "id": "a0ac9b6f-9b6f-a0ac-6f9b-aca06f9baca0",
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
    "usedLicenseCount": 0,
    "totalLicenseCount": 1,
    "releaseDateTime": "2017-01-01T00:01:34.7470482-08:00",
    "appStoreUrl": "https://example.com/appStoreUrl/",
    "licensingType": {
      "@odata.type": "microsoft.graph.vppLicensingType",
      "supportUserLicensing": true,
      "supportDeviceLicensing": true,
      "supportsUserLicensing": true,
      "supportsDeviceLicensing": true
    },
    "applicableDeviceType": {
      "@odata.type": "microsoft.graph.iosDeviceType",
      "iPad": true,
      "iPhoneAndIPod": true
    },
    "vppTokenOrganizationName": "Vpp Token Organization Name value",
    "vppTokenAccountType": "education",
    "vppTokenAppleId": "Vpp Token Apple Id value",
    "bundleId": "Bundle Id value",
    "vppTokenId": "Vpp Token Id value",
    "revokeLicenseActionResults": [
      {
        "@odata.type": "microsoft.graph.iosVppAppRevokeLicensesActionResult",
        "userId": "User Id value",
        "managedDeviceId": "Managed Device Id value",
        "totalLicensesCount": 2,
        "failedLicensesCount": 3,
        "actionFailureReason": "appleFailure",
        "actionName": "Action Name value",
        "actionState": "pending",
        "startDateTime": "2016-12-31T23:58:46.7156189-08:00",
        "lastUpdatedDateTime": "2017-01-01T00:00:56.8321556-08:00"
      }
    ]
  }
}
```






