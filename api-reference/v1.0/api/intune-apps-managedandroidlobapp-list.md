---
title: managedAndroidLobApps のリスト
description: managedAndroidLobApp オブジェクトのプロパティとリレーションシップをリストします。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 83bccc0e670db6e7ed3db144854a887514a95f00
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32578632"
---
# <a name="list-managedandroidlobapps"></a><span data-ttu-id="12460-103">managedAndroidLobApps のリスト</span><span class="sxs-lookup"><span data-stu-id="12460-103">List managedAndroidLobApps</span></span>

> <span data-ttu-id="12460-104">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="12460-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="12460-105">[managedAndroidLobApp](../resources/intune-apps-managedandroidlobapp.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="12460-105">List properties and relationships of the [managedAndroidLobApp](../resources/intune-apps-managedandroidlobapp.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="12460-106">前提条件</span><span class="sxs-lookup"><span data-stu-id="12460-106">Prerequisites</span></span>
<span data-ttu-id="12460-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="12460-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="12460-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="12460-109">Permission type</span></span>|<span data-ttu-id="12460-110">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="12460-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="12460-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="12460-111">Delegated (work or school account)</span></span>|<span data-ttu-id="12460-112">DeviceManagementApps.ReadWrite.All、DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="12460-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="12460-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="12460-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="12460-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="12460-114">Not supported.</span></span>|
|<span data-ttu-id="12460-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="12460-115">Application</span></span>|<span data-ttu-id="12460-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="12460-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="12460-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="12460-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="12460-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="12460-118">Request headers</span></span>
|<span data-ttu-id="12460-119">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="12460-119">Header</span></span>|<span data-ttu-id="12460-120">値</span><span class="sxs-lookup"><span data-stu-id="12460-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="12460-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="12460-121">Authorization</span></span>|<span data-ttu-id="12460-122">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="12460-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="12460-123">承諾</span><span class="sxs-lookup"><span data-stu-id="12460-123">Accept</span></span>|<span data-ttu-id="12460-124">application/json</span><span class="sxs-lookup"><span data-stu-id="12460-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="12460-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="12460-125">Request body</span></span>
<span data-ttu-id="12460-126">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="12460-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="12460-127">応答</span><span class="sxs-lookup"><span data-stu-id="12460-127">Response</span></span>
<span data-ttu-id="12460-128">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [managedAndroidLobApp](../resources/intune-apps-managedandroidlobapp.md) オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="12460-128">If successful, this method returns a `200 OK` response code and a collection of [managedAndroidLobApp](../resources/intune-apps-managedandroidlobapp.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="12460-129">例</span><span class="sxs-lookup"><span data-stu-id="12460-129">Example</span></span>

### <a name="request"></a><span data-ttu-id="12460-130">要求</span><span class="sxs-lookup"><span data-stu-id="12460-130">Request</span></span>
<span data-ttu-id="12460-131">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="12460-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps
```

### <a name="response"></a><span data-ttu-id="12460-132">応答</span><span class="sxs-lookup"><span data-stu-id="12460-132">Response</span></span>
<span data-ttu-id="12460-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="12460-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1510

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.managedAndroidLobApp",
      "id": "802b7ed3-7ed3-802b-d37e-2b80d37e2b80",
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
      "committedContentVersion": "Committed Content Version value",
      "fileName": "File Name value",
      "size": 4,
      "packageId": "Package Id value",
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
      },
      "versionName": "Version Name value",
      "versionCode": "Version Code value"
    }
  ]
}
```



