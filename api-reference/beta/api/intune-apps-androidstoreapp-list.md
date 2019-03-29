---
title: androidStoreApps のリスト
description: androidStoreApp オブジェクトのプロパティとリレーションシップをリストします。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: f0ab42416053a69795cb660db4eac3ab77fb6ca6
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/29/2019
ms.locfileid: "30977262"
---
# <a name="list-androidstoreapps"></a><span data-ttu-id="bd72b-103">androidStoreApps のリスト</span><span class="sxs-lookup"><span data-stu-id="bd72b-103">List androidStoreApps</span></span>

> <span data-ttu-id="bd72b-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="bd72b-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="bd72b-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="bd72b-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bd72b-106">[androidStoreApp](../resources/intune-apps-androidstoreapp.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="bd72b-106">List properties and relationships of the [androidStoreApp](../resources/intune-apps-androidstoreapp.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="bd72b-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="bd72b-107">Prerequisites</span></span>
<span data-ttu-id="bd72b-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="bd72b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bd72b-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="bd72b-110">Permission type</span></span>|<span data-ttu-id="bd72b-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="bd72b-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="bd72b-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="bd72b-112">Delegated (work or school account)</span></span>|<span data-ttu-id="bd72b-113">DeviceManagementApps.ReadWrite.All、DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="bd72b-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="bd72b-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="bd72b-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="bd72b-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="bd72b-115">Not supported.</span></span>|
|<span data-ttu-id="bd72b-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="bd72b-116">Application</span></span>|<span data-ttu-id="bd72b-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="bd72b-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="bd72b-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="bd72b-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="bd72b-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="bd72b-119">Request headers</span></span>
|<span data-ttu-id="bd72b-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="bd72b-120">Header</span></span>|<span data-ttu-id="bd72b-121">値</span><span class="sxs-lookup"><span data-stu-id="bd72b-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="bd72b-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="bd72b-122">Authorization</span></span>|<span data-ttu-id="bd72b-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="bd72b-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="bd72b-124">承諾</span><span class="sxs-lookup"><span data-stu-id="bd72b-124">Accept</span></span>|<span data-ttu-id="bd72b-125">application/json</span><span class="sxs-lookup"><span data-stu-id="bd72b-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="bd72b-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="bd72b-126">Request body</span></span>
<span data-ttu-id="bd72b-127">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="bd72b-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="bd72b-128">応答</span><span class="sxs-lookup"><span data-stu-id="bd72b-128">Response</span></span>
<span data-ttu-id="bd72b-129">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [androidStoreApp](../resources/intune-apps-androidstoreapp.md) オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="bd72b-129">If successful, this method returns a `200 OK` response code and a collection of [androidStoreApp](../resources/intune-apps-androidstoreapp.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bd72b-130">例</span><span class="sxs-lookup"><span data-stu-id="bd72b-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="bd72b-131">要求</span><span class="sxs-lookup"><span data-stu-id="bd72b-131">Request</span></span>
<span data-ttu-id="bd72b-132">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="bd72b-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileApps
```

### <a name="response"></a><span data-ttu-id="bd72b-133">応答</span><span class="sxs-lookup"><span data-stu-id="bd72b-133">Response</span></span>
<span data-ttu-id="bd72b-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="bd72b-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1584

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.androidStoreApp",
      "id": "1f2b7654-7654-1f2b-5476-2b1f54762b1f",
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
      "packageId": "Package Id value",
      "appIdentifier": "App Identifier value",
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
        "v5_1": true,
        "v6_0": true,
        "v7_0": true,
        "v7_1": true,
        "v8_0": true,
        "v8_1": true,
        "v9_0": true
      }
    }
  ]
}
```




