---
title: Get managedApp
description: managedApp オブジェクトのプロパティとリレーションシップを読み取ります。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 9a14d16cc8ab64eb019919f9b8f12bc1a4dcc015
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32578541"
---
# <a name="get-managedapp"></a><span data-ttu-id="d28bf-103">Get managedApp</span><span class="sxs-lookup"><span data-stu-id="d28bf-103">Get managedApp</span></span>

> <span data-ttu-id="d28bf-104">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="d28bf-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d28bf-105">[managedApp](../resources/intune-apps-managedapp.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="d28bf-105">Read properties and relationships of the [managedApp](../resources/intune-apps-managedapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d28bf-106">前提条件</span><span class="sxs-lookup"><span data-stu-id="d28bf-106">Prerequisites</span></span>
<span data-ttu-id="d28bf-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="d28bf-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d28bf-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="d28bf-109">Permission type</span></span>|<span data-ttu-id="d28bf-110">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="d28bf-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d28bf-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="d28bf-111">Delegated (work or school account)</span></span>|<span data-ttu-id="d28bf-112">DeviceManagementApps.ReadWrite.All、DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="d28bf-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="d28bf-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="d28bf-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d28bf-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d28bf-114">Not supported.</span></span>|
|<span data-ttu-id="d28bf-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="d28bf-115">Application</span></span>|<span data-ttu-id="d28bf-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d28bf-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d28bf-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="d28bf-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps/{mobileAppId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="d28bf-118">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="d28bf-118">Optional query parameters</span></span>
<span data-ttu-id="d28bf-119">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://docs.microsoft.com/en-us/graph/query-parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="d28bf-119">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="d28bf-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="d28bf-120">Request headers</span></span>
|<span data-ttu-id="d28bf-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="d28bf-121">Header</span></span>|<span data-ttu-id="d28bf-122">値</span><span class="sxs-lookup"><span data-stu-id="d28bf-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d28bf-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="d28bf-123">Authorization</span></span>|<span data-ttu-id="d28bf-124">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="d28bf-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d28bf-125">承諾</span><span class="sxs-lookup"><span data-stu-id="d28bf-125">Accept</span></span>|<span data-ttu-id="d28bf-126">application/json</span><span class="sxs-lookup"><span data-stu-id="d28bf-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d28bf-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="d28bf-127">Request body</span></span>
<span data-ttu-id="d28bf-128">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="d28bf-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d28bf-129">応答</span><span class="sxs-lookup"><span data-stu-id="d28bf-129">Response</span></span>
<span data-ttu-id="d28bf-130">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [managedApp](../resources/intune-apps-managedapp.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="d28bf-130">If successful, this method returns a `200 OK` response code and [managedApp](../resources/intune-apps-managedapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d28bf-131">例</span><span class="sxs-lookup"><span data-stu-id="d28bf-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="d28bf-132">要求</span><span class="sxs-lookup"><span data-stu-id="d28bf-132">Request</span></span>
<span data-ttu-id="d28bf-133">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="d28bf-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps/{mobileAppId}
```

### <a name="response"></a><span data-ttu-id="d28bf-134">応答</span><span class="sxs-lookup"><span data-stu-id="d28bf-134">Response</span></span>
<span data-ttu-id="d28bf-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="d28bf-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 879

{
  "value": {
    "@odata.type": "#microsoft.graph.managedApp",
    "id": "f687dd85-dd85-f687-85dd-87f685dd87f6",
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
    "version": "Version value"
  }
}
```



