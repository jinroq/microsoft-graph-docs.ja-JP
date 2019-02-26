---
title: macoslobapps のリスト
description: macoslobapp オブジェクトのプロパティとリレーションシップをリストします。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 9c3cb679b3ec0afc8de9f2b9ae2fa98e77784e84
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/21/2019
ms.locfileid: "30140748"
---
# <a name="list-macoslobapps"></a><span data-ttu-id="77375-103">macoslobapps のリスト</span><span class="sxs-lookup"><span data-stu-id="77375-103">List macOSLobApps</span></span>

> <span data-ttu-id="77375-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="77375-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="77375-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="77375-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="77375-106">[macoslobapp](../resources/intune-apps-macoslobapp.md)オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="77375-106">List properties and relationships of the [macOSLobApp](../resources/intune-apps-macoslobapp.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="77375-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="77375-107">Prerequisites</span></span>
<span data-ttu-id="77375-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/concepts/permissions-reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="77375-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="77375-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="77375-110">Permission type</span></span>|<span data-ttu-id="77375-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="77375-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="77375-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="77375-112">Delegated (work or school account)</span></span>|<span data-ttu-id="77375-113">DeviceManagementApps.ReadWrite.All、DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="77375-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="77375-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="77375-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="77375-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="77375-115">Not supported.</span></span>|
|<span data-ttu-id="77375-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="77375-116">Application</span></span>|<span data-ttu-id="77375-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="77375-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="77375-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="77375-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="77375-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="77375-119">Request headers</span></span>
|<span data-ttu-id="77375-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="77375-120">Header</span></span>|<span data-ttu-id="77375-121">値</span><span class="sxs-lookup"><span data-stu-id="77375-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="77375-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="77375-122">Authorization</span></span>|<span data-ttu-id="77375-123">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="77375-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="77375-124">承諾</span><span class="sxs-lookup"><span data-stu-id="77375-124">Accept</span></span>|<span data-ttu-id="77375-125">application/json</span><span class="sxs-lookup"><span data-stu-id="77375-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="77375-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="77375-126">Request body</span></span>
<span data-ttu-id="77375-127">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="77375-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="77375-128">応答</span><span class="sxs-lookup"><span data-stu-id="77375-128">Response</span></span>
<span data-ttu-id="77375-129">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で[macoslobapp](../resources/intune-apps-macoslobapp.md)オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="77375-129">If successful, this method returns a `200 OK` response code and a collection of [macOSLobApp](../resources/intune-apps-macoslobapp.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="77375-130">例</span><span class="sxs-lookup"><span data-stu-id="77375-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="77375-131">要求</span><span class="sxs-lookup"><span data-stu-id="77375-131">Request</span></span>
<span data-ttu-id="77375-132">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="77375-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileApps
```

### <a name="response"></a><span data-ttu-id="77375-133">応答</span><span class="sxs-lookup"><span data-stu-id="77375-133">Response</span></span>
<span data-ttu-id="77375-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="77375-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1968

{
  "value": [
    {
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
  ]
}
```




