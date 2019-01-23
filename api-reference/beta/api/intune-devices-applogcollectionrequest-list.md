---
title: リスト appLogCollectionRequests
description: AppLogCollectionRequest オブジェクトのプロパティと関係を一覧表示します。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: f5cab95b3a7c4315e1d895e8dcc73c1f0cfc0278
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29430487"
---
# <a name="list-applogcollectionrequests"></a><span data-ttu-id="4e7ad-103">リスト appLogCollectionRequests</span><span class="sxs-lookup"><span data-stu-id="4e7ad-103">List appLogCollectionRequests</span></span>

> <span data-ttu-id="4e7ad-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="4e7ad-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="4e7ad-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="4e7ad-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="4e7ad-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="4e7ad-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4e7ad-107">[AppLogCollectionRequest](../resources/intune-devices-applogcollectionrequest.md)オブジェクトのプロパティと関係を一覧表示します。</span><span class="sxs-lookup"><span data-stu-id="4e7ad-107">List properties and relationships of the [appLogCollectionRequest](../resources/intune-devices-applogcollectionrequest.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="4e7ad-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="4e7ad-108">Prerequisites</span></span>
<span data-ttu-id="4e7ad-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/concepts/permissions-reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="4e7ad-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="4e7ad-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="4e7ad-111">Permission type</span></span>|<span data-ttu-id="4e7ad-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="4e7ad-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4e7ad-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="4e7ad-113">Delegated (work or school account)</span></span>|<span data-ttu-id="4e7ad-114">DeviceManagementManagedDevices.ReadWrite.All、DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="4e7ad-114">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="4e7ad-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="4e7ad-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4e7ad-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="4e7ad-116">Not supported.</span></span>|
|<span data-ttu-id="4e7ad-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="4e7ad-117">Application</span></span>|<span data-ttu-id="4e7ad-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="4e7ad-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="4e7ad-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="4e7ad-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/mobileAppTroubleshootingEvents/{mobileAppTroubleshootingEventId}/appLogCollectionRequests
```

## <a name="request-headers"></a><span data-ttu-id="4e7ad-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="4e7ad-120">Request headers</span></span>
|<span data-ttu-id="4e7ad-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="4e7ad-121">Header</span></span>|<span data-ttu-id="4e7ad-122">値</span><span class="sxs-lookup"><span data-stu-id="4e7ad-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4e7ad-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="4e7ad-123">Authorization</span></span>|<span data-ttu-id="4e7ad-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="4e7ad-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4e7ad-125">Accept</span><span class="sxs-lookup"><span data-stu-id="4e7ad-125">Accept</span></span>|<span data-ttu-id="4e7ad-126">application/json</span><span class="sxs-lookup"><span data-stu-id="4e7ad-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4e7ad-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="4e7ad-127">Request body</span></span>
<span data-ttu-id="4e7ad-128">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="4e7ad-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4e7ad-129">応答</span><span class="sxs-lookup"><span data-stu-id="4e7ad-129">Response</span></span>
<span data-ttu-id="4e7ad-130">かどうかは成功すると、このメソッドが返されます、`200 OK`応答コードおよび応答の本文に[appLogCollectionRequest](../resources/intune-devices-applogcollectionrequest.md)オブジェクトのコレクションです。</span><span class="sxs-lookup"><span data-stu-id="4e7ad-130">If successful, this method returns a `200 OK` response code and a collection of [appLogCollectionRequest](../resources/intune-devices-applogcollectionrequest.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4e7ad-131">例</span><span class="sxs-lookup"><span data-stu-id="4e7ad-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="4e7ad-132">要求</span><span class="sxs-lookup"><span data-stu-id="4e7ad-132">Request</span></span>
<span data-ttu-id="4e7ad-133">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="4e7ad-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/mobileAppTroubleshootingEvents/{mobileAppTroubleshootingEventId}/appLogCollectionRequests
```

### <a name="response"></a><span data-ttu-id="4e7ad-134">応答</span><span class="sxs-lookup"><span data-stu-id="4e7ad-134">Response</span></span>
<span data-ttu-id="4e7ad-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="4e7ad-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




