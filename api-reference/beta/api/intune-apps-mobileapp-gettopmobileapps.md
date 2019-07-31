---
title: getTopMobileApps 関数
description: まだ文書化されていません
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 56d1fc98281591fdf331992ddd7b3a5f23053234
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35961050"
---
# <a name="gettopmobileapps-function"></a><span data-ttu-id="53041-103">getTopMobileApps 関数</span><span class="sxs-lookup"><span data-stu-id="53041-103">getTopMobileApps function</span></span>

> <span data-ttu-id="53041-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="53041-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="53041-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="53041-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="53041-106">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="53041-106">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="53041-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="53041-107">Prerequisites</span></span>
<span data-ttu-id="53041-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="53041-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="53041-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="53041-110">Permission type</span></span>|<span data-ttu-id="53041-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="53041-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="53041-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="53041-112">Delegated (work or school account)</span></span>|<span data-ttu-id="53041-113">DeviceManagementApps.ReadWrite.All、DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="53041-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="53041-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="53041-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="53041-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="53041-115">Not supported.</span></span>|
|<span data-ttu-id="53041-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="53041-116">Application</span></span>|<span data-ttu-id="53041-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="53041-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="53041-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="53041-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps/getTopMobileApps
```

## <a name="request-headers"></a><span data-ttu-id="53041-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="53041-119">Request headers</span></span>
|<span data-ttu-id="53041-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="53041-120">Header</span></span>|<span data-ttu-id="53041-121">値</span><span class="sxs-lookup"><span data-stu-id="53041-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="53041-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="53041-122">Authorization</span></span>|<span data-ttu-id="53041-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="53041-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="53041-124">承諾</span><span class="sxs-lookup"><span data-stu-id="53041-124">Accept</span></span>|<span data-ttu-id="53041-125">application/json</span><span class="sxs-lookup"><span data-stu-id="53041-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="53041-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="53041-126">Request body</span></span>
<span data-ttu-id="53041-127">要求 URL で、次のクエリ パラメーターに値を指定します。</span><span class="sxs-lookup"><span data-stu-id="53041-127">In the request URL, provide the following query parameters with values.</span></span>
<span data-ttu-id="53041-128">次の表に、この関数で使用できるパラメーターを示します。</span><span class="sxs-lookup"><span data-stu-id="53041-128">The following table shows the parameters that can be used with this function.</span></span>

|<span data-ttu-id="53041-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="53041-129">Property</span></span>|<span data-ttu-id="53041-130">型</span><span class="sxs-lookup"><span data-stu-id="53041-130">Type</span></span>|<span data-ttu-id="53041-131">説明</span><span class="sxs-lookup"><span data-stu-id="53041-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="53041-132">status</span><span class="sxs-lookup"><span data-stu-id="53041-132">status</span></span>|<span data-ttu-id="53041-133">String</span><span class="sxs-lookup"><span data-stu-id="53041-133">String</span></span>|<span data-ttu-id="53041-134">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="53041-134">Not yet documented</span></span>|
|<span data-ttu-id="53041-135">count</span><span class="sxs-lookup"><span data-stu-id="53041-135">count</span></span>|<span data-ttu-id="53041-136">Int64</span><span class="sxs-lookup"><span data-stu-id="53041-136">Int64</span></span>|<span data-ttu-id="53041-137">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="53041-137">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="53041-138">応答</span><span class="sxs-lookup"><span data-stu-id="53041-138">Response</span></span>
<span data-ttu-id="53041-139">成功した場合、この関数`200 OK`は応答コードと、応答本文で[mobileApp](../resources/intune-apps-mobileapp.md)コレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="53041-139">If successful, this function returns a `200 OK` response code and a [mobileApp](../resources/intune-apps-mobileapp.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="53041-140">例</span><span class="sxs-lookup"><span data-stu-id="53041-140">Example</span></span>

### <a name="request"></a><span data-ttu-id="53041-141">要求</span><span class="sxs-lookup"><span data-stu-id="53041-141">Request</span></span>
<span data-ttu-id="53041-142">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="53041-142">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/getTopMobileApps(status='parameterValue',count=5)
```

### <a name="response"></a><span data-ttu-id="53041-143">応答</span><span class="sxs-lookup"><span data-stu-id="53041-143">Response</span></span>
<span data-ttu-id="53041-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="53041-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1013

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.mobileApp",
      "id": "0177548a-548a-0177-8a54-77018a547701",
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
      "dependentAppCount": 1
    }
  ]
}
```





