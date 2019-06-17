---
title: リスト mobileAppInstallStatuses
description: MobileAppInstallStatus オブジェクトのプロパティとリレーションシップをリストします。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 590bb3d10b94e66095466e73f24fb8fab76844c3
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/14/2019
ms.locfileid: "34973909"
---
# <a name="list-mobileappinstallstatuses"></a><span data-ttu-id="335b0-103">リスト mobileAppInstallStatuses</span><span class="sxs-lookup"><span data-stu-id="335b0-103">List mobileAppInstallStatuses</span></span>

> <span data-ttu-id="335b0-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="335b0-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="335b0-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="335b0-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="335b0-106">[MobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md)オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="335b0-106">List properties and relationships of the [mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="335b0-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="335b0-107">Prerequisites</span></span>
<span data-ttu-id="335b0-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="335b0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="335b0-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="335b0-110">Permission type</span></span>|<span data-ttu-id="335b0-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="335b0-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="335b0-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="335b0-112">Delegated (work or school account)</span></span>|<span data-ttu-id="335b0-113">DeviceManagementApps.ReadWrite.All、DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="335b0-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="335b0-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="335b0-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="335b0-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="335b0-115">Not supported.</span></span>|
|<span data-ttu-id="335b0-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="335b0-116">Application</span></span>|<span data-ttu-id="335b0-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="335b0-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="335b0-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="335b0-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses
GET /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/deviceStatuses
```

## <a name="request-headers"></a><span data-ttu-id="335b0-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="335b0-119">Request headers</span></span>
|<span data-ttu-id="335b0-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="335b0-120">Header</span></span>|<span data-ttu-id="335b0-121">値</span><span class="sxs-lookup"><span data-stu-id="335b0-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="335b0-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="335b0-122">Authorization</span></span>|<span data-ttu-id="335b0-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="335b0-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="335b0-124">承諾</span><span class="sxs-lookup"><span data-stu-id="335b0-124">Accept</span></span>|<span data-ttu-id="335b0-125">application/json</span><span class="sxs-lookup"><span data-stu-id="335b0-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="335b0-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="335b0-126">Request body</span></span>
<span data-ttu-id="335b0-127">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="335b0-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="335b0-128">応答</span><span class="sxs-lookup"><span data-stu-id="335b0-128">Response</span></span>
<span data-ttu-id="335b0-129">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で[mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md)オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="335b0-129">If successful, this method returns a `200 OK` response code and a collection of [mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="335b0-130">例</span><span class="sxs-lookup"><span data-stu-id="335b0-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="335b0-131">要求</span><span class="sxs-lookup"><span data-stu-id="335b0-131">Request</span></span>
<span data-ttu-id="335b0-132">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="335b0-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses
```

### <a name="response"></a><span data-ttu-id="335b0-133">応答</span><span class="sxs-lookup"><span data-stu-id="335b0-133">Response</span></span>
<span data-ttu-id="335b0-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="335b0-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 693

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
      "installStateDetail": "dependencyFailedToInstall",
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





