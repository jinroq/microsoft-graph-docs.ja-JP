---
title: windowsappx を取得する
description: windowsappx オブジェクトのプロパティとリレーションシップを読み取ります。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 525dd806a1fab98b9158a60d0523e980d03f792d
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/21/2019
ms.locfileid: "30145508"
---
# <a name="get-windowsappx"></a><span data-ttu-id="0eba5-103">windowsappx を取得する</span><span class="sxs-lookup"><span data-stu-id="0eba5-103">Get windowsAppX</span></span>

> <span data-ttu-id="0eba5-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="0eba5-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0eba5-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="0eba5-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0eba5-106">[windowsappx](../resources/intune-apps-windowsappx.md)オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="0eba5-106">Read properties and relationships of the [windowsAppX](../resources/intune-apps-windowsappx.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="0eba5-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="0eba5-107">Prerequisites</span></span>
<span data-ttu-id="0eba5-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/concepts/permissions-reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="0eba5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="0eba5-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="0eba5-110">Permission type</span></span>|<span data-ttu-id="0eba5-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="0eba5-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0eba5-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="0eba5-112">Delegated (work or school account)</span></span>|<span data-ttu-id="0eba5-113">DeviceManagementApps.ReadWrite.All、DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="0eba5-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="0eba5-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="0eba5-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0eba5-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="0eba5-115">Not supported.</span></span>|
|<span data-ttu-id="0eba5-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="0eba5-116">Application</span></span>|<span data-ttu-id="0eba5-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="0eba5-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="0eba5-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="0eba5-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps/{mobileAppId}
GET /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
GET /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="optional-query-parameters"></a><span data-ttu-id="0eba5-119">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="0eba5-119">Optional query parameters</span></span>
<span data-ttu-id="0eba5-120">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://docs.microsoft.com/en-us/graph/query-parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="0eba5-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="0eba5-121">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="0eba5-121">Request headers</span></span>
|<span data-ttu-id="0eba5-122">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="0eba5-122">Header</span></span>|<span data-ttu-id="0eba5-123">値</span><span class="sxs-lookup"><span data-stu-id="0eba5-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0eba5-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="0eba5-124">Authorization</span></span>|<span data-ttu-id="0eba5-125">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="0eba5-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0eba5-126">承諾</span><span class="sxs-lookup"><span data-stu-id="0eba5-126">Accept</span></span>|<span data-ttu-id="0eba5-127">application/json</span><span class="sxs-lookup"><span data-stu-id="0eba5-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0eba5-128">要求本文</span><span class="sxs-lookup"><span data-stu-id="0eba5-128">Request body</span></span>
<span data-ttu-id="0eba5-129">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="0eba5-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0eba5-130">応答</span><span class="sxs-lookup"><span data-stu-id="0eba5-130">Response</span></span>
<span data-ttu-id="0eba5-131">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で[windowsappx](../resources/intune-apps-windowsappx.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="0eba5-131">If successful, this method returns a `200 OK` response code and [windowsAppX](../resources/intune-apps-windowsappx.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0eba5-132">例</span><span class="sxs-lookup"><span data-stu-id="0eba5-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="0eba5-133">要求</span><span class="sxs-lookup"><span data-stu-id="0eba5-133">Request</span></span>
<span data-ttu-id="0eba5-134">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="0eba5-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}
```

### <a name="response"></a><span data-ttu-id="0eba5-135">応答</span><span class="sxs-lookup"><span data-stu-id="0eba5-135">Response</span></span>
<span data-ttu-id="0eba5-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="0eba5-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1617

{
  "value": {
    "@odata.type": "#microsoft.graph.windowsAppX",
    "id": "b5179a93-9a93-b517-939a-17b5939a17b5",
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
    "applicableArchitectures": "x86",
    "identityName": "Identity Name value",
    "identityPublisherHash": "Identity Publisher Hash value",
    "identityResourceIdentifier": "Identity Resource Identifier value",
    "isBundle": true,
    "minimumSupportedOperatingSystem": {
      "@odata.type": "microsoft.graph.windowsMinimumOperatingSystem",
      "v8_0": true,
      "v8_1": true,
      "v10_0": true,
      "v10_1607": true,
      "v10_1703": true,
      "v10_1709": true,
      "v10_1803": true
    },
    "identityVersion": "Identity Version value"
  }
}
```




