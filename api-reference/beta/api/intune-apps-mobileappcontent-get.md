---
title: Get mobileAppContent
description: mobileAppContent オブジェクトのプロパティとリレーションシップを読み取ります。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 5edb196c3f7e6cb156aefe7063e4314099f47a4a
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36329251"
---
# <a name="get-mobileappcontent"></a><span data-ttu-id="e3259-103">Get mobileAppContent</span><span class="sxs-lookup"><span data-stu-id="e3259-103">Get mobileAppContent</span></span>

> <span data-ttu-id="e3259-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e3259-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e3259-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="e3259-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e3259-106">[mobileAppContent](../resources/intune-apps-mobileappcontent.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="e3259-106">Read properties and relationships of the [mobileAppContent](../resources/intune-apps-mobileappcontent.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e3259-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="e3259-107">Prerequisites</span></span>
<span data-ttu-id="e3259-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="e3259-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e3259-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="e3259-110">Permission type</span></span>|<span data-ttu-id="e3259-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="e3259-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e3259-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="e3259-112">Delegated (work or school account)</span></span>|<span data-ttu-id="e3259-113">DeviceManagementApps.ReadWrite.All、DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="e3259-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="e3259-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="e3259-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e3259-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e3259-115">Not supported.</span></span>|
|<span data-ttu-id="e3259-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="e3259-116">Application</span></span>|<span data-ttu-id="e3259-117">DeviceManagementApps.ReadWrite.All、DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="e3259-117">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="e3259-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="e3259-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps/{mobileAppId}/contentVersions/{mobileAppContentId}
GET /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.mobileLobApp/contentVersions/{mobileAppContentId}
GET /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.managedMobileLobApp/contentVersions/{mobileAppContentId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="e3259-119">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="e3259-119">Optional query parameters</span></span>
<span data-ttu-id="e3259-120">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://docs.microsoft.com/en-us/graph/query-parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="e3259-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="e3259-121">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="e3259-121">Request headers</span></span>
|<span data-ttu-id="e3259-122">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="e3259-122">Header</span></span>|<span data-ttu-id="e3259-123">値</span><span class="sxs-lookup"><span data-stu-id="e3259-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e3259-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="e3259-124">Authorization</span></span>|<span data-ttu-id="e3259-125">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="e3259-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e3259-126">承諾</span><span class="sxs-lookup"><span data-stu-id="e3259-126">Accept</span></span>|<span data-ttu-id="e3259-127">application/json</span><span class="sxs-lookup"><span data-stu-id="e3259-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e3259-128">要求本文</span><span class="sxs-lookup"><span data-stu-id="e3259-128">Request body</span></span>
<span data-ttu-id="e3259-129">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="e3259-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e3259-130">応答</span><span class="sxs-lookup"><span data-stu-id="e3259-130">Response</span></span>
<span data-ttu-id="e3259-131">成功した場合、このメソッドは `200 OK` 応答コードと応答本文で [mobileAppContent](../resources/intune-apps-mobileappcontent.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="e3259-131">If successful, this method returns a `200 OK` response code and [mobileAppContent](../resources/intune-apps-mobileappcontent.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e3259-132">例</span><span class="sxs-lookup"><span data-stu-id="e3259-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="e3259-133">要求</span><span class="sxs-lookup"><span data-stu-id="e3259-133">Request</span></span>
<span data-ttu-id="e3259-134">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="e3259-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/contentVersions/{mobileAppContentId}
```

### <a name="response"></a><span data-ttu-id="e3259-135">応答</span><span class="sxs-lookup"><span data-stu-id="e3259-135">Response</span></span>
<span data-ttu-id="e3259-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="e3259-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 130

{
  "value": {
    "@odata.type": "#microsoft.graph.mobileAppContent",
    "id": "fe0bb9a9-b9a9-fe0b-a9b9-0bfea9b90bfe"
  }
}
```






