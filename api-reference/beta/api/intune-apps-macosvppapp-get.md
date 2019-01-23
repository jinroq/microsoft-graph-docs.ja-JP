---
title: MacOsVppApp を取得します。
description: MacOsVppApp オブジェクトのプロパティと関係を参照してください。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 8ca675cf066ebe28619a3e5408c877f2b05a9414
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29431603"
---
# <a name="get-macosvppapp"></a><span data-ttu-id="e272b-103">MacOsVppApp を取得します。</span><span class="sxs-lookup"><span data-stu-id="e272b-103">Get macOsVppApp</span></span>

> <span data-ttu-id="e272b-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="e272b-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="e272b-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e272b-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="e272b-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="e272b-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e272b-107">[MacOsVppApp](../resources/intune-apps-macosvppapp.md)オブジェクトのプロパティと関係を参照してください。</span><span class="sxs-lookup"><span data-stu-id="e272b-107">Read properties and relationships of the [macOsVppApp](../resources/intune-apps-macosvppapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e272b-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="e272b-108">Prerequisites</span></span>
<span data-ttu-id="e272b-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/concepts/permissions-reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="e272b-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="e272b-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="e272b-111">Permission type</span></span>|<span data-ttu-id="e272b-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="e272b-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e272b-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="e272b-113">Delegated (work or school account)</span></span>|<span data-ttu-id="e272b-114">DeviceManagementApps.ReadWrite.All、DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="e272b-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="e272b-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="e272b-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e272b-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e272b-116">Not supported.</span></span>|
|<span data-ttu-id="e272b-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="e272b-117">Application</span></span>|<span data-ttu-id="e272b-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e272b-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e272b-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="e272b-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps/{mobileAppId}
GET /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
GET /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="optional-query-parameters"></a><span data-ttu-id="e272b-120">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="e272b-120">Optional query parameters</span></span>
<span data-ttu-id="e272b-121">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://docs.microsoft.com/en-us/graph/query-parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="e272b-121">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="e272b-122">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="e272b-122">Request headers</span></span>
|<span data-ttu-id="e272b-123">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="e272b-123">Header</span></span>|<span data-ttu-id="e272b-124">値</span><span class="sxs-lookup"><span data-stu-id="e272b-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e272b-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="e272b-125">Authorization</span></span>|<span data-ttu-id="e272b-126">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="e272b-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e272b-127">Accept</span><span class="sxs-lookup"><span data-stu-id="e272b-127">Accept</span></span>|<span data-ttu-id="e272b-128">application/json</span><span class="sxs-lookup"><span data-stu-id="e272b-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e272b-129">要求本文</span><span class="sxs-lookup"><span data-stu-id="e272b-129">Request body</span></span>
<span data-ttu-id="e272b-130">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="e272b-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e272b-131">応答</span><span class="sxs-lookup"><span data-stu-id="e272b-131">Response</span></span>
<span data-ttu-id="e272b-132">かどうかは成功すると、このメソッドが返されます、 `200 OK` 、応答の本体で応答コードと[macOsVppApp](../resources/intune-apps-macosvppapp.md)のオブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="e272b-132">If successful, this method returns a `200 OK` response code and [macOsVppApp](../resources/intune-apps-macosvppapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e272b-133">例</span><span class="sxs-lookup"><span data-stu-id="e272b-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="e272b-134">要求</span><span class="sxs-lookup"><span data-stu-id="e272b-134">Request</span></span>
<span data-ttu-id="e272b-135">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="e272b-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}
```

### <a name="response"></a><span data-ttu-id="e272b-136">応答</span><span class="sxs-lookup"><span data-stu-id="e272b-136">Response</span></span>
<span data-ttu-id="e272b-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="e272b-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2141

{
  "value": {
    "@odata.type": "#microsoft.graph.macOsVppApp",
    "id": "10b95265-5265-10b9-6552-b9106552b910",
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
    "vppTokenOrganizationName": "Vpp Token Organization Name value",
    "vppTokenAccountType": "education",
    "vppTokenAppleId": "Vpp Token Apple Id value",
    "bundleId": "Bundle Id value",
    "vppTokenId": "Vpp Token Id value",
    "revokeLicenseActionResults": [
      {
        "@odata.type": "microsoft.graph.macOsVppAppRevokeLicensesActionResult",
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




