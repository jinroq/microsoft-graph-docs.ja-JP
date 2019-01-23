---
title: リスト mobileAppInstallStatuses
description: MobileAppInstallStatus オブジェクトのプロパティと関係を一覧表示します。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: e227f2c03bdbbf4f09826a1dd58150704119550e
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29401664"
---
# <a name="list-mobileappinstallstatuses"></a><span data-ttu-id="79b7b-103">リスト mobileAppInstallStatuses</span><span class="sxs-lookup"><span data-stu-id="79b7b-103">List mobileAppInstallStatuses</span></span>

> <span data-ttu-id="79b7b-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="79b7b-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="79b7b-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="79b7b-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="79b7b-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="79b7b-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="79b7b-107">[MobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md)オブジェクトのプロパティと関係を一覧表示します。</span><span class="sxs-lookup"><span data-stu-id="79b7b-107">List properties and relationships of the [mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="79b7b-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="79b7b-108">Prerequisites</span></span>
<span data-ttu-id="79b7b-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/concepts/permissions-reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="79b7b-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="79b7b-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="79b7b-111">Permission type</span></span>|<span data-ttu-id="79b7b-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="79b7b-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="79b7b-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="79b7b-113">Delegated (work or school account)</span></span>|<span data-ttu-id="79b7b-114">DeviceManagementApps.ReadWrite.All、DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="79b7b-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="79b7b-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="79b7b-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="79b7b-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="79b7b-116">Not supported.</span></span>|
|<span data-ttu-id="79b7b-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="79b7b-117">Application</span></span>|<span data-ttu-id="79b7b-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="79b7b-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="79b7b-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="79b7b-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses
GET /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/deviceStatuses
```

## <a name="request-headers"></a><span data-ttu-id="79b7b-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="79b7b-120">Request headers</span></span>
|<span data-ttu-id="79b7b-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="79b7b-121">Header</span></span>|<span data-ttu-id="79b7b-122">値</span><span class="sxs-lookup"><span data-stu-id="79b7b-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="79b7b-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="79b7b-123">Authorization</span></span>|<span data-ttu-id="79b7b-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="79b7b-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="79b7b-125">Accept</span><span class="sxs-lookup"><span data-stu-id="79b7b-125">Accept</span></span>|<span data-ttu-id="79b7b-126">application/json</span><span class="sxs-lookup"><span data-stu-id="79b7b-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="79b7b-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="79b7b-127">Request body</span></span>
<span data-ttu-id="79b7b-128">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="79b7b-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="79b7b-129">応答</span><span class="sxs-lookup"><span data-stu-id="79b7b-129">Response</span></span>
<span data-ttu-id="79b7b-130">かどうかは成功すると、このメソッドが返されます、`200 OK`応答コードおよび応答の本文に[mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md)オブジェクトのコレクションです。</span><span class="sxs-lookup"><span data-stu-id="79b7b-130">If successful, this method returns a `200 OK` response code and a collection of [mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="79b7b-131">例</span><span class="sxs-lookup"><span data-stu-id="79b7b-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="79b7b-132">要求</span><span class="sxs-lookup"><span data-stu-id="79b7b-132">Request</span></span>
<span data-ttu-id="79b7b-133">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="79b7b-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses
```

### <a name="response"></a><span data-ttu-id="79b7b-134">応答</span><span class="sxs-lookup"><span data-stu-id="79b7b-134">Response</span></span>
<span data-ttu-id="79b7b-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="79b7b-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 687

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.mobileAppInstallStatus",
      "id": "7560ee45-ee45-7560-45ee-607545ee6075",
      "deviceName": "Device Name value",
      "deviceId": "Device Id value",
      "lastSyncDateTime": "2017-01-01T00:02:49.3205976-08:00",
      "mobileAppInstallStatusValue": "failed",
      "installState": "failed",
      "installStateDetail": "seeInstallErrorCode",
      "errorCode": 9,
      "osVersion": "Os Version value",
      "osDescription": "Os Description value",
      "userName": "User Name value",
      "userPrincipalName": "User Principal Name value",
      "displayVersion": "Display Version value"
    }
  ]
}
```




