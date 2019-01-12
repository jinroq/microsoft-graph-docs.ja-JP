---
title: managedIOSLobApps のリスト
description: managedIOSLobApp オブジェクトのプロパティとリレーションシップをリストします。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: d499dc28d8e592b199d65504bd4516b7c0efc4d9
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27915929"
---
# <a name="list-managedioslobapps"></a><span data-ttu-id="fa9e6-103">managedIOSLobApps のリスト</span><span class="sxs-lookup"><span data-stu-id="fa9e6-103">List managedIOSLobApps</span></span>

> <span data-ttu-id="fa9e6-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="fa9e6-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="fa9e6-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="fa9e6-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="fa9e6-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="fa9e6-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="fa9e6-107">[managedIOSLobApp](../resources/intune-apps-managedioslobapp.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="fa9e6-107">List properties and relationships of the [managedIOSLobApp](../resources/intune-apps-managedioslobapp.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="fa9e6-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="fa9e6-108">Prerequisites</span></span>
<span data-ttu-id="fa9e6-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="fa9e6-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fa9e6-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="fa9e6-111">Permission type</span></span>|<span data-ttu-id="fa9e6-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="fa9e6-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="fa9e6-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="fa9e6-113">Delegated (work or school account)</span></span>|<span data-ttu-id="fa9e6-114">DeviceManagementApps.ReadWrite.All、DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="fa9e6-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="fa9e6-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="fa9e6-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fa9e6-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="fa9e6-116">Not supported.</span></span>|
|<span data-ttu-id="fa9e6-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="fa9e6-117">Application</span></span>|<span data-ttu-id="fa9e6-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="fa9e6-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="fa9e6-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="fa9e6-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="fa9e6-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="fa9e6-120">Request headers</span></span>
|<span data-ttu-id="fa9e6-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="fa9e6-121">Header</span></span>|<span data-ttu-id="fa9e6-122">値</span><span class="sxs-lookup"><span data-stu-id="fa9e6-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="fa9e6-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="fa9e6-123">Authorization</span></span>|<span data-ttu-id="fa9e6-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="fa9e6-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="fa9e6-125">Accept</span><span class="sxs-lookup"><span data-stu-id="fa9e6-125">Accept</span></span>|<span data-ttu-id="fa9e6-126">application/json</span><span class="sxs-lookup"><span data-stu-id="fa9e6-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="fa9e6-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="fa9e6-127">Request body</span></span>
<span data-ttu-id="fa9e6-128">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="fa9e6-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="fa9e6-129">応答</span><span class="sxs-lookup"><span data-stu-id="fa9e6-129">Response</span></span>
<span data-ttu-id="fa9e6-130">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [managedIOSLobApp](../resources/intune-apps-managedioslobapp.md) オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="fa9e6-130">If successful, this method returns a `200 OK` response code and a collection of [managedIOSLobApp](../resources/intune-apps-managedioslobapp.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fa9e6-131">例</span><span class="sxs-lookup"><span data-stu-id="fa9e6-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="fa9e6-132">要求</span><span class="sxs-lookup"><span data-stu-id="fa9e6-132">Request</span></span>
<span data-ttu-id="fa9e6-133">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="fa9e6-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileApps
```

### <a name="response"></a><span data-ttu-id="fa9e6-134">応答</span><span class="sxs-lookup"><span data-stu-id="fa9e6-134">Response</span></span>
<span data-ttu-id="fa9e6-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="fa9e6-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1734

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.managedIOSLobApp",
      "id": "8f59792d-792d-8f59-2d79-598f2d79598f",
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
      "appAvailability": "lineOfBusiness",
      "version": "Version value",
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
  ]
}
```





