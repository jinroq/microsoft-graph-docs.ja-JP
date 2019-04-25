---
title: managedAndroidStoreApps のリスト
description: managedAndroidStoreApp オブジェクトのプロパティとリレーションシップをリストします。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: d19d219822ad852cc881c813b5e13ff86d4d1622
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32578534"
---
# <a name="list-managedandroidstoreapps"></a><span data-ttu-id="561d9-103">managedAndroidStoreApps のリスト</span><span class="sxs-lookup"><span data-stu-id="561d9-103">List managedAndroidStoreApps</span></span>

> <span data-ttu-id="561d9-104">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="561d9-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="561d9-105">[managedAndroidStoreApp](../resources/intune-apps-managedandroidstoreapp.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="561d9-105">List properties and relationships of the [managedAndroidStoreApp](../resources/intune-apps-managedandroidstoreapp.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="561d9-106">前提条件</span><span class="sxs-lookup"><span data-stu-id="561d9-106">Prerequisites</span></span>
<span data-ttu-id="561d9-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="561d9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="561d9-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="561d9-109">Permission type</span></span>|<span data-ttu-id="561d9-110">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="561d9-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="561d9-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="561d9-111">Delegated (work or school account)</span></span>|<span data-ttu-id="561d9-112">DeviceManagementApps.ReadWrite.All、DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="561d9-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="561d9-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="561d9-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="561d9-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="561d9-114">Not supported.</span></span>|
|<span data-ttu-id="561d9-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="561d9-115">Application</span></span>|<span data-ttu-id="561d9-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="561d9-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="561d9-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="561d9-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="561d9-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="561d9-118">Request headers</span></span>
|<span data-ttu-id="561d9-119">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="561d9-119">Header</span></span>|<span data-ttu-id="561d9-120">値</span><span class="sxs-lookup"><span data-stu-id="561d9-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="561d9-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="561d9-121">Authorization</span></span>|<span data-ttu-id="561d9-122">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="561d9-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="561d9-123">承諾</span><span class="sxs-lookup"><span data-stu-id="561d9-123">Accept</span></span>|<span data-ttu-id="561d9-124">application/json</span><span class="sxs-lookup"><span data-stu-id="561d9-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="561d9-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="561d9-125">Request body</span></span>
<span data-ttu-id="561d9-126">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="561d9-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="561d9-127">応答</span><span class="sxs-lookup"><span data-stu-id="561d9-127">Response</span></span>
<span data-ttu-id="561d9-128">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [managedAndroidStoreApp](../resources/intune-apps-managedandroidstoreapp.md) オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="561d9-128">If successful, this method returns a `200 OK` response code and a collection of [managedAndroidStoreApp](../resources/intune-apps-managedandroidstoreapp.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="561d9-129">例</span><span class="sxs-lookup"><span data-stu-id="561d9-129">Example</span></span>

### <a name="request"></a><span data-ttu-id="561d9-130">要求</span><span class="sxs-lookup"><span data-stu-id="561d9-130">Request</span></span>
<span data-ttu-id="561d9-131">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="561d9-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps
```

### <a name="response"></a><span data-ttu-id="561d9-132">応答</span><span class="sxs-lookup"><span data-stu-id="561d9-132">Response</span></span>
<span data-ttu-id="561d9-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="561d9-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1357

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.managedAndroidStoreApp",
      "id": "89e7e991-e991-89e7-91e9-e78991e9e789",
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
      "publishingState": "processing",
      "appAvailability": "lineOfBusiness",
      "version": "Version value",
      "packageId": "Package Id value",
      "appStoreUrl": "https://example.com/appStoreUrl/",
      "minimumSupportedOperatingSystem": {
        "@odata.type": "microsoft.graph.androidMinimumOperatingSystem",
        "v4_0": true,
        "v4_0_3": true,
        "v4_1": true,
        "v4_2": true,
        "v4_3": true,
        "v4_4": true,
        "v5_0": true,
        "v5_1": true
      }
    }
  ]
}
```



