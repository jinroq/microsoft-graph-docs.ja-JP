---
title: リスト appLogCollectionRequests
description: AppLogCollectionRequest オブジェクトのプロパティとリレーションシップをリストします。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 90fcf1d6e3eb5997466bc967e443712f7c8fb2f2
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36310725"
---
# <a name="list-applogcollectionrequests"></a><span data-ttu-id="0cac1-103">リスト appLogCollectionRequests</span><span class="sxs-lookup"><span data-stu-id="0cac1-103">List appLogCollectionRequests</span></span>

> <span data-ttu-id="0cac1-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="0cac1-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0cac1-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="0cac1-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0cac1-106">[AppLogCollectionRequest](../resources/intune-devices-applogcollectionrequest.md)オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="0cac1-106">List properties and relationships of the [appLogCollectionRequest](../resources/intune-devices-applogcollectionrequest.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="0cac1-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="0cac1-107">Prerequisites</span></span>
<span data-ttu-id="0cac1-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="0cac1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0cac1-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="0cac1-110">Permission type</span></span>|<span data-ttu-id="0cac1-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="0cac1-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0cac1-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="0cac1-112">Delegated (work or school account)</span></span>|<span data-ttu-id="0cac1-113">DeviceManagementManagedDevices.ReadWrite.All、DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="0cac1-113">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="0cac1-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="0cac1-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0cac1-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="0cac1-115">Not supported.</span></span>|
|<span data-ttu-id="0cac1-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="0cac1-116">Application</span></span>|<span data-ttu-id="0cac1-117">DeviceManagementManagedDevices.ReadWrite.All、DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="0cac1-117">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="0cac1-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="0cac1-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/mobileAppTroubleshootingEvents/{mobileAppTroubleshootingEventId}/appLogCollectionRequests
```

## <a name="request-headers"></a><span data-ttu-id="0cac1-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="0cac1-119">Request headers</span></span>
|<span data-ttu-id="0cac1-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="0cac1-120">Header</span></span>|<span data-ttu-id="0cac1-121">値</span><span class="sxs-lookup"><span data-stu-id="0cac1-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0cac1-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="0cac1-122">Authorization</span></span>|<span data-ttu-id="0cac1-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="0cac1-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0cac1-124">承諾</span><span class="sxs-lookup"><span data-stu-id="0cac1-124">Accept</span></span>|<span data-ttu-id="0cac1-125">application/json</span><span class="sxs-lookup"><span data-stu-id="0cac1-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0cac1-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="0cac1-126">Request body</span></span>
<span data-ttu-id="0cac1-127">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="0cac1-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0cac1-128">応答</span><span class="sxs-lookup"><span data-stu-id="0cac1-128">Response</span></span>
<span data-ttu-id="0cac1-129">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で[appLogCollectionRequest](../resources/intune-devices-applogcollectionrequest.md)オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="0cac1-129">If successful, this method returns a `200 OK` response code and a collection of [appLogCollectionRequest](../resources/intune-devices-applogcollectionrequest.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0cac1-130">例</span><span class="sxs-lookup"><span data-stu-id="0cac1-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="0cac1-131">要求</span><span class="sxs-lookup"><span data-stu-id="0cac1-131">Request</span></span>
<span data-ttu-id="0cac1-132">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="0cac1-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/mobileAppTroubleshootingEvents/{mobileAppTroubleshootingEventId}/appLogCollectionRequests
```

### <a name="response"></a><span data-ttu-id="0cac1-133">応答</span><span class="sxs-lookup"><span data-stu-id="0cac1-133">Response</span></span>
<span data-ttu-id="0cac1-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="0cac1-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 371

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.appLogCollectionRequest",
      "id": "cca685ff-85ff-cca6-ff85-a6ccff85a6cc",
      "status": "completed",
      "errorMessage": "Error Message value",
      "customLogFolders": [
        "Custom Log Folders value"
      ],
      "completedDateTime": "2016-12-31T23:58:52.3534526-08:00"
    }
  ]
}
```






