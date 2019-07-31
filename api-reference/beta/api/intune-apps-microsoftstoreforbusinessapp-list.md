---
title: microsoftStoreForBusinessApps のリスト
description: microsoftStoreForBusinessApp オブジェクトのプロパティとリレーションシップをリストします。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: fe78ffd739f2b8cb926843333f8867b9dbb33944
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35961204"
---
# <a name="list-microsoftstoreforbusinessapps"></a><span data-ttu-id="11648-103">microsoftStoreForBusinessApps のリスト</span><span class="sxs-lookup"><span data-stu-id="11648-103">List microsoftStoreForBusinessApps</span></span>

> <span data-ttu-id="11648-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="11648-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="11648-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="11648-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="11648-106">[microsoftStoreForBusinessApp](../resources/intune-apps-microsoftstoreforbusinessapp.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="11648-106">List properties and relationships of the [microsoftStoreForBusinessApp](../resources/intune-apps-microsoftstoreforbusinessapp.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="11648-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="11648-107">Prerequisites</span></span>
<span data-ttu-id="11648-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="11648-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="11648-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="11648-110">Permission type</span></span>|<span data-ttu-id="11648-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="11648-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="11648-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="11648-112">Delegated (work or school account)</span></span>|<span data-ttu-id="11648-113">DeviceManagementApps.ReadWrite.All、DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="11648-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="11648-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="11648-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="11648-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="11648-115">Not supported.</span></span>|
|<span data-ttu-id="11648-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="11648-116">Application</span></span>|<span data-ttu-id="11648-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="11648-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="11648-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="11648-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="11648-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="11648-119">Request headers</span></span>
|<span data-ttu-id="11648-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="11648-120">Header</span></span>|<span data-ttu-id="11648-121">値</span><span class="sxs-lookup"><span data-stu-id="11648-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="11648-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="11648-122">Authorization</span></span>|<span data-ttu-id="11648-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="11648-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="11648-124">承諾</span><span class="sxs-lookup"><span data-stu-id="11648-124">Accept</span></span>|<span data-ttu-id="11648-125">application/json</span><span class="sxs-lookup"><span data-stu-id="11648-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="11648-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="11648-126">Request body</span></span>
<span data-ttu-id="11648-127">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="11648-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="11648-128">応答</span><span class="sxs-lookup"><span data-stu-id="11648-128">Response</span></span>
<span data-ttu-id="11648-129">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [microsoftStoreForBusinessApp](../resources/intune-apps-microsoftstoreforbusinessapp.md) オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="11648-129">If successful, this method returns a `200 OK` response code and a collection of [microsoftStoreForBusinessApp](../resources/intune-apps-microsoftstoreforbusinessapp.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="11648-130">例</span><span class="sxs-lookup"><span data-stu-id="11648-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="11648-131">要求</span><span class="sxs-lookup"><span data-stu-id="11648-131">Request</span></span>
<span data-ttu-id="11648-132">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="11648-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileApps
```

### <a name="response"></a><span data-ttu-id="11648-133">応答</span><span class="sxs-lookup"><span data-stu-id="11648-133">Response</span></span>
<span data-ttu-id="11648-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="11648-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1485

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.microsoftStoreForBusinessApp",
      "id": "f33358bc-58bc-f333-bc58-33f3bc5833f3",
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
      "productKey": "Product Key value",
      "licenseType": "online",
      "packageIdentityName": "Package Identity Name value",
      "licensingType": {
        "@odata.type": "microsoft.graph.vppLicensingType",
        "supportUserLicensing": true,
        "supportDeviceLicensing": true,
        "supportsUserLicensing": true,
        "supportsDeviceLicensing": true
      }
    }
  ]
}
```





