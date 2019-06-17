---
title: Get mobileLobApp
description: mobileLobApp オブジェクトのプロパティとリレーションシップを読み取ります。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 71ca4b489ee1ec9478f77a337e08b3730cc94c56
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/14/2019
ms.locfileid: "34973587"
---
# <a name="get-mobilelobapp"></a><span data-ttu-id="56625-103">Get mobileLobApp</span><span class="sxs-lookup"><span data-stu-id="56625-103">Get mobileLobApp</span></span>

> <span data-ttu-id="56625-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="56625-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="56625-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="56625-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="56625-106">[mobileLobApp](../resources/intune-apps-mobilelobapp.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="56625-106">Read properties and relationships of the [mobileLobApp](../resources/intune-apps-mobilelobapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="56625-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="56625-107">Prerequisites</span></span>
<span data-ttu-id="56625-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="56625-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="56625-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="56625-110">Permission type</span></span>|<span data-ttu-id="56625-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="56625-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="56625-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="56625-112">Delegated (work or school account)</span></span>|<span data-ttu-id="56625-113">DeviceManagementApps.ReadWrite.All、DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="56625-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="56625-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="56625-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="56625-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="56625-115">Not supported.</span></span>|
|<span data-ttu-id="56625-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="56625-116">Application</span></span>|<span data-ttu-id="56625-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="56625-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="56625-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="56625-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps/{mobileAppId}
GET /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
GET /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="optional-query-parameters"></a><span data-ttu-id="56625-119">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="56625-119">Optional query parameters</span></span>
<span data-ttu-id="56625-120">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://docs.microsoft.com/en-us/graph/query-parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="56625-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="56625-121">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="56625-121">Request headers</span></span>
|<span data-ttu-id="56625-122">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="56625-122">Header</span></span>|<span data-ttu-id="56625-123">値</span><span class="sxs-lookup"><span data-stu-id="56625-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="56625-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="56625-124">Authorization</span></span>|<span data-ttu-id="56625-125">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="56625-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="56625-126">承諾</span><span class="sxs-lookup"><span data-stu-id="56625-126">Accept</span></span>|<span data-ttu-id="56625-127">application/json</span><span class="sxs-lookup"><span data-stu-id="56625-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="56625-128">要求本文</span><span class="sxs-lookup"><span data-stu-id="56625-128">Request body</span></span>
<span data-ttu-id="56625-129">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="56625-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="56625-130">応答</span><span class="sxs-lookup"><span data-stu-id="56625-130">Response</span></span>
<span data-ttu-id="56625-131">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [mobileLobApp](../resources/intune-apps-mobilelobapp.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="56625-131">If successful, this method returns a `200 OK` response code and [mobileLobApp](../resources/intune-apps-mobilelobapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="56625-132">例</span><span class="sxs-lookup"><span data-stu-id="56625-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="56625-133">要求</span><span class="sxs-lookup"><span data-stu-id="56625-133">Request</span></span>
<span data-ttu-id="56625-134">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="56625-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}
```

### <a name="response"></a><span data-ttu-id="56625-135">応答</span><span class="sxs-lookup"><span data-stu-id="56625-135">Response</span></span>
<span data-ttu-id="56625-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="56625-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1071

{
  "value": {
    "@odata.type": "#microsoft.graph.mobileLobApp",
    "id": "2fc11935-1935-2fc1-3519-c12f3519c12f",
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
    "size": 4
  }
}
```





