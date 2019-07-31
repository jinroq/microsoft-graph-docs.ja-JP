---
title: windowsMobileMSIs のリスト
description: windowsMobileMSI オブジェクトのプロパティとリレーションシップをリストします。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 0a7c61dfafb96f0a6e4a8e8211ac416d5c7734a2
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35960084"
---
# <a name="list-windowsmobilemsis"></a><span data-ttu-id="86a10-103">windowsMobileMSIs のリスト</span><span class="sxs-lookup"><span data-stu-id="86a10-103">List windowsMobileMSIs</span></span>

> <span data-ttu-id="86a10-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="86a10-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="86a10-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="86a10-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="86a10-106">[windowsMobileMSI](../resources/intune-apps-windowsmobilemsi.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="86a10-106">List properties and relationships of the [windowsMobileMSI](../resources/intune-apps-windowsmobilemsi.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="86a10-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="86a10-107">Prerequisites</span></span>
<span data-ttu-id="86a10-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="86a10-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="86a10-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="86a10-110">Permission type</span></span>|<span data-ttu-id="86a10-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="86a10-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="86a10-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="86a10-112">Delegated (work or school account)</span></span>|<span data-ttu-id="86a10-113">DeviceManagementApps.ReadWrite.All、DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="86a10-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="86a10-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="86a10-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="86a10-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="86a10-115">Not supported.</span></span>|
|<span data-ttu-id="86a10-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="86a10-116">Application</span></span>|<span data-ttu-id="86a10-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="86a10-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="86a10-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="86a10-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="86a10-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="86a10-119">Request headers</span></span>
|<span data-ttu-id="86a10-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="86a10-120">Header</span></span>|<span data-ttu-id="86a10-121">値</span><span class="sxs-lookup"><span data-stu-id="86a10-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="86a10-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="86a10-122">Authorization</span></span>|<span data-ttu-id="86a10-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="86a10-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="86a10-124">承諾</span><span class="sxs-lookup"><span data-stu-id="86a10-124">Accept</span></span>|<span data-ttu-id="86a10-125">application/json</span><span class="sxs-lookup"><span data-stu-id="86a10-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="86a10-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="86a10-126">Request body</span></span>
<span data-ttu-id="86a10-127">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="86a10-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="86a10-128">応答</span><span class="sxs-lookup"><span data-stu-id="86a10-128">Response</span></span>
<span data-ttu-id="86a10-129">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [windowsMobileMSI](../resources/intune-apps-windowsmobilemsi.md) オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="86a10-129">If successful, this method returns a `200 OK` response code and a collection of [windowsMobileMSI](../resources/intune-apps-windowsmobilemsi.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="86a10-130">例</span><span class="sxs-lookup"><span data-stu-id="86a10-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="86a10-131">要求</span><span class="sxs-lookup"><span data-stu-id="86a10-131">Request</span></span>
<span data-ttu-id="86a10-132">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="86a10-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileApps
```

### <a name="response"></a><span data-ttu-id="86a10-133">応答</span><span class="sxs-lookup"><span data-stu-id="86a10-133">Response</span></span>
<span data-ttu-id="86a10-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="86a10-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1407

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.windowsMobileMSI",
      "id": "aa453e5d-3e5d-aa45-5d3e-45aa5d3e45aa",
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
      "size": 4,
      "commandLine": "Command Line value",
      "productCode": "Product Code value",
      "productVersion": "Product Version value",
      "ignoreVersionDetection": true,
      "identityVersion": "Identity Version value",
      "useDeviceContext": true
    }
  ]
}
```





