---
title: iosVppApps のリスト
description: iosVppApp オブジェクトのプロパティとリレーションシップをリストします。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 3f5c2d2aeff71786e80790c50a31ca250474489f
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/14/2019
ms.locfileid: "34966006"
---
# <a name="list-iosvppapps"></a><span data-ttu-id="b1ee0-103">iosVppApps のリスト</span><span class="sxs-lookup"><span data-stu-id="b1ee0-103">List iosVppApps</span></span>

> <span data-ttu-id="b1ee0-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b1ee0-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b1ee0-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="b1ee0-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b1ee0-106">[iosVppApp](../resources/intune-apps-iosvppapp.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="b1ee0-106">List properties and relationships of the [iosVppApp](../resources/intune-apps-iosvppapp.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b1ee0-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="b1ee0-107">Prerequisites</span></span>
<span data-ttu-id="b1ee0-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="b1ee0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b1ee0-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="b1ee0-110">Permission type</span></span>|<span data-ttu-id="b1ee0-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="b1ee0-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b1ee0-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="b1ee0-112">Delegated (work or school account)</span></span>|<span data-ttu-id="b1ee0-113">DeviceManagementApps.ReadWrite.All、DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="b1ee0-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="b1ee0-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="b1ee0-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b1ee0-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b1ee0-115">Not supported.</span></span>|
|<span data-ttu-id="b1ee0-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="b1ee0-116">Application</span></span>|<span data-ttu-id="b1ee0-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b1ee0-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b1ee0-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="b1ee0-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="b1ee0-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="b1ee0-119">Request headers</span></span>
|<span data-ttu-id="b1ee0-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="b1ee0-120">Header</span></span>|<span data-ttu-id="b1ee0-121">値</span><span class="sxs-lookup"><span data-stu-id="b1ee0-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b1ee0-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="b1ee0-122">Authorization</span></span>|<span data-ttu-id="b1ee0-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="b1ee0-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b1ee0-124">承諾</span><span class="sxs-lookup"><span data-stu-id="b1ee0-124">Accept</span></span>|<span data-ttu-id="b1ee0-125">application/json</span><span class="sxs-lookup"><span data-stu-id="b1ee0-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b1ee0-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="b1ee0-126">Request body</span></span>
<span data-ttu-id="b1ee0-127">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="b1ee0-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b1ee0-128">応答</span><span class="sxs-lookup"><span data-stu-id="b1ee0-128">Response</span></span>
<span data-ttu-id="b1ee0-129">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [iosVppApp](../resources/intune-apps-iosvppapp.md) オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="b1ee0-129">If successful, this method returns a `200 OK` response code and a collection of [iosVppApp](../resources/intune-apps-iosvppapp.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b1ee0-130">例</span><span class="sxs-lookup"><span data-stu-id="b1ee0-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="b1ee0-131">要求</span><span class="sxs-lookup"><span data-stu-id="b1ee0-131">Request</span></span>
<span data-ttu-id="b1ee0-132">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="b1ee0-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileApps
```

### <a name="response"></a><span data-ttu-id="b1ee0-133">応答</span><span class="sxs-lookup"><span data-stu-id="b1ee0-133">Response</span></span>
<span data-ttu-id="b1ee0-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="b1ee0-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2444

{
  "value": [
    {
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
  ]
}
```





